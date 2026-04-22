# Clash 规则集

这是一个为 [Clash](https://github.com/Dreamacro/clash) 提供的规则集，适用于中文用户，帮助优化国内流量直连，国际流量代理的策略。

## 简介

本项目提供了一组 Clash 的规则集配置，主要目标是：

- 中国大陆 IP 流量直连
- 中国大陆域名直连
- 其他流量通过代理
- 包含一些额外的域名规则，以优化体验

## 使用方法

1. 下载 `custom_cn.txt` 文件。
2. 将其放置在 Clash 的配置目录中。
3. 在 Clash 的配置文件中引用规则集：

```yaml
rules:
  - GEOIP,CN,DIRECT
  - MATCH,Proxy
```

## 规则说明

- `custom_cn.txt`：适用于中文用户的规则集，包含中国大陆 IP 和域名的直连规则。
- `custom.txt`：基础规则集，未针对特定地区优化。

## 贡献

欢迎提交 PR 来改进规则集，例如添加新的域名或 IP 段。

## 许可证

本项目遵循 MIT 许可证。详情请查看仓库中的 `LICENSE` 文件。

---

如果你有任何问题或建议，请在 [Gitee 项目页面](https://gitee.com/imh/clash-rules) 提交 issue。