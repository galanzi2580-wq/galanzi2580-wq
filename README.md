# Zen Wu｜应用安全与 AI 基础设施安全

应用安全工程师，关注 AI 平台、机器学习工具和数据基础设施的安全，重点研究身份认证、访问权限与文件隔离边界。

## 已公开的漏洞研究

以下四条公开 CVE 记录关联了我通过 [Huntr](https://huntr.com/users/galanzi2580-wq) 提交的漏洞报告。

| CVE 编号 | 项目 | 问题概述 | CNA 评分 |
| --- | --- | --- | --- |
| [CVE-2026-3514](https://www.cve.org/CVERecord?id=CVE-2026-3514) | Prefect Server | 身份认证检查不完整，可能允许未经认证的访问 | 高危 7.5 |
| [CVE-2026-2734](https://www.cve.org/CVERecord?id=CVE-2026-2734) | MLflow | 普通账号可能超出权限查看模型版本信息 | 中危 6.5 |
| [CVE-2026-3198](https://www.cve.org/CVERecord?id=CVE-2026-3198) | MLflow AI Gateway | 网关资源列表缺少完整的权限校验 | 中危 6.5 |
| [CVE-2026-5422](https://www.cve.org/CVERecord?id=CVE-2026-5422) | Jupyter Server | 特定条件下，文件访问可越过配置的目录边界 | 中危 6.8 |

查看 [中文研究说明、影响范围与修复建议](https://github.com/galanzi2580-wq/cve-writeups)。公开页面以防御性分析为主，省略完整利用步骤与可执行 PoC。

> 状态说明：Huntr 公开报告的发现者姓名为 **Zen Wu**；截至 2026 年 10 月 26 日，四条 CVE 官方 JSON 的 Credits 字段尚未列入姓名。CVE-2026-5422 的 GitHub 聚合公告另有重复标记，详见[对应研究说明](https://github.com/galanzi2580-wq/cve-writeups/tree/main/cve-2026-5422-jupyter-path)。

## 相关链接

- [Huntr 研究者主页](https://huntr.com/users/galanzi2580-wq)
- [中文 CVE 研究说明](https://github.com/galanzi2580-wq/cve-writeups)
