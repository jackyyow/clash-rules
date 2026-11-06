# clash-rules

OpenClash / Clash 自定义规则集，托管在 GitHub 供 `rule-providers` 以 `http` 类型引用、自动更新。

| 规则集 | 内容 | 策略 |
|---|---|---|
| `muse.list` | muse.ai | 代理 |
| `Polymarket.list` | Polymarket | 代理 |
| `GoogleDrive.list` | Google Drive | 代理 |
| `MPlan.list` | 计划M bot（drpc.org） | 代理 |

## 引用方式

在 OpenClash 配置的 `rule-providers` 中：

```yaml
  Muse:
    type: http
    behavior: classical
    format: text
    interval: 86400
    url: https://raw.githubusercontent.com/jackyyow/clash-rules/main/muse.list
    path: ./rule_provider/muse.list
```
