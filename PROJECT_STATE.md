# Project State
- project: ai-for-good-2026
- method_version: Competition OS V0.1
- updated_at: 2026-10-19
- timezone: Asia/Shanghai
- phase: Competition Evaluation / Application
- participation: undecided
- track: undecided
- product: undecided
- state_integrator: 当前任务的执行 Agent；后续由 Human 指派
- human_owner: 发起本次任务的用户（GitHub: slowhot112）

## Goal / Boundaries
建立可复用协作框架，并以本次比赛评估为首个实例。当前不启动产品，不默认参赛，不提交报名。比赛优先；自动化未启用。

## Confirmed Decisions
| ID | status | scope | source |
|---|---|---|---|
| [DEC-0001](decisions/DEC-0001-framework-and-stage.md) | accepted | 双仓库 V0.1、权责和阶段边界 | 用户本次明确请求，原话摘录见 Decision |

## Tasks
| ID | status | owner | next |
|---|---|---|---|
| [TASK-0001](tasks/TASK-0001-bootstrap.md) | review | Codex（本次执行 Agent） | Human 体验并验收 V0.1 |
| [TASK-0002](tasks/TASK-0002-verify-competition.md) | draft | unassigned | 补齐官方材料，由 Human 分配并授权 |

## Evidence / Unknowns
- 双仓库的结构、链接和方法快照验证见 [V0.1 检查记录](docs/VALIDATION.md)。自检不等于 Human 验收。
- 目前只有引用对话作为背景，没有完整报名图或官方原文；不能确认截止时间、参赛资格、赛道、赛制或机构对接安排。
- 养老、防诈骗、社区动物、环保均为历史假设，未采纳、未验证。
- 未访谈公益机构，未获取业务数据；没有产品、真实效果或报名提交结果。

## Blockers / Human Decisions Needed
正式评估需要官方入口和完整报名材料；后续需 Human 决定是否参赛、投入上限、赛道与产品。TASK-0002 是 draft，未声称已分配或开始。

## Next Action
Human 先验收框架；准备好官方链接/原图后分配 TASK-0002。Agent 核实资料、提出参赛判断建议，Human 另立编号 Decision 确认。

## Recovery / Sync
先读此文件，再读 DEC-0001、所接 TASK、docs/SOP.md 和相关输入。规范 Task/Decision 是细节依据，此处是恢复索引。任务结束要写实际完成、阻塞、待确认项和下一位行动者。
发布状态及远端提交由仓库外交付记录 DELIVERY.md（随本地交付提供） 记录；未发布的改动注明 local pending，不宣称 main 已生效。此文件随本次初始化提交发布，不代表 Human 已验收。
