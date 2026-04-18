# trade_Report

用于存放交易报告体系中的稳定 Prompt 与模板。

## 当前范围
- 加密裁决日报 Prompt v1.2
- 加密裁决日报模板 v1.2
- 版本变更记录

## 核心原则
- 中文默认
- 数字优先
- 结论先行
- 因果链使用 `→`
- 给单一方向，不做对冲表述
- 结构识别先于交易动作

## 当前结构标准
### 1. 路径标签
回答价格怎么走：
- 区间
- 震荡上行
- 加速上行
- 区间下行
- 加速下行
- 失控级联

### 2. 主结构
回答谁在推价格：
- Type 1 现货主导型
- Type 2 杠杆抢跑型
- Type 3 共振趋势型
- Type 4 单侧挤压型
- Type 6 缓慢出清型
- Type 7 级联踩踏型
- Type 8 存量震荡型

### 3. 风险标签
回答结构是否已经脆弱：
- Type 5+ 多头拥挤
- Type 5- 空头拥挤
- 无

## 当前版本要点
- 保留 8-Type 数量与三问框架
- Type 5 不再作为主结构，改为风险 overlay
- Type 7 优先级高于 Type 4
- 方向从 Type 中拆出，统一用 `+ / - / 0`
- 宏观三链、远端锚、conviction 拆解保持不变

## 文件结构
- `prompts/crypto_daily_prompt_v1.2.md`
- `templates/crypto_daily_template_v1.2.md`
- `CHANGELOG.md`

## 后续扩展
- crypto weekly template
- all-asset mapping layer
- quant rules / state machine draft
