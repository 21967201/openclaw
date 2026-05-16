# PR 正文（中文）

**标题**：将上游 steipete/openclaw 的 main 同步到 main（2026-05-16）

**描述**：
将上游仓库 steipete/openclaw（分支：main）同步到本仓库的 sync/upstream-main-20260516 分支，并准备合并到 main。

**变更摘要**：
- 从 steipete/openclaw/main 拉取最新提交并合并到 sync/upstream-main-20260516。
- 包含上游的修复与改进；请在合并前运行测试并审查变更。

**合并前检查清单**：
- [ ] `git fetch origin && git checkout main && git pull origin main`
- [ ] 在本地或 CI 上运行所有单元和集成测试并确认通过
- [ ] 运行 lint/格式化工具并修复警告
- [ ] 验证依赖变更（package.json / go.mod / requirements.txt / pyproject.toml）并确认兼容性
- [ ] 如果存在数据库或配置迁移，先在测试环境验证迁移脚本
- [ ] 启动应用并对关键功能做 smoke 测试
- [ ] 确认该分支与 main 的 CI 作业（GitHub Actions）均通过
- [ ] 解决冲突（如有）并重新运行测试
- [ ] 指定 reviewers 并至少获得一次批准
- [ ] 确认合并策略（merge commit / squash / rebase）
- [ ] 合并后监控 CI/部署并准备回滚方案

**建议 reviewers**：@steipete, @pashpashpash
**建议 labels**：sync、needs review、ci-required

**备注**：
- 如需我把 PR 正文加入关键 commit 或文件级别变更摘要，或把这段以 heredoc 形式打包成 pr_body.md（方便用 gh pr edit 自动替换），我可以立刻生成。
