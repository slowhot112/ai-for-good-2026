# TASK-0001 · 建立 Competition OS V0.1 与首个实例
- id: TASK-0001
- status: review
- owner: Codex（本次执行 Agent）
- integrator: Codex（仅本次初始化范围）
- human_reviewer: 发起本次任务的用户
- priority: high
- depends_on: none
- related_decisions: DEC-0001
- updated_at: 2026-10-19
- issue_url: none
- branch_or_pr: 初始化提交 main；提交记录见仓库外交付记录
- blocked_reason: none
- resume_condition: none
- accepted_by: pending
- accepted_at: pending
- acceptance_evidence: pending

## Goal / Scope
搭建可复用手动框架和评估阶段实例；发布到用户个人账号两个私有仓库，不实现比赛产品。
## Inputs
用户本次请求与 DEC-0001；引用对话只作背景。
## Write Scope
本次新建 competition-os/ 和 ai-for-good-2026/ 全部文件，及仓库外交付记录；不修改既有项目。
## Deliverables
双仓库、六类模板、Issue/PR 模板、SOP、状态入口、扩展说明和检查记录。
## Acceptance Criteria
- [ ] AC1: 两个独立仓库包含请求的所有文件/目录，模板可复制使用。
- [ ] AC2: Idea/Decision 分离、编号、人类验收、状态恢复和交接规则相互一致。
- [ ] AC3: 实例明确参赛/赛道/产品待定，无虚构规则、访谈或实现。
- [ ] AC4: 链接和模板快照检查通过，无运行中的自动化。
- [ ] AC5: 发布到指定账号的两个私有仓库，远端内容与交付提交一致。
## Verification
逐条 Agent 自检结果见 [VALIDATION](../docs/VALIDATION.md) 与仓库外交付记录。上方复选框保留给 Human 验收。
## Handoff
### Summary
交付 V0.1 手动协作框架与评估实例，等待 Human 验收。
### Artifacts
README、PROJECT_STATE、DEC-0001、模板、SOP；两仓库地址见各自 README。
### Verification
文件、相对链接、方法快照与无自动化检查见 VALIDATION；远端核验见交付记录。
### Open Issues
Human 尚未验收；官方赛事材料缺失，方法尚未经真实比赛验证。
### Next Step
Human 验收 TASK-0001；准备原始赛事资料并分配 TASK-0002。
## Human Acceptance
pending。通过后记录验收人、时间和证据，integrator 再改 done 并更新 PROJECT_STATE。
