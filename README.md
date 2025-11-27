# Surge

本仓库用于维护个人 Surge 使用的规则文件与域名分类列表，便于统一管理与远程引用。

## 文件说明
- AppleIntelligence.list  
  Apple Intelligence / Siri 相关域名（语音请求、推理中继、Relay 服务等）
  Raw 地址：  
  https://raw.githubusercontent.com/eric24lu/Surge/main/AppleIntelligence.list

## 使用方式（示例）
在 Surge 配置中添加：
```
[Rule]
RULE-SET,AppleIntelligence,MyStrategyGroup
```
或在配置文件中引用：
```
[RuleSet]
AppleIntelligence = https://raw.githubusercontent.com/eric24lu/Surge/main/AppleIntelligence.list, interval=86400, policy=MyStrategyGroup
```
（将 MyStrategyGroup 替换为你的策略组名称）

## 更新策略
- 不定期手动维护
- 若域名废弃将加入注释或移除
- 后续可补充更多分类（例如：AI、语音、CDN、隐私相关）

## 贡献 / 建议
目前为个人使用，后续可考虑开放 Issue 供建议。

## 免责声明
列表仅供个人学习与网络访问优化使用，不保证完整性或绝对准确性。

## 许可
暂未指定 License（如需可添加 MIT / Apache-2.0）。
