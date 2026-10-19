# Competition OS SOP · V0.1

## 一次最小工作循环
1. Human 说明目标、约束、投入上限；Agent 读 PROJECT_STATE 和已接受 Decision。
2. 将猜想写 IDEA；将调查写 RESEARCH，注明原始来源、时间、已核实事实和推断。无证据不晋升结论。
3. 涉及目标、投入、赛道、产品或推翻旧方案时，创建 DECISION 草案，由 Human 确认并记录原话/Issue/PR 链接。
4. 把可执行工作写 TASK，唯一 owner 和 integrator，明确输入、允许修改的文件、依赖、交付物、逐条可观察验收标准。Human 授权后设 ready。
5. owner 领取后设 in_progress，完成范围内工作并验证；阻塞就记原因、恢复条件和下一步负责人。
6. 提交任务分支/PR，填写交接段和证据，状态设 review。整合人检查差异、Decision 一致性、来源及敏感信息。
7. Human 逐条验收。通过后记 accepted_by / accepted_at / acceptance_evidence，任务设 done 并整合；不通过回 in_progress，保留反馈。不得把 Agent 自检当成人工批准。
8. 整合人同步 PROJECT_STATE；有活动的当天写 DAILY。里程碑或出现重复摩擦后写 RETROSPECTIVE，只提炼有实际收益的 SOP 改动。

无需每件小事都创建六类文档。简单任务只需 TASK、证据和状态更新；方向变化才需 Decision；没有活动不写空日报。

## 状态、编号与一致性
- Task: draft → ready → in_progress → review → done；blocked 可从 ready / in_progress / review 进入，解除后回原状态，记录原因与恢复依据。取消用 cancelled，写明 Human 依据。
- Decision: proposed → accepted / rejected；accepted 仅在新决策被 Human 接受后标 superseded，保留旧内容与替代链接。
- Idea: hypothesis / researching / archived。只有明确 Decision 引用才表示被采纳，不能靠移动文件夹表示确认。
- 编号按仓库独立递增：IDEA-0001、RES-0001、DEC-0001、TASK-0001；文件名为编号加英文短名。编号不复用，GitHub Issue # 号不是这些编号。
- 新建编号前检查索引和开放分支/PR；V0.1 由单一 integrator 分配，避免并发碰撞。
- Task 文件权威保存任务细节；Decision 文件权威保存决策；PROJECT_STATE 是它们的恢复入口和摘要，冲突时检查原记录及批准证据后修正摘要，不能靠改摘要推翻决定。
- 未整合变化注明 branch/PR 或 local pending；不能把本地改动写成 main 已生效。离线时先记待同步项，恢复连接后比较差异再整合。

## 统一 Definition of Done
- 范围与已接受 Decision 一致，交付文件可打开，链接可追溯。
- 每条 acceptance_criteria 都有 pass / fail / not_run 和对应证据；not_run 必须解释，不能算通过。
- 研究区分来源事实/推断；代码变化执行与风险相称的测试；仅文档变化检查结构、链接、一致性即可。
- 交接段齐全，已知问题写清；不复制不必要的数据或凭据。
- Human 明确验收并留记录，整合人完成整合和 PROJECT_STATE 同步；发布前核对 GitHub 与本地提交一致。

## 日常接入
新 Agent 的启动指令：阅读 AGENTS.md；从 PROJECT_STATE.md 恢复上下文；读取 TASK-ID 和关联 Decision；复述目标、可写范围及验收标准；只执行该任务；附验证证据并交回 review，更新待整合状态。

角色是职责，不要求部署多个机器人：Human 可兼 integrator，一名 Agent 可兼研究、执行和技术审查，但不能替代 Human 批准。外部 Agent 无仓库权限时，以同样字段交接，integrator 负责落库。

## 两仓库演进
competition-os 保存通用规则与模板；比赛实例固定使用版本快照，docs/OS_VERSION.md 记录来源。实例可先修正自己的 SOP，复盘后再将通用经验提回 competition-os。上游更新不会自动覆盖实例，更不会覆盖已接受 Decision。

## 远端启用
发布到目标私有仓库；核对账号、可见性、main 分支与提交。Issue/PR 模板只有在 GitHub 对应入口创建新记录时生效。V0.1 未配置 labels、Actions、自动 Reviewer、分支保护或通知机器人；文档规则不等于平台强制。
