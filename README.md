# astra-skill-deploy-register

Mandatory registration checklist after deploying a new service or facility for Hermes Agent. Ensures every newly deployed service is registered in the service inventory, wired into health checks, and cleaned of residuals.

## Features

- Automated registration: forces registration of name / port / purpose / health check method after deployment
- Health check integration: ensures the service is immediately wired into automated checks
- Cleanup check: old versions / old processes / temp files + future removal plan

## Install

Copy `SKILL.md` to your Hermes profile's `skills/` directory:

```bash
cp SKILL.md ~/.hermes/profiles/default/skills/deploy-register.md
```

## Dependencies

This skill has no external dependencies. Its checklist is self-contained.

## License

MIT — see [LICENSE](LICENSE).

---

## 中文版

### 功能

- 自动化登记：服务部署后强制注册名称/端口/用途/健康检查方式
- 健康检查接入：确保部署后立即接入自动化检查
- 清理检查：旧版本/旧进程/临时文件清理 + 未来移除计划

### 安装

将 `SKILL.md` 复制到 Hermes profile 的 `skills/` 目录下：

```bash
cp SKILL.md ~/.hermes/profiles/default/skills/deploy-register.md
```

### 依赖关系

此 skill 无外部依赖，检查清单完全自包含。
