# Clash Rule Set

This is a rule set for [Clash](https://github.com/Dreamacro/clash), designed for Chinese users to optimize routing strategies by directly connecting domestic traffic and proxying international traffic.

## Introduction

This project provides a set of Clash rule configurations with the primary goals of:

- Direct connection for China mainland IP traffic
- Direct connection for China mainland domain names
- Proxying all other traffic
- Including additional domain rules to enhance user experience

## Usage

1. Download the `custom_cn.txt` file.
2. Place it in Clash's configuration directory.
3. Reference the rule set in your Clash configuration file:

```yaml
rules:
  - GEOIP,CN,DIRECT
  - MATCH,Proxy
```

## Rule Details

- `custom_cn.txt`: A rule set tailored for Chinese users, containing direct connection rules for China mainland IPs and domains.
- `custom.txt`: A basic rule set without region-specific optimizations.

## Contribution

Pull requests are welcome to improve the rule set, such as adding new domains or IP ranges.

## License

This project is licensed under the MIT License. See the `LICENSE` file in the repository for details.

---

If you have any questions or suggestions, please open an issue on the [Gitee project page](https://gitee.com/imh/clash-rules).