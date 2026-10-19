# DEC-0001 · V0.1 框架与评估阶段边界
- id: DEC-0001
- status: accepted
- proposed_by: Human
- accepted_by: 发起本次任务的用户
- accepted_at: 2026-10-19（Asia/Shanghai，原始指令日期）
- approval_evidence: 本次用户搭建请求；关键原话摘录如下
- supersedes: none
- superseded_by: none

## Context
需要一套可复用 Human × AI Agent 团队 SOP，并将本次比赛作为首个实例。此 Decision 记录用户已经明确给出的边界，不代表交付物已被验收。

## Decision
1. competition-os 为长期方法/模板仓库，ai-for-good-2026 为独立比赛实例。
2. GitHub 为 Single Source of Truth；Idea 与 Decision 分离；Human 管目标、关键决策和验收，Agent 管执行及状态同步。
3. Agent 不得自行推翻已接受 Decision；PROJECT_STATE 为首要业务恢复入口，任务有统一验收标准。
4. 当前阶段为 Competition Evaluation / Application；是否参赛、赛道和产品未确定。
5. 只建最小文档与结构，自动化保留未来接口；比赛优先，SOP 随真实实践迭代。

## Approval Evidence
用户原话：“先做最小可用框架，不要过度自动化。”
用户原话：“是否参赛和最终赛道/产品均未正式确定，不要把养老、防诈骗、社区动物、环保等脑暴写成已确认方向。”
用户原话：“Agent 不得自行推翻已确认 Decision”。
另：用户对仓库发布选择“我的个人 GitHub 账号，两个都设为私有”（2026-10-19）。

## Consequences / Revisit Trigger
当前不会启动候选产品开发或自动化服务。获得真实规则/场景后，用新的编号 Decision 决定是否参赛及方向；不得覆盖此历史记录。
