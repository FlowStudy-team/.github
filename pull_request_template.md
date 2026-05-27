# Pull Request Template

## 📝 变更说明 (Description)

请简要说明本次 PR 的主要改动内容，建议使用清晰、可验证的描述。

- 
- 
- 

## 🎯 变更目的 (Motivation)

请说明为什么需要本次改动，例如新增功能、修复问题、重构代码、补充文档、完善工程配置等。

- 

## 🔗 关联 Issue (Related Issue)

Resolves #

如果没有关联 Issue，请填写：

```text
N/A
```

## 🏭 影响范围 (Scope)

请勾选本次 PR 涉及的范围。

- [ ] `core`：Java 核心业务与调度服务
- [ ] `frontend`：前端页面与交互
- [ ] `judge`：Go 判题服务 / 沙箱执行
- [ ] `ai`：Python AI Agent 服务
- [ ] `docs`：项目文档 / 接口契约 / 开发规范
- [ ] `infra`：Docker Compose / CI/CD / 部署脚本 / 中间件配置
- [ ] 数据库表结构变更
- [ ] RabbitMQ 消息契约变更
- [ ] RESTful API 接口变更
- [ ] 其他：

## 🧩 具体改动 (Changes)

请按模块描述本次改动。没有涉及的模块可以填写 `N/A`。

### Core

- 

### Frontend

- 

### Judge

- 

### AI

- 

### Docs / Infra

- 

## 🧪 测试说明 (Test Plan)

请说明你如何验证本次改动。

- [ ] 已在本地启动相关服务并验证功能正常
- [ ] 已执行单元测试
- [ ] 已执行接口测试
- [ ] 已执行前后端联调
- [ ] 已验证数据库迁移或初始化脚本
- [ ] 已验证 RabbitMQ 消息发送 / 消费流程
- [ ] 本次改动仅涉及文档，无需运行服务

测试命令或验证过程：

```bash

```

## 📸 测试截图 / 日志 (Screenshots / Logs)

如涉及页面、接口返回、服务启动、判题结果、MQ 消息等，请贴出截图或关键日志。

```text

```

## ⚠️ 风险与影响 (Risks)

请说明本次改动可能带来的风险。

- [ ] 无明显风险
- [ ] 可能影响已有接口
- [ ] 可能影响数据库结构
- [ ] 可能影响消息队列消费
- [ ] 可能影响鉴权 / 权限控制
- [ ] 可能影响部署环境
- [ ] 其他：

风险说明：

```text

```

## 🔄 回滚方案 (Rollback Plan)

如果本次 PR 合并后出现问题，请说明如何回滚。

- [ ] 直接 revert 本次 PR
- [ ] 回滚数据库变更
- [ ] 回滚配置文件
- [ ] 关闭相关功能开关
- [ ] 其他：

说明：

```text

```

## ✅ 提交前自查表 (Checklist)

- [ ] 我已经仔细 Review 过自己的代码或文档改动。
- [ ] 没有遗留无意义的 `System.out.println`、`console.log`、临时代码或调试注释。
- [ ] Git Commit Message 遵守约定式提交规范，例如 `feat:`、`fix:`、`docs:`、`refactor:`。
- [ ] Controller 没有直接返回数据库 Entity。
- [ ] RESTful API 返回格式符合 `Result<T>` 规范。
- [ ] 如果新增或修改了接口，已同步更新 API 文档。
- [ ] 如果新增或修改了错误码，已同步更新错误码文档。
- [ ] 如果修改了数据库结构，已同步更新 SQL 脚本或数据库设计文档。
- [ ] 如果修改了 RabbitMQ 消息结构，已同步更新 MQ 契约文档。
- [ ] 如果涉及敏感配置，没有提交真实 API Key、Token、密码或本地 `.env` 文件。
- [ ] 本次改动不会破坏已有主流程，或已在上方说明风险与回滚方案。

## 🧾 备注 (Additional Notes)

其他需要 Reviewer 注意的信息。

```text

```
