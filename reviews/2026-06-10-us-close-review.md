# 2026-06-10 美股收盘复盘

## 市场复盘

本次自动化运行未能完成 Longbridge 数据采集，因此不输出 `SPY.US`、`QQQ.US`、`DIA.US`、`.VIX.US` 的强弱判断，也不对当天市场定性为风险偏好、避险主导或分化震荡。

数据采集阻塞点如下：当前运行环境中 `longbridge --help` 返回“无法将 longbridge 项识别为 cmdlet、函数、脚本文件或可运行程序的名称”；尝试直接执行 `C:\Users\31497\AppData\Local\Programs\longbridge\longbridge.exe` 返回“拒绝访问”；`where.exe longbridge` 未找到可执行文件。由于关键约束要求必须优先使用 longbridge-skills 且不得用外部网页抓取替代核心行情分析，本次不使用其他行情源补齐价格、分时、K 线或新闻。

`BTCUSD.HAS` 与 `GLD.US` 也未取得 Longbridge 行情或新闻数据，因此不能判断 BTC 与黄金相对表现所反映的市场情绪变化。

## 核心驱动与新闻

当日新闻驱动证据有限，以下判断以价格行为为主。但本次同样未取得 Longbridge 价格行为数据，因此不提炼 2026-06-10 的市场驱动因素。

- `SPY.US`、`QQQ.US`、`DIA.US`、`.VIX.US`：quote、intraday、kline、news 均未获取。
- `NVDA.US`、`TSM.US`、`APP.US`、`MU.US`：quote、intraday、kline、trades、depth、news 均未获取。
- `BTCUSD.HAS`：quote、intraday、kline、trades、depth、news 均未获取。
- `GLD.US`：quote、intraday、kline、trades、depth、news 均未获取。

## 标的逐一复盘

### NVDA.US

收盘表现、日内路径、技术观察、成交/盘口观察和驱动因素均缺少 Longbridge 数据支持。由于 quote、intraday、kline、trades、depth、news 均未获取，本次不判断其是否跑赢市场，也不划定支撑阻力。

次日计划倾向观望。原因不是走势偏弱或偏强，而是数据链路缺失，无法确认 AI 主线是否延续。次日重点应先恢复 Longbridge quote、intraday 与 kline 数据，再观察是否相对 `QQQ.US` 继续走强；在数据恢复且价格行为显示放量突破或明显失守关键区间后，才改变观望判断。

### TSM.US

收盘表现、日内路径、技术观察、成交/盘口观察和驱动因素均缺少 Longbridge 数据支持。由于 quote、intraday、kline、trades、depth、news 均未获取，本次不判断其相对半导体链条的强弱。

次日计划倾向观望。需要先恢复 Longbridge 行情与新闻，再判断台积电是否跟随 AI/半导体主线。若数据恢复后显示其强于 `QQQ.US` 并有量价配合，可以转为偏多观察；若恢复后显示冲高回落且弱于指数，则继续观望或转弱。

### APP.US

收盘表现、日内路径、技术观察、成交/盘口观察和驱动因素均缺少 Longbridge 数据支持。由于 quote、intraday、kline、trades、depth、news 均未获取，本次不对其高波动区间和关键价位作判断。

次日计划倾向观望。APP 对风险偏好和成长股情绪较敏感，但本次没有 Longbridge 市场锚点与个股数据，不能判断资金是否继续追逐高 beta 成长股。若数据恢复后显示其放量强于 `QQQ.US`，再考虑偏多；若继续弱于指数或尾盘无承接，则维持观望。

### MU.US

收盘表现、日内路径、技术观察、成交/盘口观察和驱动因素均缺少 Longbridge 数据支持。由于 quote、intraday、kline、trades、depth、news 均未获取，本次不能判断存储链是否继续领涨 AI 主线。

次日计划倾向观望。若 Longbridge 数据恢复后，MU 继续强于 `QQQ.US` 且成交放大，可以作为重点偏多观察标的；若只是跟随指数反弹而无量能，则不追高。当前改变看法的前提是恢复 quote、intraday、kline 和 news 数据。

### BTCUSD.HAS

未获取到 BTC 实时/历史数据，可能是账户未开通该品类访问。

由于 `BTCUSD.HAS` 未取得 Longbridge quote、intraday、kline、trades、depth 或 news，本次停止对 BTC 做技术性结论，不判断趋势、支撑阻力或市场风险偏好信号。

次日计划只能观望。只有在 Longbridge 恢复该品类访问，并能取得实时/历史数据后，才重新评估 BTC 对风险偏好的指示意义。

### GLD.US

收盘表现、日内路径、技术观察、成交/盘口观察和驱动因素均缺少 Longbridge 数据支持。由于 quote、intraday、kline、trades、depth、news 均未获取，本次不判断黄金是否体现避险需求或利率压力。

次日计划倾向观望。需要先恢复 `GLD.US` 的 quote、intraday、kline 和 news，再看其是否与 `.VIX.US` 或美股指数形成避险背离。若恢复后显示黄金放量上行且指数走弱，可转向偏多避险观察；若恢复后仍弱于风险资产，则继续观望。

## 次日交易计划

整体市场层面，次日第一优先级不是交易，而是恢复 Longbridge 数据链路。没有 `SPY.US`、`QQQ.US`、`DIA.US`、`.VIX.US` 的 quote、intraday 与 kline，就无法判断 AI 主线是否延续、风险偏好是否扩散，或当月降息可能性变化是否已经反映到价格里。

最值得恢复后优先观察的标的是 `NVDA.US`、`MU.US`、`TSM.US` 和 `GLD.US`。前三者用于判断 AI 与半导体主线是否继续，`GLD.US` 用于观察利率和避险交易是否压过风险偏好。`APP.US` 作为高 beta 成长股可以放在第二梯队，等市场方向明确后再处理。`BTCUSD.HAS` 在 Longbridge 数据恢复前不纳入交易判断。

交易上，本次结论是继续观察、不急于交易。改变看法的条件很明确：Longbridge quote、intraday、kline、news 至少恢复到市场锚点和自选股层面；若同时 trades 或 depth 仍缺失，可以继续做价格与 K 线分析，但必须注明成交/盘口证据不足。

## 风险点与需要跟踪的变量

主要风险不是某个标的走势，而是数据缺口导致判断置信度不足。当前需要跟踪的变量是 Longbridge CLI 是否可在自动化环境中执行、`C:\Users\31497\AppData\Local\Programs\longbridge\longbridge.exe` 的访问权限是否恢复、以及 `longbridge` 是否重新出现在 `PATH` 可发现位置。

因数据不足而降低判断置信度的标的是全部标的：`SPY.US`、`QQQ.US`、`DIA.US`、`.VIX.US`、`NVDA.US`、`TSM.US`、`APP.US`、`MU.US`、`BTCUSD.HAS`、`GLD.US`。其中 `BTCUSD.HAS` 按要求不做任何技术性结论；所有美股与 `GLD.US` 也因缺少 quote、intraday、kline、trades、depth、news 而只保留观望计划。
