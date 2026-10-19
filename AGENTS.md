# Agent 工作规则 · V0.1

## 开始前
先读本文件以遵守规则；恢复业务上下文时首先读 PROJECT_STATE.md（方法仓库无此文件时读 README.md），随后读已接受 Decision、所接任务、对应证据和 SOP。聊天历史不是可靠的状态数据库。

## 权责与事实
- Human 负责目标、投入、参赛/赛道/产品等关键决策及最终验收；Agent 负责调研、整理、计划、执行、测试、状态同步。
- GitHub 默认分支是已整合事实的 Single Source of Truth；分支/PR 是待整合变更。Issue 用于讨论与排队；规范任务文件保存验收与交接，Issue 只链接它，避免复制两套状态。
- 未发布时，本地文件只是待同步工作副本，不能声称 GitHub 已同步。外部聊天、网盘、看板不是第二套决策源；重要信息须落入仓库并附来源。
- Idea 是假设，Research 是带来源的证据，Decision 是 Human 确认的选择。Agent 建议写 proposed，不能自行标为 accepted。
- 已接受 Decision 不得静默改写或推翻。新证据记录到 Research，另提新编号 Decision；Human 接受后用 supersedes 连接旧编号，保留旧正文及历史。
- 不确定的事实标记 unverified；禁止编造报名信息、截止时间、采访、数据、测试和批准记录。

## 接任务与交接
- 仅执行已授权范围。任务须有唯一 owner、inputs、deliverables、acceptance_criteria、depends_on、write_scope 和 human_reviewer。
- 无验收标准不进入 in_progress。无明确 owner 的 ready 任务不能抢占执行；分配由 Human 或已授权协调人记录。
- 同一文件同时只有一位写入者，尤其 PROJECT_STATE.md。Agent 各自在任务分支或独立副本交付，由任务指定 integrator 整合；冲突保留双方信息并记录处理依据。
- 发现 Decision 冲突，暂停冲突部分并记录 blocked_reason，其他独立授权工作可继续。
- 交付须填写 Summary / Artifacts / Verification / Open Issues / Next Step，并更新状态文件的任务链接、阻塞及下一步。
- Agent 只能提交 review；Human 明确验收后记录 accepted_by、accepted_at、acceptance_evidence 才能 done。技术审查通过不等于 Human 验收。
- 新会话不能假定共享文件访问权。无法读仓库的协作者须收到版本、任务、相关 Decision、输入和输出位置构成的交接包。

## 最小化与隐私
- 比赛优先，SOP 只解决真实摩擦；不要自行增加服务、依赖、定时器或多 Agent 编排。
- .gitignore 不能防止已追踪文件泄露；提交前检查差异，匿名化材料；不提交密钥、个人身份或未授权公益业务原始记录。私有仓库也须遵守此规则。
- AGENTS.md 是协作约定，不是权限系统。V0.1 靠任务记录、差异检查、单人整合与 Human 验收执行；未配置自动守卫或分支保护。


## 本实例边界
当前仅 Competition Evaluation / Application；参赛与产品均待 Human 决策。养老、防诈骗、社区动物、环保只是历史脑暴，不是已确认方向，也不构成已经验证的需求。
正式规则、完整报名表原图、截止时间、资格与赛制均未在本仓库核实。不能把引用聊天中的概述当作主办方证据。当前不代填或提交报名，不访问公益对象数据，不实现候选产品。
