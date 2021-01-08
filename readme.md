![Navbar](images/navbar.png)

![Logo](images/logo.svg)

[v1 __](javascript:;)

  * [v1](/docs/spot/v1/en/)

[现货](/docs/spot/v1/en/) [交割合约](/docs/dm/v1/en/)
[币本位永续合约](/docs/coin_margined_swap/v1/en/)
[USDT本位永续合约](/docs/usdt_swap/v1/en/) [期权合约](/docs/option/v1/en/)

[简体中文](/docs/spot/v1/cn/)

shell

  * 简介
    * API 简介
    * 做市商项目
  * 更新日志
    * 1.2.1 2020年12月2日 【修改获取订单明细信息接口（查询无成交撤单数据时，如果不传“created_at”和“order_type”参数，由原来的只能查询到最近12小时数据，改为只能查询到最近2小时数据）；修改获取合约历史委托接口（查询无成交撤单数据时，由原来的只保留最近24小时数据，改为只保留最近2小时数据。）；修改组合查询合约历史委托接口（查询无成交撤单数据时，由原来的只保留最近24小时数据，改为只保留最近2小时数据。）】
    * 1.2.0 2020年11月24日 【新增：查询平台历史结算记录；修改：获取强平订单接口新增返参字段，订阅强平订单数据接口新增返参字段】
    * 1.1.9 2020年10月28日 【新增：1、新增组合查询财务记录接口、组合查询合约历史委托接口、组合查询历史成交记录接口。】
    * 1.1.8 2020年10月15日 【新增：切换杠杆倍数接口；修改：切换杠杆成功时 WS 资产接口推送更新信息，切换杠杆成功时 WS 持仓接口推送更新信息，订单撮合推送接口新增返参字段，获取合约订单信息接口（将原支持查询 24 小时的撤单数据改为支持查询 4 小时撤单数据）】
    * 1.1.7 2020年10月10日 【新增：订阅系统状态更新推送的 WebSocket 接口】
    * 1.1.6 2020年9月22日 【新增：市场行情接口已支持按照合约code调用，包括rest和ws接口。请求参数的“symbol”字段中，新增合约code类型，格式固定为“品种”、“年”、“月”、“日”，比如：BTC200925；通过合约code调用暂时只支持查询当前上市中的合约。】
    * 1.1.5 2020年8月6日 【新增：查询用户结算记录接口；订阅计划委托订单更新接口】
    * 1.1.4 2020年6月19日 【订阅订单撮合数据接口推送结果新增client_order_id字段】
    * 1.1.3 2020年6月14日 【增加合约信息变动 WS 接口; 增加买一卖一逐笔行情 WS 接口; 订阅 Market Depth 接口新增 4 个深度类型可选值; 新增查询用户可用杠杆倍数; 资产变动与持仓变动 WS 接口新增定期推送; 下单接口支持高倍杠杆; 优化查询订单相关接口的返回参数;私有推送接口新增 uid 返回参数;订单撮合推送接口新增字段;合约类型参数新增次季度合约】
    * 1.1.2 2020年4月9日 【增加：增加免鉴权的强平订单WS推送接口】
    * 1.1.1 2020年3月12日 【增加：增加WS订阅推送指数K线数据接口；增加WS订阅推送基差数据接口；增加获取指数K线数据restful接口；增加获取基差数据restful接口】
    * 1.1.0 2020年3月5日【增加：增加母子账号划转；增加多个下单类型；WS增加撮合订单推送】
    * 1.0.11 2020年2月21日【更新：批量20个订单改成批量最多10个订单】
    * 1.0.10 2020年1月15日【更新:更改K线等接口】
    * 1.0.9 2019年12月2日【更新:新增计划委托接口】
    * 1.0.8 2019年10月17日【更新:增加order_id_str字段】
    * 1.0.7 2019年10月15日
    * 1.0.6 2019年8月8日【更新:新增rest接口】
    * 1.0.5 2019年7月10日【更新:查询及下单功能】
    * 1.0.4 2019年6月6日【更新: Restful查询接口】
    * 1.0.3 2019年5月28日【更新：WS增加资产信息推送】
    * 1.0.2 2019年5月14日【更新: 币币账户和合约账户间进行资金的划转】
    * 1.0.1 2019年5月9日【更新：post_only高级限价委托功能上线】
    * 1.0.0 于2018年12月10日上线
  * 合约交易接入说明
    * 合约交易接口列表
    * 访问地址
    * 签名认证
    * 访问次数限制
    * 撤单率限制
    * 停服维护
    * 获取当前系统状态
    * 查询系统是否可用
    * 获取当前系统时间戳
    * 错误码详情
    * API 最佳实践
    * 代码实例
  * 常见问题
    * 接入验签相关
    * 行情及WS推送相关
    * 交易相关
    * 错误码相关
    * 如何更有效的解决问题
  * 合约市场行情接口
    * 获取合约信息
    * 获取合约指数信息
    * 获取合约最高限价和最低限价
    * 获取当前可用合约总持仓量
    * 获取预估交割价
    * 查询系统状态
    * 获取行情深度数据
    * 获取K线数据
    * 获取聚合行情
    * 获取市场最近成交记录
    * 批量获取最近的交易记录
    * 查询合约风险准备金余额和预估分摊比例
    * 查询合约风险准备金余额历史数据
    * 查询平台阶梯调整系数
    * 平台持仓量的查询
    * 精英账户多空持仓对比-账户数
    * 精英账户多空持仓对比-持仓量
    * 获取强平订单
    * 查询平台历史结算记录
    * 获取指数K线数据
    * 获取基差数据
  * 合约资产接口
    * 获取用户账户信息
    * 获取用户持仓信息
    * 查询母账户下所有子账户资产信息
    * 查询单个子账户资产信息
    * 查询单个子账户持仓信息
    * 查询用户财务记录
    * 组合查询用户财务记录
    * 查询用户结算记录
    * 查询用户当前的下单量限制
    * 查询用户当前的手续费费率
    * 查询用户当前的划转限制
    * 用户持仓量限制的查询
    * 查询用户账户和持仓信息
    * 母子账户划转
    * 获取母账户下的所有母子账户划转记录
    * 获取用户的API指标禁用信息
    * 查询用户可用杠杆倍数
  * 合约交易接口
    * 合约下单
    * 合约批量下单
    * 撤销订单
    * 全部撤单
    * 切换杠杆
    * 获取合约订单信息
    * 获取订单明细信息
    * 获取合约当前未成交委托
    * 获取合约历史委托
    * 组合查询合约历史委托
    * 获取历史成交记录
    * 组合查询历史成交记录接口
    * 闪电平仓下单
    * 合约计划委托下单
    * 合约计划委托撤单
    * 合约计划委托全部撤单
    * 获取计划委托当前委托
    * 获取计划委托历史委托
  * 合约划转接口
    * 现货-交割合约账户间进行资金的划转
    * err-code列表
    * base-msg对应的err-msg列表
  * 合约Websocket简介
    * 接口列表
    * 合约订阅地址
    * 访问次数限制
  * WebSocket心跳以及鉴权接口
    * 市场行情心跳
    * 订单推送心跳
    * 订单推送访问地址
    * 服务方主动断开连接
    * 服务方返回错误，但不断开连接
    * 鉴权-Authentication
  * WebSocket市场行情接口
    * 订阅 KLine 数据
    * 请求 KLine 数据
    * 订阅 Market Depth 数据
    * 订阅Market Depth增量数据
    * 订阅买一卖一逐笔行情数据(BBO)
    * 订阅 Market Detail 数据
    * 请求 Trade Detail 数据
    * 订阅 Trade Detail 数据
  * WebSocket指数与基差数据接口
    * 订阅(sub)指数K线数据
    * 请求(req)指数K线数据
    * 订阅(sub)基差数据
    * 请求(req)基差数据
  * WebSocket订单和用户数据接口
    * 订阅订单成交数据（sub）
    * 取消订阅订单成交数据（unsub）
    * 订阅订单撮合数据（sub）
    * 取消订阅订单撮合数据（unsub）
    * 订阅资产变动数据（sub）
    * 取消订阅资产变动数据（unsub）
    * 订阅持仓变动更新数据（sub）
    * 取消订阅持仓变动更新数据（unsub）
    * 订阅强平订单数据(免鉴权)（sub）
    * 取消订阅强平订单(免鉴权)（unsub）
    * 订阅合约信息变动(免鉴权)（sub）
    * 取消订阅合约信息变动(免鉴权)（unsub）
    * 订阅计划委托订单更新
    * 取消订阅计划委托订单更新（unsub）
  * WebSocket系统状态更新接口
    * 订阅系统状态更新
  * WebSocket附录
    * 操作类型（OP）说明
    * 主题（topic）类型说明
    * 响应码（Err-Code）说明

  * [创建 API Key ](https://www.hbg.com/zh-cn/apikey/)

# 简介

## API 简介

欢迎使用火币合约 API！ 你可以使用此 API 获得市场行情数据，进行交易，并且管理你的账户。

在文档的右侧是代码示例，目前我们仅提供针对 `shell` 的代码示例。

你可以通过选择上方下拉菜单的版本号来切换文档对应的 API 版本，也可以通过点击右上方的语言按钮来切换文档语言。

## 做市商项目

做市商项目不支持点卡抵扣、VIP、交易量相关活动以及任何形式的返佣活动。

欢迎有优秀 maker 策略交易量大的用户参与长期合约做市商项目。如果您的火币交割合约账户中有折合大于 3 BTC
资产，或火币币本位永续合约账户中有折合大于 3 BTC 资产，或火币期权合约账户中有折合大于 3 BTC 资产，或火币USDT本位永续合约账户中有大于
30000 USDT 资产，请提供以下信息到 [[email protected]](/cdn-cgi/l/email-
protection)（做市商项目不支持点卡抵扣、VIP、交易量相关活动以及任何形式的返佣活动）:

  1. 提供火币UID （需不存在返佣关系的 UID）；
  2. 提供其他交易平台 maker 交易量截图证明（比如30天内成交量，或者 VIP 等级等）；

# 更新日志

## 1.2.1 2020年12月2日
【修改获取订单明细信息接口（查询无成交撤单数据时，如果不传“created_at”和“order_type”参数，由原来的只能查询到最近12小时数据，改为只能查询到最近2小时数据）；修改获取合约历史委托接口（查询无成交撤单数据时，由原来的只保留最近24小时数据，改为只保留最近2小时数据。）；修改组合查询合约历史委托接口（查询无成交撤单数据时，由原来的只保留最近24小时数据，改为只保留最近2小时数据。）】

###
1、修改获取订单明细信息接口（查询无成交撤单数据时，如果不传“created_at”和“order_type”参数，由原来的只能查询到最近12小时数据，改为只能查询到最近2小时数据）

  * 接口名称：获取订单明细信息

  * 接口类型：私有接口

  * 接口URL：api/v1/contract_order_detail

### 2、修改获取合约历史委托接口（查询无成交撤单数据时，由原来的只保留最近24小时数据，改为只保留最近2小时数据。）

  * 接口名称：获取合约历史委托

  * 接口类型：私有接口

  * 接口URL：api/v1/contract_hisorders

### 3、修改组合查询合约历史委托接口（查询无成交撤单数据时，由原来的只保留最近24小时数据，改为只保留最近2小时数据。）

  * 接口名称：组合查询合约历史委托

  * 接口类型：私有接口

  * 接口URL：api/v1/contract_hisorders_exact

## 1.2.0 2020年11月24日 【新增：查询平台历史结算记录；修改：获取强平订单接口新增返参字段，订阅强平订单数据接口新增返参字段】

### 1、新增查询平台历史结算记录接口

  * 接口名称：查询平台历史结算记录

  * 接口类型：公共接口

  * 接口URL：api/v1/contract_settlement_records

### 2、获取强平订单接口新增返参字段（返回参数中的 orders 参数下增加 amount 字段，表示强平数量(币)）

  * 接口名称：获取强平订单接口

  * 接口类型：公共接口

  * 接口URL：api/v1/contract_liquidation_orders

### 3、订阅强平订单数据接口新增返参字段（返回参数中的data参数下增加amount字段，表示强平数量(币)）

  * 接口名称：订阅强平订单数据

  * 接口类型：公共接口

  * 订阅主题：public.$symbol.liquidation_orders

## 1.1.9 2020年10月28日 【新增：1、新增组合查询财务记录接口、组合查询合约历史委托接口、组合查询历史成交记录接口。】

### 1、新增组合查询合约历史成交记录接口

  * 接口名称：组合查询合约历史成交记录

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_matchresults_exact

### 2、新增组合查询合约历史委托接口

  * 接口名称：组合查询合约历史委托

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_hisorders_exact

### 3、新增组合查询财务记录接口

  * 接口名称：组合查询财务记录

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_financial_record_exact

## 1.1.8 2020年10月15日 【新增：切换杠杆倍数接口；修改：切换杠杆成功时 WS 资产接口推送更新信息，切换杠杆成功时 WS
持仓接口推送更新信息，订单撮合推送接口新增返参字段，获取合约订单信息接口（将原支持查询 24 小时的撤单数据改为支持查询 4 小时撤单数据）】

### 1、新增切换杠杆倍数接口

  * 接口名称：切换杠杆

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_switch_lever_rate

###
2、订阅资产接口推送更新（返参event新增事件类型，switch_lever_rate表示切换倍数。在用户切换倍数成功时，需推送一次最新的资产信息，event为switch_lever_rate。）

  * 接口名称：订阅资产变动数据

  * 接口类型：私有接口

  * 订阅主题：accounts.$symbol

###
3、订阅持仓接口推送更新（返参event新增事件类型，switch_lever_rate表示切换杠杆。在用户切换杠杆倍数成功时，需推送一次最新的持仓信息（若用户持仓量为0，则不会触发推送），event为switch_lever_rate。）

  * 接口名称：订阅持仓变动数据

  * 接口类型：私有接口

  * 订阅主题：positions.$symbol 

### 4、订阅订单撮合推送接口更新（返回参数新增以下字段:direction(买卖方向)、offset
(开平方向)、lever_rate(杠杆倍数)、price(委托价格)、created_at(创建时间)、order_source
(订单来源)、order_price_type(订单报价类型)。）

  * 接口名称：订阅订单撮合推送

  * 接口类型：私有接口

  * 订阅主题：matchOrders.$symbol 

### 5、获取合约订单信息接口（将原支持查询 24 小时的撤单数据改为支持查询 4 小时撤单数据）

  * 接口名称：获取合约订单信息

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_order_info

## 1.1.7 2020年10月10日 【新增：订阅系统状态更新推送的 WebSocket 接口】

### 1、新增订阅系统状态更新推送的 WebSocket 接口

  * 接口名称：订阅系统状态更新
  * 接口类型: 公共接口
  * 订阅主题：public.$service.heartbeat

## 1.1.6 2020年9月22日
【新增：市场行情接口已支持按照合约code调用，包括rest和ws接口。请求参数的“symbol”字段中，新增合约code类型，格式固定为“品种”、“年”、“月”、“日”，比如：BTC200925；通过合约code调用暂时只支持查询当前上市中的合约。】

### 1、获取行情深度数据

  * 接口名称：获取行情深度数据
  * 接口类型: 公共接口
  * 接口URL：/market/depth

### 2、获取K线数据

  * 接口名称：获取K线数据
  * 接口类型: 公共接口
  * 接口URL：/market/history/kline

### 3、获取聚合行情

  * 接口名称：获取聚合行情
  * 接口类型: 公共接口
  * 接口URL：/market/detail/merged

### 4、获取市场最近成交记录

  * 接口名称：获取市场最近成交记录
  * 接口类型: 公共接口
  * 接口URL：/market/trade

### 5、批量获取最近的交易记录

  * 接口名称：批量获取最近的交易记录
  * 接口类型: 公共接口
  * 接口URL：/market/history/trade

### 6、订阅 KLine 数据

  * 接口名称：订阅 KLine 数据
  * 接口类型: 公共接口
  * 订阅主题：market.$symbol.kline.$period

### 7、请求 KLine 数据

  * 接口名称：请求 KLine 数据
  * 接口类型: 公共接口
  * 订阅主题：market.$symbol.kline.$period

### 8、订阅 Market Depth 数据

  * 接口名称：订阅 Market Depth 数据
  * 接口类型: 公共接口
  * 订阅主题：market.$symbol.depth.$type

### 9、订阅 Market Detail 数据

  * 接口名称：订阅 Market Detail 数据
  * 接口类型: 公共接口
  * 订阅主题：market.$symbol.detail

### 10、订阅 Trade Detail 数据

  * 接口名称：订阅 Trade Detail 数据
  * 接口类型: 公共接口
  * 订阅主题：market.$symbol.trade.detail

### 11、请求 Trade Detail 数据

  * 接口名称：请求 Trade Detail 数据
  * 接口类型: 公共接口
  * 订阅主题：market.$symbol.trade.detail

### 12、订阅 Market Depth 增量数据

  * 接口名称：订阅 Market Depth 增量数据
  * 接口类型: 公共接口
  * 订阅主题：market.$symbol.depth.size_${size}.high_freq

### 13、订阅买一卖一逐笔行情推送

  * 接口名称：订阅买一卖一逐笔行情推送
  * 接口类型: 公共接口
  * 订阅主题：market.$symbol.bbo

## 1.1.5 2020年8月6日 【新增：查询用户结算记录接口；订阅计划委托订单更新接口】

### 1、新增查询用户结算记录接口

  * 接口名称：查询用户结算记录

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_user_settlement_records 

### 2、订阅计划委托订单更新

  * 接口名称：订阅计划委托订单更新

  * 接口类型：私有接口

  * 订阅主题：trigger_order.$symbol

## 1.1.4 2020年6月19日 【订阅订单撮合数据接口推送结果新增client_order_id字段】

### 1、订阅订单撮合数据接口推送结果新增client_order_id字段

  * 接口名称：订阅订单撮合数据

  * 接口类型： 私有接口

  * 订阅主题：matchOrders.$symbol

## 1.1.3 2020年6月14日 【增加合约信息变动 WS 接口; 增加买一卖一逐笔行情 WS 接口; 订阅 Market Depth 接口新增 4
个深度类型可选值; 新增查询用户可用杠杆倍数; 资产变动与持仓变动 WS 接口新增定期推送; 下单接口支持高倍杠杆;
优化查询订单相关接口的返回参数;私有推送接口新增 uid 返回参数;订单撮合推送接口新增字段;合约类型参数新增次季度合约】

### 1、增加合约信息变动ws推送接口

  * 接口名称：增加合约信息变动ws推送接口

  * 接口类型：公开接口

  * 订阅主题：public.$symbol.contract_info

### 2、增加买一卖一逐笔行情 WS 接口

  * 接口名称：订阅买一卖一逐笔行情推送

  * 接口类型：公开接口

  * 订阅主题：market.$symbol.bbo

### 3、订阅 Market Depth 接口新增 4 个深度类型可选值:step12、step13、step14、step15

  * 接口名称：订阅 Market Depth 数据

  * 接口类型：公开接口

  * 订阅主题：market.$symbol.depth.$type

### 4、新增查询用户可用杠杆倍数

  * 接口名称：查询用户可用杠杆倍数

  * 接口类型：私有

  * 接口地址：api/v1/contract_available_level_rate

### 5、资产变动WS 接口新增定期推送: 5秒一次定期推送

  * 接口名称：订阅资产变动数据

  * 接口类型：私有接口

  * 订阅主题： accounts.$symbol

### 6、仓位变动WS 接口新增定期推送: 5秒一次定期推送

  * 接口名称：订阅持仓变动数据

  * 接口类型：私有接口

  * 订阅主题：positions.$symbol

### 7、下单接口支持高倍杠杆

  * 接口名称：合约下单

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_order

  * 接口名称：合约批量下单

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_batchorder

  * 接口名称：合约计划委托下单

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_trigger_order

###
8、获取订单明细信息接口返回参数,增加9个字段：fee（总手续费）、order_id（订单id）、order_id_str（string格式的订单id）、client_order_id（客户订单id）、order_type（订单类型）、status（订单状态）、trade_avg_price（成交均价）、trade_turnover（成交总金额）、trade_volume（成交总数量）

  * 接口名称：获取订单明细信息

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_order_detail

### 9、获取订单信息接口返回参数,增加2个字段：liquidation_type（强平类型）、 canceled_at（撤单时间）

  * 接口名称：获取订单信息接口 

  * 接口类型：私有接口

  * 接口地址：api/v1/contract_order_info

### 10、订阅成交订单推送，增加2个字段：canceled_at（撤单时间）、fee_asset （手续费币种）

  * 接口名称：订阅成交订单推送

  * 接口类型：私有接口

  * 订阅主题：orders.$symbol

### 11、私有推送接口新增 uid 返回参数

  * 接口名称：订阅成交订单推送

  * 接口类型：私有接口

  * 订阅主题：orders.$symbol

  * 接口名称：订阅资产变动推送

  * 接口类型：私有接口

  * 订阅主题：accounts.$symbol

  * 接口名称：订阅持仓变动推送

  * 接口类型：私有接口

  * 订阅主题：positions.$symbol

  * 接口名称：订阅订单撮合推送

  * 接口类型：私有接口

  * 订阅主题：matchOrders.$symbol

### 12、订单撮合推送新增接口新增字段，在返回参数的外层新增两个字段：trade_volume（订单已成交数量） 、volume（订单总委托数量）

  * 接口名称：订阅订单撮合推送

  * 接口类型：私有接口

  * 订阅主题：matchOrders.$symbol

### 13、合约类型参数新增次季度合约,合约类型（contract_type）参数新增次季度合约可选值

  * 接口名称：行情市场、资产以及交易(restful及websocket)接口

  * 接口类型: 公开/私有

## 1.1.2 2020年4月9日 【增加：增加免鉴权的强平订单WS推送接口】

  * 接口名称：WS订阅强平订单(免鉴权)
  * 接口类型：公共接口
  * 订阅主题：public.$symbol.liquidation_orders

## 1.1.1 2020年3月12日
【增加：增加WS订阅推送指数K线数据接口；增加WS订阅推送基差数据接口；增加获取指数K线数据restful接口；增加获取基差数据restful接口】

### 1、增加WS订阅推送指数K线数据

  * 接口名称：WS指数K线推送
  * 接口类型：公共接口
  * 订阅主题：market.$symbol.index.$period

### 2、增加WS订阅推送基差数据

  * 接口名称：WS指数基差推送
  * 接口类型： 公共接口
  * 订阅主题：market.$symbol.basis.$period.$basis_price_type

### 3、增加restful接口获取指数K线数据

  * 接口名称： 获取指数K线数据
  * 接口类型： 公共接口
  * 接口URL：/index/market/history/index

### 4、增加restful接口获取基差数据

  * 接口名称：获取基差数据
  * 接口类型：公共接口
  * 接口URL：/index/market/history/basis

## 1.1.0 2020年3月5日【增加：增加母子账号划转；增加多个下单类型；WS增加撮合订单推送】

###
1、在Web端和API端新增合约母子账户资产划转功能，Web端只有母账户有划转权限，可以进行母转子或者子转母，但是不能进行子账户之间相互划转。API端划转只能通过母账户的API
Key进行母子账户的互相划转。

#### 1.1、增加母子账户划转的API接口，母账户与每个子账户相互划转限频10次/分钟。

  * 接口名称：母子账户划转
  * 接口类型：私有接口
  * 接口URL：api/v1/contract_master_sub_transfer

####
1.2、查询系统状态的接口增加母子划转权限参数，在返回参数的数组"data"中，增加两个字段："master_transfer_sub"、"sub_transfer_master"。

  * 接口名称：查询系统状态
  * 接口类型：公共接口
  * 接口URL：api/v1/contract_api_state

#### 1.3、增加查询母账户下的所有母子账户的划转记录的功能。

  * 接口名称：获取母账户下的所有母子账户划转记录
  * 接口类型：私有接口
  * 接口URL：api/v1/contract_master_sub_transfer_record

#### 1.4、返回财务记录的接口中，增加返回4种母子账户划转的流水

  * 接口名称：查询用户财务记录
  * 接口类型：私有接口
  * 接口URL：api/v1/contract_financial_record

### 2、合约资产接口和合约交易接口中涉及到更改的如下：

#### 2.1、获取下单量限制的接口增加10种订单价格类型，包括：opponent_ioc（对手价-IOC下单），lightning_ioc（闪电平仓-
IOC下单），optimal_5_ioc（最优5档-IOC下单），optimal_10_ioc（最优10档-IOC下单），optimal_20_ioc（最优20档-IOC下单），opponent_fok（对手价-
FOK下单），lightning_fok（闪电平仓-
FOK下单），optimal_5_fok（最优5档-FOK下单），optimal_10_fok（最优10档-FOK下单），optimal_20_fok（最优20档-FOK下单）。

  * 接口名称：查询用户当前的下单量限制
  * 接口类型：私有接口
  * 接口URL：POST api/v1/contract_order_limit

#### 2.2、合约下单接口增加8种订单价格类型，分别为：opponent_ioc（对手价-
IOC下单），optimal_5_ioc（最优5档-IOC下单），optimal_10_ioc（最优10档-IOC下单），optimal_20_ioc（最优20档-IOC下单）,
opponent_fok（对手价-
FOK下单），optimal_5_fok（最优5档-FOK下单），optimal_10_fok（最优10档-FOK下单），optimal_20_fok（最优20档-FOK下单）。

  * 接口名称：合约下单
  * 接口类型：私有接口
  * 接口URL：api/v1/contract_order

#### 2.3、合约批量下单接口增加8种订单价格类型，分别为：opponent_ioc（对手价-
IOC下单），optimal_5_ioc（最优5档-IOC下单），optimal_10_ioc（最优10档-IOC下单），optimal_20_ioc（最优20档-IOC下单），opponent_fok（对手价-
FOK下单），optimal_5_fok（最优5档-FOK下单），optimal_10_fok（最优10档-FOK下单），optimal_20_fok（最优20档-FOK下单）。

  * 接口名称：合约批量下单
  * 接口类型：私有接口
  * 接口URL：api/v1/contract_batchorder

#### 2.4、获取订单明细信息增加字段liquidation_type

  * 接口名称：获取订单明细信息
  * 接口类型：私有接口
  * 接口URL：POST api/v1/contract_order_detail

####
2.5、获取合约历史委托trade_type和orders修改，请求参数的trade_type中，增加类型：减仓平多，减仓平空；返回参数的orders数组增加字段"liquidation_type"。

  * 接口名称：获取合约历史委托
  * 接口类型：私有接口
  * 接口URL：POST api/v1/contract_hisorders

#### 2.6、闪电平仓下单接口请求参数增加字段order_price_type，值分别为：lightning_ioc（闪电平仓-
IOC下单），lightning_fok（闪电平仓-FOK下单），lightning(闪电平仓-默认值）。

  * 接口名称：闪电平仓下单
  * 接口类型：私有接口
  * 接口URL：api/v1/lightning_close_position

#### 2.7、WS订单成交推送增加字段liquidation_type

  * 接口名称：WS订单成交
  * 接口类型：私有接口
  * 订阅主题：orders.$symbol

#### 2.8、增加WS撮合订单成交推送接口

  * 接口名称：WS撮合订单成交推送
  * 接口类型：私有接口
  * 订阅主题：matchOrders.$symbol

####
2.9、查询系统是否可用接口，增加永续合约相关状态字段，在返回参数的数组"data"中，增加两个字段："swap_heartbeat"、"swap_estimated_recovery_time"。

  * 接口名称：查询系统是否可用
  * 接口类型：公共接口
  * 接口URL：https://api.hbdm.com/heartbeat/

#### 2.10、增加获取用户的API指标禁用信息的API接口

  * 接口名称：获取用户的API指标禁用信息
  * 接口类型：私有接口
  * 接口URL：api/v1/contract_api_trading_status

## 1.0.11 2020年2月21日【更新：批量20个订单改成批量最多10个订单】

### 1、接口名称：合约批量下单

  * 接口URL：api/v1/contract_batchorder
  * 接口类型：私有接口
  * 优化点：批量下单的请求参数“orders_data”的一次最多允许批量请求订单数由20个改为10个。

### 2、接口名称：撤销订单

  * 接口URL：api/v1/contract_cancel
  * 接口类型：私有接口
  * 优化点：撤单接口的请求参数“order_id” 与 “client_order_id” 的一次最多允许撤消订单数由20个改为10个，多个订单ID中间以","分隔。

## 1.0.10 2020年1月15日【更新:更改K线等接口】

###
1、获取K线数据的接口中增加了两个请求参数“from”和“to”，“from”表示开始时间点（时间戳精确到秒），“to”表示结束时间点（时间戳精确到秒），最多可获取连续两年的数据。请求参数“size”改为非必填项。

  * /market/history/kline 获取K线数据

### 2、获取合约订单信息接口查询撤单信息，只能查询最近24小时内的撤单信息。

  * /api/v1/contract_order_info 获取合约订单信息

### 3、历史委托查询接口查询撤单信息，只能查询最近24小时内的撤单信息。

  * /api/v1/contract_hisorders 历史委托查询

###
4、获取订单明细接口查询撤单数据时，如果传“created_at”和“order_type”参数则能查询最近90天数据，如果不传“created_at”和“order_type”参数只能查询到最近24小时数据。

  * /api/v1/contract_order_detail 获取订单明细

## 1.0.9 2019年12月2日【更新:新增计划委托接口】

### 1、新增查询资金持仓接口

rest接口api/v1/contract_account_position_info，用于获取到当前的资产和持仓信息。

### 2、新增计划委托接口

  * `api/v1/contract_trigger_order`合约计划委托下单接口

  * `api/v1/contract_trigger_cancel`合约计划委托撤单接口

  * `api/v1/contract_trigger_cancelall`合约计划委托全部撤单接口

  * `api/v1/contract_trigger_openorders`获取计划委托当前委托接口

  * `api/v1/contract_trigger_hisorders`获取计划委托历史委托接口

### 3、部分接口增加返回“手续费币种”字段

部分API和内部接口增加返回字段表示手续费对应的币种：

  * `api/v1/contract_fee`查询用户当前的手续费费率

  * `api/v1/contract_order_info`获取合约订单信息

  * `api/v1/contract_order_detail`获取订单明细

  * `api/v1/contract_openorders`获取合约当前未成交委托

  * `api/v1/contract_hisorders`获取合约历史委托

  * `api/v1/contract_matchresults`获取历史成交记录

  * WS成交推送，增加返回“手续费币种”字段

### 4、部分接口请求参数的天数改为可随意输入

部分接口的请求参数“create_date”，由只能填写7或90 改为 可随意输入正整数，如果参数超过90则默认查询90天的数据：

  * `api/v1/contract_hisorders`获取限价单历史委托的接口

  * `api/v1/contract_trigger_hisorders`获取计划委托的历史委托接口

  * `api/v1/contract_matchresults`获取成交记录的接口

  * `api/v1/contract_financial_record`获取财务记录的接口

## 1.0.8 2019年10月17日【更新:增加order_id_str字段】

  * 为了解决nodejs和Javascript的用户order_id返回是18位数字长度过长的问题,接口返回增加order_id_str字段，类型为字符串，来表示订单号。

涉及接口:

api/v1/contract_order

api/v1/contract_batchorder

api/v1/contract_matchresults

api/v1/contract_hisorders

api/v1/contract_openorders

api/v1/lightning_close_position

api/v1/contract_order_info

  * 订单推送ws 增加 order_id_str

## 1.0.7 2019年10月15日

nodejs和Javascript的用户请特别注意：order_id返回是18位，nodejs和javascript默认解析18位有问题，nodejs和javascript里面JSON.parse默认是int，大于等于18位的数字用json-
bigint的包解析。 具体参考nodejs的demo，点击[查看](https://github.com/huobiapi/Futures-
Node.js-demo/tree/master/REST-Node.js-demo)。
详细说明，请点击[下载](https://github.com/huobiapi/Futures-Node.js-
demo/blob/master/Nodejs%20%E5%90%88%E7%BA%A6%20DEMO%E4%BF%AE%E6%94%B9.docx?raw=true)

### 1、修改接口获取用户账户信息

rest接口api/v1/contract_account_info增加返回字段‘ margin_static’，表示用户的静态权益

### 2、修改获取订单明细信息

rest接口api/v1/contract_order_detail、查询用户的成交记录

rest接口api/v1/contract_matchresults、用户订单的成交推送的ws增加字段id,表示成交唯一ID

### 3、修改下单

rest接口api/v1/contract_order和批量下单

rest接口api/v1/contract_batchorder

请求参数order_price_type中增加订单价格类型“ioc”(ioc:立即成交并取消剩余);

请求参数order_price_type中增加订单价格类型“fok”(fok:全部成交或立即取消);

### 4、修改查询用户当前的下单量限制

rest接口api/v1/contract_order_limit返回参数的“ order_price_type”，表示订单报价类型，

增加"fok":FOK订单(fok:全部成交或立即取消)，"ioc":IOC订单(ioc:立即成交并取消剩余)

### 5、新增查询系统状态的API

rest接口api/v1/contract_api_state

### 6、新增账户多空持仓对比-账户数

rest接口api/v1/contract_elite_account_ratio

### 7、新增精英账户多空持仓对比-持仓量

rest接口api/v1/contract_elite_position_ratio

### 8、新增获取强平订单

rest接口api/v1/contract_liquidation_orders和ws推送

## 1.0.6 2019年8月8日【更新:新增rest接口】

### 新增rest接口：

请求访问地址：https://api.hbdm.com/heartbeat/

备注：查询系统是否可用，其中heartbeat为1是可用，为0不可用。

## 1.0.5 2019年7月10日【更新:查询及下单功能】

### 新增接口：

新增rest接口,查询用户的下单量限制；

新增rest接口,查询用户的手续费费率；

新增rest接口,查询用户的划转限制；

新增rest接口,查询用户的持仓量限制；

新增rest接口,查询平台的风险准备金、预估分摊比例；

新增rest接口,查询平台持仓量；

新增rest接口,查询平台的风险准备金历史数据；

新增rest接口,查询平台的阶梯调整系数；

新增rest接口,闪电平仓下单；

### 对已有接口的修改：

rest接口，查询用户账户信息接口增加返回用户的调整系数；

rest接口，查询单个子账户资产信息接口增加返回用户的调整系数；

ws接口，资金推送增加返回用户的调整系数；

rest接口，下单接口和批量下单接口新增最优5、10、20档下单；

rest接口，获取成交记录增加按照合约code查询；

## 1.0.4 2019年6月6日【更新: Restful查询接口】

### 1.查询母账户下所有子账户资产信息

URL：api/v1/contract_sub_account_list

备注：只返回已经开通合约交易的子账户数据

### 2.查询单个子账户资产信息

URL：api/v1/contract_sub_account_info

备注：只能查询到开通合约交易的子账户信息；子账户来过合约系统但是未开通合约交易也不返回对应的数据

### 3.查询单个子账户持仓信息

URL：api/v1/contract_sub_position_info

### 4.查询用户财务记录

URL：api/v1/contract_financial_record

## 1.0.3 2019年5月28日【更新：WS增加资产信息推送】

WS增加资产信息推送

WS增加持仓信息推送

rest接口获取用户的持仓信息接口api/v1/contract_position_info增加返回字段“最新价”

## 1.0.2 2019年5月14日【更新: 币币账户和合约账户间进行资金的划转】

### 新增账户接口/v1/futures/transfer

币币账户和合约账户间进行资金的划转

从现货现货账户转至合约账户，类型为pro-to-futures; 从合约账户转至现货账户，类型为futures-to-pro

该接口的访问频次的限制为1分钟10次

### API限频

限频时间间隔从1秒变为3秒

私有接口限频由原来的10次/s变更为30次/3s，即请求发送3秒内不超过30次

其他非行情类的公开接口限频由原来的20次/s变更为60次/3s，即请求发送3秒内不超过60次

## 1.0.1 2019年5月9日【更新：post_only高级限价委托功能上线】

### 全部撤单接口/v1/contract_cancelall

只传symbol，撤销该品种下所有周期的合约

只要有contract_code，则撤销该code的合约

只传symbol+contract_type， 则撤销二者拼接所成的合约订单

### 下单接口/v1/ contract_order

报单字段order_price_type中增加订单价格类型post_only，post_only是“只做Maker（post_only）”，不会立刻在市场成交，保证用户始终为Maker；如果委托会立即与已有委托成交，那么该委托会被取消。

Post only只受用户持仓数量限制，单笔下单不受下单数量限制。

### 批量下单接口/v1/ contract_batchorder

报单字段order_price_type中增加订单价格类型post_only，post_only是“只做Maker（post_only）”，不会立刻在市场成交，保证用户始终为Maker；如果委托会立即与已有委托成交，那么该委托会被取消。

Post only只受用户持仓数量限制，单笔下单不受下单数量限制。

### 所有API接口返回数据中增加限频信息

将在api接口response中的header返回以下字段

ratelimit-limit： 单轮请求数上限，单位：次数

ratelimit-interval：请求数重置的时间间隔，单位：毫秒

ratelimit-remaining：本轮剩余可用请求数，单位：次数

ratelimit-reset：请求数上限重置时间，单位：毫秒

### 查询订单详细信息/v1/contract_order_detail

trades增加成交角色字段role：taker或maker

获取成交记录/v1/contract_matchresults

trades增加成交角色字段role：taker或maker

获取该用户在某品种上的最新成交记录，可以按照交易类型进行过滤筛选。注意，该接口是需要API KEY验签的私有接口，只能查询属于该用户自己的最新成交记录。

### WS成交推送接口

trades增加成交角色字段role：taker或maker

WebSocket私有订单成交推送接口(需要API KEY验签)

一个UID最多同时建立30个私有订单成交推送WS链接。该用户在一个品种(包含该品种的所有周期的合约)上，仅需要维持一个订单推送WS链接即可。

注意: 订单推送WS的限频，跟用户RESTFUL私有接口的限频是分开的，相互不影响。

## 1.0.0 于2018年12月10日上线

# 合约交易接入说明

## 合约交易接口列表

### 接口列表

权限类型 | 接口数据类型 | 请求方法 | 类型 | 描述 | 需要验签  
---|---|---|---|---|---  
读取 | 基础信息接口 | /api/v1/contract_contract_info | GET | 获取合约信息 | 否  
读取 | 基础信息接口 | /api/v1/contract_index | GET | 获取合约指数信息 | 否  
读取 | 基础信息接口 | /api/v1/contract_price_limit | GET | 获取合约最高限价和最低限价 | 否  
读取 | 基础信息接口 | /api/v1/contract_open_interest | GET | 获取当前可用合约总持仓量 | 否  
读取 | 基础信息接口 | /api/v1/contract_delivery_price | GET | 获取预估交割价 | 否  
读取 | 基础信息接口 | /api/v1/contract_api_state | GET | 查询系统状态 | 否  
读取 | 市场行情接口 | /market/depth | GET | 获取行情深度数据 | 否  
读取 | 市场行情接口 | /market/history/kline | GET | 获取K线数据 | 否  
读取 | 市场行情接口 | /market/detail/merged | GET | 获取聚合行情 | 否  
读取 | 市场行情接口 | /market/trade | GET | 获取市场最近成交记录 | 否  
读取 | 市场行情接口 | /market/history/trade | GET | 批量获取最近的交易记录 | 否  
读取 | 市场行情接口 | /api/v1/contract_risk_info | GET | 查询合约风险准备金余额和预估分摊比例 | 否  
读取 | 市场行情接口 | /api/v1/contract_insurance_fund | GET | 查询合约风险准备金余额历史数据 | 否  
读取 | 市场行情接口 | /api/v1/contract_adjustfactor | GET | 查询平台阶梯调整系数 | 否  
读取 | 市场行情接口 | /api/v1/contract_his_open_interest | GET | 平台持仓量的查询 | 否  
读取 | 市场行情接口 | /api/v1/contract_elite_account_ratio | GET | 精英账户多空持仓对比-账户数 | 否  
读取 | 市场行情接口 | /api/v1/contract_elite_position_ratio | GET | 精英账户多空持仓对比-持仓量 | 否  
读取 | 市场行情接口 | /api/v1/contract_liquidation_orders | GET | 获取强平订单 | 否  
读取 | 市场行情接口 | /api/v1/contract_settlement_records | GET | 查询平台历史结算记录 | 否  
读取 | 市场行情接口 | /index/market/history/index | GET | 获取指数K线数据 | 否  
读取 | 市场行情接口 | /index/market/history/basis | GET | 获取基差数据 | 否  
读取 | 资产接口 | /api/v1/contract_account_info | POST | 获取用户账户信息 | 是  
读取 | 资产接口 | /api/v1/contract_position_info | POST | 获取用户持仓信息 | 是  
读取 | 账户接口 | /api/v1/contract_sub_account_list | POST | 币查询母账户下所有子账户资产信息 | 是  
读取 | 账户接口 | /api/v1/contract_sub_account_info | POST | 查询单个子账户资产信息 | 是  
读取 | 账户接口 | /api/v1/contract_sub_position_info | POST | 查询单个子账户持仓信息的 | 是  
读取 | 账户接口 | /api/v1/contract_financial_record | POST | 查询用户财务记录 | 是  
读取 | 账户接口 | /api/v1/contract_financial_record_exact | POST | 组合查询财务记录 | 是  
读取 | 账户接口 | /api/v1/contract_user_settlement_records | POST | 查询用户结算记录 | 是  
读取 | 账户接口 | /api/v1/contract_order_limit | POST | 查询用户当前的下单量限制 | 是  
读取 | 账户接口 | /api/v1/contract_fee | POST | 查询用户当前的手续费费率 | 是  
读取 | 账户接口 | /api/v1/contract_transfer_limit | POST | 查询用户当前的划转限制 | 是  
读取 | 账户接口 | /api/v1/contract_position_limit | POST | 用户持仓量限制的查询 | 是  
读取 | 账户接口 | /api/v1/contract_account_position_info | POST | 查询用户账户和持仓信息 | 是  
交易 | 账户接口 | /api/v1/contract_master_sub_transfer | POST | 母子账户划转 | 是  
读取 | 账户接口 | /api/v1/contract_master_sub_transfer_record | POST |
获取母账户下的所有母子账户划转记录 | 是  
交易 | 交易接口 | /api/v1/contract_order | POST | 合约下单 | 是  
交易 | 交易接口 | /api/v1/contract_batchorder | POST | 合约批量下单 | 是  
交易 | 交易接口 | /api/v1/contract_cancel | POST | 撤销订单 | 是  
交易 | 交易接口 | /api/v1/contract_cancelall | POST | 全部撤单 | 是  
交易 | 交易接口 | /api/v1/contract_switch_lever_rate | POST | 切换杠杆 | 是  
读取 | 交易接口 | /api/v1/contract_order_info | POST | 获取合约订单信息 | 是  
读取 | 交易接口 | /api/v1/contract_order_detail | POST | 获取订单明细信息 | 是  
读取 | 交易接口 | /api/v1/contract_openorders | POST | 获取合约当前未成交委托 | 是  
读取 | 交易接口 | /api/v1/contract_hisorders | POST | 获取合约历史委托 | 是  
读取 | 交易接口 | /api/v1/contract_hisorders_exact | POST | 组合查询合约历史委托 | 是  
读取 | 交易接口 | /api/v1/contract_matchresults | POST | 获取历史成交记录 | 是  
读取 | 交易接口 | /api/v1/contract_matchresults_exact | POST | 组合查询合约历史成交记录 | 是  
读取 | 账户接口 | /api/v1/contract_trigger_openorders | POST | 获取计划委托当前委托接口 | 是  
读取 | 账户接口 | /api/v1/contract_trigger_hisorders | POST | 获取计划委托历史委托接口 | 是  
交易 | 账户接口 | /v1/futures/transfer | POST | 币币账户和合约账户间进行资金的划转 | 是  
交易 | 交易接口 | /api/v1/lightning_close_position | POST | 闪电平仓下单 | 是  
交易 | 交易接口 | /api/v1/contract_trigger_order | POST | 合约计划委托下单 | 是  
交易 | 交易接口 | /api/v1/contract_trigger_cancel | POST | 合约计划委托撤单 | 是  
交易 | 交易接口 | /api/v1/contract_trigger_cancelall | POST | 合约计划委托全部撤单 | 是  
  
## 访问地址

访问地址 | 适用站点 | 适用功能 | 适用交易对  
---|---|---|---  
https://api.hbdm.com | 火币合约 | 行情 | 火币合约的交易品种  
  
### 备注

如果api.hbdm.com无法访问，可以使用api.btcgateway.pro来做调试，AWS服务器用户推荐使用api.hbdm.vn；

## 签名认证

### 签名说明

API 请求在通过 internet 传输的过程中极有可能被篡改，为了确保请求未被更改，除公共接口（基础信息，行情数据）外的私有接口均必须使用您的 API
Key 做签名认证，以校验参数或参数值在传输途中是否发生了更改。

一个合法的请求由以下几部分组成：

  * 方法请求地址：即访问服务器地址 api.hbdm.com，比如 api.hbdm.com/api/v1/contract_order。

  * API 访问密钥（AccessKeyId）：您申请的 API Key 中的 Access Key。

  * 签名方法（SignatureMethod）：用户计算签名的基于哈希的协议，此处使用 HmacSHA256。

  * 签名版本（SignatureVersion）：签名协议的版本，此处使用2。

  * 时间戳（Timestamp）：您发出请求的时间 (UTC 时区) (UTC 时区) (UTC 时区) 。如：2017-05-11T16:22:06。在查询请求中包含此值有助于防止第三方截取您的请求。

  * 必选和可选参数：每个方法都有一组用于定义 API 调用的必需参数和可选参数。可以在每个方法的说明中查看这些参数及其含义。 请一定注意：对于 GET 请求，每个方法自带的参数都需要进行签名运算； 对于 POST 请求，每个方法自带的参数不进行签名认证，即 POST 请求中需要进行签名运算的只有 AccessKeyId、SignatureMethod、SignatureVersion、Timestamp 四个参数，其它参数放在 body 中。

  * 签名：签名计算得出的值，用于确保签名有效和未被篡改。

### 创建 API Key

您可以在 [这里 ](https://www.hbg.com/zh-cn/apikey/) 创建 API Key。

API Key 包括以下两部分

  * `Access Key` API 访问密钥

  * `Secret Key` 签名认证加密所使用的密钥（仅申请时可见）

创建 API Key 时可以选择绑定 IP 地址，未绑定 IP 地址的 API Key 有效期为90天。  API Key
具有包括交易、借贷和充提币等所有操作权限。  这两个密钥与账号安全紧密相关，无论何时都请勿向其它人透露。

### 签名步骤

规范要计算签名的请求 因为使用 HMAC
进行签名计算时，使用不同内容计算得到的结果会完全不同。所以在进行签名计算前，请先对请求进行规范化处理。下面以查询某订单详情请求为例进行说明：

查询某订单详情

`https://api.hbdm.com/api/v1/contract_order?`

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx`

`&SignatureMethod=HmacSHA256`

`&SignatureVersion=2`

`&Timestamp=2017-05-11T15:19:30`

#### 1\. 请求方法（GET 或 POST），后面添加换行符 “\n”

`GET\n`

#### 2\. 添加小写的访问地址，后面添加换行符 “\n”

` api.hbdm.com\n `

#### 3\. 访问方法的路径，后面添加换行符 “\n”

` /api/v1/contract_order\n `

#### 4\. 按照ASCII码的顺序对参数名进行排序。例如，下面是请求参数的原始顺序，进行过编码后

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx`

`SignatureMethod=HmacSHA256`

`SignatureVersion=2`

`Timestamp=2017-05-11T15%3A19%3A30`

使用 UTF-8 编码，且进行了 URI 编码，十六进制字符必须大写，如 “:” 会被编码为 “%3A” ，空格被编码为 “%20”。
时间戳（Timestamp）需要以YYYY-MM-DDThh:mm:ss格式添加并且进行 URI 编码。

#### 5\. 经过排序之后

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx`

`SignatureMethod=HmacSHA256`

`SignatureVersion=2`

`Timestamp=2017-05-11T15%3A19%3A30`

#### 6\. 按照以上顺序，将各参数使用字符 “&” 连接

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx&SignatureMethod=HmacSHA256&SignatureVersion=2&Timestamp=2017-05-11T15%3A19%3A30`

#### 7\. 组成最终的要进行签名计算的字符串如下

`POST\n`

`api.hbdm.com\n`

`/api/v1/contract_order\n`

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx&SignatureMethod=HmacSHA256&SignatureVersion=2&Timestamp=2017-05-11T15%3A19%3A30`

#### 8\. 用上一步里生成的 “请求字符串” 和你的密钥 (Secret Key) 生成一个数字签名

`4F65x5A2bLyMWVQj3Aqp+B4w+ivaA7n5Oi2SuYtCJ9o=`

  1. 将上一步得到的请求字符串和 API 私钥作为两个参数，调用HmacSHA256哈希函数来获得哈希值。

  2. 将此哈希值用base-64编码，得到的值作为此次接口调用的数字签名。

#### 9\. 将生成的数字签名加入到请求的路径参数里

最终，发送到服务器的 API 请求应该为

`https://api.hbdm.com/api/v1/contract_order?AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx&SignatureMethod=HmacSHA256&SignatureVersion=2&Timestamp=2017-05-11T15%3A19%3A30&Signature=4F65x5A2bLyMWVQj3Aqp%2BB4w%2BivaA7n5Oi2SuYtCJ9o%3D`

  1. 把所有必须的认证参数添加到接口调用的路径参数里

  2. 把数字签名在URL编码后加入到路径参数里，参数名为“Signature”。

## 访问次数限制

  * 交割合约、币本位永续合约、期权合约和USDT本位永续合约都分开限频

  * 公开行情接口和用户私有接口都有访问次数限制

  * 普通用户，需要密钥的私有接口，每个UID 3秒最多 72 次请求(交易接口3秒最多 36 次请求，查询接口3秒最多 36 次请求) (该UID的所有币种和不同到期日的合约的所有私有接口共享该限制) [查看API接口类型列表(其中读取即查询,交易即交易)](https://docs.huobigroup.com/docs/dm/v1/cn/#ab0b26742c)

  * 其他非行情类的公开接口，比如获取指数信息，限价信息，交割结算、平台持仓信息等，所有用户都是每个IP3秒最多120次请求（所有该IP的非行情类的公开接口请求共享3秒120次的额度）

  * 行情类的公开接口，比如：获取K线数据、获取聚合行情、市场行情、获取行情深度数据、获取指数k线、获取基差数、获取市场最近成交记录：

（1） restful接口：同一个IP, 所有业务（交割合约、币本位永续合约、期权合约和USDT本位永续合约）总共1秒最多800个请求

（2） websocket：req请求，同一时刻最多请求50次；sub请求，无限制，服务器主动推送数据

  * WebSocket私有订单成交推送接口(需要API KEY验签)

一个UID最多同时建立30个私有订单成交推送WS链接。该用户在一个品种(包含该品种的所有周期的合约)上，仅需要维持一个订单推送WS链接即可。

注意: 订单推送WS的限频，跟用户RESTFUL私有接口的限频是分开的，相互不影响。

  * 查询与交易API接口返回的header中会有限频信息。比如：查询订单信息接口(/api/v1/contract_order_info)，返回的header中的ratelimit-limit即查询接口的总限制频率次数，ratelimit-remaining即查询接口的剩余总限制频率次数。下单接口(/api/v1/contract_order)，返回的header中的ratelimit-limit即交易接口的总限制频率次数，ratelimit-remaining即交易接口的剩余总限制频率次数。[查看API接口类型列表(其中读取即查询,交易即交易)](https://docs.huobigroup.com/docs/dm/v1/cn/#ab0b26742c)

将在api接口response中的header返回以下字段：

ratelimit-limit： 单轮请求数上限，单位：次数

ratelimit-interval：请求数重置的时间间隔，单位：毫秒

ratelimit-remaining：本轮剩余可用请求数，单位：次数

ratelimit-reset：请求数上限重置时间，单位：毫秒

如果触发了撤单率限制，您的api接口response返回header中会包括字段：

recovery-time：禁用的恢复时间戳，单位为毫秒，表示禁用结束时间，可恢复访问的时间戳；

如果不在禁用期间，header不返回recovery-time字段；

  * 一个uid对应计划委托下单接口请求1秒5次、一个uid对应计划委托撤单接口请求1秒5次、一个uid对应计划委托全部撤单接口请求1秒5次。

## 撤单率限制

  * 当用户通过API在10分钟内特定订单价格类型的委托单总笔数大于或等于3000笔时，系统会自动计算撤单率，如果撤单率大于99%，则禁止该用户通过API特定价格类型进行下单5分钟（如果下单会报：1084 您的合约API挂单接口被禁用,请于{0} (GMT+8) 后再试）；

  * 当API用户在1小时的总禁用次数达到3次时，则禁止用户通过API特定价格类型进行下单30分钟（如果下单会报：1084 您的合约API挂单接口被禁用,请于{0} (GMT+8) 后再试），待解禁恢复访问后，总禁用次数重置，且之前周期统计过的次数不计入新周期的总禁用次数;

  * 其他客户端挂撤单以及API撤单将不受影响，每次禁用会以短信和邮件形式通知；

  * 被禁用的API下单类型仅包括：限价委托、Post_only、FOK、IOC四种订单价格类型，其他下单方式如lightning（闪电平仓下单），opponent(对手价下单)，optimal_5（最优5档），optimal_10(最优10档下单），optimal_20（最优20档下单），opponent_ioc（对手价-IOC下单），lightning_ioc（闪电平仓-IOC下单），optimal_5_ioc（最优5档-IOC下单），optimal_10_ioc（最优10档-IOC下单），optimal_20_ioc（最优20档-IOC下单），opponent_fok（对手价-FOK下单），lightning_fok（闪电平仓-FOK下单），optimal_5_fok（最优5档-FOK下单），optimal_10_fok（最优10档-FOK下单），optimal_20_fok（最优20档-FOK下单）等在禁用期间将仍然可用；

  * HTTP返回的header信息：

    * 禁用期间下单类型为被禁用的四种类型时,接口返回信息header中会包括字段："recovery-time：禁用的恢复时间戳"，单位为毫秒，表示禁用结束时间，可恢复访问的时间戳；
    * 如果不在禁用期间，header中不返回该字段；
  * 委托单总笔数与撤单率的计算是基于UID，母子UID是分开单独计算的。计算撤单率的时间周期为10分钟/次（开始时间从00:00开始,结束时间00:10。每10分钟一个周期。）；

  * 指标说明：

    * 撤单率 = 无效撤单总笔数 / 委托单总笔数（订单来源均为API）。
    * 委托单总笔数=同时满足以下所有条件的委托单总笔数： 
      * 订单来源为API并且订单类型为报单（order Type = 1）；
      * 订单价格类型为限价委托、Post_only、FOK和IOC四种订单价格类型；
      * 委托单的下单时间在【当周期开始时间-3秒，当周期结束时间】内的委托单总笔数；
    * 无效撤单总笔数=同时满足以下所有条件的委托单总笔数： 
      * 订单来源为API并且订单类型为报单（order Type = 1）；
      * 订单价格类型为限价委托、Post_only、FOK和IOC四种订单价格类型；
      * 订单状态为已撤销（status = 7）；
      * 订单成交数量为0；
      * 撤单时间与下单时间间隔小于等于3秒；
      * 委托单的撤单时间在当周期内的委托单。
  * 为了保证API系统的稳定性和交易性能，请您在高峰期时段尽量降低API订单的撤单量和撤单率，以避免频繁触发API的限制机制，以下是降低撤单率的建议：

    * 1．订单的价格更靠近盘口；
    * 2、适当延长下单与撤单的时间间隔；
    * 3、适当增加单笔订单金额，减少下单次数；
    * 4、尽量增加订单成交率: 
      * 1) 优先使用对手价、最优5档、最优10档、最优20档、闪电平仓、opponent_ioc（对手价-IOC下单）、lightning_ioc（闪电平仓-IOC下单）、optimal_5_ioc（最优5档-IOC下单）、optimal_10_ioc（最优10档-IOC下单）、optimal_20_ioc（最优20档-IOC下单）、opponent_fok（对手价-FOK下单）、lightning_fok（闪电平仓-FOK下单）、optimal_5_fok（最优5档-FOK下单）、optimal_10_fok（最优10档-FOK下单）、optimal_20_fok（最优20档-FOK下单）等成交概率大的委托方式下单；
      * 2) IOC订单、FOK订单、Post_only订单尽量摆在买卖第一档的位置上；
    * 5、适当延长策略轮询时间。

## 停服维护

当该业务系统停服维护期间，除了以下2个提供给用户查询系统状态的接口能够正常使用外（[获取当前系统状态](https://docs.huobigroup.com/docs/dm/v1/cn/#cd63bde415)、[查询系统是否可用](https://docs.huobigroup.com/docs/dm/v1/cn/#bef5ec9210)），该业务所有rest接口都会固定返回响应报文:`{"status":
"maintain"}`。websocket推送接口在停服维护时，除了WebSocket系统状态更新的推送接口可以正常调用外（[WebSocket系统状态更新接口](https://docs.huobigroup.com/docs/dm/v1/cn/#websocket-6)），其他推送接口都会返回1006的错误码。

> Response
    
    
    {
        "status": "maintain"
    }
    

#### 2个接口为：

  * 查询系统是否可用：https://api.hbdm.com/heartbeat/
  * statuspage查询系统状态：https://status-dm.huobigroup.com/api/v2/summary.json

除了以上两个rest接口获取系统维护停服信息外，也可以通过订阅WebSocket系统状态更新接口获取系统维护停服信息

## 获取当前系统状态

此接口返回当前的系统状态，包含当前系统维护计划和故障进度等。

如您需要通过邮件、短信、Webhook、RSS/Atom feed接收以上信息，可点击[这里](https://status-
dm.huobigroup.com/)进入页面进行订阅。当前订阅依赖Google服务，订阅前请确保您可正常访问Google的服务，否则将订阅失败。

    
    
    curl "https://status-dm.huobigroup.com/api/v2/summary.json"
    

### HTTP 请求

  * GET `https://status-dm.huobigroup.com/api/v2/summary.json`

### 请求参数

此接口不接受任何参数。

> Response:
    
    
    {
      "page": {  // 合约页面基本信息
        "id": "p0qjfl24znv5",  // 页面id
        "name": "Huobi",  // 页面名称
        "url": "https://status-dm.huobigroup.com", // 页面地址
        "time_zone": "Etc/UTC", // 时区
        "updated_at": "2020-02-07T10:25:14.717Z" // 页面最新一次更新时间
      },
      "components": [  // 系统组件及状态
        {
          "id": "h028tnzw1n5l",  // 组件id
          "name": "Deposit", // 组件名称
          "status": "operational", // 组件状态
          "created_at": "2019-12-05T02:07:12.372Z",  // 组件创建时间
          "updated_at": "2020-02-07T09:27:15.563Z", // 组件更新时间
          "position": 1,
          "description": null,
          "showcase": true,
          "group_id": "gtd0nyr3pf0k",  
          "page_id": "p0qjfl24znv5", 
          "group": false,
          "only_show_if_degraded": false
        }
      ],
      "incidents": [ // 系统故障事件及状态
            {
                "id": "rclfxz2g21ly",  // 事件id
                "name": "Market data is delayed",  // 事件名称
                "status": "investigating",  // 事件状态
                "created_at": "2020-02-11T03:15:01.913Z",  // 事件创建时间
                "updated_at": "2020-02-11T03:15:02.003Z",   // 事件更新时间
                "monitoring_at": null,
                "resolved_at": null,
                "impact": "minor",  // 事件影响程度
                "shortlink": "http://stspg.io/pkvbwp8jppf9",
                "started_at": "2020-02-11T03:15:01.906Z",
                "page_id": "p0qjfl24znv5",
                "incident_updates": [ 
                    {
                        "id": "dwfsk5ttyvtb",  
                        "status": "investigating",  
                        "body": "Market data is delayed",  
                        "incident_id": "rclfxz2g21ly",   
                        "created_at": "2020-02-11T03:15:02.000Z",    
                        "updated_at": "2020-02-11T03:15:02.000Z",   
                        "display_at": "2020-02-11T03:15:02.000Z",    
                        "affected_components": [  
                            {
                                "code": "nctwm9tghxh6",  
                                "name": "Market data",  
                                "old_status": "operational",  
                                "new_status": "degraded_performance"   
                            }
                        ],
                        "deliver_notifications": true,
                        "custom_tweet": null,
                        "tweet_id": null
                    }
                ],
                "components": [  
                    {
                        "id": "nctwm9tghxh6",    
                        "name": "Market data", 
                        "status": "degraded_performance", 
                        "created_at": "2020-01-13T09:34:48.284Z", 
                        "updated_at": "2020-02-11T03:15:01.951Z", 
                        "position": 8,
                        "description": null,
                        "showcase": false,
                        "group_id": null,
                        "page_id": "p0qjfl24znv5",
                        "group": false,
                        "only_show_if_degraded": false                }
                ]
            }
        ],
          "scheduled_maintenances": [  // 系统计划维护事件及状态
            {
                "id": "k7g299zl765l", // 事件id
                "name": "Schedule maintenance", // 事件名称
                "status": "scheduled", // 事件状态
                "created_at": "2020-02-11T03:16:31.481Z",  // 事件创建时间
                "updated_at": "2020-02-11T03:16:31.530Z",  // 事件更新时间
                "monitoring_at": null,
                "resolved_at": null,
                "impact": "maintenance", // 事件影响
                "shortlink": "http://stspg.io/md4t4ym7nytd",
                "started_at": "2020-02-11T03:16:31.474Z",
                "page_id": "p0qjfl24znv5",
                "incident_updates": [  
                    {
                        "id": "8whgr3rlbld8",  
                        "status": "scheduled", 
                        "body": "We will be undergoing scheduled maintenance during this time.", 
                        "incident_id": "k7g299zl765l", 
                        "created_at": "2020-02-11T03:16:31.527Z",  
                        "updated_at": "2020-02-11T03:16:31.527Z",  
                        "display_at": "2020-02-11T03:16:31.527Z",  
                        "affected_components": [  
                            {
                                "code": "h028tnzw1n5l",  
                                "name": "Deposit And Withdraw - Deposit",  
                                "old_status": "operational",  
                                "new_status": "operational"  
                            }
                        ],
                        "deliver_notifications": true,
                        "custom_tweet": null,
                        "tweet_id": null
                    }
                ],
                "components": [ 
                    {
                        "id": "h028tnzw1n5l",  
                        "name": "Deposit", 
                        "status": "operational", 
                        "created_at": "2019-12-05T02:07:12.372Z",  
                        "updated_at": "2020-02-10T12:34:52.970Z",  
                        "position": 1,
                        "description": null,
                        "showcase": false,
                        "group_id": "gtd0nyr3pf0k",
                        "page_id": "p0qjfl24znv5",
                        "group": false,
                        "only_show_if_degraded": false
                    }
                ],
                "scheduled_for": "2020-02-15T00:00:00.000Z",  // 计划维护开始时间
                "scheduled_until": "2020-02-15T01:00:00.000Z"  // 计划维护结束时间
            }
        ],
        "status": {  // 系统整体状态
            "indicator": "minor",   // 系统状态指标
            "description": "Partially Degraded Service"  // 系统状态描述
        }
    }
    

### 返回字段

字段名称 | 数据类型 | 描述  
---|---|---  
page |  | status page页面基本信息  
{id | string | 页面id  
name | string | 页面名称  
url | string | 页面地址  
time_zone | string | 时区  
updated_at} | string | 页面更新时间  
components |  | 系统组件及状态  
[{id | string | 组件id  
name | string | 组件名称，如Order submission、Order cancellation、Deposit等  
status | string |
组件状态，取值范围为：operational，degraded_performance，partial_outage，major_outage，under
maintenance  
created_at | string | 组件创建时间  
updated_at | string | 组件更新时间  
.......}] |  | 其他字段明细，请参考返回示例  
incidents |  | 系统故障事件及状态，若当前无故障则返回为空  
[{id | string | 事件id  
name | string | 事件名称  
status | string | 事件状态，取值范围为：investigating，identified，monitoring，resolved  
created_at | string | 事件创建时间  
updated_at | string | 事件更新时间  
.......}] |  | 其他字段明细，请参考返回示例  
scheduled_maintenances |  | 系统计划维护事件及状态，若当前无计划维护则返回为空  
[{id | string | 事件id  
name | string | 事件名称  
status | string | 事件状态，取值范围为：scheduled，in progress，verifying，completed  
created_at | string | 事件创建时间  
updated_at | string | 事件更新时间  
scheduled_for | string | 计划维护开始时间  
scheduled_until | string | 计划维护结束时间  
.......}] |  | 其他字段明细，请参考返回示例  
status |  | 系统整体状态  
{indicator | string | 系统状态指标，取值范围为：none，minor，major，critical，maintenance  
description} | string | 系统状态描述，取值范围为：All Systems Operational，Minor Service
Outager，Partial System Outage，Partially Degraded Service，Service Under
Maintenance  
  
## 查询系统是否可用

  * Interface `https://api.hbdm.com/heartbeat/`

### 备注：

  * 注意请求时地址后面的“/”一定要带上。

### 返回参数

参数名称 | 类型 | 描述  
---|---|---  
status | string | "ok" 或 "error"...  
<data> | dict object |  
heartbeat | int | 交割合约 1: 可用 0: 不可用(即停服维护)  
swap_heartbeat | int | 币本位永续 1: 可用 0: 不可用(即停服维护)  
estimated_recovery_time | long | null: 正常. 交割合约预计恢复时间， 单位:毫秒  
swap_estimated_recovery_time | long | null: 正常. 币本位永续合约预计恢复时间，单位：毫秒.  
option_heartbeat | int | 期权合约 1: 可用 0: 不可用(即停服维护)  
option_estimated_recovery_time | long | null: 正常. 期权合约预计恢复时间，单位：毫秒.  
linear_swap_heartbeat | long | USDT本位永续 1: 可用 0: 不可用(即停服维护)  
linear_swap_estimated_recovery_time | long | null: 正常. USDT本位永续合约预计恢复时间，单位：毫秒.  
</data> |  |  
  
> 返回数据
    
    
    {
        "status":"ok",
        "data":{
            "heartbeat":1,
            "estimated_recovery_time":null,
            "swap_heartbeat":1,
            "swap_estimated_recovery_time":null,
            "option_heartbeat":1,
            "option_estimated_recovery_time":null,
            "linear_swap_heartbeat":1,
            "linear_swap_estimated_recovery_time":null
        },
        "ts":1557714418033
    }
    

## 获取当前系统时间戳

get `https://api.hbdm.com/api/v1/timestamp`

### 请求参数

无

> 返回数据
    
    
    {
        "status": "ok",
        "ts": 1578124684692
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 |  
ts | true | long | 当前系统时间戳 |  
  
#### 备注

  * 可以用于校对系统时间。

## 错误码详情

错误代码 | 错误描述  
---|---  
403 | 无效身份  
1000 | 系统异常  
1001 | 系统未准备就绪  
1002 | 查询异常  
1003 | 操作redis异常  
1004 | 系统繁忙,请稍后再试  
1010 | 用户不存在  
1011 | 用户会话不存在,请重试  
1012 | 账户不存在  
1013 | 合约品种不存在  
1014 | 合约不存在  
1015 | 指数价格不存在  
1016 | 对手价不存在  
1017 | 查询订单不存在  
1018 | 主账号不存在  
1019 | 主账号不在开通子账号白名单里  
1020 | 您的子账号数量已超出限制,请联系客服  
1021 | 开户失败。您的主账号尚未开通合约交易权限,请前往开通  
1030 | 输入错误  
1031 | 非法的请求来源  
1032 | 访问次数超出限制  
1033 | 合约周期字段值错误  
1034 | 报单价格类型字段值错误  
1035 | 报单方向字段值错误  
1036 | 报单开平字段值错误  
1037 | 倍数不符合要求,请联系客服  
1038 | 下单价格超出精度限制,请修改后下单  
1039 | 买入价必须低于{0}{1},卖出价必须高于{2}{3}  
1040 | 下单数量不能为空或者不能小于0, 请修改后下单  
1041 | 下单数量超出限制 ({0}张),请修改后下单  
1042 | 下单数量+挂单数量+持仓数量超过了单用户多仓持仓限制({0}张),请修改后下单  
1043 | 下单数量+挂单数量+持仓数量超过了单用户空仓持仓限制({0}张), 请修改后下单  
1044 | 触发平台限仓,请修改后下单  
1045 | 当前有挂单,无法切换倍数  
1046 | 当前合约持仓不存在  
1047 | 可用担保资产不足  
1048 | 可平量不足  
1049 | 暂不支持市价开仓  
1050 | 客户报单号重复  
1051 | 没有可撤销的订单  
1052 | 批量撤单、下单的订单数量超过平台限制数量  
1053 | 无法获取最新价格区间  
1054 | 无法获取最新价  
1055 | 价格不合理, 下单后将导致账户权益小于0 , 请修改价格后下单  
1056 | 结算中,暂时无法下单/撤单  
1057 | 暂停交易中,暂时无法下单  
1058 | 停牌中,暂时无法下单  
1059 | 交割中,暂时无法下单/撤单  
1060 | 合约处于非交易状态,暂时无法下单  
1061 | 订单不存在  
1062 | 撤单中,请耐心等待  
1063 | 订单已成交  
1064 | 报单主键冲突  
1065 | 客户报单号不是整数  
1066 | {0}字段不能为空  
1067 | {0}字段不合法  
1068 | 导出错误  
1069 | 价格不合理  
1070 | 数据为空,无法导出  
1071 | 订单已撤,无法撤单  
1072 | 卖出价必须低于{0}{1}  
1073 | 仓位异常,请联系客服  
1074 | 下单异常,请联系客服  
1075 | 价格不合理, 下单后将导致担保资产率小于0 , 请修改价格后下单  
1076 | 盘口无数据,请稍后再试  
1077 | 交割结算中,当前品种资金查询失败  
1078 | 交割结算中,部分品种资金查询失败  
1079 | 交割结算中,当前品种持仓查询失败  
1080 | 交割结算中,部分品种持仓查询失败  
1081 | {0}合约计划委托订单数量不得超过{1}  
1082 | 触发类型参数错误  
1083 | 您的仓位已进入强平接管,暂时无法下单  
1084 | 您的合约API挂单接口被禁用,请于{0} (GMT+8) 后再试  
1085 | 计划委托下单失败,请修改价格再次下单或联系客服  
1086 | {0}合约暂时限制{1}端开仓,请联系客服  
1087 | {0}合约暂时限制{1}端平仓,请联系客服  
1088 | {0}合约暂时限制{1}端撤单,请联系客服  
1089 | {0}账户暂时限制划转,请联系客服  
1090 | 担保资产率小于0, 无法下单  
1091 | 账户权益小于0, 无法下单  
1092 | 闪电平仓取盘口第{0}档的价格, 下单后将导致账户权益小于0 , 请改为手动输入价格或使用对手价下单  
1093 | 闪电平仓取盘口第{0}档的价格, 下单后将导致担保资产率小于0 , 请改为手动输入价格或使用对手价下单  
1094 | 倍数不能为空, 请切换倍数或联系客服  
1095 | 合约处于非交易状态, 暂时无法切换倍数  
1100 | 您没有开仓权限,请联系客服  
1101 | 您没有平仓权限,请联系客服  
1102 | 您没有转入权限,请联系客服  
1103 | 您没有转出权限,请联系客服  
1104 | 合约交易受限,当前禁止交易  
1105 | 合约交易受限,当前只能平仓  
1106 | 合约交割结算中,暂时无法划转  
1108 | Dubbo调用异常  
1109 | 子账号没有开仓权限,请联系客服  
1110 | 子账号没有平仓权限,请联系客服  
1111 | 子账号没有入金权限,请联系客服  
1112 | 子账号没有出金权限,请联系客服  
1113 | 子账号没有交易权限,请登录主账号授权  
1114 | 子账号没有划转权限,请登录主账号授权  
1115 | 您没有访问此子账号的权限  
1200 | 登录失败,请重试  
1220 | 您尚未开通合约交易,无访问权限  
1221 | 币币账户总资产不满足合约开通条件  
1222 | 开户天数不满足合约开通条件  
1223 | VIP等级不满足合约开通条件  
1224 | 您所在的国家/地区不满足合约开通条件  
1225 | 开通合约失败  
1226 | 合约已开户,无法重复开户  
1227 | 火币合约暂不支持子账户,请返回退出子账户,切换主账户登录  
1228 | 您尚未开通合约交易, 请先开通  
1229 | 重复同意协议  
1230 | 您尚未做风险认证  
1231 | 您尚未做身份认证  
1232 | 您上传的图片格式/大小不符合要求,请重新上传  
1233 | 您尚未开通高倍数协议 (使用高倍数请先使用主账号登录web或APP端同意高倍数协议)  
1234 | {0}合约开仓委托订单数量不得超过{1}  
1235 | {0}合约平仓委托订单数量不得超过{1}  
1250 | 无法获取HT_token  
1251 | 无法获取BTC净资产,请稍后再试  
1252 | 无法获取币币账户资产,请稍后再试  
1253 | 签名验证错误  
1254 | 子账号无权限开通合约，请前往web端登录主账号开通  
1300 | 划转失败  
1301 | 可划转余额不足  
1302 | 系统划转错误  
1303 | 单笔转出的数量不能低于{0}{1}  
1304 | 单笔转出的数量不能高于{0}{1}  
1305 | 单笔转入的数量不能低于{0}{1}  
1306 | 单笔转入的数量不能高于{0}{1}  
1307 | 您当日累计转出量超过{0}{1}, 暂无法转出  
1308 | 您当日累计转入量超过{0}{1}, 暂无法转入  
1309 | 您当日累计净转出量超过{0}{1}, 暂无法转出  
1310 | 您当日累计净转入量超过{0}{1}, 暂无法转入  
1311 | 超过平台当日累计最大转出量限制, 暂无法转出  
1312 | 超过平台当日累计最大转入量限制, 暂无法转入  
1313 | 超过平台当日累计最大净转出量限制, 暂无法转出  
1314 | 超过平台当日累计最大净转入量限制, 暂无法转入  
1315 | 划转类型错误  
1316 | 划转冻结失败  
1317 | 划转解冻失败  
1318 | 划转确认失败  
1319 | 查询可划转金额失败  
1320 | 此合约在非交易状态中, 无法进行系统划转  
1321 | 划转失败, 请稍后重试或联系客服  
1322 | 划转金额必须大于0  
1323 | 服务异常, 划转失败, 请稍后再试  
1325 | 设置交易单位失败  
1326 | 获取交易单位失败  
1327 | 无划转权限, 划转失败, 请联系客服  
1328 | 无划转权限, 划转失败, 请联系客服  
1329 | 无划转权限, 划转失败, 请联系客服  
1330 | 无划转权限, 划转失败, 请联系客服  
1331 | 超出划转精度限制(8位), 请修改后操作  
1332 | 永续合约不存在  
1333 | 开通跟单吃单协议失败  
1334 | 查询跟单吃单协议失败  
1335 | 查询跟单吃单二次确认设置失败  
1336 | 更新跟单吃单二次确认设置失败  
1337 | 查询跟单吃单设置失败  
1338 | 更新跟单吃单设置失败  
1339 | 昵称含有不合法词汇, 请修改  
1340 | 昵称已被使用, 请修改  
1341 | 报名阶段已结束  
1342 | 子账号无法设置昵称  
1343 | 指标失效, 请重新设置  
1344 | 抱歉, 目前可最多对{0}个合约创建行情提醒  
1345 | 抱歉, {0}合约目前可最多创建{1}个提醒  
1346 | 该指标已存在, 请勿重复设置  
1347 | {0}参数错误, 请修改  
1348 | 该合约不支持全仓模式  
1349 | 委托单倍数与当前持仓的倍数不符, 请先切换倍数  
1401 | 委托价必须小于行权价  
1403 | {0}合约止盈止损订单的委托数量不得超过{1}  
1404 | 止盈止损订单仅支持与开仓订单绑定  
1405 | 止盈价不得{0}{1}{2}  
1406 | 您的抽奖次数已用完  
1407 | 止损价不得{0}{1}{2}  
12001 | 无效的提交时间  
12002 | 错误的签名版本  
12003 | 错误的签名方法  
12004 | 密钥已经过期  
12005 | ip地址错误  
12006 | 提交时间不能为空  
12007 | 公钥错误  
12008 | 校验失败  
12009 | 用户被锁定或不存在  
  
## API 最佳实践

### 1、/api/v1/contract_hisorders 历史委托查询接口：

  * 为了保证时效性和降低延迟，强烈建议用户使用/api/v1/contract_order_info获取用户订单信息接口来查询订单信息，获取合约订单信息接口从内存里面查询，无延迟，接口响应速度更快。

  * 如果用户一定要使用/api/v1/contract_hisorders 历史委托查询接口，请尽量输入更多的查询条件，symbol、trade_type（推荐传0查询全部）、type、status、create_date尽量都输入，并且查询日期create_date参数输入尽量小的整数，最好只查询一天的数据；

### 2、/api/v1/contract_matchresults 获取历史成交记录接口：

  * 为了提升查询的性能和响应速度，查询条件 symbol 、trade_type（推荐传0查询全部） 、contract_code 、create_date 尽量都输入，并且create_date输入尽量小的整数，最好只查询一天的数据；

### 3、/api/v1/contract_financial_record 查询用户财务记录接口：

  * 为了提升查询的性能和响应速度，查询条件symbol、type（推荐不填查询全部）、create_date，尽量都输入，并且查询日期create_date参数输入尽量小的整数，最好只查询一天的数据；

### 4、/api/v1/contract_order_detail 获取订单明细接口：

  * 请求参数没有带上created_at等参数查询订单时，可能会发生查询结果延迟。建议您在使用此接口时请求字段带上：created_at（下单时间戳）和 order_type(订单类型，默认填1)，会直接查询数据库，查询结果会更及时。

  * 查询条件created_at使用13位long类型时间戳（包含毫秒时间），如果输入准确的时间戳，查询性能将会提升。

  * 例如:"2019/10/18 10:26:22"转换为时间戳为：1571365582123。也可以直接从contract_order下单接口返回报文中的ts中获取时间戳作为参数查询接口/api/v1/contract_order_detail获取订单明细，同时created_at禁止传0；；

### 5、/api/v1/contract_trigger_hisorders 获取计划委托历史委托接口：

  * 为了提升查询的性能和响应速度，参数symbol、contract_code、trade_type、status、create_date尽量都输入，并且查询日期create_date参数输入尽量小的整数，最好只查询一天的数据；

### 6、订阅Market Depth 数据的WebSocket：

  * 获得150档深度数据，使用step0, step1, step2, step3, step4, step5,step14,step15；

  * 获得20档深度数据，使用 step6, step7, step8, step9, step10, step11,step12,step13；

  * 由于每100ms推送一次150档全量数据，数据量比较大，如果客户端网络带宽不足或者处理不及时，webSocket断开可能比较频繁，强烈建议使用step6, step7, step8, step9, step10, step11, step12, step13 取20档数据。比如订阅20档数据

`{`

`"sub": "market.BTC_CQ.depth.step6",`

`"id": "id5"`

`}`

  * 我们也推荐使用增量订阅市场深度数据，增量深度数据有20档不合并数据和150档不合并数据，首次或者重连都推送全量数据，之后会推送增量数据，每30MS检查一次，如果有更新则推送，没有更新则不推送。需要维护好本地的深度数据。

`{`

`"sub": "market.BTC_CQ.depth.size_20.high_freq",`

`"data_type":"incremental",`

`"id": "id1"`

`}`

### 7、/api/v1/contract_order合约下单和api/v1/contract_batchorder合约批量下单接口：

  * 推荐传参数client_order_id（用户级别唯一），主要防止下单和批量下单接口由于网络或其它原因接口超时或者没有返回，可以根据client_order_id通过请求接口/api/v1/contract_order_info来快速获取订单是否下单正常或者快速获取订单信息。

## 代码实例

**REST**

  * [Java](https://github.com/huobiapi/Futures-Java-demo)

  * [Python](https://github.com/huobiapi/Futures-Python-demo)

  * [Golang](https://github.com/huobiapi/Futures-Go-demo)

  * [CSharp](https://github.com/huobiapi/Futures-CSharp-demo)

  * [PHP](https://github.com/huobiapi/Futures-PHP-demo)

  * [Node.js](https://github.com/huobiapi/Futures-Node.js-demo)

  * [易语言](https://github.com/huobiapi/Futures-Yi-demo)

  * [Postman](https://github.com/hbdmapi/huobi_futures_Postman)

**Websocket**

  * [Java](https://github.com/huobiapi/Futures-Java-demo/tree/master/WebSocket-JAVA-demo)

  * [Python](https://github.com/huobiapi/Futures-Python-demo/tree/master/Websocket-Python3-demo)

  * [Node.js](https://github.com/huobiapi/Futures-Node.js-demo/tree/master/WebSocket-Node.js-demo)

**合约sdk**

  * [Java sdk](https://github.com/hbdmapi/huobi_future_Java)

**异步库**

  * [ Rust ](https://github.com/hbdmapi/huobi_future_async)

# 常见问题

## 接入验签相关

### Q1: 合约API Key和现货是否同一个？

合约API Key和现货API Key是同一个，两个是一样的。您可以在 [这里 ](https://www.hbg.com/zh-cn/apikey/)
创建 API Key。

### Q2: 为什么经常出现断线、超时的错误？

如果是在大陆网络环境去请求API接口，网络连接很不稳定，很容易出现超时。建议使用AWS东京C区服务器进行访问。

国内网络可以使用api.btcgateway.pro或者api.hbdm.vn来进行调试,如果仍然无法请求，请在国外服务器上进行运行。

### Q3: 为什么WebSocket总是断开连接？

由于网络环境不同，很容易导致websocket断开连接(websocket: close 1006 (abnormal
closure))，目前最佳实践是建议您将服务器放置在AWS东京C区，并且使用api.hbdm.vn域名；同时需要做好断连重连操作；行情心跳与订单心跳均需要按照《Websocket心跳以及鉴权接口》的行情心跳与订单心跳回复不同格式的Pong消息：[这里](https://docs.huobigroup.com/docs/coin_margined_swap/v1/cn/#472585d15d)。以上操作可以有效减少断连情况。

### Q4: api.hbdm.com与api.hbdm.vn有什么区别？

api.hbdm.vn域名使用的是AWS的CDN服务，理论上AWS服务器用户使用此域名会更快更稳定；api.hbdm.com域名使用的是Cloudflare的CDN服务。

### Q5: 市商享受的colocation服务是指什么以及使用注意事项？

colo相当于是 创建一个VPC节点，直接连了火币合约的内网，会减少客户服务器和火币合约服务器的通讯时间（绕过CDN）。

火币交割合约 的Colocation和 永续合约 是共用的，即连接永续合约Colocation的域名与交割合约是一样的；

但请您注意：colo需要使用：api.hbdm.com 进行签名（鉴权），避免返回403:Verification failure [校验失败] 的错误。

### Q6: 为什么签名认证总返回失败(403:Verification failure [校验失败]) ？

交割签名过程和现货签名过程类似，除了参考以下注意事项外，请参照现货或者永续的demo代码来验证签名是否成功，demo代码验证通过后，再去核对您自己的签名代码。币本位永续的demo代码在
[ 这里 ](https://docs.huobigroup.com/docs/coin_margined_swap/v1/cn/#2cff7db524)
查看。交割的demo代码在[ 这里](https://docs.huobigroup.com/docs/dm/v1/cn/#2cff7db524)
查看。期权的demo代码在[ 这里](https://docs.huobigroup.com/docs/option/v1/cn/#2cff7db524)
查看。USDT本位永续的demo代码在 [ 这里
](https://docs.huobigroup.com/docs/usdt_swap/v1/cn/#2cff7db524) 查看。

  1. 检查 API Key 是否有效，是否复制正确

  2. 是否有绑定 IP 白名单

  3. 检查时间戳是否是 UTC 时间

  4. 检查参数是否按字母排序

  5. 检查编码，使用 UTF-8 编码

  6. 检查签名是否有 base64 编码

  7. 对于 GET 请求，每个方法自带的参数都需要进行签名运算

  8. 对于 POST 请求，每个方法自带的参数不进行签名认证

  9. 检查签名结果是否有进行 URI 编码，十六进制字符必须大写，如 “:” 会被编码为 “%3A” ，空 格被编码为 “%20”

  10. websocket构建签名与restful类似，websocket构造json请求数据时不需要URL编码。

  11. 签名时所带Host应与请求接口时Host相同。如果您使用了代理，代理可能会改变请求Host，可以尝试去掉代理；您使用的网络连接库可能会把端口包含在Host内，可以尝试在签名用到的Host中包含端口，如“api.hbdm.com:443"

  12. Api Key 与 Secret Key中是否存在隐藏特殊字符，影响签名.

### Q7: 公开行情根据ip限速，需要私钥的根据uid限速是吗？

是的。私有的根据UID来限速，不是根据API—KEY限速，母子帐号是分开分别限速，互不影响。

### Q8: 第三方框架集成火币合约是否有推荐？

目前已经有异步量化框架开源，集成了火币交割合约与永续合约： [ 异步量化框架地址
](https://github.com/hbdmapi/hbdm_Python)，有使用反馈或者问题请在github issue区进行提问。

## 行情及WS推送相关

### Q1: 全量行情orderbook订阅和增量orderbook订阅是多长时间推送？

全量orderbook深度推送(market.$symbol.depth.$type)是100MS检查一次，有更新则推送，至少1秒会推送1次。增量orderbook深度推送(market.$symbol.depth.size_${size}.high_freq)是30MS检查一次，有更新则推送，没有更新则不推送。

### Q2: 市场公开逐笔成交是多长时间推送？

市场公开逐笔成交market.$symbol.trade.detail是有成交则推送。

### Q3: 有没有历史K线数据或者历史的公开市场逐笔成交数据？

历史K线数据可以通过API接口/market/history/kline去获取，只填写from,to参数，不写size参数，最多只能获取连续两年的数据。

历史的公开市场逐笔成交数据目前没有，您可以通过订阅market.$symbol.trade.detail来本地进行存储。

### Q4: 如何获取K线上的MACD等技术指标？

API没有获取K线上的MACD等技术指标接口，您可以参考TradingView等网站来计算。

### Q5: 文档里的时间戳timestamp定义是什么？

文档里的时间戳是指格林威治时间1970年01月01日00时00分00秒(北京时间1970年01月01日08时00分00秒)起至现在的总秒数或者总毫秒数。

### Q6: 获取行情深度数据中请求参数type的 150档，20档具体是指？

订阅行情深度market.$symbol.depth.$type,150档指当前盘口的买卖盘的订单，将价格顺序切分为150个小区间，统计每个小区间的挂单数；20档指当前盘口的买卖盘的订单，将价格顺序切分为20个小区间，统计每个小区间的挂单数。

### Q7: 获取行情深度数据中请求参数type的“合并深度”是什么意思？

订阅行情深度(market.$symbol.depth.$type)：

step1和step7 按5位小数合并，买盘向下、卖盘向上 step2和step8 按4位小数合并，买盘向下、卖盘向上 step3和step9
按3位小数合并，买盘向下、卖盘向上 step4和step10 按2位小数合并，买盘向下、卖盘向上 step5和step11
按1位小数合并，买盘向下、卖盘向上 step12和step14 按个位数合并，买盘向下、卖盘向上 step13和step15
按十位数合并，买盘向下、卖盘向上 step4 合并为0.01 例如，下买单价格 100.123， 100.245， 盘口就显示下单价格 100.12，
100.24 如果是卖单 盘口显示价格： 100.13， 100.25

（“向下”和“向上”即是否四舍五入，如买盘向下则不进一位，卖盘向上则进一位） step0到step5,step14,step15是150档；
step6到step13是20档； step6是不合并小数； 结合以上举例说明：

假设当前价格1.123456 6位小数点，如果我单选step1，如果价格是买盘，显示价格是
1.12345（不四舍五入），如果是卖盘，就是1.12346（四舍五入）；

同理，如果我选择step7也是同样的，如果价格是买盘，显示价格是 1.12345（不四舍五入），如果是卖盘，就是1.12346（四舍五入）；

假设是TRX 选择20档 那么step6是不合并，如果当前价格是1.123456 6位小数点，选择step6，不论买卖盘口还是1.123456 6位小数；

假设是TRX 选择20档 那么step11按1位小数合并，假设当前价格1.123456 6位小数点，如果我单选step11，如果价格是买盘，显示价格是
1.1（不四舍五入），如果是卖盘，就是1.1（四舍五入)。

### Q8: websocket的持仓变动频道，每次是返回全量数据还是增量变化的数据？

订阅持仓推送："topic": "positions.BTC_CQ"，推送的是最新的持仓（包括持仓量、可平仓数量、冻结数量），没有变化就不推送。

### Q9: websocket持仓订阅频道，未实现盈亏有变化会推送吗?

订阅持仓推送："topic": "positions.BTC_CQ",
如果持仓有变动，包括开仓/平仓/交割等，会推送仓位变化，若只是单纯的未实现盈亏不会推送。

### Q10: WS中的market detail 和 trade detail 具体什么区别和含义?

Market Detail(market.$symbol.detail)
是市场聚合行情，0.5s检查1次，无成交不推送。包含了此时间段的开盘价、收盘价、最高价、最低价和成交数量；Trade
Detail(market.$symbol.trade.detail) 是有成交更新就会推送，包括成交价格、成交数量和成交方向等数据。

### Q11: 订阅market depth增量数据返回参数的两个ts分别是什么？

增量depth订阅：market.$symbol.depth.size_${size}.high_freq，外层ts是到行情服务器开始转发这笔数据的系统时间戳，里层ts是orderbook的检测时间点。

### Q12: 通过ws订阅market depth数据和market depth增量数据的区别是什么？订阅market depth增量数据多久推送一次？

market.$symbol.depth.$type是全量数据，market.$symbol.depth.size_${size}.high_freq是增量数据，全量数据是100ms检查一次，至少1秒推送1次；增量30MS检查1次，无更新不推送。

目前market
depth增量数据market.$symbol.depth.size_${size}.high_freq是30MS检测一次，不是随机检测，30m检查一次更新，但是有三台机同时进行，每两次的时间间隔最小可能是0，但30ms内最多推送6次，最大时间间隔无上限，30ms内最少推送次数为0。

### Q13: 增量数据market.$symbol.depth.size_${size}.high_freq推送如何维护本地数据？

增量数据首次会推送全量数据，之后推送的为增量数据。

(1) 把增量的价格与上一个全量做比较，相同的价格把挂单量替换；

(2) 没有相同价格的添加到本地全量数据；

(3) 如果某个价格挂单没有了，会推送类似[8100, 0]这样的数据，把本地相同价格的移除；

(4) 同一个websocket连接，增量数据version是递增的；如果 version不递增，您需要重新订阅并重新维护本地全量数据；

### Q14: 交割合约季度合约转为次周合约，WS推送是否会通知或者如何更改？

如果季度合约例如BTC_CQ转为次周合约BTC_NW，WS不会自动通知，您需要重新变更订阅为BTC_NW。

## 交易相关

### Q1: 交割合约什么时候结算？周五结算时通过哪些接口可以查询状态？

在结算时不能下单和撤单，若用户在结算期间下单或撤单会返回错误码“1056”，提示结算中无法下单和撤单。

建议您在结算时间点每隔几秒钟轮询获取合约信息接口：
/api/v1/contract_contract_info，当返回报文中contract_status返回状态码为5、6、7、8中的任意一个时表示在结算中，当contract_status返回状态码为1时是表示结算完成可以正常下单和撤单。

温馨提示您，交割合约在新加坡时间每周五16:00进行结算。在结算期间查询资金和持仓会返回错误码，返回的错误码及错误码表示的含义如下：

  1. 错误码"1077"表示"交割结算中，当前品种资金查询失败"；
  2. 错误码"1078"表示"交割结算中，部分品种资金查询失败"；
  3. 错误码"1079"表示"交割结算中，当前品种持仓查询失败"；
  4. 错误码"1080"表示"交割结算中，部分品种持仓查询失败"

建议您从返回的报文里读取状态码，如果状态码出现上述四种类型，请不要用这个返回的数据。

### Q2: API返回1004错误码是什么原因？

由于近段时间平台系统订单堆积情况比较严重，我们的技术人员正在努力解决和优化中，如果近段时间出现系统繁忙的情况或者出现以下提示：

{“status”:”error”,”err_code”:1004,”err_msg”:”System busy. Please try again
later.”,”ts”: }

请您耐心等待，在此过程中请不要进行重复的下单和撤单，以避免造成重复下单以及对系统性能造成额外的压力，在此期间，建议您可以通过Web和APP端进行下单和撤单。

### Q3: 同样的order id 和 match
id，可以有N多个Trade，比如，用户是一笔大的taker单，吃掉了N个maker的订单，那么，就会对应有N个trade，如何标识这些不同的trade？

订单明细信息接口/api/v1/contract_order_detail返回的的字段id是全局唯一的交易标识。如果一个maker单，分多次match掉的话是每次推送只推match的部分，撮合一笔推送一笔。

### Q4: 交割合约交易全链路延时多少？

目前交割合约全链路(从开始下单到订单的订单状态可以查询)正常情况下大约在30-50MS左右,来行情时延迟会比平时大，可能会在秒级别。

### Q5: API接口返回Connection Reset 或者 Max retris 或者 Timed out 是什么原因？

出现连接重置或者网络超时，一般是网络不稳定导致，可以尝试将服务器放置在AWS东京C区，并使用api.hbdm.vn来尝试，可以有效减少网络超时等错误。

### Q6: API接口下单时出错没有order_id如何来查询订单状态？

如果由于网络原因等API下单超时或者失败，没有返回order_id，可以通过下单时加入client_order_id自定义订单号来进行查询订单状态。

### Q7: WS 订阅私有账户，订单或者仓位一段时间，连接断开如何办？

WS订阅私有账户，订单，仓位时，请注意也要定时维护好心跳，与市场行情的心跳格式不同，详情请参照菜单《Websocket心跳以及鉴权接口》里的订单推送心跳。同时如果连接断开，请做好重连逻辑。

### Q8: 合约资产接口中的“获取合约订单信息”的订单状态1和2都是准备提交有什么不同？3已提交又是什么？

1是准备提交，2是定序的提交，是内部流程的提交。可以认为已经被系统接受了，在系统的流程中。3是已委托到市场。

### Q9: API有获取总资产BTC的接口吗？

没有的。

### Q10: API撤单成功为什么查询订单却是成交？

请注意撤单成功或者下单成功只代表您撤单命令或者下单命令的成功，并不代表订单已经撤销，您可以通过该接口/api/v1/contract_order_info去查询订单状态。

### Q11: API一般从撤单开始到撤单成功需要多久？

撤单命令执行成功一般几十ms，实际撤单状态要查询订单状态/api/v1/contract_order_info获取。

### Q12: 获取历史强平订单的方法？

需要获取历史强平订单，可以通过：获取合约历史委托（/api/v1/contract_hisorders）、获取历史成交记录（/api/v1/contract_matchresults）、组合查询合约历史委托（/api/v1/contract_hisorders_exact）、组合查询历史成交记录接口（/api/v1/contract_matchresults_exact）这四个接口中的返回字段order_source(订单来源)来判断，当order_source返回的为“risk”说明这个订单就是被强平的订单。

## 错误码相关

### Q1: 1030错误是什么原因？

如果您出现比如查询订单或者下单时遇到：{"status":"error","err_code":1030,"err_msg":"Abnormal
service. Please try again
later.","ts":1588093883199}类似错误，说明您的输入的请求参数值或者类型不对，请打印出您的request请求body及完整URL参数，并请一一核对对应API文档接口参数。常见的比如volume张数必须是整数。

### Q2: 1048错误是什么原因？

如果您出现{'index': 1, 'err_code': 1048, 'err_msg': 'Insufficient close amount
available. '}类似错误，说明此时可平仓量不足，您平仓时需查询目前已有的仓位张数再去平仓。

### Q3: API返回1032错误码是什么原因？

1032代表您的访问次数超出限制，币本位永续合约、交割合约、期权合约和USDT永续合约是分开限制频率，请查看合约交易接入说明中的访问次数限制，并且可以在api接口response中的header打印当前的频率限制次数来看是否超出限制频率。建议加大请求间隔延时避免超出限制频率。

## 如何更有效的解决问题

您在反馈API错误时，需要附上您的请求URL，请求request的原始的完整body以及完整请求URL参数，服务器的回复response的原始完整log。如果是websocket订阅，需要您提供订阅的地址，订阅的主题，server推送的原始完整log。

如果是订单相关问题，在使用API订单查询接口api/v1/contract_order_info请求后保留返回的完整log，并提供您的UID以及订单号。

# 合约市场行情接口

## 获取合约信息

### 示例

  * GET `/api/v1/contract_contract_info`

    
    
    curl "https://api.hbdm.com/api/v1/contract_contract_info"
    

### 请求参数

参数名称 | 参数类型 | 必填 | 描述  
---|---|---|---  
symbol | string | false | 支持大小写，"BTC","ETH"...  
contract_type | string | false | 合约类型: （this_week:当周 next_week:下周 quarter:当季
next_quarter:次季）  
contract_code | string | false | BTC180914  
  
### 备注：

如果不填，默认查询所有所有合约信息; 如果contract_code填了值，那就按照contract_code去查询;
如果contract_code没有填值，则按照symbol+contract_type去查询;

> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "BTC",
                "contract_code": "BTC201225",
                "contract_type": "quarter",
                "contract_size": 100,
                "price_tick": 0.01,
                "delivery_date": "20201225",
                "create_date": "20200605",
                "contract_status": 1
            }
        ],
        "ts": 1604296501822
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
contract_code | true | string | 合约代码 | "BTC180914" ...  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter",次季:"next_quarter"  
contract_size | true | decimal | 合约面值，即1张合约对应多少美元 | 10, 100...  
price_tick | true | decimal | 合约价格最小变动精度 | 0.001, 0.01...  
delivery_date | true | string | 合约交割日期 | 如"20180720"  
create_date | true | string | 合约上市日期 | 如"20180706"  
contract_status | true | int | 合约状态 | 合约状态:
0:已下市、1:上市、2:待上市、3:停牌，4:暂停上市中、5:结算中、6:交割中、7:结算完成、8:交割完成、9:暂停交易中  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
## 获取合约指数信息

### 示例

  * GET `/api/v1/contract_index`

    
    
    curl "https://api.hbdm.com/api/v1/contract_index?symbol=BTC"
    

### 请求参数

参数名称 | 参数类型 | 必填 | 描述  
---|---|---|---  
symbol | string | false | 支持大小写，"BTC","ETH"...  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "BTC",
                "index_price": 13707.26,
                "index_ts": 1604296614010
            }
        ],
        "ts": 1604296620746
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
symbol | true | string | 指数代码 | "BTC","ETH"...  
index_price | true | decimal | 指数价格 |  
index_ts | true | long | 响应生成时间点，单位：毫秒 |  
</data> |  |  |  |  
ts | true | long | 时间戳，单位：毫秒 |  
  
## 获取合约最高限价和最低限价

### 示例

  * GET `/api/v1/contract_price_limit`

    
    
    curl "https://api.hbdm.com/api/v1/contract_price_limit?symbol=BTC&contract_type=this_week"
    

### 请求参数

参数名称 | 参数类型 | 必填 | 描述  
---|---|---|---  
symbol | string | false | 支持大小写，"BTC","ETH"...  
contract_type | string | false | 合约类型 (当周:"this_week", 次周:"next_week",
当季:"quarter",次季:"next_quarter")  
contract_code | string | false | BTC180914 ...  
  
### 备注：

如果contract_code填了值，那就按照contract_code去查询；
如contract_code没有填值，则按照symbol+contract_type去查询，两个查询条件必填一个。

> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "BTC",
                "contract_code": "BTC201225",
                "contract_type": "quarter",
                "high_limit": 14724.88,
                "low_limit": 13057.92
            }
        ],
        "ts": 1604296680648
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" ,"error"  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH" ...  
high_limit | true | decimal | 最高买价 |  
low_limit | true | decimal | 最低卖价 |  
contract_code | true | string | 合约代码 | 如"BTC180914" ...  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter" ,次季:"next_quarter"  
<data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
## 获取当前可用合约总持仓量

### 示例

  * GET `/api/v1/contract_open_interest`

    
    
    curl "https://api.hbdm.com/api/v1/contract_open_interest?symbol=BTC&contract_type=this_week"
    

### 请求参数

参数名称 | 参数类型 | 必填 | 描述  
---|---|---|---  
symbol | string | false | 支持大小写，"BTC","ETH"...  
contract_type | string | false | 合约类型 (当周:"this_week", 次周:"next_week",
当季:"quarter",次季:"next_quarter")  
contract_code | string | false | BTC180914  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "volume": 3057834,
                "amount": 22013.565930537597871378,
                "symbol": "BTC",
                "contract_type": "quarter",
                "contract_code": "BTC201225"
            }
        ],
        "ts": 1604296751272
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC", "ETH" ...  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter",次季:"next_quarter"  
volume | true | decimal | 持仓量(张) |  
amount | true | decimal | 持仓量(币) |  
contract_code | true | string | 合约代码 | 如"BTC180914" ...  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
## 获取预估交割价

### 示例

  * GET `/api/v1/contract_delivery_price`

    
    
    curl "https://api.hbdm.com/api/v1/contract_delivery_price?symbol=BTC"
    

### 请求参数

参数名称 | 参数类型 | 必填 | 描述  
---|---|---|---  
symbol | string | true | 支持大小写，"BTC","ETH"...  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "delivery_price": 13212.3643864774624373956594
        },
        "ts": 1604296995036
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
delivery_price | true | float | 预估交割价 |  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
## 查询系统状态

### 示例

  * GET `/api/v1/contract_api_state`

    
    
    curl "https://api.hbdm.com/api/v1/contract_api_state"
    

### 请求参数

参数名称 | 参数类型 | 必填 | 描述  
---|---|---|---  
symbol | string | false | 支持大小写，"BTC","ETH"...，如果缺省，默认返回所有品种  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "BTC",
                "open": 1,
                "close": 1,
                "cancel": 1,
                "transfer_in": 1,
                "transfer_out": 1,
                "master_transfer_sub": 1,
                "sub_transfer_master": 1
            }
        ],
        "ts": 1604297099976
    }
    
    

### 返回参数

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
open | true | int | 开仓下单权限："1"表示可用，“0”表示不可用 |  
close | true | int | 平仓下单权限："1"表示可用，“0”表示不可用 |  
cancel | true | int | 撤单权限："1"表示可用，“0”表示不可用 |  
transfer_in | true | int | 从币币转入的权限："1"表示可用，“0”表示不可用 |  
transfer_out | true | int | 转出至币币的权限："1"表示可用，“0”表示不可用 |  
master_transfer_sub | true | int | 从母账号划转到子账号的权限："1"表示可用，“0”表示不可用 |  
sub_transfer_master | true | int | 从子账号划转到母账号的权限："1"表示可用，“0”表示不可用 |  
</data> |  |  |  |  
  
### 备注

  * open，指交易权限中对应的“API-开仓-普通订单”的权限，开启为可用，关闭为不可用；

  * close，指交易权限中对应的“API-平仓-普通订单”的权限，开启为可用，关闭为不可用；

  * cancel，指交易权限中对应的“API-撤单-普通订单”的权限，开启为可用，关闭为不可用；

  * transfer_in，指交易权限中对应的“其他-划转-从币币转入”的权限，开启为可用，关闭为不可用；

  * transfer_out，指交易权限中对应的“其他-划转-转出至币币”的权限，开启为可用，关闭为不可用；

## 获取行情深度数据

### 示例

  * GET `/market/depth`

    
    
    curl "https://api.hbdm.com/market/depth?symbol=BTC_CQ&type=step5"
    

### 请求参数

参数名称 | 参数类型 | 必填 | 描述  
---|---|---|---  
symbol | string | true |
支持大小写，如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示BTC次季合约。支持使用合约code来查询数据，
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
type | string | true | 仅支持小写，获得150档深度数据，使用step0, step1, step2, step3, step4,
step5, step14, step15（step1至step5,step14，step15
是进行了深度合并后的深度），使用step0时，不合并深度获取150档数据;获得20档深度数据，使用 step6, step7, step8, step9,
step10, step11, step12, step13（step7至step13是进行了深度合并后的深度），使用step6时，不合并深度获取20档数据  
  
> tick 说明:
    
    
        "tick": {
          "id": 消息id.
          "ts": 消息生成时间，单位：毫秒.
          "bids": 买盘,[price(挂单价), vol(此价格挂单张数)], //按price降序.
          "asks": 卖盘,[price(挂单价), vol(此价格挂单张数)]  //按price升序.
          "ch": 数据所属的 channel,
          "mrid": 订单ID,
          "ts": 时间戳,
          "version": 版本
        }
    

> Response:
    
    
    {
        "ch":"market.BTC_NQ.depth.step6",
        "status":"ok",
        "tick":{
            "asks":[
                [
                    14100.87,
                    163
                ],
                [
                    14100.88,
                    20
                ]
            ],
            "bids":[
                [
                    14098.09,
                    53
                ],
                [
                    14098.08,
                    75
                ]
            ],
            "ch":"market.BTC_NQ.depth.step6",
            "id":1604297395,
            "mrid":113765352864,
            "ts":1604297395012,
            "version":1604297395
        },
        "ts":1604297395085
    }
    

### 返回参数

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
ch | true | string | 数据所属的 channel，格式：market.$symbol.depth.$type |  
status | true | string | 请求处理结果 | "ok" , "error"  
<tick> | true | object |  |  
asks | true | array | 卖盘,[price(挂单价), vol(此价格挂单张数)], 按price升序 |  
bids | true | array | 买盘,[price(挂单价), vol(此价格挂单张数)], 按price降序 |  
ch | true | string | 数据所属的 channel，格式：market.$symbol.depth.$type |  
id | true | long | 消息id |  
mrid | true | long | 订单ID |  
ts | true | long | 消息生成时间，单位：毫秒. |  
version | true | long | 版本 |  
</tick> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
### 备注

  * 合并深度时，一定报价精度内的市场挂单将予以合并显示。合并深度仅改变显示方式，不改变实际成交价格。

  * step1至step5,step14,step15是进行了深度合并后的150档深度数据，step7至step13是进行了深度合并后的20档深度数据，对应精度如下：

Depth 类型 | 精度  
---|---  
step1、step7 | 0.00001  
step2、step8 | 0.0001  
step3、step9 | 0.001  
step4、step10 | 0.01  
step5、step11 | 0.1  
step14、step12 | 1  
step15、step13 | 10  
  
## 获取K线数据

### 示例

  * GET `/market/history/kline`

    
    
    curl "https://api.hbdm.com/market/history/kline?period=1min&size=200&symbol=BTC_CQ"
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 合约名称 |  | 支持大小写，
如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示次季度合约"。支持使用合约code来查询数据，
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
period | true | string | K线类型 |  | 1min, 5min, 15min, 30min, 60min,4hour,1day,
1mon  
size | false | int | 获取数量 | 150 | [1,2000]  
from | false | long | 开始时间戳 10位 单位S |  |  
to | false | long | 结束时间戳 10位 单位S |  |  
  
### Note

  * 1、size字段或者from、to字段至少要填写一个。
  * 2、如果size、from、to 均不填写，则返回错误。
  * 3、如果填写from，也要填写to。最多可获取连续两年的数据。
  * 4、如果size、from、to 均填写，会忽略from、to参数。

> Data说明：
    
    
    "data": [
      {
        "id": K线id,
        "vol": 成交量(张)，买卖双边成交量之和,
        "count": 成交笔数,
        "open": 开盘价,
        "close": 收盘价,当K线为最晚的一根时，是最新成交价
        "low": 最低价,
        "high": 最高价,
        "amount": 成交量(币), 即 sum(每一笔成交量(张)*单张合约面值/该笔成交价)
       }
    ]
    

> Response:
    
    
    {
        "ch": "market.BTC_NQ.kline.5min",
        "data": [
            {
                "amount": 4.30994018951037,
                "close": 14103.1,
                "count": 39,
                "high": 14110,
                "id": 1604297400,
                "low": 14098.29,
                "open": 14098.75,
                "vol": 608
            },
            {
                "amount": 0.19851299586596685,
                "close": 14104.87,
                "count": 1,
                "high": 14104.87,
                "id": 1604297700,
                "low": 14104.87,
                "open": 14104.87,
                "vol": 28
            }
        ],
        "status": "ok",
        "ts": 1604297729928
    }
    

### 返回参数

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
ch | true | string | 数据所属的 channel，格式：market.$symbol.kline.$period |  
data | true | object | KLine 数据 |  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
### data参数

**参数名称** | **类型** | **描述** |  
---|---|---|---  
id | int | K线id,也就是K线时间戳，K线起始时间 |  
vol | decimal | 成交量张数 |  
count | decimal | 成交笔数 |  
open | decimal | 开盘价 |  
close | decimal | 收盘价 |  
low | decimal | 最低价 |  
high | decimal | 最高价 |  
amount | decimal | 成交量(币) |  
  
## 获取聚合行情

### 示例

  * GET `/market/detail/merged`

    
    
    curl "https://api.hbdm.com/market/detail/merged?symbol=BTC_CQ"
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 合约名称 |  |
支持大小写，如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示次季度合约"。支持使用合约code来查询数据，
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
  
> tick说明:
    
    
        "tick": {
          "id": K线id,
          "vol": 成交量（张），买卖双边成交量之和,
          "count": 成交笔数,
          "open": 开盘价,
          "close": 收盘价,当K线为最晚的一根时，是最新成交价
          "low": 最低价,
          "high": 最高价,
          "amount": 成交量(币), 即 sum(每一笔成交量(张)*单张合约面值/该笔成交价)
          "bid": [买1价,买1量(张)],
          "ask": [卖1价,卖1量(张)]
        }
    

> Response:
    
    
    {
        "ch": "market.BTC_NQ.detail.merged",
        "status": "ok",
        "tick": {
            "amount": "4478.2911316482577028620799060719867257944",
            "ask": [
                14114.01,
                177
            ],
            "bid": [
                14112.71,
                28
            ],
            "close": "14114",
            "count": 18805,
            "high": "14299.99",
            "id": 1604298319,
            "low": "14028.78",
            "open": "14229.47",
            "ts": 1604298319019,
            "vol": "633708"
        },
        "ts": 1604298319019
    }
    

### 返回参数

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
ch | true | string | 数据所属的 channel，格式： market.$symbol.detail.merged |  
status | true | string | 请求处理结果 | "ok" , "error"  
tick | true | object | 开盘价和收盘价（从当天零点(UTC+8)开始） |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
### tick参数

**参数名称** | **类型** | **描述** |  
---|---|---|---  
id | int | K线id,也就是K线时间戳 |  
vol | string | 成交量张数（最近24（当前时间-24小时）小时成交量张） |  
count | decimal | 成交笔数（最近24（当前时间-24小时）小时成交笔数） |  
open | string | 开盘价 |  
close | string | 收盘价 |  
low | string | 最低价 |  
high | string | 最高价 |  
amount | string | 成交量(币) （最近24（当前时间-24小时）小时成交量币） |  
ts | long | 时间戳 |  
ask | true | object | 卖盘,[price(挂单价), vol(此价格挂单张数)], 按price升序  
bid | true | object | 买盘,[price(挂单价), vol(此价格挂单张数)], 按price降序  
  
## 获取市场最近成交记录

### 示例

  * GET `/market/trade`

    
    
    curl "https://api.hbdm.com/market/trade?symbol=BTC_CQ"
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 合约名称 |  |
支持大小写，如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示次季度合约"。支持使用合约code来查询数据，
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
  
> Tick说明：
    
    
        "tick": {
          "id": 订单唯一id（品种唯一),
          "ts": 最新成交时间,
          "data": [
             {
                "id": 成交唯一id（品种唯一）,
                "price": 成交价钱,
                "amount": 成交量(张)，买卖双边成交量之和,
                "direction": 主动成交方向,
                "ts": 成交时间
             }
          ]
        }
    

> Response:
    
    
    {
        "ch": "market.BTC_NQ.trade.detail",
        "status": "ok",
        "tick": {
            "data": [
                {
                    "amount": "4",
                    "ts": 1604298443540,
                    "id": 1137660004780000,
                    "price": "14117.98",
                    "direction": "sell"
                }
            ],
            "id": 1604298454352,
            "ts": 1604298454352
        },
        "ts": 1604298454352
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
ch | true | string | 数据所属的 channel，格式： market.$symbol.trade.detail |  
status | true | string |  | "ok","error"  
<tick> | true | object |  |  
id | true | long | 订单唯一id（品种唯一） |  
ts | true | long | 最新成交时间 |  
<data> | true | object array |  |  
amount | true | string | 成交量(张)，买卖双边成交量之和 |  
direction | true | string | 主动成交方向 |  
id | true | long | 成交唯一id（品种唯一） |  
price | true | string | 成交价 |  
ts | true | long | 成交时间 |  
</data> |  |  |  |  
</tick> |  |  |  |  
ts | true | long | 发送时间 |  
  
## 批量获取最近的交易记录

### 示例

  * GET `/market/history/trade`

    
    
    curl "https://api.hbdm.com/market/history/trade?symbol=BTC_CQ&size=100"
    

### 请求参数：

参数名称 | 是否必须 | 数据类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 合约名称 |  |
支持大小写，如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示次季度合约"。支持使用合约code来查询数据，
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
size | true | int | 获取交易记录的数量 |  | [1, 2000]  
  
> data说明：
    
    
        "data": {
          "id": 订单唯一id（品种唯一）,
          "ts": 最新成交时间,
          "data": [
            {
              "id": 成交唯一id（品种唯一）,
              "price": 成交价,
              "amount": 成交量(张)，买卖双边成交量之和,
              "direction": 主动成交方向,
              "ts": 成交时间
            }
          ]
        }
    

> Response:
    
    
    {
        "ch": "market.BTC_NQ.trade.detail",
        "data": [
            {
                "data": [
                    {
                        "amount": 12,
                        "direction": "buy",
                        "id": 1137660361550000,
                        "price": 14119.84,
                        "ts": 1604298530920
                    }
                ],
                "id": 113766036155,
                "ts": 1604298530920
            },
            {
                "data": [
                    {
                        "amount": 4,
                        "direction": "sell",
                        "id": 1137660376740000,
                        "price": 14123.14,
                        "ts": 1604298531331
                    }
                ],
                "id": 113766037674,
                "ts": 1604298531331
            }
        ],
        "status": "ok",
        "ts": 1604298553734
    }
    

### 返回参数

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
ch | true | string | 数据所属的 channel，格式： market.$symbol.trade.detail |  
<data> | true | object array |  |  
<data> | true | object array |  |  
amount | true | decimal | 成交量(张)，买卖双边成交量之和 |  
direction | true | string | 主动成交方向 |  
id | true | long | 成交唯一id（品种唯一） |  
price | true | decimal | 成交价格 |  
ts | true | long | 成交时间 |  
</data> |  |  |  |  
id | true | long | 订单唯一id（品种唯一） |  
ts | true | long | 最新成交时间 |  
</data> |  |  |  |  
status | true | string |  | "ok"，"error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
## 查询合约风险准备金余额和预估分摊比例

  * GET `/api/v1/contract_risk_info`

    
    
    curl "https://api.hbdm.com/api/v1/contract_risk_info"
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | false | string | 品种代码 | 支持大小写，"BTC","ETH"...，如果缺省，默认返回所有品种  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "BTC",
                "insurance_fund": 1909.852579486750035041,
                "estimated_clawback": 0
            }
        ],
        "ts": 1604298633195
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
insurance_fund | true | decimal | 风险准备金余额 |  
estimated_clawback | true | decimal | 预估分摊比例 |  
</data> |  |  |  |  
  
## 查询合约风险准备金余额历史数据

  * GET `/api/v1/contract_insurance_fund`

    
    
    curl "https://api.hbdm.com/api/v1/contract_insurance_fund?symbol=ETH"
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | true | string | 品种代码 | 支持大小写，"BTC","ETH"...  
  
> Response:
    
    
    {
        "status":"ok",
        "data":{
            "symbol":"BTC",
            "tick":[
                {
                    "insurance_fund":1909.852579486750035041,
                    "ts":1604217600000
                },
                {
                    "insurance_fund":1907.646552903264189201,
                    "ts":1604131200000
                }
            ]
        },
        "ts":1604298695848
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  | 字典数据  
symbol | true | string | 品种代码 | "BTC","ETH"...  
<tick> |  |  |  |  
insurance_fund | true | decimal | 风险准备金余额 |  
ts | true | long | 数据时间点，单位：毫秒 |  
</tick> |  |  |  |  
</data> |  |  |  |  
  
## 查询平台阶梯调整系数

  * GET `/api/v1/contract_adjustfactor`

    
    
    curl "https://api.hbdm.com/api/v1/contract_adjustfactor"
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | false | string | 品种代码 | 支持大小写，"BTC","ETH"...，如果缺省，默认返回所有品种  
  
> Response:
    
    
    {
        "status":"ok",
        "data":[
            {
                "symbol":"BTC",
                "list":[
                    {
                        "lever_rate":125,
                        "ladders":[
                            {
                                "ladder":0,
                                "min_size":0,
                                "max_size":1999,
                                "adjust_factor":0.65
                            },
                            {
                                "ladder":1,
                                "min_size":2000,
                                "max_size":14999,
                                "adjust_factor":0.8
                            },
                            {
                                "ladder":2,
                                "min_size":15000,
                                "max_size":null,
                                "adjust_factor":0.85
                            }
                        ]
                    }
                ]
            }
        ],
        "ts":1604298785020
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
<list> |  |  |  |  
lever_rate | true | decimal | 杠杆倍数 |  
<ladderDetail> |  |  |  |  
min_size | true | decimal | 净持仓量的最小值 |  
max_size | true | decimal | 净持仓量的最大值 |  
ladder | true | int | 档位 |  
adjust_factor | true | decimal | 调整系数 |  
</ladderDetail> |  |  |  |  
</list> |  |  |  |  
</data> |  |  |  |  
  
## 平台持仓量的查询

### 实例

  * GET `/api/v1/contract_his_open_interest`

    
    
    curl "https://api.hbdm.com/api/v1/contract_his_open_interest?symbol=BTC&contract_type=this_week&period=60min&amount_type=1"
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | true | string | 品种代码 | 支持大小写，"BTC","ETH"...  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter",次季:"next_quarter"  
period | true | string | 时间周期类型 |
1小时:"60min"，4小时:"4hour"，12小时:"12hour"，1天:"1day"  
size | false | int | 获取数量 | 默认为：48，取值范围 [1,200]  
amount_type | true | int | 计价单位 | 1:张，2:币  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "symbol": "BTC",
            "contract_type": "quarter",
            "tick": [
                {
                    "volume": "3058980.0000000000000000",
                    "amount_type": 1,
                    "ts": 1604296800000
                },
                {
                    "volume": "3049899.0000000000000000",
                    "amount_type": 1,
                    "ts": 1604293200000
                }
            ]
        },
        "ts": 1604298943494
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  | 字典数据 |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter",次季:"next_quarter"  
<tick> |  |  |  |  
volume | true | string | 持仓量 |  
amount_type | true | int | 计价单位 | 1:张，2:币  
ts | true | long | 统计时间 |  
</tick> |  |  |  |  
</data> |  |  |  |  
  
### 注意：

tick字段：数组内的数据按照时间倒序排列； data字段：字典类型。

## 精英账户多空持仓对比-账户数

### 实例

  * GET `/api/v1/contract_elite_account_ratio`

    
    
    curl "https://api.hbdm.com/api/v1/contract_elite_account_ratio?symbol=BTC&period=60min"
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | true | string | 品种代码 | 支持大小写，"BTC","ETH"...  
period | true | string | 周期 | 5min, 15min, 30min, 60min,4hour,1day  
  
> Response:
    
    
    {
        "status":"ok",
        "data":{
            "list":[
                {
                    "buy_ratio":0.52,
                    "sell_ratio":0.45,
                    "locked_ratio":0.03,
                    "ts":1604290200000
                }
            ],
            "symbol":"BTC"
        },
        "ts":1604299070097
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
<list> |  |  |  |  
buy_ratio | true | decimal | 净多仓的账户比例 |  
sell_ratio | true | decimal | 净空仓的账户比例 |  
locked_ratio | true | decimal | 锁仓的账户比例 |  
ts | true | long | 生成时间 |  
</list> |  |  |  |  
</data> |  |  |  |  
  
## 精英账户多空持仓对比-持仓量

### 实例

  * GET `/api/v1/contract_elite_position_ratio`

    
    
    curl "https://api.hbdm.com/api/v1/contract_elite_position_ratio?symbol=BTC&period=60min"
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | true | string | 品种代码 | 支持大小写，"BTC","ETH"...  
period | true | string | 周期 | 5min, 15min, 30min, 60min,4hour,1day  
  
> Response:
    
    
    {
        "status":"ok",
        "data":{
            "list":[
                {
                    "buy_ratio":0.51,
                    "sell_ratio":0.49,
                    "ts":1604290500000
                },
                {
                    "buy_ratio":0.508,
                    "sell_ratio":0.492,
                    "ts":1604290800000
                }
            ],
            "symbol":"BTC"
        },
        "ts":1604299402211
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
<list> |  |  |  |  
buy_ratio | true | decimal | 多仓的总持仓量占比 |  
sell_ratio | true | decimal | 空仓的总持仓量占比 |  
ts | true | long | 生成时间 |  
</list> |  |  |  |  
</data> |  |  |  |  
  
## 获取强平订单

### 实例

  * GET `/api/v1/contract_liquidation_orders`

    
    
    curl "https://api.hbdm.com/api/v1/contract_liquidation_orders?symbol=BTC&trade_type=0&create_date=7"
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 品种代码 |  | 支持大小写，"BTC","ETH"...  
trade_type | true | int | 交易类型 |  | 0:全部,5: 卖出强平,6: 买入强平  
create_date | true | int | 日期 |  | 7，90（7天或者90天）  
page_index | false | int | 页码,不填默认第1页 | 1 |  
page_size | false | int | 不填默认20，不得多于50 | 20 | [1-50]  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "contract_code": "BTC201225",
                    "symbol": "BTC",
                    "direction": "buy",
                    "offset": "close",
                    "volume": 26,
                    "price": 19674.96,
                    "created_at": 1606293144641,
                    "amount": 0.132147663832607537
                }
            ],
            "total_page": 114,
            "current_page": 1,
            "total_size": 2264
        },
        "ts": 1604299610722
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 |  
<data> |  |  |  |  
<orders> |  |  |  |  
symbol | true | string | 品种代码 |  
contract_code | true | string | 合约代码 | "BTC180914" ...  
direction | true | string | "buy":买 "sell":卖 |  
offset | true | string | "open":开 "close":平 |  
volume | true | decimal | 强平数量（张） |  
amount | true | decimal | 强平数量（币） |  
price | true | decimal | 破产价格 |  
created_at | true | long | 强平时间 |  
</orders> |  |  |  |  
total_page | true | int | 总页数 |  
current_page | true | int | 当前页 |  
total_size | true | int | 总条数 |  
</data> |  |  |  |  
ts | true | long | 时间戳 |  
  
## 查询平台历史结算记录

  * GET `/api/v1/contract_settlement_records`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | true | string | 品种代码 | "BTC","ETH"...  
start_time | false | long | 起始时间 （时间戳，单位毫秒） | 取值范围：[(当前时间 - 90天), 当前时间]
，默认取当前时间- 90天  
end_time | false | long | 结束时间（时间戳，单位毫秒） | 取值范围：(start_time, 当前时间)，默认取当前时间  
page_index | false | int | 页码，不填默认第1页 |  
page_size | false | int | 页长，不填默认20，不得多于50 |  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "total_page": 13,
            "current_page": 1,
            "total_size": 13,
            "settlement_record": [
                {
                    "symbol": "BTC",
                    "settlement_time": 1605859200000,
                    "clawback_ratio": 0,
                    "list": [
                        {
                            "contract_code": "BTC201120",
                            "settlement_price": 18217.62,
                            "settlement_type": "delivery"
                        },
                        {
                            "contract_code": "BTC201127",
                            "settlement_price": 18292.24,
                            "settlement_type": "settlement"
                        },
                        {
                            "contract_code": "BTC201225",
                            "settlement_price": 18490.42,
                            "settlement_type": "settlement"
                        },
                        {
                            "contract_code": "BTC210326",
                            "settlement_price": 18788.7,
                            "settlement_type": "settlement"
                        }
                    ]
                }
            ]
        },
        "ts": 1606295834648
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> | true | object array |  |  
<settlement_record> | true | object array |  |  
symbol | true | string | 品种代码 |  
settlement_time | true | long | 结算时间（时间戳，单位毫秒）
（当settlement_type为交割时，该时间为交割时间；当settlement_type为结算时，该时间为结算时间；） |  
clawback_ratio | true | decimal | 分摊比例 |  
<list> | true | object array |  |  
contract_code | true | string | 合约代码 | "BTC180914" ...  
settlement_price | true | decimal |
结算价格（当settlement_type为交割时，该价格为交割价格；当settlement_type为结算时，该价格为结算价格；） |  
settlement_type | true | string | 结算类型 | “delivery”：交割，“settlement”：结算  
</list> |  |  |  |  
</settlement_record> |  |  |  |  
total_page | true | int | 总页数 |  
current_page | true | int | 当前页 |  
total_size | true | int | 总条数 |  
</data> |  |  |  |  
  
## 获取指数K线数据

### 实例

  * GET `/index/market/history/index`

    
    
    curl "https://api.hbdm.com/index/market/history/index?symbol=BTC-USD&period=1min&size=150"
    

### 请求参数

**参数名称** | **是否必须** | **类型** | **描述** | **默认值** | **取值范围**  
---|---|---|---|---|---  
symbol | true | string | 指数标识 |  | 支持大小写，"BTC-USD","ETH-USD"...  
period | true | string | K线类型 |  | 1min, 5min, 15min, 30min, 60min,4hour,1day,
1mon  
size | true | int | K线获取数量 |  | [1,2000]  
  
> 返回示例：
    
    
    {
        "ch": "market.BTC-USD.index.60min",
        "data": [
            {
                "amount": 0,
                "close": 13703.4175,
                "count": 0,
                "high": 13720.84,
                "id": 1604293200,
                "low": 13658.245,
                "open": 13709.6175,
                "vol": 0
            },
            {
                "amount": 0,
                "close": 13751.6,
                "count": 0,
                "high": 13771.21,
                "id": 1604296800,
                "low": 13693.16,
                "open": 13703.365,
                "vol": 0
            }
        ],
        "status": "ok",
        "ts": 1604299755097
    }
    

### 返回参数：

**参数名称** | **是否必须** | **类型** | **描述** | **取值范围**  
---|---|---|---|---  
ch | true | string | 数据所属的 channel 格式： market.$symbol.index.$period |  
<data> | true | object | 指数KLine 数据 |  
id | true | decimal | 指数K线id,也就是K线时间戳，K线起始时间 |  
vol | true | decimal | 成交量张数,值为0 |  
count | true | decimal | 成交笔数，值为0 |  
open | true | decimal | 开盘指数价 |  
close | true | decimal | 收盘指数价,当K线为最晚的一根时，是最新成交价 |  
low | true | decimal | 最低指数价 |  
high | true | decimal | 最高指数价 |  
amount | true | decimal | 成交量(币), 即 sum(每一笔成交量(张)*单张合约面值/该笔成交价)，值为0 |  
</data> |  |  |  |  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点 单位：毫秒 |  
  
## 获取基差数据

### 实例

  * GET `/index/market/history/basis`

    
    
    curl "https://api.hbdm.com/index/market/history/basis?symbol=BTC_CQ&period=1min&size=150&basis_price_type=open"
    

### 请求参数

**参数名称** | **是否必须** | **类型** | **描述** | **默认值** | **取值范围**  
---|---|---|---|---|---  
symbol | true | string | 合约名称 |  |
支持大小写，如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约, "BTC_NQ"表示次季度合约"  
period | true | string | 周期 |  | 仅支持小写，1min,5min, 15min, 30min,
60min,4hour,1day,1mon  
basis_price_type | false | string | 基差价格类型，表示在周期内计算基差使用的价格类型 | 不填，默认使用开盘价 |
仅支持小写，开盘价：open，收盘价：close，最高价：high，最低价：low，平均价=（最高价+最低价）/2：average  
size | true | int | 基差获取数量 |  | [1,2000]  
  
> 返回示例：
    
    
    {
        "ch": "market.BTC-USD.basis.5min.open",
        "data": [
            {
                "basis": "-2.1850000000013097",
                "basis_rate": "-0.00015880531885174013",
                "contract_price": "13756.8",
                "id": 1604299500,
                "index_price": "13758.985"
            },
            {
                "basis": "-4.235000000000582",
                "basis_rate": "-0.00030799697602973224",
                "contract_price": "13745.9",
                "id": 1604299800,
                "index_price": "13750.135"
            }
        ],
        "status": "ok",
        "ts": 1604299816352
    }
    

### 返回参数

**参数名称** | **是否必须** | **类型** | **描述** | **取值范围**  
---|---|---|---|---  
ch | true | string | 主题 |  
status | true | string | 状态 |  
<data> | true | object | 基差数据 |  
id | true | long | 唯一标识 |  
contract_price | true | string | 合约最新成交价 |  
index_price | true | string | 指数基准价，与基差价格类型匹配 |  
basis | true | string | 基差=合约基准价 - 指数基准价 |  
basis_rate | true | string | 基差率=基差/指数基准价 |  
<\data> |  |  |  |  
ts | true | long | 生成时间 |  
  
### 说明：

一次最多2000条数据；

次季度的基差数据在2020/6/15 14:00:00后才开始生成。

# 合约资产接口

## 获取用户账户信息

### 示例

  * POST `/api/v1/contract_account_info`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | false | string | 品种代码 |  | 支持大小写,"BTC","ETH"...如果缺省，默认返回所有品种  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "margin_balance": 453.151955780787465997,
                "margin_position": 0,
                "margin_frozen": 0,
                "margin_available": 453.151955780787465997,
                "profit_real": 16.35635155751274032,
                "profit_unreal": 0,
                "risk_rate": null,
                "withdraw_available": 436.795604223274725677,
                "liquidation_price": null,
                "lever_rate": 10,
                "adjust_factor": 0.2,
                "margin_static": 453.151955780787465997,
                "is_debit": 0
            }
        ],
        "ts": 1604300060777
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
margin_balance | true | decimal | 账户权益 |  
margin_position | true | decimal | 持仓保证金（当前持有仓位所占用的保证金） |  
margin_frozen | true | decimal | 冻结保证金 |  
margin_available | true | decimal | 可用保证金 |  
profit_real | true | decimal | 已实现盈亏 |  
profit_unreal | true | decimal | 未实现盈亏 |  
risk_rate | true | decimal | 保证金率 |  
liquidation_price | true | decimal | 预估强平价 |  
withdraw_available | true | decimal | 可划转数量 |  
lever_rate | true | decimal | 杠杠倍数 |  
adjust_factor | true | decimal | 调整系数 |  
margin_static | true | decimal | 静态权益 |  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
## 获取用户持仓信息

### 示例

  * POST `/api/v1/contract_position_info`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | false | string | 品种代码 |  | 支持大小写,""BTC","ETH"...如果缺省，默认返回所有品种  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "contract_code": "ADA201225",
                "contract_type": "quarter",
                "volume": 1,
                "available": 1,
                "frozen": 0,
                "cost_open": 0.0991,
                "cost_hold": 0.0991,
                "profit_unreal": 0,
                "profit_rate": 0,
                "lever_rate": 10,
                "position_margin": 10.090817356205852674,
                "direction": "sell",
                "profit": 0,
                "last_price": 0.0991
            }
        ],
        "ts": 1604301441639
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
contract_code | true | string | 合约代码 | "BTC180914" ...  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter", 次季:"next_quarter"  
volume | true | decimal | 持仓量 |  
available | true | decimal | 可平仓数量 |  
frozen | true | decimal | 冻结数量 |  
cost_open | true | decimal | 开仓均价 |  
cost_hold | true | decimal | 持仓均价 |  
profit_unreal | true | decimal | 未实现盈亏 |  
profit_rate | true | decimal | 收益率 |  
profit | true | decimal | 收益 |  
position_margin | true | decimal | 持仓保证金 |  
lever_rate | true | int | 杠杠倍数 |  
direction | true | string | "buy":买 "sell":卖 |  
last_price | true | decimal | 最新价 |  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
#### 备注

  * 如果有某个品种在结算中，不带请求参数去查询持仓，会返回错误码1080(1080 In settlement or delivery. Unable to get positions of some contracts. )。建议您带上请求参数去查询持仓，避免报错查询不到持仓。

## 查询母账户下所有子账户资产信息

### 请求参数

  * POST `/api/v1/contract_sub_account_list`

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | false | string | 品种代码 |  | 支持大小写, "BTC","ETH"... ,如果缺省，默认返回所有品种  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "sub_uid": 123456789,
                "list": [
                    {
                        "symbol": "ADA",
                        "margin_balance": 50,
                        "liquidation_price": null,
                        "risk_rate": null
                    }
                ]
            }
        ],
        "ts": 1604301647427
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
sub_uid | true | long | 子账户UID |  
<list> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
margin_balance | true | decimal | 账户权益 |  
liquidation_price | true | decimal | 预估强平价 |  
risk_rate | true | decimal | 保证金率 |  
</list> |  |  |  |  
</data> |  |  |  |  
  
### 备注

只返回已经开通合约交易的子账户数据.

## 查询单个子账户资产信息

  * POST `/api/v1/contract_sub_account_info`

> Request:
    
    
    {
        "symbol":"BTC",
        "sub_uid":123456789
    }
    

### 请求参数*

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | false | string | 品种代码 |  | 支持大小写,"BTC","ETH"...，如果缺省，默认返回所有品种  
sub_uid | true | long | 子账户的UID |  |  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "margin_balance": 50,
                "margin_position": 0,
                "margin_frozen": 0,
                "margin_available": 50,
                "profit_real": 0,
                "profit_unreal": 0,
                "risk_rate": null,
                "withdraw_available": 50,
                "liquidation_price": null,
                "lever_rate": 5,
                "adjust_factor": 0.1,
                "margin_static": 50,
                "is_debit": 0
            }
        ],
        "ts": 1604301730723
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...，  
margin_balance | true | decimal | 账户权益 |  
margin_position | true | decimal | 持仓保证金（当前持有仓位所占用的保证金） |  
margin_frozen | true | decimal | 冻结保证金 |  
margin_available | true | decimal | 可用保证金 |  
profit_real | true | decimal | 已实现盈亏 |  
profit_unreal | true | decimal | 未实现盈亏 |  
risk_rate | true | decimal | 保证金率 |  
liquidation_price | true | decimal | 预估爆仓价 |  
withdraw_available | true | decimal | 可划转数量 |  
lever_rate | true | decimal | 杠杆倍数 |  
adjust_factor | true | decimal | 调整系数 |  
margin_static | true | decimal | 静态权益 |  
</data> |  |  |  |  
  
### 备注

只能查询到开通合约交易的子账户信息；

子账户来过合约系统但是未开通合约交易也不返回对应的数据；

## 查询单个子账户持仓信息

  * POST `/api/v1/contract_sub_position_info`

> Request:
    
    
    {
        "symbol":"BTC",
        "sub_uid":123456789
    }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | false | string | 品种代码 |  | 支持大小写, "BTC","ETH"...，如果缺省，默认返回所有品种  
sub_uid | true | long | 子账户的UID |  |  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "contract_code": "ADA201225",
                "contract_type": "quarter",
                "volume": 1,
                "available": 1,
                "frozen": 0,
                "cost_open": 0.0991,
                "cost_hold": 0.0991,
                "profit_unreal": -0.04686106551835051,
                "profit_rate": -0.002321965796434265,
                "lever_rate": 5,
                "position_margin": 20.191006925515375451,
                "direction": "buy",
                "profit": -0.04686106551835051,
                "last_price": 0.099054
            }
        ],
        "ts": 1604302891178
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
symbol | true | string | 品种代码 | 支持大小写, "BTC","ETH"...  
contract_code | true | string | 合约代码 | "BTC180914" ...  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter", 次季：“next_quarter”  
volume | true | decimal | 持仓量 |  
available | true | decimal | 可平仓数量 |  
frozen | true | decimal | 冻结数量 |  
cost_open | true | decimal | 开仓均价 |  
cost_hold | true | decimal | 持仓均价 |  
profit_unreal | true | decimal | 未实现盈亏 |  
profit_rate | true | decimal | 收益率 |  
profit | true | decimal | 收益 |  
position_margin | true | decimal | 持仓保证金 |  
lever_rate | true | int | 杠杆倍数 |  
direction | true | string | 仓位方向 | "buy":多 "sell":空  
last_price | true | decimal | 最新价 |  
</data> |  |  |  |  
  
## 查询用户财务记录

  * POST `/api/v1/contract_financial_record`

> Request:
    
    
    {
        "create_date":7,
        "page_index":1,
        "symbol":"btc",
        "type":"3,4",
        "page_size":20
    }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol  | true  | string | 品种代码  | 支持大小写,"BTC","ETH"...  
type | false | string | 不填查询全部类型,【查询多类型中间用，隔开】 | 3:平多; 4:平空; 5:开仓手续费-吃单;
6:开仓手续费-挂单; 7:平仓手续费-吃单; 8:平仓手续费-挂单; 9:交割平多; 10:交割平空; 11:交割手续费; 12:强制平多;
13:强制平空; 14:从币币转入; 15:转出至币币; 16:结算未实现盈亏-多仓; 17:结算未实现盈亏-空仓; 19:穿仓分摊; 26:系统;
28:活动奖励; 29:返利; 30:资金费-收入; 31:资金费-支出; 34:转出到子账号合约账户; 35:从子账号合约账户转入;
36:转出到母账号合约账户; 37:从母账号合约账户转入;  
create_date | false | int | 可随意输入正整数，如果参数超过90则默认查询90天的数据 |  
page_index | false | int | 第几页,不填默认第一页 |  
page_size | false | int | 不填默认20，不得多于50 |  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "total_page": 15,
            "current_page": 1,
            "total_size": 15,
            "financial_record": [
                {
                    "id": 3662498355,
                    "symbol": "ADA",
                    "type": 8,
                    "amount": -0.074766355140186915,
                    "ts": 1605014144415,
                    "contract_code": "ADA201225"
                }
            ]
        },
        "ts": 1604306015124
    }                                
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status  | true  | string | 请求处理结果  | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  | 字典类型 |  
<financial_record> |  |  |  |  
id | true | long | 财务记录ID（唯一） |  
ts | true | long | 创建时间 |  
symbol | true | string | 品种代码 | 支持大小写,"BTC","ETH"...  
type | true | int | 交易类型 | 3:平多; 4:平空; 5:开仓手续费-吃单; 6:开仓手续费-挂单; 7:平仓手续费-吃单;
8:平仓手续费-挂单; 9:交割平多; 10:交割平空; 11:交割手续费; 12:强制平多; 13:强制平空; 14:从币币转入; 15:转出至币币;
16:结算未实现盈亏-多仓; 17:结算未实现盈亏-空仓; 19:穿仓分摊; 26:系统; 28:活动奖励; 29:返利; 30:资金费-收入;
31:资金费-支出; 34:转出到子账号合约账户; 35:从子账号合约账户转入; 36:转出到母账号合约账户; 37:从母账号合约账户转入;  
amount | true | decimal | 金额 |  
contract_code | true | string | 合约代码 |  
</financial_record> |  |  |  |  
total_page | true | int | 总页数 |  
current_page | true | int | 当前页 |  
total_size | true | int | 总条数 |  
</data> |  |  |  |  
  
## 组合查询用户财务记录

  * POST `/api/v1/contract_financial_record_exact`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol  | true  | string | 品种代码  | "BTC","ETH"...  
type | false | string | 不填查询全部类型,【查询多类型中间用，隔开】 | 3:平多; 4:平空; 5:开仓手续费-吃单;
6:开仓手续费-挂单; 7:平仓手续费-吃单; 8:平仓手续费-挂单; 9:交割平多; 10:交割平空; 11:交割手续费; 12:强制平多;
13:强制平空; 14:从币币转入; 15:转出至币币; 16:结算未实现盈亏-多仓; 17:结算未实现盈亏-空仓; 19:穿仓分摊; 26:系统;
28:活动奖励; 29:返利; 30:资金费-收入; 31:资金费-支出; 34:转出到子账号合约账户; 35:从子账号合约账户转入;
36:转出到母账号合约账户; 37:从母账号合约账户转入;  
start_time | false | long | 起始时间（时间戳，单位毫秒） | 详见备注  
end_time | false | long | 结束时间（时间戳，单位毫秒） | 详见备注  
from_id | false | long | 查询起始id（取返回数据的id ） |  
size | false | int | 数据条数 | 默认取20，最大50  
direct | false | string | 查询方向 | prev 向前；next 向后；默认值取prev  
  
#### 备注：

  * 起始与结束时间取值说明： 
    * start_time：取值范围为[(当前时间 - 90天)，当前时间] ；默认值取clamp（end_time - 10天，当前时间-90天，当前时间-10天），即时间最远取当前时间-90天，最近取当前时间-10天。
    * end_time：取值范围为：[(当前时间 - 90天)，above++)，若大于当前时间则直接取当前时间；若填写了start_time，则end_time必须大于start_time。默认值直接取当前时间。
  * 当from_id缺省时，查询方向为prev则从结束时间往前查，查询方向为向后则从起始时间往后查；即查询创建时间大于等于起始时间，且小于等于结束时间的财务记录数据。
  * 无论查询方向是向前还是向后，返回的数据都是按创建时间倒序。
  * 当start_time或end_time填写值不符合取值范围，则报错参数不合法。
  * 仅支持查询90天内数据。

#### 查询案例如下（特殊错误情况未罗列）如当前时间为"2020-07-31"：

start_time | end_time | from_id | size | direct | 查询结果  
---|---|---|---|---|---  
缺省，取10天前（2020-07-21） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | prev |
查询最近10天的数据，从当前时间开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取60天前（2020-06-01） | 50天前（2020-06-11） | 缺省 | 20条 | prev |
查询60天前到50天前之间的数据，从50天前开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
5天前（2020-07-26） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | prev |
查询最近5天的数据，从当前时间开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
20天前（2020-07-11） | 10天前（2020-07-21） | 缺省 | 20条 | prev |
查询20天前到10天前之间的数据，从10天前开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取10天前（2020-07-21） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | next |
查询最近10天的数据，从10天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取60天前（2020-06-01） | 50天前（2020-06-11） | 缺省 | 20条 | next |
查询60天前到50天前之间的数据，从60天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
5天前（2020-07-26） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | next |
查询最近5天的数据，从5天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
20天前（2020-07-11） | 10天前 （2020-07-21） | 缺省 | 20条 | next |
查询20天前到10天前之间的数据，从20天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取10天前（2020-07-21） | 缺省，取当前时间 （2020-07-31） | 1000 | 20条 | prev |
查询最近10天的数据，从成交id为1000的数据开始往前查20条更旧的数据，成交id为1000的数据排在第一条，越新的数据排在越前  
20天前 （2020-07-11） | 10天前 （2020-07-21） | 1000 | 20条 | next |
查询20天前到10天前之间的数据，从成交id为1000的数据开始往后查20条更新的数据，成交id为1000的数据排在最后一条，越新的数据排在越前  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "financial_record": [
                {
                    "id": 3657420903,
                    "symbol": "ADA",
                    "type": 34,
                    "amount": -50,
                    "ts": 1604301623306,
                    "contract_code": "ADA"
                },
                {
                    "id": 3657420101,
                    "symbol": "ADA",
                    "type": 6,
                    "amount": -0.020181634712411705,
                    "ts": 1604301416067,
                    "contract_code": "ADA201225"
                }
            ],
            "remain_size": 22,
            "next_id": 3657309434
        },
        "ts": 1604305081144
    }                              
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status  | true  | string | 请求处理结果  | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> | true | object | 字典类型 |  
<financial_record> | true | object array |  |  
id | true | long | 流水id |  
ts | true | long | 创建时间 |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
contract_code | true | string | 合约代码 | "BTC200919"...  
type | true | int | 交易类型 | 3:平多; 4:平空; 5:开仓手续费-吃单; 6:开仓手续费-挂单; 7:平仓手续费-吃单;
8:平仓手续费-挂单; 9:交割平多; 10:交割平空; 11:交割手续费; 12:强制平多; 13:强制平空; 14:从币币转入; 15:转出至币币;
16:结算未实现盈亏-多仓; 17:结算未实现盈亏-空仓; 19:穿仓分摊; 26:系统; 28:活动奖励; 29:返利; 30:资金费-收入;
31:资金费-支出; 34:转出到子账号合约账户; 35:从子账号合约账户转入; 36:转出到母账号合约账户; 37:从母账号合约账户转入;  
amount | true | decimal | 金额 |  
</financial_record> |  |  |  |  
remain_size | true | int | 剩余数据条数（在时间范围内，因受到数据条数限制而未查询到的数据条数） |  
next_id | true | long | 下一条数据的流水id（仅在查询结果超过数据条数限制时才有值） |  
</data> |  |  |  |  
  
#### 备注：

  * 当查询结果超过数据条数限制时，next_id为下一条数据的流水id（查询方向为prev时，next_id为下一页查询的第一条数据；查询方向为next时，next_id为下一页查询的最后一条数据）

## 查询用户结算记录

  * POST `/api/v1/contract_user_settlement_records`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | true | string | 品种代码 | "BTC","ETH"...  
start_time | false | long | 起始时间（时间戳，单位毫秒） | 取值范围：[(当前时间 - 90天), 当前时间]
，默认取当前时间- 90天  
end_time | false | long | 结束时间（时间戳，单位毫秒） | 取值范围：(start_time, 当前时间]，默认取当前时间  
page_index | false | int | 页码 | 不填默认第1页  
page_size | false | int | 页大小 | 不填默认20，不得多于50（超过则按照50进行查询）  
  
#### 备注：

  * 默认按时间倒序查询，新数据排在前。
  * 起始时间与结束时间不符合取值范围时，报错1067，参数不合法。
  * 查询结算开始时间在起始时间之后，结束时间之前的用户结算记录数据。

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "total_page": 13,
            "current_page": 1,
            "total_size": 13,
            "settlement_records": [
                {
                    "symbol": "ADA",
                    "margin_balance_init": 436.415907066107795161,
                    "margin_balance": 436.795604223274725677,
                    "settlement_profit_real": 0.379697157166930517,
                    "settlement_time": 1604044800130,
                    "clawback": 0,
                    "delivery_fee": 0,
                    "offset_profitloss": 13.25977319159553892,
                    "fee": -0.565357129977092573,
                    "fee_asset": "ADA",
                    "positions": [
                        {
                            "symbol": "ADA",
                            "contract_code": "ADA201225",
                            "direction": "buy",
                            "volume": 2,
                            "cost_open": 0.098,
                            "cost_hold_pre": 0.098,
                            "cost_hold": 0.092423,
                            "settlement_profit_unreal": -12.31471890445151583,
                            "settlement_price": 0.092423,
                            "settlement_type": "settlement"
                        }
                    ]
                }
            ]
        },
        "ts": 1604305358564
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 |  
<data> | true | object |  |  
<settlement_records> | true | object array |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
margin_balance_init | true | decimal | 本期初始账户权益 |  
margin_balance | true | decimal | 本期结算后账户权益 |  
settlement_profit_real | true | decimal | 本期结算已实现盈亏 |  
settlement_time | true | long | 本期结算时间，交割时为交割时间 |  
clawback | true | decimal | 本期分摊费用 |  
delivery_fee | true | decimal | 本期交割手续费（多空仓位汇总值），仅有仓位进行交割时该字段才有值 |  
offset_profitloss | true | decimal | 本期平仓盈亏 |  
fee | true | decimal | 本期交易手续费 |  
fee_asset | true | string | 手续费币种 |  
<positions> | true | object array |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
contract_code | true | string | 合约代码 | "BTC200619" ...  
direction | true | string | 仓位方向 | "buy":买 "sell":卖  
volume | true | decimal | 本期结算前持仓量（张） |  
cost_open | true | decimal | 开仓均价 |  
cost_hold_pre | true | decimal | 本期结算前持仓均价 |  
cost_hold | true | decimal | 本期结算后持仓均价 |  
settlement_profit_unreal | true | decimal | 本期结算未实现盈亏 |  
settlement_price | true | decimal | 本期结算价格，交割时即为交割价格 |  
settlement_type | true | string | 结算类型 | settlement：结算；delivery：交割；  
</positions> |  |  |  |  
</settlement_records> |  |  |  |  
total_page | true | int | 总页数 |  
current_page | true | int | 当前页 |  
total_size | true | int | 总条数 |  
</data> |  |  |  |  
ts | true | long | 时间戳 |  
  
#### 说明：

  * settlement_time本期结算时间为结算开始时间。
  * 只要用户曾有过资金，就会有结算记录。若查询的用户没有结算记录，则直接返回空数据（data为空数组）

## 查询用户当前的下单量限制

  * POST `/api/v1/contract_order_limit`

> Request:
    
    
    {
        "symbol":"btc",
        "order_price_type":"limit"
    }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol  | false  | string  | 品种代码  | 支持大小写,"BTC","ETH"...，如果缺省，默认返回所有品种  
order_price_type | true | string | 订单报价类型 |
"limit":限价，"opponent":对手价，"lightning":闪电平仓，"optimal_5":最优5档，"optimal_10":最优10档，"optimal_20":最优20档，"fok":FOK订单，"ioc":IOC订单,"opponent_ioc"：
对手价-IOC下单，"lightning_ioc"：闪电平仓-
IOC下单，"optimal_5_ioc"：最优5档-IOC下单，"optimal_10_ioc"：最优10档-IOC下单，"optimal_20_ioc"：最优20档-IOC下单,"opponent_fok"：
对手价-FOK下单，"lightning_fok"：闪电平仓-
FOK下单，"optimal_5_fok"：最优5档-FOK下单，"optimal_10_fok"：最优10档-FOK下单，"optimal_20_fok"：最优20档-FOK下单  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "order_price_type": "limit",
            "list": [
                {
                    "symbol": "ADA",
                    "types": [
                        {
                            "contract_type": "this_week",
                            "open_limit": 6000,
                            "close_limit": 12000
                        },
                        {
                            "contract_type": "next_week",
                            "open_limit": 6000,
                            "close_limit": 12000
                        },
                        {
                            "contract_type": "quarter",
                            "open_limit": 6000,
                            "close_limit": 12000
                        },
                        {
                            "contract_type": "next_quarter",
                            "open_limit": 6000,
                            "close_limit": 12000
                        }
                    ]
                }
            ]
        },
        "ts": 1604306946036
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
order_price_type | true | string | 订单报价类型 |
"limit":限价，"opponent":对手价，"lightning":闪电平仓，"optimal_5":最优5档，"optimal_10":最优10档，"optimal_20":最优20档，"fok":FOK订单，"ioc":IOC订单  
<list> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
<types> |  |  |  |  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter", 次季:"next_quarter"  
open_limit | true | long | 合约开仓单笔下单量最大值 |  
close_limit | true | long | 合约平仓单笔下单量最大值 |  
</types> |  |  |  |  
</list> |  |  |  |  
</data> |  |  |  |  
  
## 查询用户当前的手续费费率

  * POST `/api/v1/contract_fee`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | false | string | 品种代码 | 支持大小写,"BTC","ETH"...，如果缺省，默认返回所有品种  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "open_maker_fee": "0.0002",
                "open_taker_fee": "0.0004",
                "close_maker_fee": "0.0002",
                "close_taker_fee": "0.0004",
                "delivery_fee": "0.0005",
                "fee_asset": "ADA"
            }
        ],
        "ts": 1604307012954
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
fee_asset | true | string | 手续费币种 | "BTC","ETH"...  
open_maker_fee | true | string | 开仓挂单的手续费费率，小数形式 |  
open_taker_fee | true | string | 开仓吃单的手续费费率，小数形式 |  
close_maker_fee | true | string | 平仓挂单的手续费费率，小数形式 |  
close_taker_fee | true | string | 平仓吃单的手续费费率，小数形式 |  
delivery_fee | true | string | 交割的手续费费率，小数形式 |  
</data> |  |  |  |  
  
## 查询用户当前的划转限制

  * POST `/api/v1/contract_transfer_limit`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | false | string | 品种代码 | 支持大小写,"BTC","ETH"...，如果缺省，默认返回所有品种  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "transfer_in_max_each": 1500000000,
                "transfer_in_min_each": 16,
                "transfer_out_max_each": 150000000,
                "transfer_out_min_each": 0.000001,
                "transfer_in_max_daily": 15000000000,
                "transfer_out_max_daily": 3000000000,
                "net_transfer_in_max_daily": 7500000000,
                "net_transfer_out_max_daily": 1500000000
            }
        ],
        "ts": 1604307084954
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
transfer_in_max_each | true | decimal | 单笔最大转入量 |  
transfer_in_min_each | true | decimal | 单笔最小转入量 |  
transfer_out_max_each | true | decimal | 单笔最大转出量 |  
transfer_out_min_each | true | decimal | 单笔最小转出量 |  
transfer_in_max_daily | true | decimal | 单日累计最大转入量 |  
transfer_out_max_daily | true | decimal | 单日累计最大转出量 |  
net_transfer_in_max_daily | true | decimal | 单日累计最大净转入量 |  
net_transfer_out_max_daily | true | decimal | 单日累计最大净转出量 |  
</data> |  |  |  |  
  
## 用户持仓量限制的查询

  * post `/api/v1/contract_position_limit`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | false | string | 品种代码 | 支持大小写,"BTC","ETH"...，如果缺省，默认返回所有品种  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "list": [
                    {
                        "contract_type": "this_week",
                        "buy_limit": 60000,
                        "sell_limit": 60000
                    },
                    {
                        "contract_type": "next_week",
                        "buy_limit": 60000,
                        "sell_limit": 60000
                    },
                    {
                        "contract_type": "quarter",
                        "buy_limit": 60000,
                        "sell_limit": 60000
                    },
                    {
                        "contract_type": "next_quarter",
                        "buy_limit": 60000,
                        "sell_limit": 60000
                    },
                    {
                        "contract_type": "all",
                        "buy_limit": 240000,
                        "sell_limit": 240000
                    }
                ]
            }
        ],
        "ts": 1604307195501
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
<list> |  |  |  |  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter"，次季：“next_quarter”， 所有合约:“all”  
buy_limit | true | decimal | 合约多仓持仓的最大值，单位为张 |  
sell_limit | true | decimal | 合约空仓持仓的最大值，单位为张 |  
</list> |  |  |  |  
</data> |  |  |  |  
  
## 查询用户账户和持仓信息

  * post `/api/v1/contract_account_position_info`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | true | string | 品种代码 | 支持大小写,"BTC","ETH"...  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "margin_balance": 405.226124145843792312,
                "margin_position": 10.300252356182726476,
                "margin_frozen": 0,
                "margin_available": 394.925871789661065836,
                "profit_real": 16.336169922800328615,
                "profit_unreal": 2.09434999976873802,
                "risk_rate": 39.141378262699244579,
                "withdraw_available": 386.795604223274725677,
                "liquidation_price": null,
                "lever_rate": 10,
                "adjust_factor": 0.2,
                "margin_static": 403.131774146075054292,
                "positions": [
                    {
                        "symbol": "ADA",
                        "contract_code": "ADA201225",
                        "contract_type": "quarter",
                        "volume": 1,
                        "available": 1,
                        "frozen": 0,
                        "cost_open": 0.0991,
                        "cost_hold": 0.0991,
                        "profit_unreal": 2.09434999976873802,
                        "profit_rate": 0.20755008497708193,
                        "lever_rate": 10,
                        "position_margin": 10.300252356182726476,
                        "direction": "sell",
                        "profit": 2.09434999976873802,
                        "last_price": 0.097085
                    }
                ]
            }
        ],
        "ts": 1604307305267
    }
    

### 返回参数

属性 | 数据类型 | 是否必填 | 说明  
---|---|---|---  
status | true | string | 请求处理结果 "ok" , "error"  
ts | long | long | 响应生成时间点，单位：毫秒  
<data> | true | object array |  
symbol | string | true | 合约品种  
margin_balance | decimal | true | 账户权益  
margin_position | decimal | true | 持仓保证金  
margin_frozen | decimal | true | 冻结保证金  
margin_available | decimal | true | 可用保证金  
profit_real | decimal | true | 已实现盈亏  
profit_unreal | decimal | true | 未实现盈亏  
risk_rate | decimal | true | 保证金率  
withdraw_available | decimal | true | 可划转数量  
liquidation_price | decimal | true | 预估爆仓价  
lever_rate | int | true | 杠杆倍数  
adjust_factor | float | true | 调整系数  
margin_static | decimal | true | 静态权益  
<positions> |  |  |  
symbol | string | true | 合约品种  
contract_code | string | true | 合约代码 "BTC180914" ...  
contract_type | string | true | 合约类型 当周:"this_week", 次周:"next_week",
当季:"quarter", 次季:"next_quarter"  
volume | decimal | true | 持仓量  
available | decimal | true | 可平仓数量  
frozen | decimal | true | 冻结数量  
cost_open | decimal | true | 开仓均价  
cost_hold | decimal | true | 持仓均价  
profit_unreal | decimal | true | 未实现盈亏  
profit_rate | decimal | true | 收益率  
profit | decimal | true | 收益  
position_margin | decimal | true | 持仓保证金  
lever_rate | int | true | 杠杆倍数  
direction | string | true | "buy":买 "sell":卖  
last_price | decimal | true | 最新价  
</positions> |  |  |  
</data> |  |  |  
  
## 母子账户划转

  * post `/api/v1/contract_master_sub_transfer`

> Request:
    
    
    {
        "sub_uid": "123456789",
        "symbol": "BTC",
        "amount": "123",
        "type": "master_to_sub"
    }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
sub_uid | true | long | 子账号uid |  
symbol | true | string | 品种代码 | 支持大小写,"BTC","ETH"...  
amount | true | decimal | 划转金额 |  
type | true | string | 划转类型 | 仅支持小写,master_to_sub：母账户划转到子账户，
sub_to_master：子账户划转到母账户  
  
### 备注：

母账户与每个子账户相互划转限频10次/分钟。

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "order_id": "772874532490125313"
        },
        "ts": 1604309247876
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> | true | object |  |  
order_id | true | string | 划转订单ID |  
</data> |  |  |  |  
  
## 获取母账户下的所有母子账户划转记录

  * post `/api/v1/contract_master_sub_transfer_record`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | true | string | 品种代码 | 支持大小写, "BTC","ETH"...  
transfer_type | false | string | 划转类型，不填查询全部类型,【查询多类型中间用，隔开】 | 34:转出到子账号合约账户
35:从子账号合约账户转入  
create_date | true | int | 日期 | 可随意输入正整数，如果参数超过90则默认查询90天的数据  
page_index | false | int | 页码，不填默认第1页 |  
page_size | false | int | 不填默认20，不得多于50 | [1-50]  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "total_page": 1,
            "current_page": 1,
            "total_size": 2,
            "transfer_record": [
                {
                    "id": 3657499070,
                    "symbol": "ADA",
                    "transfer_type": 34,
                    "amount": -1,
                    "ts": 1604309247860,
                    "sub_uid": "123456789",
                    "sub_account_name": "tom"
                },
                {
                    "id": 3657420904,
                    "symbol": "ADA",
                    "transfer_type": 34,
                    "amount": -50,
                    "ts": 1604301623314,
                    "sub_uid": "123456789",
                    "sub_account_name": "tom"
                }
            ]
        },
        "ts": 1604309883224
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> | true | object |  |  
<transfer_record> | true | object array |  |  
id | true | long | 划转订单ID |  
ts | true | long | 创建时间 |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
sub_uid | true | string | 子账户UID |  
sub_account_name | true | string | 子账户登录名 |  
transfer_type | true | int | 划转类型 | 从子账号合约账户转入：35，转出到子账号合约账户:34  
amount | true | decimal | 金额 |  
</transfer_record> |  |  |  |  
total_page | true | int | 总页数 |  
current_page | true | int | 当前页 |  
total_size | true | int | 总条数 |  
</data> |  |  |  |  
  
## 获取用户的API指标禁用信息

  * get `/api/v1/contract_api_trading_status`

### 请求参数

无

### Response:

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> | true | array object |  |  
is_disable | true | long | 是否被禁用ID | 1：被禁用中，0：没有被禁用  
order_price_types | true | string |
触发禁用的订单价格类型，多个订单价格类型以英文逗号分割，例如：“limit,post_only,FOK,IOC” |  
disable_reason | true | string | 触发禁用的原因，表示当前的禁用是由哪个指标触发 | "COR":撤单率（Cancel
Order Ratio），“TDN”：总禁用次数（Total Disable Number）  
disable_interval | true | long | 禁用时间间隔，单位：毫秒 |  
recovery_time | true | long | 计划恢复时间，单位：毫秒 |  
<COR> | true | dict object | 表示撤单率的指标（Cancel Order Ratio） |  
orders_threshold | true | long | 委托单笔数的阈值 |  
orders | true | long | 用户委托单笔数的实际值 |  
invalid_cancel_orders | true | long | 用户委托单中的无效撤单笔数 |  
cancel_ratio_threshold | true | decimal | 撤单率的阈值 |  
cancel_ratio | true | decimal | 用户撤单率的实际值 |  
is_trigger | true | int | 用户是否触发该指标 | 1：已经触发，0：没有触发  
is_active | true | int | 该指标是否开启 | 1：已启用，0：未启用  
</COR> |  |  |  |  
<TDN> | true | dict object | 表示总禁用次数的指标（Total Disable Number） |  
disables_threshold | true | long | 总禁用次数的阈值 |  
disables | true | long | 总禁用次数的实际值 |  
is_trigger | true | long | 用户是否触发该指标 | 1：已经触发，0：没有触发  
is_active | true | long | 该指标是否开启 | 1：已启用，0：未启用  
</TDN> |  |  |  |  
</data> |  |  |  |  
  
> 例子：
    
    
      {
      "status": "ok",
      "data":
      [{
          "is_disable": 1,   //是否被禁用
          "order_price_types": “limit,post_only,FOK,IOC”,  // 触发禁用的订单价格类型
          "disable_reason":"COR",  // 触发禁用的原因
          "disable_interval": 5,  // 禁用时间间隔
          "recovery_time": 1, // 计划恢复时间
          "COR":  //撤单率的指标（Cancel Order Ratio）
           {
               "orders_threshold": 150,  //委托单笔数的阈值
               "orders": 150,  //用户委托单笔数的实际值
               "invalid_cancel_orders": 150,  //委托单中的无效撤单笔数 
               "cancel_ratio_threshold": 0.98,   //撤单率的阈值
               "cancel_ratio": 0.98,   //用户撤单率的实际值
               "is_trigger": 1,  //用户是否触发该指标
               "is_active": 1   //该指标是否开启
          } ,
          "TDN":  //总禁用次数的指标（Total  Disable Number）
           {
               "disables_threshold": 3,  //总禁用次数的阈值
               "disables": 3,  /总禁用次数的实际值
               "is_trigger": 1,  //用户是否触发该指标
               "is_active": 1   //该指标是否开启
          } 
       }],
     "ts": 158797866555
    }
    
    
    

## 查询用户可用杠杆倍数

  * Post `/api/v1/contract_available_level_rate`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | false | string | 品种代码（大小写不敏感，均支持），不填默认返回所有品种的实际可用杠杆倍数 | 比如"BTC","ETH"  
  
### Response:

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> | true | array object |  |  
symbol | true | string | 品种 | 比如 "BTC"  
available_level_rate | true | string | 实际可用杠杆倍数，多个以英文逗号隔开 | 比如 "1,5,10"  
</data> |  |  |  |  
  
> 回复例子:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "available_level_rate": "1,2,3,5,10,20,30,50,75"
            }
        ],
        "ts": 1604312615051
    }
    

# 合约交易接口

## 合约下单

### 示例

  * POST `/api/v1/contract_order`

> Request:
    
    
    {
        "client_order_id":11223344556677,
        "contract_code":"btc200925",
        "contract_type":"quarter",
        "direction":"BUY",
        "lever_rate":75,
        "offset":"OPEN",
        "order_price_type":"post_only",
        "price":9988,
        "symbol":"btc",
        "volume":1
    }
    

### 请求参数

参数名 | 参数类型 | 必填 | 描述  
---|---|---|---  
symbol | string | false | 支持大小写,"BTC","ETH"...  
contract_type | string | false | 合约类型 ("this_week":当周 "next_week":下周
"quarter":当季 "next_quarter":次季)  
contract_code | string | false | BTC180914  
client_order_id | long | false | 客户自己填写和维护，必须为数字,请注意必须小于等于9223372036854775807  
price | decimal | false | 价格  
volume | long | true | 委托数量(张)  
direction | string | true | "buy":买 "sell":卖  
offset | string | true | "open":开 "close":平  
lever_rate | int | true | 杠杆倍数[“开仓”若有10倍多单，就不能再下20倍多单,
"平仓"可以不填杠杆倍数;首次使用高倍杠杆(>20倍)，请使用主账号登录web端同意高倍杠杆协议后，才能使用接口下高倍杠杆(>20倍)]  
order_price_type | string | true | 订单报价类型 "limit":限价 "opponent":对手价
"post_only":只做maker单,post
only下单只受用户持仓数量限制,optimal_5：最优5档、optimal_10：最优10档、optimal_20：最优20档，ioc:IOC订单，fok：FOK订单,
"opponent_ioc"： 对手价-
IOC下单，"optimal_5_ioc"：最优5档-IOC下单，"optimal_10_ioc"：最优10档-IOC下单，"optimal_20_ioc"：最优20档-IOC下单,"opponent_fok"：
对手价-
FOK下单，"optimal_5_fok"：最优5档-FOK下单，"optimal_10_fok"：最优10档-FOK下单，"optimal_20_fok"：最优20档-FOK下单  
  
### 备注

如果contract_code填了值，那就按照contract_code去下单，如果contract_code没有填值，则按照symbol+contract_type去下单。

对手价下单price价格参数不用传，对手价下单价格是买一和卖一价,optimal_5：最优5档、optimal_10：最优10档、optimal_20：最优20档下单price价格参数不用传，"limit":限价，"post_only":只做maker单
需要传价格，"fok"：全部成交或立即取消，"ioc":立即成交并取消剩余。

Post only(也叫maker only订单，只下maker单)每个周期合约的开仓/平仓的下单数量限制为500000，同时也会受到用户持仓数量限制。

若存在持仓，那么下单时杠杆倍数必须与持仓杠杆相同，否则下单失败。若需使用新杠杆下单，则必须先使用切换杠杆接口将持仓杠杆切换成功后再下单。

### 开平方向

开多：买入开多(direction用buy、offset用open)

平多：卖出平多(direction用sell、offset用close)

开空：卖出开空(direction用sell、offset用open)

平空：买入平空(direction用buy、offset用close)

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "order_id": 773119326353580033,
            "order_id_str": "773119326353580033"
        },
        "ts": 1604367611267
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
order_id | true | long | 订单ID |  
order_id_str | true | string | string类型订单ID |  
client_order_id | true | int | 用户下单时填写的客户端订单ID，没填则不返回 |  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
### 备注

order_id返回是18位，nodejs和javascript默认解析18有问题，nodejs和javascript里面JSON.parse默认是int，超过18位的数字用json-
bigint的包解析。

## 合约批量下单

  * POST `/api/v1/contract_batchorder`

> Request:
    
    
    {
        "orders_data":[
            {
                "clientOrderId":11223344556688,
                "contract_code":"btc200925",
                "contract_type":"quarter",
                "direction":"BUY",
                "leverRate":75,
                "offset":"OPEN",
                "order_price_type":"post_only",
                "price":9988,
                "symbol":"btc",
                "volume":1
            },
            {
                "clientOrderId":11223344556699,
                "contract_code":"btc200925",
                "contract_type":"quarter",
                "direction":"BUY",
                "leverRate":75,
                "offset":"OPEN",
                "order_price_type":"post_only",
                "price":9988,
                "symbol":"btc",
                "volume":1
            }
        ]
    }
    

### 请求参数

参数名 | 参数类型 | 必填 | 描述  
---|---|---|---  
orders_data | List<Object> | 一次最多10个订单 |  
  
### orders_data参数对象详情：

参数名 | 参数类型 | 必填 | 描述  
---|---|---|---  
symbol | string | false | 支持大小写,"BTC","ETH"...  
contract_type | string | false | 合约类型: "this_week":当周 "next_week":下周
"quarter":当季 "next_quarter":次季  
contract_code | string | false | BTC180914  
client_order_id | long | false | 客户自己填写和维护，必须为数字,请注意必须小于等于9223372036854775807  
price | decimal | false | 价格  
volume | long | true | 委托数量(张)  
direction | string | true | "buy":买 "sell":卖  
offset | string | true | "open":开 "close":平  
leverRate | int | true |
杠杆倍数[“开仓”若有10倍多单，就不能再下20倍多单;首次使用高倍杠杆(>20倍)，请使用主账号登录web端同意高倍杠杆协议后，才能使用接口下高倍杠杆(>20倍)]  
orderPriceType | string | true | 订单报价类型 "limit":限价 "opponent":对手价
"post_only":只做maker单,post
only下单只受用户持仓数量限制,optimal_5：最优5档、optimal_10：最优10档、optimal_20：最优20档，ioc：IOC订单，fok：FOK订单,"opponent_ioc"：
对手价-
IOC下单，"optimal_5_ioc"：最优5档-IOC下单，"optimal_10_ioc"：最优10档-IOC下单，"optimal_20_ioc"：最优20档-IOC下单,"opponent_fok"：
对手价-
FOK下单，"optimal_5_fok"：最优5档-FOK下单，"optimal_10_fok"：最优10档-FOK下单，"optimal_20_fok"：最优20档-FOK下单  
  
### 备注

如果contract_code填了值，那就按照contract_code去下单，如果contract_code没有填值，则按照symbol+contract_type去下单。

对手价下单price价格参数不用传，对手价下单价格是买一和卖一价,optimal_5：最优5档、optimal_10：最优10档、optimal_20：最优20档下单price价格参数不用传，"limit":限价，"post_only":只做maker单
需要传价格，"fok"：全部成交或立即取消，"ioc":立即成交并取消剩余。

若存在持仓，那么下单时杠杆倍数必须与持仓杠杆相同，否则下单失败。若需使用新杠杆下单，则必须先使用切换杠杆接口将持仓杠杆切换成功后再下单。

请注意：一次最多允许10个订单。

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "errors": [
                {
                    "index": 1,
                    "err_code": 1037,
                    "err_msg": "The leverage is invalid. Please contact the customer service."
                }
            ],
            "success": [
                {
                    "order_id": 773120304138219520,
                    "index": 2,
                    "order_id_str": "773120304138219520"
                }
            ]
        },
        "ts": 1604367844388
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
<errors> |  |  |  |  
index | true | int | 订单索引 |  
err_code | true | int | 错误码 |  
err_msg | true | string | 错误信息 |  
</errors> |  |  |  |  
<success> |  |  |  |  
index | true | int | 订单索引 |  
order_id | true | long | 订单ID |  
order_id_str | true | string | 订单ID |  
client_order_id | true | long | 用户下单时填写的客户端订单ID，没填则不返回 |  
</success> |  |  |  |  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
### 备注

order_id返回是18位，nodejs和javascript默认解析18有问题，nodejs和javascript里面JSON.parse默认是int，超过18位的数字用json-
bigint的包解析。

## 撤销订单

### 示例

  * POST `/api/v1/contract_cancel`

> Request:
    
    
    {
        "client_order_id":"11223344556688,11223344556699",
        "order_id":"634696656176029696,634693443368525824",
        "symbol":"btc"
    }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述  
---|---|---|---  
order_id | false | string | 订单ID(多个订单ID中间以","分隔,一次最多允许撤消10个订单)  
client_order_id | false | string | 客户订单ID(多个订单ID中间以","分隔,一次最多允许撤消10个订单)  
symbol | true | string | 支持大小写,"BTC","ETH"...  
  
### 备注：

  * order_id和client_order_id都可以用来撤单，同时只可以设置其中一种，如果设置了两种，默认以order_id来撤单。

  * 撤单接口返回结果只代表撤单命令发送成功，建议根据订单查询接口查询订单的状态来确定订单是否已真正撤销。

  * client_order_id，24小时有效，超过24小时的订单根据client_order_id将查询不到。

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "errors": [
                {
                    "order_id": "769206471845261312",
                    "err_code": 1061,
                    "err_msg": "This order doesnt exist."
                }
            ],
            "successes": "773120304138219520"
        },
        "ts": 1604367997451
    } 
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
<errors> |  |  |  |  
order_id | true | string | 订单ID |  
err_code | true | int | 错误码 |  
err_msg | true | string | 错误信息 |  
</errors> |  |  |  |  
successes | true | string | 撤销成功的订单的order_id或client_order_id列表 |  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
## 全部撤单

### 示例

  * POST `/api/v1/contract_cancelall`

> Request:
    
    
    {
        "symbol":"btc",
        "contract_code":"btc200925",
        "contract_type":"quarter"
    }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述  
---|---|---|---  
symbol | true | string | 品种代码，支持大小写，如"BTC","ETH"...  
contract_code | false | string | 合约code  
contract_type | false | string | 合约类型  
  
### 备注

  * 只传symbol，撤该该品种下所有周期的合约
  * 只要有contract_code，则撤销该code的合约
  * 只传symbol+contract_type， 则撤销二者拼接所成的合约订单

> Response:(多笔订单返回结果(成功订单ID,失败订单ID))
    
    
    {
        "status": "ok",
        "data": {
            "errors": [],
            "successes": "773120045672095744,773120045684678656"
        },
        "ts": 1604369127577
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
<errors> |  |  |  |  
order_id | true | string | 订单id |  
err_code | true | int | 订单失败错误码 |  
err_msg | true | string | 订单失败信息 |  
</errors> |  |  |  |  
successes | true | string | 成功的订单 |  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
## 切换杠杆

  * POST `/api/v1/contract_switch_lever_rate`

#### 备注

  * 只有在单个品种下只有持仓，且没有挂单的场景下，才可以切换该品种当前的倍数。

  * 接口限制请求次数为每3秒一次。

### 请求参数

**参数名称** | **是否必须** | **类型** | **描述** | **取值范围**  
---|---|---|---|---  
symbol | true | String | 品种代码 | "BTC","ETH"...  
lever_rate | true | int |
要切换的杠杆倍数。[首次使用高倍杠杆(>20倍)，请使用主账号登录web端同意高倍杠杆协议后，才能使用接口下高倍杠杆(>20倍)] |  
  
> Response:
    
    
    正确：
    
    {
        "status": "ok",
        "data": {
            "symbol": "ada",
            "lever_rate": 20
        },
        "ts": 1604369902689
    }
    错误：
    
    {
        "status": "error",
        "err_code": 1037,
        "err_msg": "The leverage is invalid. Please contact the customer service.",
        "ts": 1604369954194
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 响应状态: ok,error |  
<data> | false | object |  |  
symbol | false | string | 品种代码 |  
lever_rate | false | int | 切换成功后的杠杆倍数 |  
</data> |  |  |  |  
err_code | false | int | 错误码 |  
err_msg | false | string | 错误信息 |  
ts | true | long | 时间戳 |  
  
## 获取合约订单信息

### 示例

  * POST `/api/v1/contract_order_info`

### 请求参数

> Request:
    
    
    {
        "client_order_id":"11223344556688,11223344556699",
        "order_id":"634696656176029696,634693443368525824",
        "symbol":"btc"
    }
    

参数名称 | 是否必须 | 类型 | 描述  
---|---|---|---  
order_id | false | string | 订单ID(多个订单ID中间以","分隔,一次最多允许查询50个订单)  
client_order_id | false | string | 客户订单ID(多个订单ID中间以","分隔,一次最多允许查询50个订单)  
symbol | true | string | 支持大小写，"BTC","ETH"...  
  
### 备注：

  * 最多只能查询 4 小时内的撤单信息。

  * order_id和client_order_id至少要填写一个。

  * order_id和client_order_id都可以用来查询，同时只可以设置其中一种，如果设置了两种，默认以order_id来查询。周五交割结算后，会把结束状态的订单（5部分成交已撤单 6全部成交 7已撤单）删除掉。

  * client_order_id，24小时有效，超过24小时的订单根据client_order_id将查询不到。

> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "contract_code": "ADA201225",
                "contract_type": "quarter",
                "volume": 1,
                "price": 0.0933,
                "order_price_type": "post_only",
                "order_type": 1,
                "direction": "sell",
                "offset": "open",
                "lever_rate": 10,
                "order_id": 773119326353580033,
                "client_order_id": null,
                "created_at": 1604367611263,
                "trade_volume": 1,
                "trade_turnover": 10,
                "fee": -0.021436227224008574,
                "trade_avg_price": 0.0933,
                "margin_frozen": 0,
                "profit": 0,
                "status": 6,
                "order_source": "api",
                "order_id_str": "773119326353580033",
                "fee_asset": "ADA",
                "liquidation_type": "0",
                "canceled_at": 0
            }
        ],
        "ts": 1604370179844
    }
    

### 返回数据

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
symbol | true | string | 品种代码 |  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter",次季:"next_quarter"  
contract_code | true | string | 合约代码 | "BTC180914" ...  
volume | true | decimal | 委托数量 |  
price | true | decimal | 委托价格 |  
order_price_type | true | string | 订单报价类型 | 订单报价类型 订单报价类型 "limit":限价
"opponent":对手价 "post_only":只做maker单,post
only下单只受用户持仓数量限制,optimal_5：最优5档、optimal_10：最优10档、optimal_20：最优20档，ioc:IOC订单，fok：FOK订单  
direction | true | string | 买卖方向 | "buy":买 "sell":卖  
offset | true | string | 开平方向 | "open":开 "close":平  
lever_rate | true | int | 杠杆倍数 | 1\5\10\20  
order_id | true | long | 订单ID |  
order_id_str | true | string | String类型订单ID |  
client_order_id | true | long | 客户订单ID |  
created_at | true | long | 创建时间 |  
canceled_at | true | long | 撤单时间 |  
trade_volume | true | decimal | 成交数量 |  
trade_turnover | true | decimal | 成交总金额 |  
fee | true | decimal | 手续费 |  
trade_avg_price | true | decimal | 成交均价 |  
margin_frozen | true | decimal | 冻结保证金 |  
profit | true | decimal | 收益 |  
status | true | int | 订单状态 | (1准备提交 2准备提交 3已提交 4部分成交 5部分成交已撤单 6全部成交 7已撤单
11撤单中)  
order_type | true | int | 订单类型 | 1:报单 、 2:撤单 、 3:强平、4:交割  
order_source | true | string | 订单来源 |
（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
fee_asset | true | string | 手续费币种 | （"BTC","ETH"...）  
liquidation_type | true | string | 强平类型 | 0:非强平类型，1：多空轧差， 2:部分接管，3：全部接管  
</data> |  |  |  |  
ts | true | long | 时间戳 |  
  
## 获取订单明细信息

### 示例

  * POST `/api/v1/contract_order_detail`

> Request:
    
    
    {
        "created_at":1593765713010,
        "order_id":727181510507044864,
        "order_type":1,
        "page_index":1,
        "page_size":20,
        "symbol":"BTC"
    }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述  
---|---|---|---  
symbol | true | string | 支持大小写,"BTC","ETH"...  
order_id | true | long | 订单id  
created_at | false | long | 下单时间戳  
order_type | false | int | 订单类型，1:报单 、 2:撤单 、 3:强平、4:交割  
page_index | false | int | 第几页,不填第一页  
page_size | false | int | 不填默认20,不得多于50  
  
### 备注

获取订单明细接口查询撤单数据时，如果传“created_at”和“order_type”参数则能查询最近24小时数据，如果不传“created_at”和“order_type”参数只能查询到最近2小时数据。

order_id返回是18位，nodejs和javascript默认解析18有问题，nodejs和javascript里面JSON.parse默认是int，超过18位的数字用json-
bigint的包解析。

created_at使用13位long类型时间戳（包含毫秒时间），如果输入准确的时间戳，查询性能将会提升。例如:"2019/10/18
10:26:22"转换为时间戳为：1571365582123。也可以直接从contract_order下单接口返回的ts中获取时间戳查询对应的订单。

created_at禁止传0。

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "symbol": "ADA",
            "contract_code": "ADA201225",
            "contract_type": "quarter",
            "instrument_price": 0,
            "final_interest": 0,
            "adjust_value": 0,
            "lever_rate": 10,
            "direction": "sell",
            "offset": "open",
            "volume": 1,
            "price": 0.0933,
            "created_at": 1604367611263,
            "canceled_at": 0,
            "order_source": "api",
            "order_price_type": "post_only",
            "margin_frozen": 0,
            "profit": 0,
            "trades": [
                {
                    "trade_id": 113887800667,
                    "trade_price": 0.0933,
                    "trade_volume": 1,
                    "trade_turnover": 10,
                    "trade_fee": -0.021436227224008574,
                    "created_at": 1604368087894,
                    "role": "maker",
                    "id": "113887800667-773119326353580033-1"
                }
            ],
            "total_page": 1,
            "current_page": 1,
            "total_size": 1,
            "liquidation_type": "0",
            "fee_asset": "ADA",
            "order_id": 773119326353580033,
            "order_id_str": "773119326353580033",
            "client_order_id": null,
            "order_type": "1",
            "status": 6,
            "trade_avg_price": 0.0933,
            "trade_turnover": 10,
            "trade_volume": 1,
            "fee": -0.021436227224008574
        },
        "ts": 1604370259827
    }
    

### 返回数据

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
symbol | true | string | 品种代码 |  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter",次季:"next_quarter"  
contract_code | true | string | 合约代码 | "BTC180914" ...  
lever_rate | true | int | 杠杆倍数 | 1,5,10,20  
direction | true | string | 买卖方向 | "buy":买 "sell":卖  
offset | true | string | 开平方向 | "open":开 "close":平  
volume | true | decimal | 委托数量 |  
price | true | decimal | 委托价格 |  
created_at | true | long | 创建时间 |  
canceled_at | true | long | 撤单时间 |  
order_source | true | string | 订单来源 |
（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
order_price_type | true | string | 订单报价类型 | 订单报价类型 "limit":限价 "opponent":对手价
"post_only":只做maker单,post
only下单只受用户持仓数量限制,optimal_5：最优5档、optimal_10：最优10档、optimal_20：最优20档，ioc:IOC订单，fok：FOK订单  
margin_frozen | true | decimal | 冻结保证金 |  
profit | true | decimal | 收益 |  
total_page | true | int | 总共页数 |  
current_page | true | int | 当前页数 |  
total_size | true | int | 总条数 |  
instrument_price | true | decimal | 爆仓单合约价格 |  
final_interest | true | decimal | 爆仓时合约权益 |  
adjust_value | true | decimal | 爆仓时调整系数 |  
fee_asset | true | string | 手续费币种 | （"BTC","ETH"...）  
liquidation_type | true | string | 强平类型 | 0:非强平类型，1：多空轧差， 2:部分接管，3：全部接管  
order_id | true | long | 订单ID |  
order_id_str | true | string | String类型订单ID |  
client_order_id | true | long | 客户订单ID |  
trade_volume | true | decimal | 成交数量 |  
trade_turnover | true | decimal | 成交总金额 |  
fee | true | decimal | 手续费 |  
trade_avg_price | true | decimal | 成交均价 |  
status | true | int | 订单状态 | (1准备提交 2准备提交 3已提交 4部分成交 5部分成交已撤单 6全部成交 7已撤单
11撤单中)  
order_type | true | int | 订单类型 | 1:报单 、 2:撤单 、 3:强平、4:交割  
<trades> |  |  |  |  
id | true | string | 全局唯一的交易标识 |  
trade_id | true | long |
与api/v1/contract_matchresults返回结果中的match_id一样，是撮合结果id，
非唯一，可重复，注意：一个撮合结果代表一个taker单和N个maker单的成交记录的集合，如果一个taker单吃了N个maker单，那这N笔trade都是一样的撮合结果id
|  
trade_price | true | decimal | 撮合价格 |  
trade_volume | true | decimal | 成交量 |  
trade_turnover | true | decimal | 成交金额 |  
trade_fee | true | decimal | 成交手续费 |  
role | true | string | taker或maker |  
created_at | true | long | 创建时间 |  
</trades> |  |  |  |  
</data > |  |  |  |  
ts | true | long | 时间戳 |  
  
## 获取合约当前未成交委托

### 示例

  * POST `/api/v1/contract_openorders`  

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 品种代码 |  | 支持大小写, "BTC","ETH"...  
page_index | false | int | 页码，不填默认第1页 | 1 |  
page_size | false | int | 不填默认20，不得多于50 | 20 | [1-50]  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "symbol": "ADA",
                    "contract_code": "ADA201225",
                    "contract_type": "quarter",
                    "volume": 1,
                    "price": 0.0925,
                    "order_price_type": "post_only",
                    "order_type": 1,
                    "direction": "buy",
                    "offset": "close",
                    "lever_rate": 20,
                    "order_id": 773131315209248768,
                    "client_order_id": null,
                    "created_at": 1604370469629,
                    "trade_volume": 0,
                    "trade_turnover": 0,
                    "fee": 0,
                    "trade_avg_price": null,
                    "margin_frozen": 0,
                    "profit": 0,
                    "status": 3,
                    "order_source": "web",
                    "order_id_str": "773131315209248768",
                    "fee_asset": "ADA",
                    "liquidation_type": null,
                    "canceled_at": null
                }
            ],
            "total_page": 1,
            "current_page": 1,
            "total_size": 1
        },
        "ts": 1604370488518
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 |  
<data> |  |  |  |  
<orders> |  |  |  |  
symbol | true | string | 品种代码 |  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter",次季:"next_quarter"  
contract_code | true | string | 合约代码 | "BTC180914" ...  
volume | true | decimal | 委托数量 |  
price | true | decimal | 委托价格 |  
order_price_type | true | string | 订单报价类型 | "limit":限价 "opponent":对手价
"post_only":只做maker单,post only下单只受用户持仓数量限制  
order_type | true | int | 订单类型 | 1:报单 、 2:撤单 、 3:强平、4:交割  
direction | true | string | 买卖方向 | "buy":买 "sell":卖  
offset | true | string | 开平方向 | "open":开 "close":平  
lever_rate | true | int | 杠杆倍数 | 1,5,10,20  
order_id | true | long | 订单ID |  
order_id_str | true | string | String订单ID |  
client_order_id | true | long | 客户订单ID |  
created_at | true | long | 订单创建时间 |  
trade_volume | true | decimal | 成交数量 |  
trade_turnover | true | decimal | 成交总金额 |  
fee | true | decimal | 手续费 |  
trade_avg_price | true | decimal | 成交均价 |  
margin_frozen | true | decimal | 冻结保证金 |  
profit | true | decimal | 收益 |  
status | true | int | 订单状态 | (3未成交， 4部分成交， 5部分成交已撤单， 6全部成交， 7已撤单)  
order_source | true | string | 订单来源 |
（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
fee_asset | true | string | 手续费币种 | （"BTC","ETH"...）  
</orders> |  |  |  |  
total_page | true | int | 总页数 |  
current_page | true | int | 当前页 |  
total_size | true | int | 总条数 |  
</data> |  |  |  |  
ts | true | long | 时间戳 |  
  
## 获取合约历史委托

### 示例

  * POST `/api/v1/contract_hisorders`

> Request:
    
    
    {
        "symbol": "BTC",
        "trade_type": 0,
        "type": 1,
        "status": "0,3,4,5",
        "create_date": 1,
        "page_index": 1,
        "page_size": 20,
        "contract_code": "BTC180914",
        "order_type": "limit"
    }
    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 品种代码 |  | 支持大小写,"BTC","ETH"...  
trade_type | true | int | 交易类型 |  | 0:全部,1:买入开多,2: 卖出开空,3: 买入平空,4: 卖出平多,5:
卖出强平,6: 买入强平,7:交割平多,8: 交割平空, 11:减仓平多，12:减仓平空  
type | true | int | 类型 |  | 1:所有订单,2:结束状态的订单  
status | true | string | 订单状态 |  | 可查询多个状态，"3,4,5" , 0:全部,3:未成交, 4: 部分成交,5:
部分成交已撤单,6: 全部成交,7:已撤单  
create_date | true | int | 日期 |  | 可随意输入正整数, ，如果参数超过90则默认查询90天的数据  
page_index | false | int | 页码，不填默认第1页 | 1 |  
page_size | false | int | 每页条数，不填默认20,不得多于50 | 20 | [1-50]  
contract_code | false | string | 合约代码 |  |  
order_type | false | string | 订单类型 |  |
1：限价单、3：对手价、4：闪电平仓、5：计划委托、6：post_only、7：最优5档、8：最优10档、9：最优20档、10：fok、11：ioc  
  
### 备注

  * 所有已撤销且无成交的API限价订单记录只保留最近2小时。

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "order_id": 773131315209248768,
                    "contract_code": "ADA201225",
                    "symbol": "ADA",
                    "lever_rate": 20,
                    "direction": "buy",
                    "offset": "close",
                    "volume": 1,
                    "price": 0.0925,
                    "create_date": 1604370469629,
                    "order_source": "web",
                    "order_price_type": 6,
                    "order_type": 1,
                    "margin_frozen": 0,
                    "profit": 0,
                    "contract_type": "quarter",
                    "trade_volume": 0,
                    "trade_turnover": 0,
                    "fee": 0,
                    "trade_avg_price": 0,
                    "status": 3,
                    "order_id_str": "773131315209248768",
                    "fee_asset": "ADA",
                    "liquidation_type": "0"
                }
            ],
            "total_page": 19,
            "current_page": 1,
            "total_size": 19
        },
        "ts": 1604370617322
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status  | true  | string | 请求处理结果  |  
<data> |  |  |  |  
<orders> |  |  |  |  
order_id | true | long | 订单ID |  
order_id_str | true | string | String类型订单ID |  
symbol | true | string | 品种代码 |  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter", 次季:"next_quarter"  
contract_code | true | string | 合约代码 | "BTC180914" ...  
lever_rate | true | int | 杠杆倍数 | 1,5,10,20  
direction | true | string | 买卖方向 | "buy":买 "sell":卖  
offset | true | string | 开平方向 | "open":开 "close":平  
volume | true | decimal | 委托数量 |  
price | true | decimal | 委托价格 |  
create_date | true | long | 创建时间 |  
order_source | true | string | 订单来源 |
（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
order_price_type | true | int | 订单报价类型 |
1：限价单（limit），2：市价单（market），3：对手价（opponent），4：闪电平仓（lightning），5：计划委托（trigger），6：post_only
，7：最优5档（optimal_5） ，8：最优10档（optimal_10） ，9：最优20档（optimal_20），10：FOK ，11：IOC
，12：对手价_IOC（opponent_ioc），13：闪电平仓_IOC（lightning_ioc），14：最优5档_IOC（optimal_5_ioc），15：最优10档_IOC（optimal_10_ioc），16：最优20档_IOC（optimal_20_ioc），17：对手价_FOK（opponent_fok），18：闪电平仓_FOK（lightning_fok），19：最优5档_FOK（optimal_5_fok），40：最优10档_FOK（optimal_10_fok），41：最优20档_FOK（optimal_20_fok）。  
margin_frozen | true | decimal | 冻结保证金 |  
profit | true | decimal | 收益 |  
trade_volume | true | decimal | 成交数量 |  
trade_turnover | true | decimal | 成交总金额 |  
fee | true | decimal | 手续费 |  
trade_avg_price | true | decimal | 成交均价 |  
status | true | int | 订单状态 |  
order_type | true | int | 订单类型 | 1:报单 、 2:撤单 、 3:强平、4:交割  
fee_asset | true | string | 手续费币种 | （"BTC","ETH"...）  
liquidation_type | true | string | 强平类型 | 0:非强平类型，1：多空轧差， 2:部分接管，3：全部接管  
</orders> |  |  |  |  
total_page | true | int | 总页数 |  
current_page | true | int | 当前页 |  
total_size | true | int | 总条数 |  
</data> |  |  |  |  
ts | true | long | 时间戳 |  
  
### 备注

  * order_id返回是18位，nodejs和javascript默认解析18有问题，nodejs和javascript里面JSON.parse默认是int，超过18位的数字用json-bigint的包解析。

## 组合查询合约历史委托

  * POST `/api/v1/contract_hisorders_exact`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol  | true  | string | 品种代码  | "BTC","ETH"...  
trade_type | true | int | 交易类型 | 0:全部,1:买入开多,2: 卖出开空,3: 买入平空,4: 卖出平多,5:
卖出强平,6: 买入强平,7:交割平多,8: 交割平空, 11:减仓平多，12:减仓平空  
type | true | int | 类型 | 1:所有订单,2:结束状态的订单  
status | true | string | 订单状态 | 可查询多个状态，"3,4,5" , 0:全部,3:未成交, 4: 部分成交,5:
部分成交已撤单,6: 全部成交,7:已撤单  
contract_code | false | string | 合约代码 |  
order_price_type | false | string | 订单报价类型 | 订单报价类型 "limit":限价 "opponent":对手价
"post_only":只做maker单,post
only下单只受用户持仓数量限制,optimal_5：最优5档、optimal_10：最优10档、optimal_20：最优20档，ioc:IOC订单，fok：FOK订单,
"opponent_ioc"： 对手价-
IOC下单，"optimal_5_ioc"：最优5档-IOC下单，"optimal_10_ioc"：最优10档-IOC下单，"optimal_20_ioc"：最优20档-IOC下单,"opponent_fok"：
对手价-
FOK下单，"optimal_5_fok"：最优5档-FOK下单，"optimal_10_fok"：最优10档-FOK下单，"optimal_20_fok"：最优20档-FOK下单  
start_time | false | long | 起始时间（时间戳，单位毫秒） | 详见备注  
end_time | false | long | 结束时间（时间戳，单位毫秒） | 详见备注  
from_id | false | long | 查询起始id（取返回数据的query_id字段） |  
size | false | int | 数据条数 | 默认取20，最大50  
direct | false | string | 查询方向 | prev 向前；next 向后；默认值取prev  
  
#### 备注：

  * 所有已撤销且无成交的API限价订单记录只保留最近2小时。
  * 起始与结束时间取值说明： 
    * start_time：取值范围为[(当前时间 - 90天)，当前时间] ；默认值取clamp（end_time - 10天，当前时间-90天，当前时间-10天），即时间最远取当前时间-90天，最近取当前时间-10天。
    * end_time：取值范围为：[(当前时间 - 90天)，above++)]，若大于当前时间则直接取当前时间；若填写了start_time，则end_time必须大于start_time。默认值直接取当前时间。
  * 当from_id缺省时，查询方向为prev则从结束时间往前查，查询方向为向后则从起始时间往后查；即查询创建时间大于等于起始时间，且小于等于结束时间的历史委托数据。
  * 无论查询方向是向前还是向后，返回的数据都是按创建时间倒序。
  * 当start_time或end_time填写值不符合取值范围，则报错参数不合法。
  * 仅支持查询90天内数据。

#### 查询案例如下（特殊错误情况未罗列）如当前时间为"2020-07-31"：

start_time | end_time | from_id | size | direct | 查询结果  
---|---|---|---|---|---  
缺省，取10天前（2020-07-21） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | prev |
查询最近10天的数据，从当前时间开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取60天前（2020-06-01） | 50天前（2020-06-11） | 缺省 | 20条 | prev |
查询60天前到50天前之间的数据，从50天前开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
5天前（2020-07-26） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | prev |
查询最近5天的数据，从当前时间开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
20天前（2020-07-11） | 10天前（2020-07-21） | 缺省 | 20条 | prev |
查询20天前到10天前之间的数据，从10天前开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取10天前（2020-07-21） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | next |
查询最近10天的数据，从10天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取60天前（2020-06-01） | 50天前（2020-06-11） | 缺省 | 20条 | next |
查询60天前到50天前之间的数据，从60天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
5天前（2020-07-26） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | next |
查询最近5天的数据，从5天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
20天前（2020-07-11） | 10天前 （2020-07-21） | 缺省 | 20条 | next |
查询20天前到10天前之间的数据，从20天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取10天前（2020-07-21） | 缺省，取当前时间 （2020-07-31） | 1000 | 20条 | prev |
查询最近10天的数据，从成交id为1000的数据开始往前查20条更旧的数据，成交id为1000的数据排在第一条，越新的数据排在越前  
20天前 （2020-07-11） | 10天前 （2020-07-21） | 1000 | 20条 | next |
查询20天前到10天前之间的数据，从成交id为1000的数据开始往后查20条更新的数据，成交id为1000的数据排在最后一条，越新的数据排在越前  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "query_id": 113957564277,
                    "order_id": 773135295142658048,
                    "contract_code": "ADA201225",
                    "symbol": "ADA",
                    "lever_rate": 20,
                    "direction": "buy",
                    "offset": "open",
                    "volume": 1,
                    "price": 0.092,
                    "create_date": 1604371418518,
                    "order_source": "web",
                    "order_price_type": "post_only",
                    "order_type": 1,
                    "margin_frozen": 0,
                    "profit": 0,
                    "contract_type": "quarter",
                    "trade_volume": 1,
                    "trade_turnover": 10,
                    "fee": -0.021739130434782608,
                    "trade_avg_price": 0.092,
                    "status": 6,
                    "order_id_str": "773135295142658048",
                    "fee_asset": "ADA",
                    "liquidation_type": "0"
                }
            ],
            "remain_size": 19,
            "next_id": 113956362239
        },
        "ts": 1604371805794
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status  | true  | string | 请求处理结果  |  
<data> | true | object |  |  
<orders> | true | object array |  |  
query_id | true | long | 查询id，可作为下一次查询请求的from_id字段 |  
order_id | true | long | 订单ID |  
order_id_str | true | string | string格式的订单ID |  
symbol | true | string | 品种代码 |  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter"，次季度：“next_quarter”  
contract_code | true | string | 合约代码 | "BTC180914" ...  
lever_rate | true | int | 杠杆倍数 |  
direction | true | string | 买卖方向 | "buy":买 "sell":卖  
offset | true | string | 开平方向 | "open":开 "close":平  
volume | true | decimal | 委托数量 |  
price | true | decimal | 委托价格 |  
create_date | true | long | 创建时间 |  
order_source | true | string | 订单来源 |
（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
order_price_type | true | string | 订单报价类型 | 订单报价类型 "limit":限价 "opponent":对手价
"post_only":只做maker单,post
only下单只受用户持仓数量限制,optimal_5：最优5档、optimal_10：最优10档、optimal_20：最优20档，ioc:IOC订单，fok：FOK订单,
"opponent_ioc"： 对手价-
IOC下单，"optimal_5_ioc"：最优5档-IOC下单，"optimal_10_ioc"：最优10档-IOC下单，"optimal_20_ioc"：最优20档-IOC下单,"opponent_fok"：
对手价-
FOK下单，"optimal_5_fok"：最优5档-FOK下单，"optimal_10_fok"：最优10档-FOK下单，"optimal_20_fok"：最优20档-FOK下单  
margin_frozen | true | decimal | 冻结保证金 |  
profit | true | decimal | 收益 |  
trade_volume | true | decimal | 成交数量 |  
trade_turnover | true | decimal | 成交总金额 |  
fee | true | decimal | 手续费 |  
trade_avg_price | true | decimal | 成交均价 |  
status | true | int | 订单状态 | 1准备提交 2准备提交 3已提交 4部分成交 5部分成交已撤单 6全部成交 7已撤单 11撤单中  
order_type | true | int | 订单类型 | 1:报单 、 2:撤单 、 3:强平、4:交割  
fee_asset | true | string | 手续费币种 | （"BTC","ETH"...）  
liquidation_type | true | string | 强平类型 | 0:非强平类型，1：多空轧差， 2:部分接管，3：全部接管  
</orders> |  |  |  |  
remain_size | true | int | 剩余数据条数（在时间范围内，因受到数据条数限制而未查询到的数据条数） |  
next_id | true | long | 下一条数据的query_id（仅在查询结果超过数据条数限制时才有值） |  
</data> |  |  |  |  
ts | true | long | 时间戳 |  
  
#### 备注：

  * 当查询结果超过数据条数限制时，next_id为下一条数据的query_id（查询方向为prev时，next_id为下一页查询的第一条数据；查询方向为next时，next_id为下一页查询的最后一条数据）

## 获取历史成交记录

### 实例

  * POST `/api/v1/contract_matchresults`

> Request:
    
    
    {
        "symbol":"btc",
        "trade_type":0,
        "create_date":20,
        "contract_code":"btc200925",
        "page_index":1,
        "page_size":20
    }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 品种代码 |  | 支持大小写,"BTC","ETH"...  
trade_type | true | int | 交易类型 |  | 0:全部,1:买入开多,2: 卖出开空,3: 买入平空,4: 卖出平多,5:
卖出强平,6: 买入强平  
create_date | true | int | 日期 |  | 可随意输入正整数，如果参数超过90则默认查询90天的数据  
contract_code | false | string | 合约code |  |  
page_index | false | int | 页码，不填默认第1页 | 1 |  
page_size | false | int | 不填默认20，不得多于50 | 20 | [1-50]  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "trades": [
                {
                    "match_id": 113891764710,
                    "order_id": 773135295142658048,
                    "symbol": "ADA",
                    "contract_type": "quarter",
                    "contract_code": "ADA201225",
                    "direction": "buy",
                    "offset": "open",
                    "trade_volume": 1,
                    "trade_price": 0.092,
                    "trade_turnover": 10,
                    "trade_fee": -0.021739130434782608,
                    "offset_profitloss": 0,
                    "create_date": 1604371703183,
                    "role": "Maker",
                    "order_source": "web",
                    "order_id_str": "773135295142658048",
                    "fee_asset": "ADA",
                    "id": "113891764710-773135295142658048-1"
                }
            ],
            "total_page": 16,
            "current_page": 1,
            "total_size": 16
        },
        "ts": 1604371918571
    }                                             
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status  | true  | string | 请求处理结果  |  
<data> |  |  |  |  
<trades> |  |  |  |  
id | true | string | 全局唯一的交易标识 |  
match_id | true | long | 撮合结果id,
与订单ws推送orders.$symbol以及撮合订单ws推送matchOrders.$symbol推送结果中的trade_id是相同的，非唯一，可重复，注意：一个撮合结果代表一个taker单和N个maker单的成交记录的集合，如果一个taker单吃了N个maker单，那这N笔trade都是一样的撮合结果id
|  
order_id | true | long | 订单ID |  
order_id_str | true | string | String类型订单ID |  
symbol | true | string | 品种代码 |  
order_source | true | string | 订单来源 |
（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter", 次季:"next_quarter"  
contract_code | true | string | 合约代码 | "BTC180914" ...  
direction | true | string | "buy":买 "sell":卖 |  
offset | true | string | "open":开 "close":平 |  
trade_volume | true | decimal | 累计成交数量 |  
trade_price | true | decimal | 成交价格 |  
trade_turnover | true | decimal | 本笔成交金额 |  
create_date | true | long | 成交时间 |  
offset_profitloss | true | decimal | 平仓盈亏 |  
trade_fee | true | decimal | 成交手续费 |  
role | true | string | taker或maker |  
fee_asset | true | string | 手续费币种 | （"BTC","ETH"...）  
</trades> |  |  |  |  
total_page | true | int | 总页数 |  
current_page | true | int | 当前页 |  
total_size | true | int | 总条数 |  
</data> |  |  |  |  
ts | true | long | 时间戳 |  
  
### 备注

  * order_id返回是18位，nodejs和javascript默认解析18有问题，nodejs和javascript里面JSON.parse默认是int，超过18位的数字用json-bigint的包解析。

## 组合查询历史成交记录接口

  * POST `/api/v1/contract_matchresults_exact`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | true | string | 品种代码 | "BTC","ETH"...  
trade_type | true | int | 交易类型 | 0:全部,1:买入开多,2: 卖出开空,3: 买入平空,4: 卖出平多,5:
卖出强平,6: 买入强平  
contract_code | false | string | 合约code |  
start_time | false | long | 起始时间（时间戳，单位毫秒） | 详见备注  
end_time | false | long | 结束时间（时间戳，单位毫秒） | 详见备注  
from_id | false | long | 查询起始id（取返回数据的query_id字段） |  
size | false | int | 数据条数 | 默认取20，最大50  
direct | false | string | 查询方向 | prev 向前；next 向后；默认值取prev  
  
#### 备注：

  * 起始与结束时间取值说明： 
    * start_time：取值范围为[(当前时间 - 90天)，当前时间] ；默认值取clamp（end_time - 10天，当前时间-90天，当前时间-10天），即时间最远取当前时间-90天，最近取当前时间-10天。
    * end_time：取值范围为：[(当前时间 - 90天)，above++)]，若大于当前时间则直接取当前时间；若填写了start_time，则end_time必须大于start_time。默认值直接取当前时间。
  * 当from_id缺省时，查询方向为prev则从结束时间往前查，查询方向为向后则从起始时间往后查；即查询成交时间大于等于起始时间，且小于等于结束时间的成交数据。
  * 无论查询方向是向前还是向后，返回的数据都是按成交时间倒序。
  * 当start_time或end_time填写值不符合取值范围，则报错参数不合法。
  * 仅支持查询90天内数据。

#### 查询案例如下（特殊错误情况未罗列）如当前时间为"2020-07-31"：

start_time | end_time | from_id | size | direct | 查询结果  
---|---|---|---|---|---  
缺省，取10天前（2020-07-21） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | prev |
查询最近10天的数据，从当前时间开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取60天前（2020-06-01） | 50天前（2020-06-11） | 缺省 | 20条 | prev |
查询60天前到50天前之间的数据，从50天前开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
5天前（2020-07-26） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | prev |
查询最近5天的数据，从当前时间开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
20天前（2020-07-11） | 10天前（2020-07-21） | 缺省 | 20条 | prev |
查询20天前到10天前之间的数据，从10天前开始往前查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取10天前（2020-07-21） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | next |
查询最近10天的数据，从10天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取60天前（2020-06-01） | 50天前（2020-06-11） | 缺省 | 20条 | next |
查询60天前到50天前之间的数据，从60天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
5天前（2020-07-26） | 缺省，取当前时间（2020-07-31） | 缺省 | 20条 | next |
查询最近5天的数据，从5天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
20天前（2020-07-11） | 10天前 （2020-07-21） | 缺省 | 20条 | next |
查询20天前到10天前之间的数据，从20天前开始往后查20条数据，返回数据按创建时间倒序，越新的数据排在越前  
缺省，取10天前（2020-07-21） | 缺省，取当前时间 （2020-07-31） | 1000 | 20条 | prev |
查询最近10天的数据，从成交id为1000的数据开始往前查20条更旧的数据，成交id为1000的数据排在第一条，越新的数据排在越前  
20天前 （2020-07-11） | 10天前 （2020-07-21） | 1000 | 20条 | next |
查询20天前到10天前之间的数据，从成交id为1000的数据开始往后查20条更新的数据，成交id为1000的数据排在最后一条，越新的数据排在越前  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "trades": [
                {
                    "query_id": 2424420723,
                    "match_id": 113891764710,
                    "order_id": 773135295142658048,
                    "symbol": "ADA",
                    "contract_type": "quarter",
                    "contract_code": "ADA201225",
                    "direction": "buy",
                    "offset": "open",
                    "trade_volume": 1,
                    "trade_price": 0.092,
                    "trade_turnover": 10,
                    "trade_fee": -0.021739130434782608,
                    "offset_profitloss": 0,
                    "create_date": 1604371703183,
                    "role": "Maker",
                    "order_source": "web",
                    "order_id_str": "773135295142658048",
                    "fee_asset": "ADA",
                    "id": "113891764710-773135295142658048-1"
                }
            ],
            "remain_size": 15,
            "next_id": 2424413094
        },
        "ts": 1604372202243
    }                 
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 |  
<data> | true | object |  |  
<trades> | true | object array |  |  
id | true | string | 全局唯一的交易标识 |  
query_id | true | long | 查询id，可作为下一次查询请求的from_id字段 |  
match_id | true | long | 撮合结果id,
与订单ws推送orders.$symbol以及撮合订单ws推送matchOrders.$symbol推送结果中的trade_id是相同的，非唯一，可重复，注意：一个撮合结果代表一个taker单和N个maker单的成交记录的集合，如果一个taker单吃了N个maker单，那这N笔trade都是一样的撮合结果id
|  
order_id | true | long | 订单ID |  
order_id_str | true | string | string格式的订单ID |  
symbol | true | string | 品种代码 |  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter"，次季度：“next_quarter”  
contract_code | true | string | 合约代码 | "BTC180914" ...  
direction | true | string | 买卖方向 | "buy":买 "sell":卖  
offset | true | string | 开平方向 | "open":开 "close":平  
trade_volume | true | decimal | 成交数量 |  
trade_price | true | decimal | 成交价格 |  
trade_turnover | true | decimal | 成交总金额 |  
create_date | true | long | 成交时间 |  
offset_profitloss | true | decimal | 平仓盈亏 |  
traded_fee | true | decimal | 成交手续费 |  
role | true | string | taker或maker |  
fee_asset | true | string | 手续费币种 | （"BTC","ETH"...）  
order_source | true | string | 订单来源 |
（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
</trades> |  |  |  |  
remain_size | true | int | 剩余数据条数（在时间范围内，因受到数据条数限制而未查询到的数据条数） |  
next_id | true | long | 下一条数据的query_id（仅在查询结果超过数据条数限制时才有值） |  
</data> |  |  |  |  
ts | true | long | 时间戳 |  
  
#### 备注：

  * 当查询结果超过数据条数限制时，next_id为下一条数据的query_id（查询方向为prev时，next_id为下一页查询的第一条数据；查询方向为next时，next_id为下一页查询的最后一条数据）

## 闪电平仓下单

  * POST `/api/v1/lightning_close_position`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | false | string | 品种代码 | 支持大小写,"BTC","ETH"...  
contract_type | false | string | 合约类型 |
“this_week”:当周，“next_week”:次周，“quarter”:当季, "next_quarter":次季  
contract_code | false | string | 合约代码 | BTC190903  
volume | true | long | 委托数量（张） |  
direction | true | string | “buy”:买，“sell”:卖 |  
client_order_id | false | long |
（API）客户自己填写和维护，必须保持唯一,请注意必须小于等于9223372036854775807 |  
order_price_type | false | string | 订单报价类型 |
不填，默认为“闪电平仓”，"lightning"：闪电平仓，"lightning_fok"：闪电平仓-FOK,"lightning_ioc"：闪电平仓-
IOC  
  
### 说明

  * 如果contract_code填了值，那就按照contract_code去下单，如果contract_code没有填值，则按照symbol+contract_type去下单。

  * 闪电平仓，是指在对手价平仓的基础上，实行'最优30档'成交，即用户发出的平仓订单能够迅速以30档范围内对手方价格进行成交，未成交部分自动转为限价委托单。

  * client_order_id，24小时有效，超过24小时的订单根据client_order_id将查询不到。

> Response:
    
    
    {
        "status":"ok",
        "data":{
            "order_id":633766664829804544,
            "order_id_str":"633766664829804544",
            "client_order_id":9086
        },
        "ts":158797866555
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" :成功, "error"：失败  
ts | true | long | 响应生成时间点，单位：毫秒 |  
<data> |  |  |  | 字典  
order_id | true | long | 订单ID[用户级别的，不同的用户order_id可能相同] |  
order_id_str | true | string | String类型订单ID |  
client_order_id | false | long | 用户自己的订单id |  
</data> |  |  |  |  
  
> 错误信息：
    
    
    {
        "status": "error",
        "err_code": 1048,
        "err_msg": "Insufficient close amount available.",
        "ts": 1604372431440
    }
    

## 合约计划委托下单

  * POST `/api/v1/contract_trigger_order`

### 备注

  * 如果contract_code填了值，那就按照contract_code去下单，如果contract_code没有填值，则按照symbol+contract_type去下单；

  * optimal_5：最优5档、optimal_10：最优10档、optimal_20：最优20档下单order_price价格参数不用传，"limit":限价需要传价格。

  * 若存在持仓，那么下单时杠杆倍数必须与持仓杠杆相同，否则下单失败。若需使用新杠杆下单，则必须先使用切换杠杆接口将持仓杠杆切换成功后再下单。

> Request:
    
    
     {
         "contract_code":"btc200925",
         "contract_type":"quarter",
         "direction":"BUY",
         "lever_rate":5,
         "offset":"OPEN",
         "order_price":10000,
         "order_price_type":"limit",
         "symbol":"btc",
         "trigger_price":10000,
         "trigger_type":"ge",
         "volume":1
     }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
symbol | false | string | 品种代码 | 支持大小写,"BTC","ETH"...  
contract_type | false | string | 合约类型 |
“this_week”:当周，“next_week”:次周，“quarter”:当季, "next_quarter":次季  
contract_code | false | string | 合约代码 | BTC190903  
trigger_type | true | string | 触发类型： ge大于等于(触发价比最新价大)；le小于(触发价比最新价小) |  
trigger_price | true | decimal | 触发价，精度超过最小变动单位会报错 |  
order_price | true | decimal | 委托价，精度超过最小变动单位会报错 |  
order_price_type | false | string | 委托类型： 不填默认为limit; 限价：limit
，最优5档：optimal_5，最优10档：optimal_10，最优20档：optimal_20 |  
volume | true | long | 委托数量(张) |  
direction | true | string | buy:买 sell:卖 |  
offset | true | string | open:开 close:平 |  
lever_rate | true | int |
杠杆倍数[开仓若有10倍多单，就不能再下20倍多单;首次使用高倍杠杆(>20倍)，请使用主账号登录web端同意高倍杠杆协议后，才能使用接口下高倍杠杆(>20倍)]
|  
  
> 正确的返回:
    
    
    {
        "status": "ok",
        "data": {
            "order_id": 28312412,
            "order_id_str": "28312412"
        },
        "ts": 1604372634548
    }
    

> 错误的返回:
    
    
    {
        "status": "error",
        "err_code": 1037,
        "err_msg": "The leverage is invalid. Please contact the customer service.",
        "ts": 1605495536623
    }
    

### 返回参数

属性 | 数据类型 | 是否必填 | 说明  
---|---|---|---  
status | string | true | 响应状态: ok,error  
err_code | int | false | 错误码  
err_msg | string | false | 错误信息  
data | List<OrderInsertRspInfo> | false | 返回数据-泛型，支持各种返回的数据格式类型  
ts | long | true | 时间戳  
  
  * OrderInsertRspInfo

属性 | 数据类型 | 是否必填 | 说明  
---|---|---|---  
order_id | long | true | 订单ID : 用户级别的，不同的用户order_id可能相同  
order_id_str | string | true | 字符串类型的订单ID  
  
## 合约计划委托撤单

  * POST `/api/v1/contract_trigger_cancel`

### 请求参数

属性 | 数据类型 | 是否必填 | 说明  
---|---|---|---  
symbol | string | true | 支持大小写,BTC,LTC...  
order_id | string | true | 用户订单ID（多个订单ID中间以","分隔,一次最多允许撤消10个订单 ）  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "errors": [
                {
                    "order_id": "28312406",
                    "err_code": 1061,
                    "err_msg": "This order doesnt exist."
                }
            ],
            "successes": "28312412"
        },
        "ts": 1604372746401
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
<errors> |  |  |  |  
order_id | true | string | 订单id |  
err_code | true | int | 订单失败错误码 |  
err_msg | true | string | 订单失败信息 |  
</errors> |  |  |  |  
successes | true | string | 成功的订单 |  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
## 合约计划委托全部撤单

  * POST `/api/v1/contract_trigger_cancelall`

### 请求参数

属性 | 数据类型 | 是否必填 | 说明  
---|---|---|---  
symbol | string | true | 支持大小写,BTC、LTC...  
contract_code | string | false | 合约代码,"BTC180914" ...  
contract_type | string | false | 合约类型 当周:"this_week", 次周:"next_week",
当季:"quarter", 次季:"next_quarter"  
  
### 备注

  * 只传symbol，撤该该品种下所有周期的合约

  * 只要有contract_code，则撤销该code的合约

  * 只传symbol+contract_type， 则撤销二者拼接所成的合约订单

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "errors": [],
            "successes": "28312413,28312414"
        },
        "ts": 1604373863946
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
<data> |  |  |  |  
<errors> |  |  |  |  
order_id | true | string | 订单id |  
err_code | true | int | 订单失败错误码 |  
err_msg | true | string | 订单失败信息 |  
</errors> |  |  |  |  
successes | true | string | 成功的订单 |  
</data> |  |  |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
## 获取计划委托当前委托

  * POST `/api/v1/contract_trigger_openorders`

### 请求参数

属性 | 数据类型 | 是否必填 | 说明  
---|---|---|---  
symbol | string | true | 支持大小写,BTC,LTC...  
contract_code | string | false | 支持大小写,合约code  
page_index | int | false | 第几页，不填默认第一页  
page_size | int | false | 不填默认20，不得多于50  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "symbol": "ADA",
                    "contract_code": "ADA201225",
                    "contract_type": "quarter",
                    "trigger_type": "le",
                    "volume": 1,
                    "order_type": 1,
                    "direction": "buy",
                    "offset": "open",
                    "lever_rate": 20,
                    "order_id": 28312415,
                    "order_id_str": "28312415",
                    "order_source": "api",
                    "trigger_price": 0.0895,
                    "order_price": 0.0895,
                    "created_at": 1604374041289,
                    "order_price_type": "limit",
                    "status": 2
                }
            ],
            "total_page": 1,
            "current_page": 1,
            "total_size": 1
        },
        "ts": 1604374215911
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
data | true | object | 返回数据 |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
  * data详情：

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
total_page | int | true | 总页数 |  
current_page | int | true | 当前页 |  
total_size | int | true | 总条数 |  
<orders> |  |  |  |  
symbol | string | true | 合约品种 |  
contract_code | string | true | 合约代码 |  
contract_type | string | true | 合约类型 |  
trigger_type | string | true | 触发类型 | `ge`大于等于；`le`小于等于  
volume | decimal | true | 委托数量 |  
order_type | int | true | 订单类型 | 1、报单 2、撤单  
direction | string | true | 订单方向 | [买(buy),卖(sell)]  
offset | string | true | 开平标志 | [开(open),平(close)]  
lever_rate | int | true | 杠杆倍数 | 1，5，10，20  
order_id | int | true | 计划委托单订单ID |  
order_id_str | string | true | 字符串类型的订单ID |  
order_source | string | true | 订单来源 |
（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
trigger_price | decimal | true | 触发价 |  
order_price | decimal | true | 委托价 |  
created_at | long | true | 订单创建时间 |  
order_price_type | string | true | 订单报价类型 |
"limit":限价，"optimal_5":最优5档，"optimal_10":最优10档，"optimal_20":最优20档  
status | int | true | 订单状态 | 1:准备提交、2:已提交、3:报单中、8：撤单未找到、9：撤单中、10：失败'  
</orders> |  |  |  |  
  
## 获取计划委托历史委托

  * POST `/api/v1/contract_trigger_hisorders`

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 品种代码 |  | 支持大小写,"BTC","ETH"...  
contract_code | false | string | 合约code |  | EOS190118  
trade_type | true | int | 交易类型 |  | 0:全部,1:买入开多,2: 卖出开空,3: 买入平空,4:
卖出平多；后台是根据该值转换为offset和direction，然后去查询的； 其他值无法查询出结果  
status | true | string | 订单状态 |  |
多个以英文逗号隔开，计划委托单状态：0:全部（表示全部结束状态的订单）、4:已委托、5:委托失败、6:已撤单  
create_date | true | int | 日期 |  | 可随意输入正整数，如果参数超过90则默认查询90天的数据  
page_index | false | int | 页码，不填默认第1页 | 1 |  
page_size | false | int | 不填默认20，不得多于50 | 20 | [1-50]  
  
### 备注

  * 默认查询 已完成订单（type对应状态范围 4、5、6）；

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "symbol": "ADA",
                    "contract_code": "ADA201225",
                    "contract_type": "quarter",
                    "trigger_type": "le",
                    "volume": 1,
                    "order_type": 1,
                    "direction": "buy",
                    "offset": "open",
                    "lever_rate": 20,
                    "order_id": 28312415,
                    "order_id_str": "28312415",
                    "relation_order_id": "773147284987842560",
                    "order_price_type": "limit",
                    "status": 4,
                    "order_source": "api",
                    "trigger_price": 0.0895,
                    "triggered_price": 0.089497,
                    "order_price": 0.0895,
                    "created_at": 1604374041289,
                    "triggered_at": 1604374277082,
                    "order_insert_at": 1604374277124,
                    "canceled_at": 0,
                    "fail_code": null,
                    "fail_reason": null
                }
            ],
            "total_page": 4,
            "current_page": 1,
            "total_size": 4
        },
        "ts": 1604374349086
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 请求处理结果 | "ok" , "error"  
data | true | object | 返回数据 |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
  
  * data详情：

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
total_page | int | true | 总页数 |  
current_page | int | true | 当前页 |  
total_size | int | true | 总条数 |  
<orders> |  |  |  |  
symbol | string | true | 合约品种 |  
contract_code | string | true | 合约代码 |  
contract_type | string | true | 合约类型 |  
trigger_type | string | true | 触发类型 | `ge`大于等于；`le`小于等于  
volume | decimal | true | 委托数量 |  
order_type | int | true | 订单类型 | 1、报单 2、撤单  
direction | string | true | 订单方向 | [买(buy),卖(sell)]  
offset | string | true | 开平标志 | [开(open),平(close)]  
lever_rate | int | true | 杠杆倍数 | 1,5,10,20  
order_id | int | true | 计划委托单订单ID |  
order_id_str | string | true | 字符串类型的订单ID |  
relation_order_id | string | true | 该字段为关联限价单的订单id，未触发前数值为-1 |  
order_price_type | string | true | 订单报价类型 |
"limit":限价，"optimal_5":最优5档，"optimal_10":最优10档，"optimal_20":最优20档  
status | int | true | 订单状态 | (4:报单成功、5:报单失败、6:已撤单 )  
order_source | string | true | 来源 |
（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
trigger_price | decimal | true | 触发价 |  
triggered_price | decimal | true | 被触发时的价格 |  
order_price | decimal | true | 委托价 |  
created_at | long | true | 订单创建时间 |  
triggered_at | long | true | 触发时间 |  
order_insert_at | long | true | 下order单时间 |  
canceled_at | long | true | 撤单时间 |  
fail_code | int | true | 被触发时下order单失败错误码 |  
fail_reason | string | true | 被触发时下order单失败原因 |  
</orders> |  |  |  |  
  
# 合约划转接口

## 现货-交割合约账户间进行资金的划转

### 实例

  * POST `https://api.huobi.pro/v1/futures/transfer`

### 备注

此接口用户币币现货账户与交割合约账户之间的资金划转。

从现货现货账户转至交割合约账户，类型为`pro-to-futures`; 从交割合约账户转至现货账户，类型为`futures-to-pro`

该接口的访问频次的限制为1秒/1次。

注意：请求地址为火币Global地址

现货与交割合约划转接口，所有划转的币的精度是8位小数。

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
currency | true | string | 币种,不区分大小写 | e.g. btc,eth  
amount | true | decimal | 划转金额 |  
type | true | string | 划转类型 | 从合约账户到现货账户：“futures-to-pro”，从现货账户到合约账户： “pro-to-
futures”  
  
> Response:
    
    
    正确的返回：
    {
        "status": "ok",
        "data": 179697972
    }
    错误的返回：
    {
        "status": "error",
        "data": null,
        "err-code": "base-currency-error",
        "err-msg": "The current coin does not exist."
    }
    
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
status | true | string | 状态 | ok, error  
data | true | long | 生成的划转订单id |  
err-code | true | string | 错误码 | 具体错误码请见列表  
err-msg | true | string | 错误消息 | 具体错误码请见列表  
  
## err-code列表

err-code | err-msg(中文） | err-msg(English) | 补充说明  
---|---|---|---  
base-msg |  |  | 其他错误，具体的err-msg, 请参照对应的错误消息列表  
base-currency-error | 币种无效 | The currency is invalid |  
frequent-invoke | 操作过于频繁，请稍后重试。（如果超过1分钟10次，系统返回该error-code） | the operation is
too frequent. Please try again later | 如果请求次数超过1分钟10次，系统返回该error-code  
banned-by-blacklist | 黑名单限制 | Blacklist restriction |  
dw-insufficient-balance | 可划转余额不足，最大可划转 {0}。（币币账户的余额不足。） | Insufficient
balance. You can only transfer {0} at most. | 币币账户的余额不足。  
dw-account-transfer-unavailable | 转账暂时不可用 | account transfer unavailable |
该接口暂时不可用  
dw-account-transfer-error | 由于其他服务不可用导致的划转失败 | account transfer error |  
dw-account-transfer-failed | 划转失败。请稍后重试或联系客服 | Failed to transfer. Please try
again later. | 由于系统异常导致的划转失败  
dw-account-transfer-failed-account-abnormality | 账户异常，划转失败。请稍后重试或联系客服 |
Account abnormality, failed to transfer。Please try again later. |  
  
## base-msg对应的err-msg列表

err-msg(中文） | err-msg(English) | 补充说明  
---|---|---  
用户没有入金权限 | Unable to transfer in currently. Please contact customer service |  
用户没有出金权限 | Unable to transfer out currently. Please contact customer service |  
合约状态异常，无法出入金 | Abnormal contracts status. Can’t transfer |  
子账号没有入金权限，请联系客服 | Sub-account doesn't own the permissions to transfer in.
Please contact customer service |  
子账号没有出金权限，请联系客服 | Sub-account doesn't own the permissions to transfer out.
Please contact customer service |  
子账号没有划转权限，请登录主账号授权 | The sub-account does not have transfer permissions.
Please login main account to authorize |  
可划转余额不足 | Insufficient amount available | 合约账户的余额不足  
单笔转出的数量不能低于{0}{1} | The single transfer-out amount must be no less than {0}{1}
|  
单笔转出的数量不能高于{0}{1} | The single transfer-out amount must be no more than {0}{1}
|  
单笔转入的数量不能低于{0}{1} | The single transfer-in amount must be no less than {0}{1}
|  
单笔转入的数量不能高于{0}{1} | The single transfer-in amount must be no more than {0}{1}
|  
您当日累计转出量超过{0}{1}，暂无法转出 | Your accumulative transfer-out amount is over the
daily maximum, {0}{1}. You can't transfer out for the time being |  
您当日累计转入量超过{0}{1}，暂无法转入 | Your accumulative transfer-in amount is over the
daily maximum, {0}{1}. You can't transfer in for the time being |  
您当日累计净转出量超过{0}{1}，暂无法转出 | Your accumulative net transfer-out amount is over
the daily maximum, {0}{1}. You can't transfer out for the time being |  
您当日累计净转入量超过{0}{1}，暂无法转入 | Your accumulative net transfer-in amount is over the
daily maximum, {0}{1}. You can't transfer in for the time being |  
超过平台当日累计最大转出量限制，暂无法转出 | The platform's accumulative transfer-out amount is
over the daily maximum. You can't transfer out for the time being |  
超过平台当日累计最大转入量限制，暂无法转入 | The platform's accumulative transfer-in amount is over
the daily maximum. You can't transfer in for the time being |  
超过平台当日累计最大净转出量限制，暂无法转出 | The platform's accumulative net transfer-out amount
is over the daily maximum. You can't transfer out for the time being |  
超过平台当日累计最大净转入量限制，暂无法转入 | The platform's accumulative net transfer-in amount is
over the daily maximum. You can't transfer in for the time being |  
划转失败，请稍后重试或联系客服 | Transfer failed. Please try again later or contact customer
service |  
服务异常，划转失败，请稍后再试 | Abnormal service, transfer failed. Please try again later |  
您尚未开通合约交易，无访问权限 | You don’t have access permission as you have not opened
contracts trading |  
合约品种不存在 | This contract type doesn't exist. | 没有相应币种的合约  
  
# 合约Websocket简介

## 接口列表

权限类型 | 接口数据类型 | 请求方法 | 类型 | 描述 | 需要验签  
---|---|---|---|---|---  
读取 | 市场行情接口 | market.$symbol.kline.$period | sub | 订阅 KLine 数据 | 否  
读取 | 市场行情接口 | market.$symbol.kline.$period | req | 请求 KLine 数据 | 否  
读取 | 市场行情接口 | market.$symbol.depth.$type | sub | 订阅 Market Depth 数据 | 否  
读取 | 市场行情接口 | market.$symbol.depth.size_${size}.high_freq | sub | 订阅 Market
Depth增量推送数据 | 否  
读取 | 市场行情接口 | market.$symbol.bbo | sub | 买一卖一逐笔行情推送 | 否  
读取 | 市场行情接口 | market.$symbol.detail | sub | 订阅 Market detail 数据 | 否  
读取 | 市场行情接口 | market.$symbol.trade.detail | req | 请求 Trade detail 数据 | 否  
读取 | 市场行情接口 | market.$symbol.trade.detail | sub | 订阅 Trade Detail 数据 | 否  
读取 | 指数与基差接口 | market.$symbol.basis.$period.$basis_price_type | sub | 订阅基差数据 |
否  
读取 | 指数与基差接口 | market.$symbol.basis.$period.$basis_price_type | req | 请求基差数据 |
否  
读取 | 指数与基差接口 | market.$symbol.index.$period | sub | 订阅(sub)指数K线数据 | 否  
读取 | 指数与基差接口 | market.$symbol.index.$period | req | 请求(req)指数K线数据 | 否  
读取 | 交易接口 | public.$symbol.liquidation_orders | sub | 订阅强平订单数据（免鉴权） | 否  
读取 | 交易接口 | public.$symbol.contract_info | sub | 订阅合约信息变动数据（免鉴权） | 否  
读取 | 交易接口 | orders.$symbol | sub | 订阅订单成交数据 | 是  
读取 | 资产接口 | accounts.$symbol | sub | 订阅资产变动数据 | 是  
读取 | 资产接口 | positions.$symbol | sub | 订阅持仓变动更新数据 | 是  
读取 | 交易接口 | matchOrders.$symbol | sub | 订阅撮合订单成交数据 | 是  
读取 | 交易接口 | trigger_order.$symbol | sub | 订阅计划委托订单更新ws推送 | 是  
读取 | 系统状态接口 | public.$service.heartbeat | sub | 订阅系统状态更新 | 否  
  
## 合约订阅地址

合约站行情请求以及订阅地址为：wss://api.hbdm.com/ws

合约站订单推送订阅地址：wss://api.hbdm.com/notification

合约站指数K线及基差数据订阅地址：wss://api.hbdm.com/ws_index

合约站系统状态更新订阅地址：wss://api.hbdm.com/center-notification

如果api.hbdm.com域名访问不了，可使用：

合约站行情请求以及订阅地址为：wss://api.btcgateway.pro/ws

合约站订单推送订阅地址：wss://api.btcgateway.pro/notification

合约站指数K线及基差数据订阅地址：wss://api.btcgateway.pro/ws_index

合约站系统状态更新订阅地址：wss://api.btcgateway.pro/center-notification

如果对合约订单推送订阅有疑问，可以参考[Demo](https://github.com/huobiapi/Futures-Java-demo)

### 备注

如果api.hbdm.com无法访问，可以使用api.btcgateway.pro来做调试，AWS服务器用户推荐使用api.hbdm.vn；

## 访问次数限制

公开行情接口和用户私有接口都有访问次数限制

  * 普通用户，需要密钥的私有接口，每个UID 3秒最多 72 次请求(交易接口3秒最多 36 次请求，查询接口3秒最多 36次请求) (该UID的所有币种和不同到期日的合约的所有私有接口共享该限制)

  * 其他非行情类的公开接口，比如获取指数信息，限价信息，交割结算、平台持仓信息等，所有用户都是每个IP3秒最多120次请求（所有该IP的非行情类的公开接口请求共享3秒120次的额度）

  * 行情类的公开接口，比如：获取K线数据、获取聚合行情、市场行情、获取行情深度数据、获取指数k线、获取基差数据、获取市场最近成交记录：

（1） restful接口：同一个IP, 所有业务（交割合约、币本位永续合约、期权合约和USDT本位永续合约）总共1秒最多800个请求

（2） websocket：req请求，同一时刻最多请求50次；sub请求，无限制，服务器主动推送数据

  * WebSocket私有订单成交推送接口(需要API KEY验签)

一个UID最多同时建立30个私有订单推送WS链接。该用户在一个品种(包含该品种的所有周期的合约)上，仅需要维持一个订单推送WS链接即可。

注意: 订单推送WS的限频，跟用户RESTFUL私有接口的限频是分开的，相互不影响。

  * websocket 1秒同时最多发40个sub请求。

api接口response中的header返回以下字段

  * ratelimit-limit： 单轮请求数上限，单位：次数

  * ratelimit-interval：请求数重置的时间间隔，单位：毫秒

  * ratelimit-remaining：本轮剩余可用请求数，单位：次数

  * ratelimit-reset：请求数上限重置时间，单位：毫秒 

# WebSocket心跳以及鉴权接口

## 市场行情心跳

  * WebSocket Server 发送心跳：

`{"ping": 18212558000}`

  * WebSocket Client 应该返回：

`{"pong": 18212558000}`

注：WebSocket Client 和 WebSocket Server 建立连接之后，WebSocket Server 每隔
`5s`（这个频率可能会变化） 会向 WebSocket Client 发起一次心跳，WebSocket Client 忽略心跳 5
次后，WebSocket Server 将会主动断开连接；WebSocket
Client发送最近2次心跳message中的其中一个`ping`的值，WebSocket Server都会保持WebSocket连接。

## 订单推送心跳

  * WebSocket API 支持单向心跳，Server 发起 ping message，Client 返回 pong message。 WebSocket Server 发送心跳:

`{`

`"op": "ping",`

`"ts": "1492420473058"`

`}`

  * WebSocket Client 应该返回:

`{`

`"op": "pong"`

`"ts": "1492420473058"`

`}`

### 备注：

  * "pong"操作返回数据里面的"ts"的值为"ping"推送收到的"ts"值

  * WebSocket Client 和 WebSocket Server 建⽴立连接之后，WebSocket Server 每隔 5s(这个频率可能会变化) 会向 WebSocket Client 发起⼀一次⼼心跳，WebSocket Client 忽略心跳 5 次后，WebSocket Server 将会主动断开连接。

  * 异常情况WebSocket Server 会返回错误信息，比如：

`{`

`"op": "pong"`

`"ts": "1492420473027",`

`"err-code": 2011`

`"err-msg": “详细出错信息”`

`}`

## 订单推送访问地址

  * 统一服务地址

`wss://api.hbdm.com/notification`

### 备注

如果api.hbdm.com无法访问，可以使用api.btcgateway.pro来做调试，AWS服务器用户推荐使用api.hbdm.vn；

正常ws请求连接不能同时超过30个

### 数据压缩

WebSocket API 返回的所有数据都进⾏了 GZIP 压缩，需要 client 在收到数据之后解压

### 请求与响应数据说明

  * 字符编码：UTF-8

  * 大小写敏感，包含所有参数名和返回值

  * 数据类型：使用JSON传输数据

  * 所有请求数据都有固定格式，具体接口说明文档中只会重点介绍非通用部分，

> 请求数据结构如下:
    
    
       {
      "op": string, // 必填;Client 请求的操作类型(Server 会原样返回)，详细操作
      类型列列表请参考附录
      "cid": string, // 选填;当前请求唯一 ID(Client 自⽣成并保证本地唯一性，
      Server 会原样返回) 
      // 其余必填/可选字段
      }
    
    

> 所有响应/推送数据都会以固定的结构返回，具体接口说明文档中只会重点介绍data部分，请求响应数据结构如下:
    
    
      {
      "op": string, // 必填;本次响应 Client 请求的操作类型
      "cid": string, // 选填;Client 请求唯一 ID
      "ts": long, // 必填;Server 应答时本地时间戳
      "err-code": int, // 必填;响应码，0 代表成功;非0 代表出错，详细响应码列表请参考错误码表。
      "err-msg": string, 只在出错情况下有此信息，表明详细的出错信息 
      "data": object // 选填;返回数据对象，请求处理成功时有效
      }
    
    

> 推送数据结构如下:
    
    
      {
      "op": "string", // 必填;Server 推送的操作类型，详细操作类型列表请参考附录
      "ts": long, // 必填;Server 推送时本地时间戳
      "data": object // 必填;返回数据对象
      }
    
    

## 服务方主动断开连接

在建连和鉴权期间，如果出错，服务方会主动断开连接，在关闭之前推送数据结构如下,

`{`

`"op": "close", // 表明是服务⽅方主动断开连接`

`"ts": long // Server 推送时本地时间戳`

`}`

## 服务方返回错误，但不断开连接

鉴权成功后，在客户方提供非法Op或者某些内部错误的情况下，服务方会返回错误，但并不断开连接

`{`

`"op": "error", // 表明是收到非法op或者内部错误`

`"ts": long// Server 推送时本地时间戳`

`}`

## 鉴权-Authentication

用户自⼰在火币网⽣成Access Key和Secret Key，Secret Key由用户自⼰保存，⽤户需提供Access Key。目前关于 apikey
申请和修改，请在“账户 - API 管理 ” 创建新API Key 填写备注(可选择绑定 ip)点击创建。其中 Access Key 为 API
访问密钥，Secret Key 为用户对请求进⾏签名的密钥(仅申请时可见)。用户按规则生成签名(Signature)。

交易功能 websocket 版本接⼝建立连接时首先要做鉴权操作，具体格式如下，

重要提示：这两个密钥与账号安全紧密相关，无论何时都请勿向其它人透露。

### 鉴权请求数据格式

`{`

`"op": "auth",`

`"type": "api",`

`"AccessKeyId": "e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx",`

`"SignatureMethod": "HmacSHA256",`

`"SignatureVersion": "2",`

`"Timestamp": "2017-05-11T15:19:30",`

`"Signature": "4F65x5A2bLyMWVQj3Aqp+B4w+ivaA7n5Oi2SuYtCJ9o=",`

`}`

### 鉴权请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填；操作名称，鉴权固定值为auth  
type | string | 必填；认证方式 api表示接口认证，ticket 表示终端认证  
cid | string | 选填；Client请求唯一ID  
AccessKeyId | string | type的值为api时必填；API 访问密钥, 您申请的 APIKEY 中的 AccessKey  
SignatureMethod | string | type的值为api时必填；签名方法, 用户计算签名的基于哈希的协议，此处使用 HmacSHA256  
SignatureVersion | string | type的值为api时必填；签名协议的版本，此处使用 2  
Timestamp | string | type的值为api时必填；时间戳, 您发出请求的时间 (UTC 时区)
。在查询请求中包含此值有助于防止第三方截取您的请求。如:2017-05-11T16:22:06。再次强调是 (UTC 时区)  
Signature | string | type的值为api时必填；签名, 计算得出的值，用于确保签名有效和未被篡改  
ticket | string | type的值为ticket时必填；登陆时返回  
  
#### 注意：

  * 为了减少已有用户的接入工作量，此处使用了与REST接口同样的签名算法进行鉴权。

  * 请注意大小写

  * 当type为api时，参数op，type，cid，Signature不参加签名计算

  * 此处签名计算中请求方法固定值为`GET`,其余值请参考REST接口签名算法文档

#### 步骤：

示例例参数签名(Signature)计算过程如下，

  * 规范要计算签名的请求 因为使用 HMAC 进⾏签名计算时，使⽤不同内容计算得到的结果会完全 不同。所以在进⾏签名计算前，请先对请求进⾏规范化处理。

  * 请求方法(GET 或 POST)，后面添加换行符 `\n` 。

`GET\n`

  * 添加小写的访问地址，后面添加换行符`\n`。

`api.hbdm.com\n`

  * 访问方法的路径，后面添加换行符`\n`。

`/notification\n`

  * 按照ASCII码的顺序对参数名进行排序(使⽤ UTF-8 编码，且进⾏了 URI 编码，十六进制字符必须 大写，如‘:’会被编码为'%3A'，空格被编码为'%20')。例如，下面是请求参数的原始顺序，进⾏过 编码后。

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx&SignatureMethod=HmacSHA256&SignatureVersion=2&Timestamp=2017-05-11T15%3A19%3A30`

  * 按照以上顺序，将各参数使用字符’&’连接。 

  * 组成最终的要进行签名计算的字符串如下:

计算签名，将以下两个参数传入加密哈希函数: 要进行签名计算的字符串，进行签名的密钥(SecretKey)

得到签名计算结果并进行 Base64编码

将上述值作为参数Signature的取值添加到 API 请求中。 将此参数添加到请求时，必须将该值进⾏URI编码。

### 鉴权应答数据格式说明

名称 | 类型 | 说明  
---|---|---  
op | string | 必填；操作名称，鉴权固定值为 auth  
type | string | 必填；根据请求的参数进行返回。  
cid | string | 选填；请求时携带则会返回。  
err-code | int | 成功返回 0, 失败为其他值，详细响应码列列表请参考附录  
err-msg | string | 可选，若出错表示详细错误信息  
ts | long | 服务端应答时间戳  
user-id | long | ⽤户 id  
  
> 鉴权成功应答数据示例
    
    
    {
      "op": "auth",
      "type":"api",
      "ts": 1489474081631,
      "err-code": 0,
      "data": {
        "user-id": 12345678
      }
    }
    
    

> 鉴权失败应答返回数据示例
    
    
    {
    "op": "auth",
    "type":"api",
    "ts": 1489474081631, 
    "err-code": xxxx,
    "err-msg": "详细的错误信息"
    }
    
    

# WebSocket市场行情接口

## 订阅 KLine 数据

### 成功建立和 WebSocket API 的连接之后，向 Server发送如下格式的数据来订阅数据：

`{`

`"sub": "market.$symbol.kline.$period",`

`"id": "id generate by client"`

`}`

> 正确订阅请求参数的例子：
    
    
        {
        "sub": "market.BTC_CQ.kline.1min",
        "id": "id1"
        }
    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
sub | true | string |
需要订阅的主题，该接口固定为：market.$symbol.kline.$period，详细参数见sub订阅参数说明 |  
id | false | string | 业务方自主生成的id |  
  
### sub订阅参数说明

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 交易对 |  |
支持大小写，如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约 , "BTC_NQ"表示次季度合约
。支持使用合约code来订阅
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
period | true | string | K线周期 |  | 仅支持小写，1min, 5min, 15min, 30min,
60min,4hour,1day,1week, 1mon  
  
> 之后每当 KLine 有更新时，client 会收到数据，例子:
    
    
    {
        "ch":"market.BTC_CW.kline.1min",
        "ts":1604385120328,
        "tick":{
            "id":1604385120,
            "mrid":113842458873,
            "open":13436.12,
            "close":13436.12,
            "high":13436.12,
            "low":13436.12,
            "amount":0,
            "vol":0,
            "count":0
        }
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述  
---|---|---|---  
ch | true | string | 请求参数  
ts | true | long | 响应生成时间点，单位：毫秒  
<tick> |  |  |  
id | true | long | K线id,也就是K线时间戳，K线起始时间  
mrid | true | long | 订单ID  
vol | true | decimal | 成交量张数  
count | true | decimal | 成交笔数  
open | true | decimal | 开盘价  
close | true | decimal | 收盘价,当K线为最晚的一根时，是最新成交价  
low | true | decimal | 最低价  
high | true | decimal | 最高价  
amount | true | decimal | 成交量(币), 即 sum(每一笔成交量(张)*单张合约面值/该笔成交价)  
</tick> |  |  |  
  
## 请求 KLine 数据

### 成功建立和 WebSocket API 的连接之后，向 Server发送如下格式的数据来订阅数据：

`{`

`"req": "market.$symbol.kline.$period",`

`"id": "id generated by client",`

`"from": " type: long, 2017-07-28T00:00:00+08:00 至2050-01-01T00:00:00+08:00
之间的时间点，单位：秒",`

`"to": "type: long, 2017-07-28T00:00:00+08:00 至2050-01-01T00:00:00+08:00
之间的时间点，单位：秒，必须比 from 大"`

`}`

> 请求 KLine 数据请求参数的例子：
    
    
        {
        "req": "market.BTC_CQ.kline.1min",
        "id": "id4",
        "from":1571000000,
        "to":1573098606
        }
    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
req | true | string |
需要订阅的主题，该接口固定为：market.$symbol.kline.$period，详细参数见req请求参数说明 |  
id | false | string | 业务方自主生成的id |  
from | true | long | 开始时间 |  
to | true | long | 结束时间 |  
  
### req请求参数说明

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 交易对 |  |
支持大小写，如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示次季度合约"。支持使用合约code来订阅
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
period | true | string | K线周期 |  | 仅支持小写，1min, 5min, 15min, 30min,
60min,4hour,1day,1week, 1mon  
  
#### 备注

[t1, t5] 假设有 t1 ~ t5 的K线：

from: t1, to: t5, return [t1, t5].

from: t5, to: t1, which t5 > t1, return [].

from: t5, return [t5].

from: t3, return [t3, t5].

to: t5, return [t1, t5].

from: t which t3 < t <t4, return [t4, t5].

to: t which t3 < t <t4, return [t1, t3].

from: t1 and to: t2, should satisfy 1325347200 < t1 < t2 < 2524579200.

一次最多2000条。

### 返回参数

参数名称 | 是否必须 | 类型 | 描述  
---|---|---|---  
rep | true | string | 请求参数  
status | true | string | 状态  
id | true | string | 请求id  
wsid | true | long | wsid  
<data> |  |  |  
id | true | long | K线id,也就是K线时间戳，K线起始时间  
vol | true | decimal | 成交量张数  
count | true | decimal | 成交笔数  
open | true | decimal | 开盘价  
close | true | decimal | 收盘价,当K线为最晚的一根时，是最新成交价  
low | true | decimal | 最低价  
high | true | decimal | 最高价  
amount | true | decimal | 成交量(币), 即 sum(每一笔成交量(张)*单张合约面值/该笔成交价)  
</data> |  |  |  
  
> 之后每当 KLine 有更新时，client 会收到数据：
    
    
    {
        "id":"id4",
        "rep":"market.BTC_CQ.kline.15min",
        "wsid":498385304,
        "status":"ok",
        "data":[
            {
                "id":1599667200,
                "open":10262.31,
                "close":10244.93,
                "low":10234.84,
                "high":10282,
                "amount":1849.4984536479908439463088799853871134642,
                "vol":189634,
                "count":5342
            },
            {
                "id":1599668100,
                "open":10244.94,
                "close":10242.07,
                "low":10216.55,
                "high":10244.94,
                "amount":1586.9623024248859129381285787325037896282,
                "vol":162334,
                "count":4375
            }
        ]
    }
    
    

## 订阅 Market Depth 数据

### 成功建立和 WebSocket API 的连接之后，向 Server发送如下格式的数据来订阅数据：

`{`

`"sub": "market.$symbol.depth.$type",`

`"id": "id generated by client"`

`}`

> 正确订阅请求参数的例子：
    
    
        {
        "sub": "market.BTC_CQ.depth.step0",
        "id": "id5"
        }
    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
sub | true | string | 需要订阅的主题，该接口固定为：market.$symbol.depth.$type，详细参数见sub订阅参数说明
|  
id | false | string | 业务方自主生成的id |  
  
### sub订阅参数说明

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 交易对 |  |
支持大小写，如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示次季度合约". 支持使用合约code来订阅
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
type | true | string | Depth 类型 |  | 获得150档深度数据，使用step0, step1, step2, step3,
step4, step5, step14, step15
（step1至step15是进行了深度合并后的深度），使用step0时，不合并深度获取150档数据;获得20档深度数据，使用 step6, step7,
step8, step9, step10, step11, step12,
step13（step7至step13是进行了深度合并后的深度），使用step6时，不合并深度获取20档数据  
  
### 备注

  * 合并深度时，一定报价精度内的市场挂单将予以合并显示。合并深度仅改变显示方式，不改变实际成交价格。

  * step1至step5,step14,step15是进行了深度合并后的150档深度数据，step7至step13是进行了深度合并后的20档深度数据，对应精度如下：

  * Depth类型字段对应精度如下：

档位 | Depth 类型 | 精度  
---|---|---  
150档 | step0 | 不合并  
150档 | step1 | 0.00001  
150档 | step2 | 0.0001  
150档 | step3 | 0.001  
150档 | step4 | 0.01  
150档 | step5 | 0.1  
150档 | step14 | 1  
150档 | step15 | 10  
20档 | step6 | 不合并  
20档 | step7 | 0.00001  
20档 | step8 | 0.0001  
20档 | step9 | 0.001  
20档 | step10 | 0.01  
20档 | step11 | 0.1  
20档 | step12 | 1  
20档 | step13 | 10  
  
> 之后每当 depth 有更新时，client 会收到数据，例子：
    
    
    {
        "ch":"market.BTC_CQ.depth.step6",
        "ts":1604385453899,
        "tick":{
            "mrid":113842765361,
            "id":1604385453,
            "bids":[
                [
                    13584.33,
                    1483
                ],
                [
                    13584,
                    1
                ]
            ],
            "asks":[
                [
                    13584.34,
                    126
                ],
                [
                    13584.35,
                    24
                ]
            ],
            "ts":1604385453896,
            "version":1604385453,
            "ch":"market.BTC_CQ.depth.step6"
        }
    }
    

### 返回参数

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
ch | true | string | 数据所属的 channel，格式： market.$symbol.depth.$type |  
ts | true | long | 数据进入行情服务器时间戳，单位：毫秒 |  
<tick> |  |  |  |  
mrid | true | long | 订单ID |  
id | true | long | tick ID |  
asks | true | object | 卖盘,[price(挂单价), vol(此价格挂单张数)], 按price升序 |  
bids | true | object | 买盘,[price(挂单价), vol(此价格挂单张数)], 按price降序 |  
ts | true | long | 深度生成时间戳，100MS生成一次，单位：毫秒 |  
version | true | long | 版本号 |  
ch | true | string | 数据所属的 channel，格式：market.$symbol.depth.$type |  
</tick> |  |  |  |  
  
## 订阅Market Depth增量数据

### 成功建立和 WebSocket API 的连接之后，向 Server发送如下格式的数据来请求数据:

`{`

`"sub": "market.$symbol.depth.size_${size}.high_freq",`

`"data_type":"incremental",`

`"id": "id generated by client"`

`}`

> 正确订阅请求参数的例子：
    
    
    {
    "sub": "market.btc_cw.depth.size_20.high_freq",
    "data_type":"incremental",
    "id": "id generated by client"
    }
    

### 订阅参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
sub | true | string |
需要订阅的主题，该接口固定为：market.$symbol.depth.size_${size}.high_freq，详细参数见sub订阅参数说明 |  
id | false | string | 业务方自主生成的id |  
data_type | false | string | Depth 类型 |
数据类型，不填默认为全量数据，"incremental"：增量数据，"snapshot"：全量数据  
  
### sub订阅参数说明

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 交易对 |  | 支持大小写，
交易对,"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示BTC次季度合约。支持使用合约code来订阅
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
size | true | string | 档位数 |  | 20:表示20档不合并的深度，150:表示150档不合并的深度  
  
> response：
    
    
    {
        "ch":"market.BTC_CQ.depth.size_20.high_freq",
        "tick":{
            "asks":[
                [
                    13576.41,
                    2627
                ],
                [
                    13576.53,
                    122
                ]
            ],
            "bids":[
                [
                    13576.4,
                    1648
                ],
                [
                    13574.17,
                    398
                ]
            ],
            "ch":"market.BTC_CQ.depth.size_20.high_freq",
            "event":"snapshot",
            "id":113842925649,
            "mrid":113842925649,
            "ts":1604385634838,
            "version":330099154
        },
        "ts":1604385634838
    }
    

### 返回参数

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
ch | true | string | 数据所属的 channel，格式：
market.$symbol.depth.size_${size}.high_freq |  
ts | true | long | 进入行情服务器系统时间点，单位：毫秒 |  
<tick> |  |  |  |  
mrid | true | long | 订单ID |  
id | true | long | tick ID |  
asks | true | object | 卖盘,[price(挂单价), vol(此价格挂单张数)], 按price升序 |  
bids | true | object | 买盘,[price(挂单价), vol(此价格挂单张数)], 按price降序 |  
ts | true | long | 系统检测orderbook时间点，单位：毫秒 |  
version | true | long | 版本号 |  
ch | true | string | 数据所属的 channel，格式：
market.$symbol.depth.size_${size}.high_freq |  
event | true | string |
事件类型；"update":更新，表示推送买卖各20档或150档不合并深度的增量数据；"snapshot":快照值，表示推送买卖各20档或150档不合并深度的全量数据
|  
</tick> |  |  |  |  
  
### Note

1、
当"data_type"为incremental时，首次推送的"event"为"snapshot"的数据，且当重新发送订阅请求时，首次返回都是"snapshot"的数据；

2、深度即可以按照合约周期订阅，也可以按照合约代码订阅，行情系统在进行数据计算时，需要更新对应类型的数据；

3、version（版本号），是自增的序号，每次增加1，不管是增量还是全量数据,每个连接是唯一的。多个websocket连接的version是可能不同的。

4、每30ms检查一次orderbook，如果有更新，则推送，如果没有更新，则不推送。

5、如果是增量数据，要自己维护好本地的orderbook bids\asks 数据。

## 订阅买一卖一逐笔行情数据(BBO)

### 成功建立和 WebSocket API 的连接之后，向 Server发送如下格式的数据来请求数据:

{

"sub": "market.$symbol.bbo",

"id": "id generated by client"

}

> 正确订阅请求参数的例子：
    
    
    {
        "sub": "market.BTC_CQ.bbo",
        "id": "id generated by client"
    }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
sub | true | string | 需要订阅的主题，该接口固定为：market.$symbol.bbo，详细参数见sub订阅参数说明 |  
id | false | string | 业务方自主生成的id |  
  
### sub订阅参数说明

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 交易对 |  |
交易对（大小写不敏感，均支持）,如“BTC190412”表示BTC品种下，到期日为2019年04月12日的合约，"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约，"BTC_NQ"表示BTC次季度合约。支持使用合约code来订阅
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
  
> Response：
    
    
    {
        "ch":"market.BTC_CQ.bbo",
        "ts":1604385767803,
        "tick":{
            "mrid":113843014986,
            "id":1604385767,
            "bid":[
                13579.06,
                1488
            ],
            "ask":[
                13579.07,
                1535
            ],
            "ts":1604385767803,
            "version":113843014986,
            "ch":"market.BTC_CQ.bbo"
        }
    }
    

### 返回参数

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
ch | true | string | 数据所属的 channel，格式： market.$symbol.bbo |  
ts | true | long | 进入行情服务器系统时间点，单位：毫秒 |  
<tick> |  |  |  |  
mrid | true | long | 订单ID |  
id | true | long | tick ID |  
ask | true | object | 卖盘,[price(挂单价), vol(此价格挂单张数)] |  
bid | true | object | 买盘,[price(挂单价), vol(此价格挂单张数)] |  
ts | true | long | 系统检测orderbook时间点，单位：毫秒 |  
version | true | long | 版本号 |  
ch | true | string | 数据所属的 channel，格式： market.$symbol.bbo |  
</tick> |  |  |  |  
  
### 说明

1、当买一价、买一量、卖一价、卖一量，其中任一数据发生变化时，进行逐笔推送；

2、如果同一时刻有多个买一卖一的价格/单量的变化，直接用最新的买一卖一进行推送；

3、由于客户端网络等原因导致接收数据失败，服务端会丢弃旧的队列数据；

4、version（版本号），直接取撮合id，保证全局唯一并且最新的推送版本号都是数值最大的。

## 订阅 Market Detail 数据

### 成功建立和 WebSocket API 的连接之后，向 Server发送如下格式的数据来请求数据:

`{`

`"sub": "market.$symbol.detail",`

`"id": "id generated by client"`

`}`

> 订阅 Market Detail 数据请求参数的例子：
    
    
        {
         "sub": "market.BTC_CQ.detail",
         "id": "id6"
        }
    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
sub | true | string | 需要订阅的主题，该接口固定为：market.$symbol.detail，详细参数见sub订阅参数说明 |  
id | false | string | 业务方自主生成的id |  
  
### sub订阅参数说明

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 交易对 |  | 支持大小写，
交易对,"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示次季度合约。支持使用合约code来订阅
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
  
> 请求成功返回数据的例子：
    
    
    {
        "ch":"market.BTC_CQ.detail",
        "ts":1604385863717,
        "tick":{
            "id":1604385840,
            "mrid":113843084999,
            "open":13607.17,
            "close":13589,
            "high":13830.63,
            "low":13411.89,
            "amount":261417.4288915740193389700120854767791857974,
            "vol":35572590,
            "count":586972
        }
    }
    

### 返回参数

参数名称 | 是否必须 | 数据类型 | 描述  
---|---|---|---  
ch | true | string | 数据所属的 channel，格式： market.$symbol.detail.merged  
ts | true | long | 响应生成时间点，单位：毫秒  
<tick> |  |  |  
id | true | long | ID  
mrid | true | long | 订单ID  
open | true | decimal | 开盘价  
close | true | decimal | 收盘价,当K线为最晚的一根时，是最新成交价  
high | true | decimal | 最高价  
low | true | decimal | 最低价  
amount | true | decimal | 成交量(币), 即 sum(每一笔成交量(张)*单张合约面值/该笔成交价)  
vol | true | decimal | 成交量（张），买卖双边成交量之和  
count | true | decimal | 成交笔数  
</tick> |  |  |  
  
## 请求 Trade Detail 数据

### 成功建立和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来请求数据：

`{`

`"req": "market.$symbol.trade.detail",`

`"id": "id generated by client"//目前这个字段可以不传，暂时没有用到，不管传啥都返回null`

`"size": "Number of data"//数据条数，最多50条，不填默认50`

`}`

> 请求 Market Detail 数据请求参数的例子：
    
    
    
        {
         "req": "market.BTC_CQ.trade.detail",
         "size": 10,
         "id": "id8"
        }
    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
req | true | string |
请求数据的主题，该接口固定为：market.$symbol.trade.detail，详细参数见req请求参数说明 |  
id | false | string | 业务方自主生成的ID |  
size | false | int | 数据条数，最多50条，不填默认50 | [1,50]  
  
### req请求参数说明

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 交易对 |  | 支持大小写，
交易对,"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示次季度合约"。支持使用合约code来订阅
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
  
仅返回当前 Trade Detail

> 请求成功返回数据的例子：
    
    
    {
        "data":[
            {
                "amount":"4",
                "ts":1604386167285,
                "id":1138433247400000,
                "price":"13586.25",
                "direction":"buy"
            },
            {
                "amount":"20",
                "ts":1604386167469,
                "id":1138433248730000,
                "price":"13586.25",
                "direction":"buy"
            }
        ],
        "id":"id8",
        "rep":"market.BTC_CQ.trade.detail",
        "status":"ok",
        "ts":1604386202755
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
rep | true | string | 数据所属的 channel，格式： market.$symbol.trade.detail |  
status | true | string | 返回状态 |  
id | true | string | 请求 ID |  
<data> |  |  |  |  
id | true | long | 成交唯一id（品种唯一） |  
price | true | string | 价格 |  
amount | true | string | 成交量(张)，买卖双边成交量之和 |  
direction | true | string | 主动成交方向 |  
ts | true | long | 订单成交时间 |  
</data> |  |  |  |  
ts | true | long | 发送时间 |  
  
## 订阅 Trade Detail 数据

### 成功建立和 WebSocket API 的连接之后，向 Server发送如下格式的数据来订阅数据：

`{`

`"sub": "market.$symbol.trade.detail",`

`"id": "id generated by client"`

`}`

> 正确订阅请求参数的例子：
    
    
        {
         "sub": "market.BTC_CQ.trade.detail",
         "id": "id7"
        }
    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
sub | true | string |
需要订阅的主题，该接口固定为：market.$symbol.trade.detail，详细参数见sub订阅参数说明 |  
id | false | string | 业务方自主生成的id |  
  
### sub订阅参数说明

参数名称 | 是否必须 | 类型 | 描述 | 默认值 | 取值范围  
---|---|---|---|---|---  
symbol | true | string | 交易对 |  | 支持大小写，
交易对,"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约,
"BTC_NQ"表示次季度合约"，支持使用合约code来订阅
例如："BTC200918"(当周)，"BTC200925"(次周)，"BTC201225"(季度)，"BTC210326"(次季度)。  
  
> 之后每当 Trade Detail 有更新时，client 会收到数据，例子：
    
    
    {
        "ch":"market.BTC_CQ.trade.detail",
        "ts":1604386599136,
        "tick":{
            "id":113843672389,
            "ts":1604386599123,
            "data":[
                {
                    "amount":120,
                    "ts":1604386599123,
                    "id":1138436723890000,
                    "price":13562.5,
                    "direction":"sell"
                },
                {
                    "amount":2,
                    "ts":1604386599123,
                    "id":1138436723890001,
                    "price":13562.5,
                    "direction":"sell"
                }
            ]
        }
    }
    

### 返回参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
ch | true | string | 数据所属的 channel，格式： market.$symbol.trade.detail |  
ts | true | long | 发送时间 |  
<tick> |  |  |  |  
id | true | long | 订单唯一id（品种唯一） |  
ts | true | long | tick数据戳 |  
<data> |  |  |  |  
amount | true | decimal | 数量（张） |  
ts | true | long | 订单时间戳 |  
id | true | long | 成交唯一id（品种唯一） |  
price | true | decimal | 价格 |  
direction | true | string | 买卖方向 |  
</data> |  |  |  |  
</tick> |  |  |  |  
  
# WebSocket指数与基差数据接口

指数与基差数据订阅ws地址：wss://api.hbdm.com/ws_index

## 订阅(sub)指数K线数据

### 成功建立和 WebSocket API 的连接之后，向 Server发送如下格式的数据来订阅数据：

`{`

`"sub": "market.$symbol.index.$period",`

`"id": "id generate by client"`

`}`

> 正确订阅请求参数的例子：
    
    
        {
        "sub": "market.BTC-USD.index.1min",
        "id": "id1"
        }
    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
sub | true | string |
需要订阅的主题，该接口固定为：market.$symbol.index.$period，详细参数见sub订阅参数说明 |  
id | false | string | 业务方自主生成的id |  
  
### sub订单参数说明

**参数名称** | **是否必须** | **类型** | **描述** | **默认值** | **取值范围**  
---|---|---|---|---|---  
symbol | true | string | 指数标识 |  | 支持大小写，"BTC-USD","ETH-USD"...  
period | true | string | K线类型 |  | 仅支持小写,1min, 5min, 15min, 30min,
60min,4hour,1day, 1mon  
  
### 备注

  * 当指数有变化时会推送;

  * 指数无变化时会根据订阅的周期推送；

> 之后每当 KLine 有更新时，client 会收到数据
    
    
    {
        "ch":"market.BTC-USD.index.1min",
        "ts":1604387688243,
        "tick":{
            "id":1604387640,
            "open":"13419.4325",
            "close":"13420.3325",
            "high":"13424.4925",
            "low":"13419.4325",
            "amount":"0",
            "vol":"0",
            "count":0
        }
    }
    

### 返回参数

**参数名称** | **类型** | **描述** | **默认值** | **取值范围**  
---|---|---|---|---  
ch | string | 数据所属的 channel，格式： market.$symbol.index.$period |  |  
ts | long | 响应生成时间点，单位：毫秒 |  |  
tick | object array | tick返回，详情：推送tick参数 |  |  
  
### 推送tick参数

**参数名称** | **类型** | **描述** |  
---|---|---|---  
id | string | 指数K线id,也就是K线时间戳，K线起始时间 |  
vol | string | 成交量张数为0 |  
count | decimal | 成交笔数为0 |  
open | string | 开盘指数价 |  
close | string | 收盘指数价 |  
low | string | 最低指数价 |  
high | string | 最高指数价 |  
amount | string | 数值为0 |  
  
## 请求(req)指数K线数据

### 成功建立和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来请求数据：

`{`

`"req": "market.$symbol.index.$period",`

`"id": "id generated by client",`

`"from": "type: long, 2017-07-28T00:00:00+08:00 至2050-01-01T00:00:00+08:00
之间的时间点，单位：秒",`

`"to": "type: long, 2017-07-28T00:00:00+08:00 至2050-01-01T00:00:00+08:00
之间的时间点，单位：秒，必须比 from 大",`

`}`

> 正确订阅请求参数的例子:
    
    
        {
        "req": "market.btc-usd.index.1min",
        "id": "id4",
        "from":1571000000,
        "to":1573098606
        }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
req | true | string |
需要订阅的主题，该接口固定为：market.$symbol.index.$period，详细参数见req请求参数说明 |  
id | false | string | 业务方自主生成的id |  
from | true | long | 开始时间,2017-07-28T00:00:00+08:00 至2050-01-01T00:00:00+08:00
之间的时间点，单位：秒 |  
to | true | long | 结束时间, 2017-07-28T00:00:00+08:00 至2050-01-01T00:00:00+08:00
之间的时间点，单位：秒，必须比 from 大 |  
  
### req请求参数说明：

**参数名称** | **是否必须** | **类型** | **描述** | **默认值** | **取值范围**  
---|---|---|---|---|---  
symbol | true | string | 指数标识 |  | 支持大小写, "BTC-USD","ETH-USD"...  
period | true | string | K线类型 |  | 1min, 5min, 15min, 30min, 60min,4hour,1day,
1mon  
  
### 说明：

  * 一次返回最多2000条数据；

> 请求成功返回数据的例子：
    
    
    {
        "id":"id4",
        "rep":"market.BTC-USD.index.60min",
        "wsid":915217437,
        "status":"ok",
        "data":[
            {
                "id":1604160000,
                "open":13862.65,
                "close":13832.615,
                "low":13822.41,
                "high":13890.2225,
                "amount":0,
                "vol":0,
                "count":0
            },
            {
                "id":1604163600,
                "open":13832.7725,
                "close":13788.6625,
                "low":13751.9075,
                "high":13833.41,
                "amount":0,
                "vol":0,
                "count":0
            }
        ]
    }
    

### 返回参数

**参数名称** | **类型** | **描述** | **默认值** | **取值范围**  
---|---|---|---|---  
req | true | string | 数据所属的 channel，格式：market.$symbol.index.$period |  
status | true | string | 请求处理结果 | "ok" , "error"  
id | true | string | 业务方id |  
wsid | true | long | wsid |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
tick | object array | tick返回，详情：推送tick参数 |  |  
  
### 推送tick参数

**参数名称** | **类型** | **描述** |  
---|---|---|---  
id | decimal | 指数K线id,也就是K线时间戳，K线起始时间 |  
vol | decimal | 成交量张数为0 |  
count | decimal | 成交笔数为0 |  
open | decimal | 开盘指数价 |  
close | decimal | 收盘指数价 |  
low | decimal | 最低指数价 |  
high | decimal | 最高指数价 |  
amount | decimal | 数值为0 |  
  
## 订阅(sub)基差数据

### 成功建立和 WebSocket API 的连接之后，向 Server发送如下格式的数据来订阅数据：

`{`

`"sub": "market.$symbol.basis.$period.$basis_price_type",`

`"id": "id generate by client"`

`}`

> 正确订阅请求参数的例子：
    
    
        {
        "sub": "market.BTC_CW.basis.1min.open",
        "id": "id1"
        }
    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
sub | true | string |
需要订阅的主题，该接口固定为：market.$symbol.basis.$period.$basis_price_type，详细参数见sub订阅参数说明 |  
id | false | string | 业务方自主生成的id |  
  
### sub订阅参数说明：

**参数名称** | **是否必须** | **类型** | **描述** | **默认值** | **取值范围**  
---|---|---|---|---|---  
symbol | true | string | 合约名称 |  |
支持大小写，如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约, "BTC_NQ"表示次季合约"  
period | true | string | 周期 |  | 1min, 5min, 15min, 30min, 60min,4hour,1day,
1mon  
basis_price_type | false | string | 基差价格类型，表示在周期内计算基差使用的价格类型 | 不填，默认为使用开盘价
（open） | 开盘价：open，收盘价：close，最高价：high，最低价：low，平均价=（最高价+最低价）/2：average  
  
  * 备注：次季度的基差数据在2020/6/15 14:00:00后才开始生成

> 之后每当基差有更新时，client 会收到数据，例子
    
    
    {
        "ch":"market.BTC_CW.basis.5min.close",
        "ts":1604387856115,
        "tick":{
            "id":1604387700,
            "index_price":"13434.5075",
            "contract_price":"13454.01",
            "basis":"19.5025",
            "basis_rate":"0.0014516721212147151654052074480586653"
        }
    }
    

### 返回参数

**参数名称** | **是否必须** | **类型** | **描述** | **默认值** | **取值范围**  
---|---|---|---|---|---  
ch | true | string | 数据所属的
channel，格式：market.$symbol.basis.$period.$basis_price_type |  |  
tick | true | object array | tick返回，详情：tick参数说明 |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  |  
  
#### tick参数说明

**参数名称** | **类型** | **描述**  
---|---|---  
id | long | 唯一标识  
contract_price | string | 合约最新成交价  
index_price | string | 指数基准价，与基差价格类型匹配  
basis | string | 基差=合约基准价 - 指数基准价  
basis_rate | string | 基差率=基差/指数基准价  
  
## 请求(req)基差数据

### 成功建立和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来请求数据：

`{`

`"req": "market.$symbol.basis.$period.$basis_price_type",`

`"id": "id generated by client",`

`"from": "type: long, 2017-07-28T00:00:00+08:00 至2050-01-01T00:00:00+08:00
之间的时间点，单位：秒",`

`"to": "type: long, 2017-07-28T00:00:00+08:00 至2050-01-01T00:00:00+08:00
之间的时间点，单位：秒，必须比 from 大",`

`}`

> 正确订阅请求参数的例子:
    
    
        {
        "req": "market.btc_cw.basis.1min.open",
        "id": "id4",
        "from":1571000000,
        "to":1573098606
        }
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 默认值  
---|---|---|---|---  
sub | true | string |
需要订阅的主题，该接口固定为：market.$symbol.basis.$period.$basis_price_type，详细参数见req请求参数说明 |  
id | false | string | 业务方自主生成的id |  
from | true | long | 开始时间,2017-07-28T00:00:00+08:00 至2050-01-01T00:00:00+08:00
之间的时间点，单位：秒 |  
to | true | long | 结束时间, 2017-07-28T00:00:00+08:00 至2050-01-01T00:00:00+08:00
之间的时间点，单位：秒，必须比 from 大 |  
  
### req请求参数说明：

**参数名称** | **是否必须** | **类型** | **描述** | **默认值** | **取值范围**  
---|---|---|---|---|---  
symbol | true | string | 合约名称 |  |
支持大小写，如"BTC_CW"表示BTC当周合约，"BTC_NW"表示BTC次周合约，"BTC_CQ"表示BTC当季合约, "BTC_NQ"表示次季合约"  
period | true | string | 周期 |  | 1min, 5min, 15min, 30min, 60min,4hour,1day,
1mon  
basis_price_type | false | string | 基差价格类型，表示在周期内计算基差使用的价格类型 | 不填，默认为使用开盘价
（open） | 开盘价：open，收盘价：close，最高价：high，最低价：low，平均价=（最高价+最低价）/2：average  
  
### 说明：

  * 一次返回最多2000条数据；

> 请求成功返回数据的例子：
    
    
    {
        "data":[
            {
                "basis":"20.357500000000073",
                "basis_rate":"0.0014671752201438544",
                "contract_price":"13895.66",
                "id":1604160000,
                "index_price":"13875.3025"
            },
            {
                "basis":"20.13249999999971",
                "basis_rate":"0.001454177342461542",
                "contract_price":"13864.73",
                "id":1604160300,
                "index_price":"13844.5975"
            }
        ],
        "id":"id4",
        "rep":"market.BTC_CW.basis.5min.close",
        "status":"ok",
        "ts":1604387965575,
        "wsid":3823737955
    }
    

### 返回参数

**参数名称** | **是否必须** | **类型** | **描述** | **默认值** | **取值范围**  
---|---|---|---|---|---  
req | true | string | 数据所属的
channel，格式：market.$symbol.basis.$period.$basis_price_type |  |  
status | true | string | 请求处理结果 | "ok" , "error" |  
id | true | string | 业务方id |  |  
wsid | true | long | wsid |  |  
ts | true | long | 响应生成时间点，单位：毫秒 |  |  
data | true | object array | data返回，详情：data参数描述 |  |  
  
### data参数描述

**参数名称** | **类型** | **描述**  
---|---|---  
id | long | 唯一标识  
contract_price | string | 合约最新成交价  
index_price | string | 指数基准价，与基差价格类型匹配  
basis | string | 基差=合约基准价 - 指数基准价  
basis_rate | string | 基差率=基差/指数基准价  
  
# WebSocket订单和用户数据接口

## 订阅订单成交数据（sub）

成功建立和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来订阅数据:

### 订阅请求数据格式

`{`

`“op”: “sub”,`

`"cid": "id generated by client”,`

`“topic": "orders.$symbol”`

`}`

> 正确的订阅请求:
    
    
    {
      "op": "sub",
      "cid": "40sG903yz80oDFWr",
      "topic": "orders.btc"
    }
    
    

### 订阅请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填；操作名称，订阅固定值为sub  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填；订阅主题名称，orders.$symbol; symbol支持大小写，比如：BTC,ETH ;当 $symbol值为
* 时代表订阅所有品种;  
  
  * 备注：postOnly的报单收到的WS推送要么是报单成功，状态为3，要么是7，已撤单。

> 成交详情通知数据格式说明
    
    
    {
        "op":"notify",
        "topic":"orders.ada",
        "ts":1604388667226,
        "symbol":"ADA",
        "contract_type":"quarter",
        "contract_code":"ADA201225",
        "volume":1,
        "price":0.0905,
        "order_price_type":"post_only",
        "direction":"sell",
        "offset":"open",
        "status":6,
        "lever_rate":20,
        "order_id":773207641127878656,
        "order_id_str":"773207641127878656",
        "client_order_id":null,
        "order_source":"web",
        "order_type":1,
        "created_at":1604388667146,
        "trade_volume":1,
        "trade_turnover":10,
        "fee":-0.022099447513812154,
        "trade_avg_price":0.0905,
        "margin_frozen":0,
        "profit":0,
        "trade":[
            {
                "trade_fee":-0.022099447513812154,
                "fee_asset":"ADA",
                "trade_id":113913755890,
                "id":"113913755890-773207641127878656-1",
                "trade_volume":1,
                "trade_price":0.0905,
                "trade_turnover":10,
                "created_at":1604388667194,
                "role":"maker"
            }
        ],
        "canceled_at":0,
        "fee_asset":"ADA",
        "uid":"123456789",
        "liquidation_type":"0"
    }
    

### 成交推送返回数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填;操作名称，推送固定值为 notify;  
topic | string | 必填;推送的主题  
uid | string | 必填;账户ID  
ts | long | 服务端应答时间戳  
symbol | string | 品种ID  
contract_type | string | 合约类型  
contract_code | string | 合约代码  
volume | decimal | 委托数量  
price | decimal | 委托价格  
order_price_type | string | 订单报价类型
"limit":限价，"opponent":对手价，"post_only":只做maker单,post
only下单只受用户持仓数量限制，"lightning":闪电平仓，"optimal_5":最优5档，"optimal_10":最优10档，"optimal_20":最优20档，"fok":FOK订单，"ioc":IOC订单,
"opponent_ioc": 对手价-IOC下单，"lightning_ioc": 闪电平仓-IOC下单，"optimal_5_ioc":
最优5档-IOC下单，"optimal_10_ioc":
最优10档-IOC下单，"optimal_20_ioc"：最优20档-IOC下单，"opponent_fok"： 对手价-
FOK下单，"lightning_fok"：闪电平仓-
FOK下单，"optimal_5_fok"：最优5档-FOK下单，"optimal_10_fok"：最优10档-FOK下单，"optimal_20_fok"：最优20档-FOK下单  
direction | string | "buy":买 "sell":卖  
offset | string | "open":开 "close":平  
status | int | 订单状态(1准备提交 2准备提交 3已提交 4部分成交 5部分成交已撤单 6全部成交 7已撤单)  
lever_rate | int | 杠杆倍数  
order_id | long | 订单ID  
order_id_str | string | 订单ID  
client_order_id | long | 客户订单ID  
order_source | string |
订单来源（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
order_type | int | 订单类型 1:报单 、 2:撤单 、 3:强平、4:交割  
created_at | long | 订单创建时间  
canceled_at | long | 订单撤单时间  
trade_volume | decimal | 总成交数量  
trade_turnover | decimal | 成交总金额  
fee | decimal | 手续费  
fee_asset | string | 手续费币种  
trade_avg_price | decimal | 成交均价  
margin_frozen | decimal | 冻结保证金  
profit | decimal | 收益  
liquidation_type | string | 强平类型 0:非强平类型，1：多空轧差， 2:部分接管，3：全部接管  
<trade> | list |  
id | string | 全局唯一的交易标识  
trade_id | long | 撮合结果id,与api/v1/contract_matchresults返回结果中的match_id一样，
非唯一，可重复，注意：一个撮合结果代表一个taker单和N个maker单的成交记录的集合，如果一个taker单吃了N个maker单，那这N笔trade都是一样的撮合结果id  
trade_volume | decimal | 成交量  
trade_price | decimal | 撮合价格  
trade_fee | decimal | 成交手续费  
trade_turnover | decimal | 成交金额  
created_at | long | 成交创建时间  
role | string | taker或maker  
fee_asset | string | 手续费币种  
</trade> |  |  
  
## 取消订阅订单成交数据（unsub）

成功建⽴和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来取消订阅数据:

### 取消订阅请求数据格式

`{`

`“op”: “unsub”,`

`“topic": "orders.$symbol”,`

`"cid": "id generated by client”,`

`}`

> 正确的取消订阅请求:
    
    
    {
      "op": "unsub",
      "topic": "orders.btc",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### 取消订阅请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填;操作名称，订阅固定值为 unsub;  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填;待取消订阅主题名称:orders.$symbol; symbol支持大小写，比如:BTC,ETH ; 当
$symbol值为 * 时代表取消订阅所有品种;  
  
### 订阅与取消订阅规则说明

订阅(sub) | 取消订阅(unsub) | 规则  
---|---|---  
orders.* | orders.* | 允许  
orders.symbol1 | orders.* | 允许  
orders.symbol1 | orders.symbol1 | 允许  
orders.symbol1 | orders.symbol2 | 不允许  
orders.* | orders.symbol1 | 不允许  
  
## 订阅订单撮合数据（sub）

成功建立和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来订阅数据:

### 订阅请求数据格式

`{`

`“op”: “sub”,`

`"cid": "cid”,`

`“topic": "matchOrders.$symbol”`

`}`

> 正确的订阅请求:
    
    
    {
      "op": "sub",
      "cid": "40sG903yz80oDFWr",
      "topic": "matchOrders.btc"
    }
    
    

### 订阅请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填；操作名称，订阅固定值为sub  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填，订阅主题名称:matchOrders.$symbol; symbol支持大小写，比如：BTC，ETH ; 当
$symbol值为 * 时代表订阅所有品种;  
  
#### 备注：

  * postOnly的报单收到的WS推送要么是报单成功，状态为3，要么是7，已撤单;
  * 撮合完成后就将订单的更新信息推送给客户端;
  * 交割订单不走撮合不走清算，所以撮合后不推送，清算后也不推送；
  * 强平以及轧差订单不会推送；
  * 外部划转或内部转账订单不作为订单推送；
  * 通常情况下，撮合完成后的推送要比清算完成后的推送快，但不能保证撮合完成后的推送一定比清算完成后的推送更快;
  * 撮合后的推送，假设1个matchresult包含N笔成交，包括1个taker和N个maker，那最多推送N+1笔；
  * 如果遇到推送的status状态为9或者10，可以直接忽略。

> 成交详情通知数据格式说明
    
    
    {
        "op":"notify",
        "topic":"matchOrders.ada",
        "ts":1604388667219,
        "symbol":"ADA",
        "contract_code":"ADA201225",
        "contract_type":"quarter",
        "status":6,
        "order_id":773207641127878656,
        "order_id_str":"773207641127878656",
        "client_order_id":null,
        "order_type":1,
        "created_at":1604388667146,
        "trade":[
            {
                "trade_id":113913755890,
                "id":"113913755890-773207641127878656-1",
                "trade_volume":1,
                "trade_price":0.0905,
                "trade_turnover":10,
                "created_at":1604388667194,
                "role":"maker"
            }
        ],
        "uid":"123456789",
        "volume":1,
        "trade_volume":1,
        "direction":"sell",
        "offset":"open",
        "lever_rate":20,
        "price":0.0905,
        "order_source":"web",
        "order_price_type":"post_only"
    }
    

### 成交推送返回数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 操作名称，推送固定值为 notify;  
topic | string | 推送的主题  
uid | string | 账户UID  
ts | long | 服务端应答时间戳  
symbol | string | 品种ID  
contract_type | string | 合约类型  
contract_code | string | 合约代码  
status | int | 订单状态(1准备提交 2准备提交 3已提交 4部分成交 5部分成交已撤单 6全部成交 7已撤单)  
order_id | bigint | 订单ID  
order_id_str | string | 订单ID  
client_order_id | long | 客户端订单ID  
order_type | int | 订单类型 1:报单 、 2:撤单 、 3:强平、4:交割  
trade_volume | decimal | 订单已成交数量  
volume | decimal | 订单总委托数量  
<trade> | list |  
id | string | 全局唯一交易标识  
trade_id | long | 撮合结果id，与api/v1/contract_matchresults返回结果中的match_id一样,
非唯一，可重复，注意：一个撮合结果代表一个taker单和N个maker单的成交记录的集合，如果一个taker单吃了N个maker单，那这N笔trade都是一样的撮合结果id  
trade_volume | decimal | 成交量  
trade_price | decimal | 撮合价格  
trade_turnover | decimal | 成交金额  
created_at | long | 创建时间  
role | string | taker或maker  
</trade> |  |  
direction | string | 买卖方向: "buy":买 "sell":卖  
offset | string | 开平方向: "open":开 "close":平  
lever_rate | int | 杠杆倍数  
price | decimal | 委托价格  
created_at | long | 创建时间  
order_source | string |
订单来源（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
order_price_type | string | 订单报价类型: "limit":限价 "opponent":对手价
"post_only":只做maker单,post
only下单只受用户持仓数量限制,optimal_5：最优5档、optimal_10：最优10档、optimal_20：最优20档，ioc：IOC订单，fok：FOK订单,"opponent_ioc":
对手价-IOC下单，"optimal_5_ioc": 最优5档-IOC下单，"optimal_10_ioc":
最优10档-IOC下单，"optimal_20_ioc"：最优20档-IOC下单，"opponent_fok"： 对手价-
FOK下单，"optimal_5_fok"：最优5档-FOK下单，"optimal_10_fok"：最优10档-FOK下单，"optimal_20_fok"：最优20档-FOK下单  
  
## 取消订阅订单撮合数据（unsub）

成功建⽴和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来取消订阅数据:

### 取消订阅请求数据格式

`{`

`“op”: “unsub”,`

`“topic": "matchOrders.btc”,`

`"cid": "id generated by client”,`

`}`

> 正确的取消订阅请求:
    
    
    {
      "op": "unsub",
      "topic": "matchOrders.$symbol",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### 取消订阅请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填;操作名称，订阅固定值为 unsub;  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填;待取消订阅主题名:matchOrders.$symbol; symbol支持大小写，比如:BTC,ETH ; 当
$symbol值为 * 时代表取消订阅所有品种;  
  
### 订阅与取消订阅规则说明

订阅(sub) | 取消订阅(unsub) | 规则  
---|---|---  
matchOrders.* | matchOrders.* | 允许  
matchOrders.symbol1 | matchOrders.* | 允许  
matchOrders.symbol1 | matchOrders.symbol1 | 允许  
matchOrders.symbol1 | matchOrders.symbol2 | 不允许  
matchOrders.* | matchOrders.symbol1 | 不允许  
  
## 订阅资产变动数据（sub）

成功建立和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来订阅数据:

### 订阅请求数据格式

`{`

`"op": "sub",`

`"cid": "id generated by client”,`

`“topic": "accounts.$symbol”`

`}`

> 正确的订阅请求:
    
    
    {
      "op": "sub",
      "cid": "40sG903yz80oDFWr",
      "topic": "accounts.btc"
    }
    
    

### 订阅请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填；操作名称，订阅固定值为sub  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填；订阅主题名称: accounts.$symbol; symbol支持大小写，比如：BTC，ETH ; 当
$symbol值为 * 时代表订阅所有品种;  
  
> 当资产有更新时，返回的参数示例如下:
    
    
    {
        "op":"notify",
        "topic":"accounts.ada",
        "ts":1604388667226,
        "event":"order.match",
        "data":[
            {
                "symbol":"ADA",
                "margin_balance":446.417641681222726716,
                "margin_static":445.554085945257745136,
                "margin_position":11.049723756906077348,
                "margin_frozen":0,
                "margin_available":435.367917924316649368,
                "profit_real":21.627049781983019459,
                "profit_unreal":0.86355573596498158,
                "risk_rate":40.000796572150656768,
                "liquidation_price":0.018674308027108984,
                "withdraw_available":423.927036163274725677,
                "lever_rate":20,
                "adjust_factor":0.4
            }
        ],
        "uid":"123456789"
    }
    

### 返回参数字段说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填;操作名称，推送固定值为 notify;  
topic | string | 必填;推送的主题  
uid | string | 账户UID  
ts | long | 响应生成时间点，单位：毫秒  
event | string | 资产变化通知相关事件说明，比如订单创建开仓(order.open)
、订单成交(order.match)（除开强平和结算交割）、结算交割(settlement)、订单强平成交(order.liquidation)（对钆和接管仓位）、订单撤销(order.cancel)
、合约账户划转（contract.transfer)（包括外部划转）、系统（contract.system)、其他资产变化(other)、切换杠杆（switch_lever_rate）、初始资金（init）  
<data> | list |  
symbol | string | 品种代码 ,"BTC","ETH"...，  
margin_balance | decimal | 账户权益  
margin_static | decimal | 静态权益  
margin_position | decimal | 持仓保证金（当前持有仓位所占用的保证金）  
margin_frozen | decimal | 冻结保证金  
margin_available | decimal | 可用保证金  
profit_real | decimal | 已实现盈亏  
profit_unreal | decimal | 未实现盈亏  
risk_rate | decimal | 保证金率  
liquidation_price | decimal | 预估爆仓价  
withdraw_available | decimal | 可划转数量  
lever_rate | decimal | 杠杆倍数  
adjust_factor | decimal | 调整系数  
</data> |  |  
  
### 备注:

  * 每 5 秒进行一次定期推送，由定期推送触发的数据中 event 参数值为“snapshot”，表示由系统定期推送触发。如果 5 秒内已经触发过推送，则该品种跳过该次定期推送。

## 取消订阅资产变动数据（unsub）

成功建⽴和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来取消订阅数据:

### 取消订阅请求数据格式

`{`

`“op”: “unsub”,`

`“topic": "accounts.$symbol”,`

`"cid": "id generated by client”,`

`}`

> 正确的取消订阅请求:
    
    
    {
      "op": "unsub",
      "topic": "accounts.btc",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### 取消订阅请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填;操作名称，订阅固定值为 unsub;  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填;待取消订阅主题名称: accounts.$symbol; symbol支持大小写,比如：BTC，ETH ; 当
$symbol值为 * 时代表取消订阅所有品种;  
  
### 订阅与取消订阅规则说明

订阅(sub) | 取消订阅(unsub) | 规则  
---|---|---  
accounts.* | accounts.* | 允许  
accounts.symbol1 | accounts.* | 允许  
accounts.symbol1 | accounts.symbol1 | 允许  
accounts.symbol1 | accounts.symbol2 | 不允许  
accounts.* | accounts.symbol1 | 不允许  
  
## 订阅持仓变动更新数据（sub）

成功建立和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来订阅数据:

### 订阅请求数据格式

`{`

`“op”: “sub”,`

`"cid": "id generated by client”,`

`“topic": "positions.$symbol”`

`}`

> 正确的订阅请求:
    
    
    {
      "op": "sub",
      "cid": "40sG903yz80oDFWr",
      "topic": "positions.btc"
    }
    
    

### 订阅请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填；操作名称，订阅固定值为sub  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填；订阅主题名称:positions.$symbol; symbol支持大小写,比如:BTC,ETH ; 当
$symbol值为 * 时代表订阅所有品种  
  
> 当持仓有更新时，返回的参数示例如下
    
    
    {
        "op":"notify",
        "topic":"positions.ada",
        "ts":1604388667226,
        "event":"order.match",
        "data":[
            {
                "symbol":"ADA",
                "contract_code":"ADA201225",
                "contract_type":"quarter",
                "volume":1,
                "available":1,
                "frozen":0,
                "cost_open":0.0905,
                "cost_hold":0.0905,
                "profit_unreal":0,
                "profit_rate":0,
                "profit":0,
                "position_margin":5.524861878453038674,
                "lever_rate":20,
                "direction":"sell",
                "last_price":0.0905
            }
        ],
        "uid":"123456789"
    }
    
    

### 返回参数说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填;操作名称，推送固定值为 notify;  
topic | string | 必填;推送的主题  
uid | string | 账户ID  
ts | long | 响应生成时间点，单位：毫秒  
event | string | 持仓变化通知相关事件说明，比如订单创建平仓(order.close)
、订单成交(order.match)（除开强平和结算交割）、结算交割(settlement)、订单强平成交(order.liquidation)（对钆和接管仓位）、订单撤销(order.cancel)、切换杠杆（switch_lever_rate）
、初始持仓（init）、由系统定期推送触发（snapshot）。  
<data> | list |  
symbol | string | 品种代码 ,"BTC","ETH"...，  
contract_code | string | 合约代码  
contract_type | string | 合约类型,当周:"this_week", 次周:"next_week", 当季:"quarter",
次季:"next_quarter", 已下市：“delivered”  
volume | decimal | 持仓量  
available | decimal | 可平仓数量  
frozen | decimal | 冻结数量  
cost_open | decimal | 开仓均价  
cost_hold | decimal | 持仓均价  
profit_unreal | decimal | 未实现盈亏  
profit_rate | decimal | 收益率  
profit | decimal | 收益  
position_margin | decimal | 持仓保证金  
lever_rate | decimal | 杠杆倍数  
direction | string | 仓位方向 "buy":买 "sell":卖  
last_price | decimal | 最新成交价  
</data> |  |  
  
### 备注

  * 每 5 秒进行一次定期推送，由定期推送触发的数据中 event 参数值为“snapshot”，表示由系统定期推送触发。如果 5 秒内已经触发过推送，则该品种跳过该次定期推送。

  * 当用户持仓量为0时使用切换杠杆的接口，持仓推送接口不会推送"switch_lever_rate"。

## 取消订阅持仓变动更新数据（unsub）

成功建⽴和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来取消订阅数据:

### 取消订阅请求数据格式

`{`

`“op”: “unsub”,`

`“topic": "positions.$symbol”,`

`"cid": "id generated by client”,`

`}`

> 正确的取消订阅请求:
    
    
    {
      "op": "unsub",
      "topic": "positions.btc",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### 取消订阅请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填;操作名称，订阅固定值为 unsub;  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填；待取消订阅主题名称:positions.$symbol; symbol支持大小写,比如:BTC,ETH ; 当
$symbol值为 * 时代表取消订阅所有品种  
  
### 订阅与取消订阅规则说明

订阅(sub) | 取消订阅(unsub) | 规则  
---|---|---  
positions.* | positions.* | 允许  
positions.symbol1 | positions.* | 允许  
positions.symbol1 | positions.symbol1 | 允许  
positions.symbol1 | positions.symbol2 | 不允许  
positions.* | positions.symbol1 | 不允许  
  
## 订阅强平订单数据(免鉴权)（sub）

### 订阅强平订单数据格式

`{`

`“op”: “sub”,`

`“topic": "public.$symbol.liquidation_orders”,`

`"cid": "id generated by client”,`

`}`

> 正确的订阅请求:
    
    
    {
      "op": "sub",
      "cid": "40sG903yz80oDFWr",
      "topic": "public.BTC.liquidation_orders"
    }
    
    

### **请求参数**

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
op | true | string | 订阅固定值为sub |  
cid | false | string | Client 请求唯一 ID |  
topic | true | string | 必填;订阅主题名称:public.$symbol.liquidation_orders;
订阅某个品种下的强平订单信息；$symbol为品种代码（BTC、ETH），如果值为 * 时代表订阅所有品种; symbol支持大小写 |  
  
### **返回参数说明**

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
op | true | string | 操作名称，推送固定值为 notify; |  
topic | true | string | 推送的主题 |  
ts | true | long | 服务端应答时间戳 |  
<data> | true | array object |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
contract_code | true | string | 合约代码 |  
direction | true | string | 仓位方向 | "buy":买 "sell":卖  
offset | true | string | 开平方向 | "open":开 "close":平  
volume | true | decimal | 强平数量（张） |  
amount | true | decimal | 强平数量（币） |  
price | true | decimal | 破产价格 |  
created_at | true | long | 订单创建时间 |  
</data> |  |  |  |  
  
> 当有订单被爆仓账户接管后，返回的参数示例如下：
    
    
    {
        "op":"notify",
        "topic":"public.BTC.liquidation_orders",
        "ts":1580815422403,
        "data":[
            {
                "contract_code": "BTC201225",
                "symbol": "BTC",
                "direction": "buy",
                "offset": "close",
                "volume": 26,
                "price": 19674.96,
                "created_at": 1606293144641,
                "amount": 0.132147663832607537
            }
        ]
    }
    

## 取消订阅强平订单(免鉴权)（unsub）

### 取消订阅强平订单数据格式

`{`

`“op”: “unsub”,`

`“topic": "public.$symbol.liquidation_orders”,`

`"cid": "id generated by client”,`

`}`

> 正确的取消订阅请求:
    
    
    {
      "op": "unsub",
      "topic": "public.EOS.liquidation_orders",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### 取消订阅请求参数

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填;操作名称，订阅固定值为 unsub;  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填;订阅主题名称:public.$symbol.liquidation_orders; symbol支持大小写
比如:BTC,ETH ; 当 $symbol值为 * 时代表取消订阅所有品种  
  
### 订阅与取消订阅规则说明

订阅(sub) | 取消订阅(unsub) | 规则  
---|---|---  
public.*.liquidation_orders | public.*.liquidation_orders | 允许  
public.$symbol.liquidation_orders | public.*.liquidation_orders | 允许  
public.symbol1.liquidation_orders | public.symbol1.liquidation_orders | 允许  
public.symbol1.liquidation_orders | public.symbol2.liquidation_orders | 不允许  
public.*.liquidation_orders | public.symbol1.liquidation_orders | 不允许  
  
## 订阅合约信息变动(免鉴权)（sub）

成功建立和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来订阅数据:

`{`

`"op": "sub",`

`"cid": "40sG903yz80oDFWr",`

`"topic": "public.$symbol.contract_info"`

`}`

> 正确的取消订阅请求:
    
    
    {
      "op": "sub",
      "topic": "public.btc.contract_info",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
op | true | string | 必填；订阅固定值为sub |  
cid | false | string | 选填；Client 请求唯一 ID |  
topic | true | string | 必填；订阅主题名称:public.$symbol.contract_info;
订阅某个品种下的合约变动信息；$symbol为品种代码（BTC、ETH），如果值为 * 时代表订阅所有品种; symbol支持大小写; |  
  
### 返回的参数为：

    
    
    {
        "op":"notify",
        "topic":"public.btc.contract_info",
        "ts":1604389592693,
        "event":"snapshot",
        "data":[
            {
                "symbol":"BTC",
                "contract_code":"BTC201106",
                "contract_type":"this_week",
                "contract_size":100,
                "price_tick":0.01,
                "delivery_date":"20201106",
                "create_date":"20201016",
                "contract_status":1
            },
            {
                "symbol":"BTC",
                "contract_code":"BTC201113",
                "contract_type":"next_week",
                "contract_size":100,
                "price_tick":0.01,
                "delivery_date":"20201113",
                "create_date":"20201023",
                "contract_status":1
            },
            {
                "symbol":"BTC",
                "contract_code":"BTC201225",
                "contract_type":"quarter",
                "contract_size":100,
                "price_tick":0.01,
                "delivery_date":"20201225",
                "create_date":"20200612",
                "contract_status":1
            },
            {
                "symbol":"BTC",
                "contract_code":"BTC210326",
                "contract_type":"next_quarter",
                "contract_size":100,
                "price_tick":0.01,
                "delivery_date":"20210326",
                "create_date":"20200904",
                "contract_status":1
            }
        ]
    }
    

### 返回参数

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
op | true | string | 操作名称，推送固定值为 notify |  
topic | true | string | 推送的主题 |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
event | true | string | 通知相关事件说明 |
订阅成功返回的初始合约信息（init），合约信息字段变化触发（update），系统定期推送触发（snapshot）  
<data> | true | object array |  |  
symbol | true | string | 品种代码 | "BTC","ETH"...  
contract_code | true | string | 合约代码 | "BTC200626" ...  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter".  
contract_size | true | decimal | 合约面值，即1张合约对应多少美元 | 10, 100...  
price_tick | true | decimal | 合约价格最小变动精度 | 0.001, 0.01...  
delivery_date | true | string | 合约交割日期 | 时间戳，如"20200327"  
create_date | true | string | 合约上市日期 | 如"20180706"  
contract_status | true | int | 合约状态 |
0:已下市、1:上市、2:待上市、3:停牌，4:暂停上市中、5:结算中、6:交割中、7:结算完成、8:交割完成、9:暂停交易中  
</data> |  |  |  |  
  
### 说明：

  * 合约信息变动WS推送接口有定期推送逻辑，每60秒进行一次定期推送，由定期推送触发的数据中event参数值为“snapshot”，表示由系统定期推送触发。如果60秒内已经触发过推送，则跳过该次定期推送。
  * 订阅成功时，会立即推送一条最新的合约信息，event为init。
  * 订阅成功后，当合约信息任何一个字段发生变化时推送最新合约信息，多个字段同时变化时仅推送一条最新合约信息，event为update。
  * 当合约状态流转为“交割完成”时，合约下次结算时间为空字符串。
  * 当周合约进入交割后，就不会推送该合约信息。
  * 只有状态为1：上市，才能够正常交易，其他状态不可交易；

## 取消订阅合约信息变动(免鉴权)（unsub）

成功建⽴和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来取消订阅数据:

### 取消订阅请求数据格式

`{`

`"op": "unsub",`

`"topic": "public.$symbol.contract_info",`

`"cid": "id generated by client",`

`}`

> 正确的取消订阅请求:
    
    
    {                                    
      "op": "unsub",                     
      "topic": "public.btc.contract_info",   
      "cid": "40sG903yz80oDFWr"          
    }                                    
    

### 取消订阅请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填;操作名称，订阅固定值为 unsub;  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填;待取消订阅主题名称:public.$symbol.contract_info;
symbol支持大小写，比如:BTC,ETH ; 当 $symbol值为 * 时代表取消订阅所有合约代码;  
  
### 订阅与取消订阅规则说明

订阅(sub) | 取消订阅(unsub) | 规则  
---|---|---  
public.*.contract_info | public.*.contract_info | 允许  
public.symbol1.contract_info | public.*.contract_info | 允许  
public.symbol1.contract_info | public.symbol1.contract_info | 允许  
public.symbol1.contract_info | public.symbol2.contract_info | 不允许  
public.*.contract_info | public.symbol1.contract_info | 不允许  
  
## 订阅计划委托订单更新

### 成功建立和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来订阅数据:

`{`

`"op": "sub",`

`"cid": "id generated by client",`

`"topic": "trigger_order.$symbol"`

`}`

> request
    
    
    {                                    
      "op": "sub",                     
      "topic": "trigger_order.BTC",   
      "cid": "40sG903yz80oDFWr"          
    }                                    
    

### 请求参数

参数名称 | 是否必须 | 类型 | 描述  
---|---|---|---  
op | true | string | 必填；订阅固定值为sub  
cid | false | string | 选填；Client 请求唯一 ID  
topic | true | string | 必填；订阅主题名称:trigger_order.$symbol;
订阅某个品种下的计划委托订单更新信息；$symbol为品种代码（BTC、ETH），如果值为 * 时代表订阅所有品种; symbol支持大小写;  
  
> **返回示例** :
    
    
    {
        "op":"notify",
        "topic":"trigger_order.ADA",
        "ts":1604390110568,
        "event":"order",
        "uid":"123456789",
        "data":[
            {
                "symbol":"ADA",
                "contract_code":"ADA201225",
                "contract_type":"quarter",
                "trigger_type":"le",
                "volume":1,
                "order_type":1,
                "direction":"buy",
                "offset":"close",
                "lever_rate":20,
                "order_id":28312417,
                "order_id_str":"28312417",
                "relation_order_id":"-1",
                "order_price_type":"limit",
                "status":2,
                "order_source":"web",
                "trigger_price":0.09,
                "triggered_price":null,
                "order_price":0.09,
                "created_at":1604390110565,
                "triggered_at":0,
                "order_insert_at":0,
                "canceled_at":0,
                "fail_code":null,
                "fail_reason":null
            }
        ]
    }
    

### **返回参数说明** ：

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
op | true | string | 操作名称，推送固定值为 notify |  
topic | true | string | 推送的主题，与订阅的入参一样 |  
ts | true | long | 响应生成时间点，单位：毫秒 |  
uid | true | string | 用户uid |  
event | true | string | 通知相关事件说明 |
计划委托订单下单成功（order），计划委托撤单成功（cancel），计划委托触发成功（trigger_success），计划委托触发失败（trigger_fail）  
<data> | true | object array |  |  
symbol | true | string | 品种代码 |  
contract_type | true | string | 合约类型 | 当周:"this_week", 次周:"next_week",
当季:"quarter"，次季度：“next_quarter”  
contract_code | true | string | 合约代码 | "BTC180914" ...  
trigger_type | true | string | 触发类型 | ge大于等于；le小于等于  
volume | true | decimal | 委托数量 |  
order_type | true | int | 订单类型 | 1、报单  
direction | true | string | 买卖方向 | 买："buy",卖："sell"  
offset | true | string | 开平方向 | 开："open",平："close"  
lever_rate | true | int | 杠杆倍数 |  
order_id | true | long | 计划委托单订单ID |  
order_id_str | true | string | 字符串类型的订单ID |  
relation_order_id | true | string | 该字段为关联限价单的关联字段，未触发前数值为-1 |  
order_price_type | true | string | 订单报价类型 |
"limit":限价，"optimal_5":最优5档，"optimal_10":最优10档，"optimal_20":最优20档  
status | true | int | 订单状态 | 2:已提交、4:报单成功、5:报单失败、6:已撤单  
order_source | true | string | 来源 |
（system:系统、web:用户网页、api:用户API、m:用户M站、risk:风控系统、settlement:交割结算、ios：ios客户端、android：安卓客户端、windows：windows客户端、mac：mac客户端、trigger：计划委托触发）  
trigger_price | true | decimal | 触发价 |  
triggered_price | true | decimal | 被触发时的价格 |  
order_price | true | decimal | 委托价 |  
created_at | true | long | 订单创建时间 |  
triggered_at | true | long | 触发时间 |  
order_insert_at | true | long | 下order单时间 |  
canceled_at | true | long | 撤单时间 |  
fail_code | true | int | 被触发时下order单失败错误码 |  
fail_reason | true | string | 被触发时下order单失败原因（英文） |  
</data> |  |  |  |  
  
#### 说明：

  * 订单状态系统处理的中间态不进行推送，比如报单中和撤单中；具体通知事件说明映射如下： 
    * 当订单状态流转到2（已提交），event通知事件为order（计划委托订单下单成功）；
    * 当订单状态流转到4（报单成功），event通知事件为trigger_success（计划委托触发成功）；
    * 当订单状态流转到6（已撤单），event通知事件为cancel（计划委托撤单成功）；
    * 当订单状态流转到5（报单失败），event通知事件为trigger_fail（计划委托触发失败）；
  * 订阅时，单品种无法重复订阅，全品种订阅可覆盖单品种的订阅，订阅全品种后无法订阅单品种；

## 取消订阅计划委托订单更新（unsub）

成功建⽴和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来取消订阅数据:

### 取消订阅计划委托订单更新

`{`

`"op": "unsub",`

`"topic": "trigger_order.$symbol",`

`"cid": "id generated by client",`

`}`

> 正确的取消订阅请求:
    
    
    {                                    
      "op": "unsub",                     
      "topic": "trigger_order.*",   
      "cid": "40sG903yz80oDFWr"          
    }                                    
    

### 取消订阅请求数据格式说明

字段名称 | 类型 | 说明  
---|---|---  
op | string | 必填;操作名称，订阅固定值为 unsub;  
cid | string | 选填;Client 请求唯一 ID  
topic | string | 必填;待取消订阅主题名称:trigger_order.$symbol; symbol支持大小写，比如:BTC,ETH ;
当 $symbol值为 * 时代表取消订阅所有合约代码;  
  
### 订阅与取消订阅规则说明

订阅(sub) | 取消订阅(unsub) | 规则  
---|---|---  
trigger_order.* | trigger_order.* | 允许  
trigger_order.symbol1 | trigger_order.* | 允许  
trigger_order.symbol1 | trigger_order.symbol1 | 允许  
trigger_order.symbol1 | trigger_order.symbol2 | 不允许  
trigger_order.* | trigger_order.symbol1 | 不允许  
  
# WebSocket系统状态更新接口

  * 系统状态更新订阅WS地址：wss://api.hbdm.com/center-notification

## 订阅系统状态更新

### 成功建立和 WebSocket API 的连接之后，向 Server 发送如下格式的数据来请求数据：

`{`

`"op": "sub",`

`"cid": "id generated by client",`

`"topic ": "public.$service.heartbeat"`

`}`

> 数据请求参数的例子：
    
    
    {
        "op": "sub",
        "cid": "id generated by client",
        "topic ": "public.futures.heartbeat"
    }
    

### **请求参数** :

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
op | true | string | 必填;订阅固定值为sub |  
cid | false | string | 选填;Client 请求唯一 ID |  
topic | true | string | 必填;订阅主题名称:public.$service.heartbeat; 订阅交割合约的系统状态信息 |  
  
### **sub订阅参数说明** :

参数名称 | 是否必须 | 类型 | 描述 | 取值范围  
---|---|---|---|---  
service | true | string | 业务代码 | futures：交割  
  
> **返回示例** :
    
    
    {
        "op": "notify",
        "topic": "public.futures.heartbeat",
        "event": "init",
        "ts":1580815422403,
        "data":{
            "heartbeat": 0,
            "estimated_recovery_time": 1408076414000
        }
    }
    
    

### **返回参数说明** ：

参数名称 | 是否必须 | 数据类型 | 描述 | 取值范围  
---|---|---|---|---  
op | true | string | 操作名称，推送固定值为 notify; |  
topic | true | string | 推送的主题 |  
event | true | string | 通知相关事件说明 | 订阅成功返回的初始系统状态信息（init），系统状态变化触发（update）  
ts | true | long | 服务端应答时间戳 |  
<data> |  |  |  |  
heartbeat | true | int | 系统状态 | 1是可用，0为不可用(即停服维护)  
estimated_recovery_time | true | long | 系统预估恢复时间，单位：毫秒 | 当系统状态为可用时，返回空值  
</data> |  |  |  |  
  
### 备注

  * 这个推送由于是轮询判断状态的，所以推送可能存在1—2秒的延迟。

# WebSocket附录

## 操作类型（OP）说明

类型 | 描述  
---|---  
ping | ⼼跳发起(server)  
pong | 心跳应答  
auth | 鉴权  
sub | 订阅消息  
unsub | 取消订阅消息  
notify | 推送订阅消息(server)  
  
## 主题（topic）类型说明

类型 | 使用操作类型 | 描述  
---|---|---  
orders.$symbol | sub,unsub | 订阅、取消订阅指定交易易对的订单变更更消息，当 $symbol 值为 * 时代表订阅所有交易易对  
  
## 响应码（Err-Code）说明

返回码 | 返回描述  
---|---  
0 | Request successfully.  
2001 | Invalid authentication.  
2002 | Authentication required.  
2003 | Authentication failed.  
2004 | Number of visits exceeds limit.  
2005 | Connection has been authenticated.  
2010 | Topic error.  
2011 | Contract doesn't exist.  
2012 | Topic not subscribed.  
2013 | Authentication type doesn't exist.  
2014 | Repeated subscription.  
2030 | Exceeds connection limit of single user.  
2040 | Missing required parameter.  
  
  
  
  
  

shell

![Navbar](images/navbar.png)

![Logo](images/logo.svg)

[v1 __](javascript:;)

  * [v1](/docs/spot/v1/en/)

[现货](/docs/spot/v1/en/) [交割合约](/docs/dm/v1/en/)
[币本位永续合约](/docs/coin_margined_swap/v1/en/)
[USDT本位永续合约](/docs/usdt_swap/v1/en/) [期权合约](/docs/option/v1/en/)

[简体中文](/docs/spot/v1/cn/)

shell

  * Introduction
    * Documentation Summary
    * Market Maker Program
  * Changelog
    * 1.2.1 2020-12-02 【 Modified “Order details acquisition” interface (When querying cancelation data of orders that have not been partially filled, if “created_at” and “order_type” parameters are not uploaded, the data that can be queried reduced from last 12 hours to last 2 hours.); modified “Query history orders” interface (When querying cancelation data of orders that have not been partially filled, the data that can be retained reduced from last 24 hours to last 2 hours.); modified “Query history orders via multiple fields” interface (When querying cancelation data of orders that have not been partially filled, the data that can be retained reduced from last 24 hours to last 2 hours.)】
    * 1.2.0 2020-11-24 【 Added: Query historical settlement records of the platform interface. Modified: Added fields of return parameter for "Query Liquidation Orders" interface and "Subscribe Liquidation Order Data" interface】
    * 1.1.9 2020-10-28 【Newly added：Query financial records via multiple fields, Query history orders via multiple fields, Query history transactions via multiple fields.】
    * 1.1.8 2020-10-15 【Newly added：Added switch leverage interface; Updated: websocket messages of account topic will be pushed when leverage switch succeeds; websocket messages of position topic will be pushed when leverage switch succeeds; new response fields are added on websocket topic of match orders; the interface(contract_order_info) supports query of 4-hour order cancellation data (previously only support to query 24-hour data).】
    * 1.1.7 2020-10-10 【Newly added：Added WS interface for subscribing system status updates push】
    * 1.1.6 2020-09-22 【Updated: Future Market Data Interfaces (including rest and ws interfaces) already support calls according to the contract code. Modified “symbol” field in request parameter: added contract code type, the format of which is fixed at “symbol-year-month-date”, for example, BTC200925. Only listing contracts can be queried currently if query according to the contract code. 】
    * 1.1.5 2020-08-06 【Added interfaces：Query user’s settlement records；Subscribe trigger orders updates】
    * 1.1.4 2020-06-19 【Updated: added the return field "client_order_id" of websocket subscription of Match Order】
    * 1.1.3 2020-06-14 【Added interfaces: websocket subscription of contract info event; websocket subscription of Market BBO; Restful Interface of querying available leverage rate; Modified Interfaces: added four depth level of websocket subscription of Market Depth; added periodical push of websocket subscription of accout event and position event; added response fields of querying orders related; added uid fields of websocket subscription of private event; added fields of websocket subscription of match orders; added high leverage; added next quarter contract;】
    * 1.1.2 2020-04-09【Add an interface: Futures liquidation order WS push without authentication】
    * 1.1.1 2020-03-12 【upgrade：added websocket subscription of index kline data；added websocket subscription of basis data; added restful interface of querying index kline data; added restful interface of querying basis data】
    * 1.1.0 2020-03-05【upgrade：add transfer between master account and sub-account; add more order types; add websocket subscription of match orders】
    * 1.0.11 2020-02-21 API Uprade
    * 1.0.10 2020-01-15 API Upgrade
    * 1.0.9 2019-12-02 API Upgrade: Added API interface with trigger order function
    * 1.0.8 2019-10-17 API Upgrade: Added the order_id_str field
    * 1.0.7 2019-10-15
    * 1.0.6 2019-08-08 API Upgrade: Added rest interface
    * 1.0.5 2019-07-10 API Upgrade: New Features of Query and Order Placing
    * 1.0.4 2019-06-06 API Upgrade:Restful interface
    * 1.0.3 2019-05-28 API Upgrade: WebSocket Portfolio Push
    * 1.0.2 2019-05-14 API Upgrade: Transfer margin between Spot account and Future account
    * 1.0.1 2019-05-09 API Upgrade: Post_only and more
    * 1.0.0 has launched on December 10, 2018
  * Future API Access Illustration
    * API List
    * Address
    * Signature Authentication & Verification
    * API Rate Limit Illustration
    * API Limitation on Order Cancellation Ratio
    * Maintenance with service suspended
    * Get system status
    * Query whether the system is available
    * Get current system timestamp
    * Details of Each Error Code
    * API Best Practice
    * Code Demo
  * Future API FAQ
    * Access and Authentication
    * Market and Websocket
    * Order and Trade
    * Error Codes
    * How to solve problems more effectively?
  * Future Market Data interface
    * Get Contract Info
    * Get Contract Index Price Information
    * Get Contract Price Limitation
    * Get Contract Open Interest Information
    * Get the estimated delivery price
    * Get Market Depth
    * Get Kline Data
    * Get Market Data Overview
    * Query The Last Trade of a Contract
    * Query a Batch of Trade Records of a Contract
    * Query information on contract insurance fund balance and estimated clawback rate
    * Query history records of insurance fund balance
    * Query information on Tiered Adjustment Factor
    * Query information on open interest
    * Query information on system status
    * Query Top Trader Sentiment Index Function-Account
    * Query Top Trader Sentiment Index Function-Position
    * Query Liquidation Order Information
    * Query historical settlement records of the platform interface
    * Query Index Kline Data
    * Query Basis Data
  * Future Account Interface
    * Query User’s Account Information
    * Query User’s Position Information
    * Query assets information of all sub-accounts under the master account
    * Query a single sub-account's assets information
    * Query a single sub-account's position information
    * Query account financial records
    * Query financial records via multiple fields
    * Query user’s settlement records
    * Query contract information on order limit
    * Query information on contract trading fee
    * Query information on Transfer Limit
    * Query information on position limit
    * Query Assets And Positions
    * Transfer between master and sub account
    * Get transfer records between master and sub account
    * Query user's API indicator disable information
    * Query Available Leverage Rate
  * Future Trade Interface
    * Place an Order
    * Place a Batch of Orders
    * Cancel an Order
    * Cancel All Orders
    * Switch Leverage
    * Place Flash Close Order
    * Get Information of an Order
    * Order details acquisition
    * Query Open Orders
    * Get History Orders
    * Query history orders via multiple fields
    * Get History Match Results
    * Query history transactions via multiple fields
    * Place Trigger Order
    * Cancel Trigger Order
    * Cancel All Trigger Orders
    * Query Trigger Order Open Orders
    * Query Trigger Order History
  * Future Transferring Interface
    * Transfer margin between Spot account and Future account
    * Error Code Table
    * Error message when err-code is ‘base-msg’.
  * Future WebSocket Reference
    * API List
    * Huobi Future WebSocket Subscription Address
    * API Rate Limit Illustration
  * WebSocket Heartbeat and Authentication Interface
    * Market Heartbeat
    * Order Push Heartbeat
    * Order Push Address
    * Server voluntarily disconnects connection
    * Server return error code but remain connection
    * Authentication
  * WebSocket Market Interface
    * Subscribe Kline data
    * Request Kline data
    * Subscribe Market Depth Data
    * Subscribe Incremental Market Depth Data
    * Subscribe Market BBO Data
    * Subscribe Market Detail Data
    * Request Trade Detail Data
    * Subscribe Trade Detail Data
  * WebSocket Index and Basis Interface
    * The websocket url of Index and Basis Data is：wss://api.hbdm.com/ws_index
    * Subscribe Index Kline Data
    * Request Index Kline Data
    * Subscribe Basis Data
    * Request Basis Data
  * Orders and Accounts WebSocket Interfaces
    * Subscribe Order Data(sub)
    * Unsubscribe Order Data（unsub）
    * Subscribe Match Order Data（sub）
    * Unsubscribe Match Order Data（unsub）
    * Subscribe Account Equity Updates Data(sub)
    * Unsubscribe Account Equity Updates Data (ubsub)
    * Subscribe Position Updates(sub)
    * Unsubscribe Position Updates Data(unsub)
    * Subscribe Liquidation Order Data(No authentication) (sub)
    * Unsubscribe Liquidation Order Data(no authentication)(unsub)
    * Subscribe Contract Info (no authentication)（sub）
    * Unsubscribe Contract Info Data(no authentication)(unsub)
    * Subscribe trigger orders updates
    * Unsubscribe trigger orders updates（unsub）
  * WebSocket interface for system status updates
    * Subscribe system status updates
  * Appendix
    * Operator Type(OP)
    * Topic Type
    * Response code（Err-Code）

  * [Sign Up for a Huobi API key ](https://www.huobi.pro/apikey/)
  * Login is required for creating an API key

# Introduction

## Documentation Summary

Welcome to the Huobi Future API! You can use our API to access all market
data, trading, and account management endpoints.

We have code example in Shell! You can view code examples in the dark area to
the right.

You can use the drop down list above to change the API version. You can also
use the language option at the top right to switch documentation language.

## Market Maker Program

Market maker program gives clients with good market making strategy an
opportunity to access customized trading fee structure.

Market makers will not be able to use point cards, VIP rate, rebate or any
other fee promotion.

### Eligibility Criteria as a Market Maker on Huobi Future

Welcome users, who are dedicated to maker strategy and have created large
trading volume, to participate in Huobi Futures long-term Market Maker
project.If you have more than 3 BTC in your Huobi future account, or more than
3 BTC in your Huobi coin margined swap account, or you have more than 3 BTC in
your Huobi option account,or more than 30000 USDT in your Huobi USDT Margined
swap account, please send the following information to [[email
protected]](/cdn-cgi/l/email-protection):

  1. Huobi UIDs (not linked to any rebate program in any accounts)
  2. Provide screenshot of trading volume for the past 30 days or VIP/corporate status with other Exchanges

# Changelog

## 1.2.1 2020-12-02 【 Modified “Order details acquisition” interface (When
querying cancelation data of orders that have not been partially filled, if
“created_at” and “order_type” parameters are not uploaded, the data that can
be queried reduced from last 12 hours to last 2 hours.); modified “Query
history orders” interface (When querying cancelation data of orders that have
not been partially filled, the data that can be retained reduced from last 24
hours to last 2 hours.); modified “Query history orders via multiple fields”
interface (When querying cancelation data of orders that have not been
partially filled, the data that can be retained reduced from last 24 hours to
last 2 hours.)】

### 1、Modified “Order details acquisition” interface (When querying
cancelation data of orders that have not been partially filled, if
“created_at” and “order_type” parameters are not uploaded, the data that can
be queried reduced from last 12 hours to last 2 hours.)

  * Interface Name：Order details acquisition

  * Interface Type：private

  * Interface URL：api/v1/contract_order_detail

### 2、modified “Query history orders” interface (When querying cancelation
data of orders that have not been partially filled, the data that can be
retained reduced from last 24 hours to last 2 hours.)

  * Interface Name：Get History Orders

  * Interface Type：private

  * Interface URL：api/v1/contract_hisorders

### 3、modified “Query history orders via multiple fields” interface (When
querying cancelation data of orders that have not been partially filled, the
data that can be retained reduced from last 24 hours to last 2 hours.)

  * Interface Name：Query history orders via multiple fields

  * Interface Type：private

  * Interface URL：api/v1/contract_hisorders_exact

## 1.2.0 2020-11-24 【 Added: Query historical settlement records of the
platform interface. Modified: Added fields of return parameter for "Query
Liquidation Orders" interface and "Subscribe Liquidation Order Data"
interface】

### 1、Added “Query historical settlement records of the platform” interface

  * Interface Name: Query historical settlement records of the platform

  * Interface Type: public

  * Interface URL: api/v1/contract_settlement_records

### 2、Added fields of return parameter for "Query Liquidation Orders"
interface（“amount” are added for return parameter “data". "amount" represents
the liquidation amount (token);）

  * Interface Name: Query Liquidation Orders

  * Interface Type: public

  * Interface URL: api/v1/contract_liquidation_orders

### 3、Added fields of return parameter for "Subscribe Liquidation Order Data"
interface（“amount” are added for return parameter “data". "amount" represents
the liquidation amount (token);）

  * Interface Name: Subscribe Liquidation Order Data

  * Interface Type: public

  * Subscription topic: public.$symbol.liquidation_orders

## 1.1.9 2020-10-28 【Newly added：Query financial records via multiple fields,
Query history orders via multiple fields, Query history transactions via
multiple fields.】

### 1、Query history transactions via multiple fields

  * Interface Name：Query history transactions via multiple fields

  * Interface Type：private

  * Interface URL：api/v1/contract_matchresults_exact

### 2、Query history orders via multiple fields

  * Interface Name：Query history orders via multiple fields

  * Interface Type：private

  * Interface URL：api/v1/contract_hisorders_exact

### 3、Query financial records via multiple fields

  * Interface Name：Query financial records via multiple fields

  * Interface Type：private

  * Interface URL：api/v1/contract_financial_record_exact

## 1.1.8 2020-10-15 【Newly added：Added switch leverage interface; Updated:
websocket messages of account topic will be pushed when leverage switch
succeeds; websocket messages of position topic will be pushed when leverage
switch succeeds; new response fields are added on websocket topic of match
orders; the interface(contract_order_info) supports query of 4-hour order
cancellation data (previously only support to query 24-hour data).】

### 1、Added switch leverage interface

  * Interface Name：Switch Leverage

  * Interface Type：private

  * Interface URL：api/v1/contract_switch_lever_rate

### 2、Subscribe Account Equity Updates Data（Return parameters added
“switch_lever_rate” event type to represent switching leverages. When the
leverage is successfully switched, a latest information on assets will be
pushed with event“switch_lever_rate".）

  * Interface Name：Subscribe Account Equity Updates Data

  * Interface Type：private

  * Subscribe topic：accounts.$symbol

### 3、Subscribe Position Updates（Return parameters added “switch_lever_rate”
event type to represent switching leverages. When the leverage is successfully
switched, a latest information on positions will be pushed with
event“switch_lever_rate" (the information will not be pushed when the user's
position is 0).）

  * Interface Name：Subscribe Position Updates

  * Interface Type：private

  * Subscribe topic：positions.$symbol 

### 4、Subscribe Match Order Data（Added the following fields in return
parameters: direction (buy/sell direction), offset (open/close direction),
lever_rate (leverages), price (order price), created_at (creation time),
order_source (order source), order_price_type (order quotation type).）

  * Interface Name：Subscribe Match Order Data

  * Interface Type：private

  * Subscribe topic：matchOrders.$symbol 

### 5、The interface(contract_order_info) supports query of 4-hour order
cancellation data (previously only support to query 24-hour data).

  * Interface Name：Get Information of an Order

  * Interface Type：private

  * Interface URL：api/v1/contract_order_info

## 1.1.7 2020-10-10 【Newly added：Added WS interface for subscribing system
status updates push】

### 1\. Added WS interface for subscribing system status updates push

  * Interface name: subscribe system status updates
  * Interface type: public
  * Subscription topic：public.$service.heartbeat

## 1.1.6 2020-09-22 【Updated: Future Market Data Interfaces (including rest
and ws interfaces) already support calls according to the contract code.
Modified “symbol” field in request parameter: added contract code type, the
format of which is fixed at “symbol-year-month-date”, for example, BTC200925.
Only listing contracts can be queried currently if query according to the
contract code. 】

### 1、Get Market Depth

  * Interface Name：Get Market Depth
  * Interface type: public interface
  * Interface URL：/market/depth

### 2、Get Kline Data

  * Interface Name：Get Kline Data
  * Interface type: public interface
  * Interface URL：/market/history/kline

### 3、Get Market Data Overview

  * Interface Name：Get Market Data Overview
  * Interface type: public interface
  * Interface URL：/market/detail/merged

### 4、Query The Last Trade of a Contract

  * Interface Name：Query The Last Trade of a Contract
  * Interface type: public interface
  * Interface URL：/market/trade

### 5、Query a Batch of Trade Records of a Contract

  * Interface Name：Query a Batch of Trade Records of a Contract
  * Interface type: public interface
  * Interface URL：/market/history/trade

### 6、Subscribe Kline data

  * Interface Name：Subscribe Kline data
  * Interface type: public interface
  * Subscribe topic：market.$symbol.kline.$period

### 7、Request Kline data

  * Interface Name：Request Kline data
  * Interface type: public interface
  * Subscribe topic：market.$symbol.kline.$period

### 8、Subscribe Market Depth Data

  * Interface Name：Subscribe Market Depth Data
  * Interface type: public interface
  * Subscribe topic：market.$symbol.depth.$type

### 9、Subscribe Market Detail Data

  * Interface Name：Subscribe Market Detail Data
  * Interface type: public interface
  * Subscribe topic：market.$symbol.detail

### 10、Subscribe Trade Detail Data

  * Interface Name：Subscribe Trade Detail Data
  * Interface type: public interface
  * Subscribe topic：market.$symbol.trade.detail

### 11、Request Trade Detail Data

  * Interface Name：Request Trade Detail Data
  * Interface type: public interface
  * Subscribe topic：market.$symbol.trade.detail

### 12、Subscribe Incremental Market Depth Data

  * Interface Name：Subscribe Incremental Market Depth Data
  * Interface type: public interface
  * Subscribe topic：market.$symbol.depth.size_${size}.high_freq

### 13、Subscribe Market BBO Data

  * Interface Name：Subscribe Market BBO Data
  * Interface type: public interface
  * Subscribe topic：market.$symbol.bbo

## 1.1.5 2020-08-06 【Added interfaces：Query user’s settlement
records；Subscribe trigger orders updates】

### 1、Query user’s settlement records

  * Interface Name：Query user’s settlement records
  * Interface Type：private
  * Interface URL：api/v1/contract_user_settlement_records 

### 2、Subscribe trigger orders updates

  * Interface Name：Subscribe trigger orders updates
  * Interface Type：private
  * Subscribe topic：trigger_order.$symbol

## 1.1.4 2020-06-19 【Updated: added the return field "client_order_id" of
websocket subscription of Match Order】

### 1、Modified futures subscribe match order data interface: added
client_order_id in outer return parameter.

  * Interface name: Subscribe Match Order
  * Interface type: Private Interface
  * Subscription topic: matchOrders.$symbol

## 1.1.3 2020-06-14 【Added interfaces: websocket subscription of contract info
event; websocket subscription of Market BBO; Restful Interface of querying
available leverage rate; Modified Interfaces: added four depth level of
websocket subscription of Market Depth; added periodical push of websocket
subscription of accout event and position event; added response fields of
querying orders related; added uid fields of websocket subscription of private
event; added fields of websocket subscription of match orders; added high
leverage; added next quarter contract;】

### 1、Added websocket subscription of contract info

  * Interface name: Subscribe Contract Info
  * Interface type: public interface
  * Subscribe topic: public.$symbol.contract_info

### 2、Added websocket subscription of Market BBO

  * Interface name: Subscribe Market BBO
  * Interface type: public interface
  * Subscribe topic: market.$symbol.bbo

### 3、Added four depth level of websocket subscription of market depth:
step12、step13、step14、step15

  * Interface name: Subscribe Market Depth
  * Interface type: public interface
  * Subscribe topic: market.$symbol.depth.$type

### 4、Added the interface of querying available leverage rate

  * Interface name: Query Available leverage Rate
  * Interface type: private interface
  * Interface URL: /api/v1/contract_available_level_rate

### 5、Added periodical push of websocket subscription of account: push every 5
seconds

  * Interface name: Subscribe Account Update
  * Interface type: private interface
  * Subscribe topic: accounts.$symbol

### 6、Added periodical push of websocket subscription of position: push every
5 seconds

  * Interface name: Subscribe Position Update
  * Interface type: private interface
  * Subscribe topic: positions.$symbol

### 7、Added high leverage support of placing orders

#### 7.1

  * Interface name: Place an Order
  * Interface type: private interface
  * Interface URL: api/v1/contract_order

#### 7.2

  * Interface name: Place Orders
  * Interface type: private interface
  * Interface URL: api/v1/contract_batchorder

#### 7.3

  * Interface name: Place Trigger Order
  * Interface type: private interface
  * Interface URL: api/v1/contract_trigger_order

### 8、Added 9 fields of querying order detail interface:
fee、order_id、order_id_str、client_order_id、order_type、status、trade_avg_price、trade_turnover、trade_volume.

  * Interface name: Query order detail
  * Interface type: Private Interface
  * Interface URL: api/v1/contract_order_detail

### 9、Added 2 fields of querying order info interface:
liquidation_type、canceled_at.

  * Interface name: Query Order Info
  * Interface type: Private interface
  * Interface URL: api/v1/contract_order_info

### 10、Added 2 fields of websocket subscription of orders:
canceled_at、fee_asset.

  * Interface name: Subscribe Orders
  * Interface type: Private interface
  * Subscribe topic: orders.$symbol

### 11、Added uid field of websocket subscription of private events.

#### 11.1

  * Interface name: Subscribe Orders
  * Interface type: Private Interface
  * Subscribe topic: orders.$symbol

#### 11.2

  * Interface name: Subscribe Accounts
  * Interface type: Private Interface
  * Subscribe topic: accounts.$symbol

#### 11.3

  * Interface name: Subscribe Positions
  * Interface type: Private Interface
  * Subscribe topic: positions.$symbol

#### 11.4

  * Interface name: Subscribe Match Orders
  * Interface type: Private Interface
  * Subscribe topic: matchOrders.$symbol

### 12、Added 2 fields of websocket subscription of match orders:
trade_volume(total filled volume of the order)、volume(total volume of the
order)

  * Interface Name: Subscribe Match Orders
  * Interface Type: Private Interface
  * Subscribe Topic: matchOrders.$symbol

### 13、Added next quarter contract type,such as BTC_NQ

  * Interface Name: Market、Account and Trade Related(Restful and websocket)

  * Interface Type: Public/Private

## 1.1.2 2020-04-09【Add an interface: Futures liquidation order WS push
without authentication】

  * Interface name: WebSocket liquidation order push
  * Subscribe topic: public.$symbol.liquidation_orders
  * Interface type: public interface

## 1.1.1 2020-03-12 【upgrade：added websocket subscription of index kline
data；added websocket subscription of basis data; added restful interface of
querying index kline data; added restful interface of querying basis data】

### 1、Added websocket subscription of index kline data

  * Interface name：Subscribe Index Kline Data
  * Interface type：public interface
  * Subscribe Topic：market.$symbol.index.$period

### 2、Added websocket subscription of basis data

  * Interface name：Subscribe Basis Data
  * Interface type： public interface
  * Subscribe Topic：market.$symbol.basis.$period.$basis_price_type

### 3、Added restful interface of querying index kline data

  * Interface name： Get Index Kline Data
  * Interface type: public interface
  * Interface URL：/index/market/history/index

### 4、Added restful interface of querying basis data

  * Interface name：Get Basis Data
  * Interface type：public interface
  * Interface URL：/index/market/history/basis

## 1.1.0 2020-03-05【upgrade：add transfer between master account and sub-
account; add more order types; add websocket subscription of match orders】

### 1、Added asset transfer function between master account and sub-account on
Web and API. When using Web, only master account has transfer authority,
including transfer master account assets to sub-account and vice versa, but
transfers between sub-accounts are not supported; When using API, only API Key
of master account has authority for the transfer operations between master and
sub account.

#### 1.1、Added an interface: transfer between master account and sub-accounts,
the rate limit between the master account and each subaccount is 10 times/
minute.Interface name: Transfer between master account and sub-accounts.

  * Interface type: User private interface
  * URL：api/v1/contract_master_sub_transfer

#### 1.2、Added a parameter: transfer permission between master account and
sub-accounts. Added strings: "master_transfer_sub" and "sub_transfer_master"
in returning parameter data array.

  * Interface name: Query information on system status
  * Interface type: Public
  * URL：api/v1/contract_api_state

#### 1.3、Added an interface: query transfer records of master account and sub-
accounts.

  * Interface name: Query transfer records of master account and sub-accounts.
  * Interface type: User private interface
  * URL: api/v1/contract_master_sub_transfer_record

#### 1.4、Added 4 kinds transfer statements of master account and sub-accounts
in query contract financial record interface.

  * Interface name: Query contract financial record
  * Interface type: User private interface
  * URL: api/v1/contract_financial_record

### 2、Modifications details of contract asset interface and contract trade
interface are laid out as following：

#### 2.1、Modified query contract information on order limit: added 10 order
price types including opponent_ioc, lightning_ioc, optimal_5_ioc,
optimal_10_ioc，optimal_20_ioc，opponent_fok，lightning_fok，optimal_5_fok，optimal_10_fok，optimal_20_fok

  * Interface name: Query contract information on order limit
  * Interface type: User private interface
  * URL: POST api/v1/contract_order_limit

#### 2.2、Modified place an order interface: added 8 order price types,
including opponent_ioc, optimal_5_ioc, optimal_10_ioc, optimal_20_ioc,
opponent_fok,optimal_5_fok, optimal_10_fok, optimal_20_fok.

  * Interface name: Place an order 
  * Interface type: User private interface
  * URL: api/v1/contract_order

#### 2.3、Modified place a batch of orders interface: added 8 order price
types, including opponent_ioc, optimal_5_ioc, optimal_10_ioc, optimal_20_ioc,
opponent_fok, optimal_5_fok, optimal_10_fok, optimal_20_fok。

  * Interface name: Place a batch of orders
  * Interface type: User private interface
  * URL: api/v1/contract_batchorder

#### 2.4、Modified get trade details of an order interface: added string
"liquidation_type".

  * Interface name: Get trade details of an order
  * Interface type: User private interface
  * URL: POST api/v1/contract_order_detail

#### 2.5、Modified "trade_type" and "orders" in query history orders interface.
Added "reduce positions to close long" and "reduce positions to close short"
types in request parameter "trade_type"; Added string "liquidation_type" in
orders array of returning parameter.

  * Interface name: Query history orders interface.
  * Interface type: User private interface
  * URL: POST api/v1/contract_hisorders

#### 2.6、Modified place flash close order interface: added string
"order_price_type", including values: lightning_ioc, lightning_fok, lightning

  * Interface name: Place flash close order
  * Interface type: User private interface
  * URL: api/v1/lightning_close_position

#### 2.7、Added string "liquidation_type" in order transaction push in
WebSocket Subscription.

  * Interface name: Match result on order push in WebSocket subscription
  * Interface type: User private interface
  * Subscribe Topic: orders.$symbol

#### 2.8、Added matching order transaction push interface in WebSocket
Subscription.

  * Interface name: WebSocket matching order transaction push
  * Interface type: User private interface
  * Subscribe Topic: matchOrders.$symbol

#### 2.9、Queried if system interface is available, added strings on perpetual
swap related status, added strings
"swap_heartbeat"、"swap_estimated_recovery_time"in the array "data" with the
returned parameters

  * Interface name: Queried if system interface is available
  * Interface type: public
  * URL: https://api.hbdm.com/heartbeat/

#### 2.10、Added API interface of getting user's API indicator disable
information

Interface name: Query user's API indicator disable information

  * Interface type: User private interface
  * Interface type: public
  * URL: api/v1/contract_api_trading_status

## 1.0.11 2020-02-21 API Uprade

### 1、 Interface URL: api/v1/contract_batchorder

the maximum number of batch order cancellation each time in request parameter
“orders_data” will be changed from 20 to 10.

### 2、Interface URL: api/v1/contract_cancel

the maximum number of order cancellation each time in request parameter
“order_id” and “client_order_id” will be changed from 20 to 10. Multiple order
IDs are separated by “,”.

## 1.0.10 2020-01-15 API Upgrade

### 1、modify get Kline data interface:Added two request parameters “from” and
“to”. Request parameter “from” stands for starting time and request parameter
“to” stands for ending time. Data can be obtained for up to two consecutive
years. Request parameter “size” was changed to non-mandatory.

  * /market/history/kline Get Kline data

### 2、When getting information on order cancellation via get contracts
Information interface, users can only query last 24-hour data.

  * /api/v1/contract_order_info Get Contracts Information

### 3、When getting information on order cancellation via query history orders
interface, users can only query last 24-hour data.

  * /api/v1/contract_hisorders

### 4、When getting information on order cancellation via query order detail
interface, users who type in parameters “created_at” and “order_type” can
query last 90-day data, while users who don’t type in parameters “created_at”
and “order_type” can only query last 24-hour data.

  * /api/v1/contract_order_detail

## 1.0.9 2019-12-02 API Upgrade: Added API interface with trigger order
function

### 1、Added API interface with query assets and positions function.

  * rest uri: api/v1/contract_account_position_info Added to get the current assets and positions.

### 2、Added API interface with trigger order function.

  * `api/v1/contract_trigger_order` Added API interface with place trigger order function 

  * `api/v1/contract_trigger_cancel` Added API interface with cancel trigger order funcion

  * `api/v1/contract_trigger_cancelall` Added API interface with cancal all trigger orders funciton

  * `api/v1/contract_trigger_openorders` Added API interface with get trigger orders function

  * `api/v1/contract_trigger_hisorders` Added API interface with get history trigger orders function

### 3、Updated API interfaces with fee coin type field added corresponding to
the given fee.

Interfaces are as follows:

  * `api/v1/contract_fee` query current fee rate

  * `api/v1/contract_order_info`query order information

  * `api/v1/contract_order_detail`query order detail 

  * `api/v1/contract_openorders`query current open orders

  * `api/v1/contract_hisorders`query history orders

  * `api/v1/contract_matchresults`query history transactions

  * add fee coin type push in websocket transactions subcription

### 4、Updated API interfaces with the 'create_date' field to support any
positive interger

Please note that the system will return with the last 90-day data by default
if the 'create_date' field exceed 90.

  * `api/v1/contract_hisorders`query history orders

  * `api/v1/contract_trigger_hisorders`query history trigger orders

  * `api/v1/contract_matchresults`query history transactions

  * `api/v1/contract_financial_record`query financial records

## 1.0.8 2019-10-17 API Upgrade: Added the order_id_str field

  * To solve the problem that the userOrderId of node.js and javascript is too long, the order_id_str field will be added to the following interface, the type is String, which is expected to go online today: 

api/v1/contract_order

api/v1/contract_batchorder

api/v1/contract_matchresults

api/v1/contract_hisorders

api/v1/contract_openorders

api/v1/lightning_close_position

api/v1/contract_order_info

  * WebSocket added the order_id_str field  

## 1.0.7 2019-10-15

The return order_id is 18 bits, it will make mistake when nodejs and
JavaScript analysed 18 bits. Because the Json.parse in nodejs and JavaScript
is int by default. so the number over 18 bits need be parsed by jaso-bigint
package. Refer to the [demo](https://github.com/huobiapi/Futures-Node.js-
demo/tree/master/REST-Node.js-demo) of nodejs for details. For
[details](https://github.com/huobiapi/Futures-Node.js-demo/blob/master/Nodejs-
DEMO.docx?raw=true), please check.

### 1、 Modified rest interface: User’s Account Information

Added return string “margin_static”in rest interface User’s Account
Information (URL: api/v1/contract_account_info). The newly added return string
“margin_static” in data array means account static equity.

### 2、 Added string “ID “in three interfaces;

Added string“ID”in rest interface Order details acquisition (URL:
api/v1/contract_order_detail) , rest interface Get History Match Results (URL:
api/v1/contract_matchresults) as well as the match result on Order Push in
WebSocket Subscription.

### 3、Added “IOC”and “FOK order types for order placement

Added order_price_type “ioc”(ioc:Immediate Or Cancel) and “fok”(fok:Fill Or
Kill)under Request Parameter in rest interface Place an Order(URL:
api/v1/contract_order) and rest interface Place a Batch of Orders(URL:
api/v1/contract_batchorder)

### 4、Modified interface: Query contract information on order limit

Added “fok”:FOK Order(fok:Fill Or Kill),“ioc”:IOC Order(ioc:Immediate Or
Cancel) into string of“ order_price_type” in Returning Parameter under rest
interface Query contract information on order limit (URL:
api/v1/contract_order_limit)

The“ order_price_type” means Order Type here.

### 5、Added rest API interface: Query information on system status

Interface URL: api/v1/contract_api_state

### 6、 Added rest interface: Top Trader Sentiment Index Function-Account

Interface URL: api/v1/contract_elite_account_ratio

### 7、Added rest interface: Top Trader Sentiment Index Function-Position

Interface URL: api/v1/contract_elite_position_ratio

### 8、Added Liquidation order query function in API and WS subscription.

Added rest interface: Request Liquidation Order Information

Interface URL: rest interface api/v1/contract_liquidation_orders

Liquidation order push is added also into WebSocket Subscription.

## 1.0.6 2019-08-08 API Upgrade: Added rest interface

### Added rest interface

Request access to address: https://api.hbdm.com/heartbeat/

Note: To query whether the system is available or not, request
https://api.hbdm.com/heartbeat/. When Heartbeat is 1, system is available;
when Heartbeat is 0, system is unavailable.

## 1.0.5 2019-07-10 API Upgrade: New Features of Query and Order Placing

### Newly Added API Restful Interface

Newly added Interface: query user’s order limit information

Newly added Interface: query user’s trading fee information

Newly added Interface: query user’s transfer limit information

Newly added Interface: query users’ position limit information

Newly added Interface: query platform information on insurance fund and
estimated clawback rate

Newly added Interface: query platform information on open interest information

Newly added Interface: query history records information on insurance fund

Newly added Interface: query platform information on Tiered Adjustment Factor

Newly added Interface: place Flash Close order

### Modified API Interface

Restful interface: add “return to users’ adjustment factor” on Query Users’
Account Information Interface;

Restful interface: add “return to users’ adjustment factor” on Query a Single
Sub-Account’s Assets Information Interface.

WebSocket Interface: add “return to users’ adjustment factor” on WebSocket
Portfolio Push Interface;

Restful Interface: add Optimal price set with optimal top 5, optimal 10 and
optimal top 20 on Order Place Interface and Place a Batch of Orders Interface

Restful Interface: add “query according contract code” on Acquire History of
Match Results Interface.

## 1.0.4 2019-06-06 API Upgrade:Restful interface

### Query assets information of all sub-accounts under the master account

URL：api/v1/contract_sub_account_list

Notice: Only return data for activated contract sub-account (i.e. sub-accounts
that have gained contract trading permission).

### Query a single sub-account's assets information

URL：api/v1/contract_sub_account_info

Notice: Only query account information for activated contract sub-account
(i.e. sub-accounts that have gained contract trading permission); No data
return for sub-accounts which has logged in hbdm but have not gained trading
permission/activated.

### Query a single sub-account's position information

URL：api/v1/contract_sub_position_info

### Query account financial records

URL：api/v1/contract_financial_record

## 1.0.3 2019-05-28 API Upgrade: WebSocket Portfolio Push

### WebSocket balance push is available:

users could subscribe the interface to get information of their balances
automatically.

### WebSocket position push is available:

users could subscribe the interface to get information of their positions
automatically.

### Acuqire positions information via Restful interface:

api/v1/contract_position_info.

The string of “latest price”is added into response

## 1.0.2 2019-05-14 API Upgrade: Transfer margin between Spot account and
Future account

### URL /v1/futures/transfer

This interface is used to transfer assets between Spot account and Future
account.

The type is “pro-to-futures” when transferring assets from Spot account to
Future; “futures-to-pro” when transferring from Future account to Spot
account.

API rate limit for this interface is up to 10 times per minute.

### API rate limit

Private interface rate limit has been increased from 10 times/second to 30
times every 3 seconds, which means users could send up to 30 requests within 3
seconds.

The rate limit of other non-market public interface has been increased from 20
times/second to 60 times every 3 seconds, which means users could send up to
60 requests within 3 seconds.

## 1.0.1 2019-05-09 API Upgrade: Post_only and more

### Cancel all interface: URL api/v1/contract_cancelall

Send symbol to cancel all the contracts of that kind of symbol, e.g. send
“BTC” to cancel all BTC weekly, biweekly and quarterly contracts.

Send contract_code to cancel the contracts of that code.

Send symbol+contract_type to cancel the certain contracts under the symbol of
that contract_type, e.g. send “BTC” and “this week”, then the BTC weekly
contracts will be cancelled.

### Order place interface: URL api/v1/contract_order

Post_only is added into the string of order_price_type.

Description of post_only: assure that the maker order remains as maker order,
it will not be filled immediately with the use of post_only, for the match
system will automatically check whether the price of the maker order is
higher/lower than the opponent first price, i.e. higher than bid price 1 or
lower than the ask price 1. If yes, the maker order will placed on the
orderbook, if not, the maker order will be cancelled.

Position limit will be applied to post_only while order limit will not.

### Place a batch of orders: URL /v1/contract_batchorder

Post_only is added into the string of order_price_type.

Description of post_only: assure that the maker order remains as maker order,
it will not be filled immediately with the use of post_only, for the match
system will automatically check whether the price of the maker order is
higher/lower than the opponent first price, i.e. higher than bid price 1 or
lower than the ask price 1. If yes, the maker order will placed on the
orderbook, if not, the maker order will be cancelled.

Position limit will be applied to post_only while order limit will not.

### Will response following string for "header" via api

ratelimit-limit: the upper limit of requests per time, unit: time

ratelimit-interval: reset interval (reset the number of request), unit: ms

ratelimit-remaining: the left available request number for this round, unit:
time

ratelimit-reset: upper limit of reset time used to reset request number, unit:
ms

### Order details acquisition: URL api/v1/contract_order_detail

The string of “role” (i.e. taker or maker) is added into “trades”

### Acquire history of match results: URL api/v1/contract_matchresults

The string of “role” (i.e. taker or maker) is added into “trades

### WebSocket, the private order push interface, requires API KEY Verification

Each UID can build at most create 30 WS connections for private order push at
the same time. For each account, contracts of the same underlying coin only
need to subscribe one WS order push, e.g. users only need to create one WS
order push connection for BTC Contract which will automatically push orders of
BTC weekly, BTC biweekly and BTC quarterly contracts.

Please note that the rate limit of WS order push and RESTFUL private interface
are separated from each other, with no relations.

## 1.0.0 has launched on December 10, 2018

# Future API Access Illustration

## API List

permission type | Content Type | Context | Request Type | Desc | Signature
Required  
---|---|---|---|---|---  
Read | Market Data | api/v1/contract_contract_info | GET | Get Contracts
Information | No  
Read | Market Data | api/v1/contract_index | GET | Get contract Index Price
Information | No  
Read | Market Data | api/v1/contract_price_limit | GET | Get Contract Price
Limitation | No  
Read | Market Data | api/v1/contract_open_interest | GET | Get Contract Open
Interest Information | No  
Read | Market Data | api/v1/contract_delivery_price | GET | Get the estimated
delivery price | No  
Read | Market Data | api/v1/contract_api_state | GET | Query information on
system status | No  
Read | Market Data | /market/depth | GET | Get Market Depth | No  
Read | Market Data | /market/history/kline | GET | Get Kline Data | No  
Read | Market Data | /market/detail/merged | GET | Get Market Data Overview |
No  
Read | Market Data | /market/trade | GET | Query The Last Trade of a Contract
| No  
Read | Market Data | /market/history/trade | GET | Query a Batch of Trade
Records of a Contract | No  
Read | Market Data | api/v1/contract_risk_info | GET | Query information on
contract insurance fund balance and estimated clawback rate | No  
Read | Market Data | api/v1/contract_insurance_fund | GET | Query history
records of insurance fund balance | No  
Read | Market Data | api/v1/contract_adjustfactor | GET | Query information on
Tiered Adjustment Factor | No  
Read | Market Data | api/v1/contract_his_open_interest | GET | Query
information on open interest | No  
Read | Market Data | api/v1/contract_elite_account_ratio | GET | Query Top
Trader Sentiment Index Function-Account | No  
Read | Market Data | api/v1/contract_elite_position_ratio | GET | Query Top
Trader Sentiment Index Function-Position | No  
Read | Market Data | api/v1/contract_liquidation_orders | GET | Query
Liquidation Order Information | No  
Read | Market Data | api/v1/contract_settlement_records | GET | Query
historical settlement records of the platform interface | No  
Read | Market Data | /index/market/history/index | GET | Query Index Kline
Data | No  
Read | Market Data | /index/market/history/basis | GET | Query Basis Data | No  
Read | Account | api/v1/contract_account_info | POST | Query User’s Account
Information | Yes  
Read | Account | api/v1/contract_position_info | POST | Query User’s Position
Information | Yes  
Read | Account | api/v1/contract_sub_account_list | POST | Query assets
information of all sub-accounts under the master account (Query by coins) |
Yes  
Read | Account | api/v1/contract_sub_account_info | POST | Query a single sub-
account's assets information | Yes  
Read | Account | api/v1/contract_sub_position_info | POST | Query a single
sub-account's position information | Yes  
Read | Account | api/v1/contract_financial_record | POST | Query account
financial records | Yes  
Read | Account | api/v1/contract_financial_record_exact | POST | Query
financial records via multiple fields | Yes  
Read | Account | api/v1/contract_user_settlement_records | POST | Query user’s
settlement records | Yes  
Read | User Account | api/v1/contract_order_limit | POST | Query contract
information on order limit | Yes  
Read | User Account | api/v1/contract_available_level_rate | POST | Query
contract available level rate | Yes  
Read | User Account | api/v1/contract_fee | POST | Query information on
contract trading fee | Yes  
Read | User Account | api/v1/contract_transfer_limit | POST | Query
information on Transfer Limit | Yes  
Read | User Account | api/v1/contract_position_limit | POST | Query
information on position limit | Yes  
Trade | User Account | api/v1/contract_master_sub_transfer | POST | Transfer
between master and sub account | Yes  
Read | User Account | api/v1/contract_account_position_info | POST | User’s
position Information And User’s position Information | Yes  
Read | Trade | api/v1/contract_trigger_openorders | POST | Query Trigger Order
Open Orders | Yes  
Read | Trade | api/v1/contract_trigger_hisorders | POST | Query Trigger Order
History | Yes  
Trade | Trade | api/v1/contract_order | POST | Place an Order | Yes  
Trade | Trade | api/v1/contract_batchorder | POST | Place a Batch of Orders |
Yes  
Trade | Trade | api/v1/contract_cancel | POST | Cancel an Order | Yes  
Trade | Trade | api/v1/contract_cancelall | POST | Cancel All Orders | Yes  
Trade | Trade | api/v1/contract_switch_lever_rate | POST | Switch Leverage |
Yes  
Trade | Trade | api/v1/lightning_close_position | POST | Place Flash Close
Order | Yes  
Read | User Order Info | api/v1/contract_order_info | POST | Get Information
of an Order | Yes  
Read | User Order Info | api/v1/contract_order_detail | POST | Get Trade
Details of an Order | Yes  
Read | User Order Info | api/v1/contract_openorders | POST | Get Current
Orders | Yes  
Read | User Order Info | api/v1/contract_hisorders | POST | Get History Orders
| Yes  
Read | User Order Info | api/v1/contract_hisorders_exact | POST | Query
history orders via multiple fields | Yes  
Read | User Order Info | api/v1/contract_matchresults | POST | Get History
Match Results | Yes  
Read | User Order Info | api/v1/contract_matchresults_exact | POST | Query
history transactions via multiple fields | Yes  
Trade | Trade | v1/futures/transfer | POST | Transfer margin between Spot
account and Future account | Yes  
Trade | Trade | api/v1/contract_trigger_order | POST | Place Trigger Order |
Yes  
Trade | Trade | api/v1/contract_trigger_cancel | POST | Cancel Trigger Order |
Yes  
Trade | Trade | api/v1/contract_trigger_cancelall | POST | Cancel All Trigger
Orders | Yes  
  
## Address

Address | Applicable sites | Applicable functions | Applicable trading pairs  
---|---|---|---  
https://api.hbdm.com | Huobi Future | Market | Trading pairs provided by Huobi
Future  
  
### Notice

If you can't connect "https://api.hbdm.com", please use
"https://api.btcgateway.pro" for debug purpose. If your server is deployed in
AWS, we recommend using "https://api.hbdm.vn".

## Signature Authentication & Verification

### Signature Illustration

Considering that API requests may get tampered in the process of transmission,
to keep the transmission secure, you have to use your API Key to do Signature
Authentication for all private interface except for public interface (used for
acuqiring basic information and market data), in this way to verify whether
the parameters/ parameter value get tampered or not in the process of
transmission

A legitimate request consists of following parts：

  * Request address of method, i.e. visit server address--api.hbdm.com, e.g.: api.hbdm.com/api/v1/contract_order

  * API Access Key ID (AccessKeyId): Access Key of the API Key that you apply.

  * Method of Signature (SignatureMethod): Based on the Hash Aggrement, users calculate the signature via HmacSHA256.

  * Signature Version (SignatureVersion): It adopts version 2 in terms of Signature Version.

  * Timestamp (Timestamp): The time when you send the request (UTC time zone) : (UTC time zone) : (UTC time zone), e.g.: 2017-05-11T16:22:06

  * Must-fill parameters & optional parameters: For each method, there are a group of must-fill parameters and optional parameters used to address the API request, which can be found in the illustration of each method as well as their meaning. Please note that, in terms of "Get" requests, it needs to do Signature calculation for all the original parameters in each method ; In terms of "Post" requests, no need to do Signature calculation for the original parameters in each method, which means only four parameters need to do Signature calculation in "Post" requests, i.e. AccessKeyId, SignatureMethod, SignatureVersion, Timestamp with other parameters placed in "body".

  * Signature: The result of Signature calculation which is used to verify if signature is valid and not tampered.

### Create API Key

[You could create API Key at](https://www.hbg.com/zh-cn/apikey/)

API Key consists of the following two parts.

  * "Access Key", the Key used to visit API.

  * "Secret Key", the Key used to do Signature authentication and verification (visible during application period).

When create API Key, users could bind IP address, as the validity of unbond IP
address is only 90 days.  API Key has operation authorization of trading,
borrowing, deposit and withdrawal etc..  Both Access Key and Secret Key are
closely related with account security, please do not disclose them to others
for any reasons anytime.

### Steps for Signature

Normative request for Signature calculation Different contents will get
totally different results when use HMAC to calculate Signature, therefore,
please normalize the requests before doing Signature calculation. Take the
request of inquering order details as an example:

query details of one order

`https://api.hbdm.com/api/v1/contract_order?`

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx`

`&SignatureMethod=HmacSHA256`

`&SignatureVersion=2`

`&Timestamp=2017-05-11T15:19:30`

#### 1\. Request methods (GET/POST): add line breaker "\n".

`POST\n`

#### 2\. Text the visit address in lowercase, adding line breake "\n"

` api.hbdm.com\n `

#### 3\. Visit the path of methods, adding line breaker "\n"

` /api/v1/contract_order\n `

#### 4\. Rank the parameter names according to the sequence of ASCII codes,
for example, below is the parameters in original sequence and the new
sequence:

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx`

`SignatureMethod=HmacSHA256`

`SignatureVersion=2`

`Timestamp=2017-05-11T15%3A19%3A30`

Use UTF-8 to encode when it has already been encoded by URI with hexadecimals
in Uppercase, e.g., ":" wiil be encoded to "%3A" while space to "%20".
Timestamp should be written in the form of YYYY-MM-DDThh:mm:ss and encoded
with URI.

#### 5\. After ranking

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx`

`SignatureMethod=HmacSHA256`

`SignatureVersion=2`

`Timestamp=2017-05-11T15%3A19%3A30`

#### 6\. Following the sequence above, link parameters with "&"

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx&SignatureMethod=HmacSHA256&SignatureVersion=2&Timestamp=2017-05-11T15%3A19%3A30`

#### 7\. Form the final character strings that need to do Signature
calculation as following:

`POST\n`

`api.hbdm.com\n`

`/api/v1/contract_order\n`

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx&SignatureMethod=HmacSHA256&SignatureVersion=2&Timestamp=2017-05-11T15%3A19%3A30`

#### 8\. Use the "request character strings" formed in the last step and your
Secret Key to create a digital Signature.

`4F65x5A2bLyMWVQj3Aqp+B4w+ivaA7n5Oi2SuYtCJ9o=`

  1. Take the request character string formed in the last step and API Secret Key as two parameters, encoding them with the Hash Function HmacSHA256 to get corresponding Hash value.

  2. Encoding the Hash value with base-64 code, the result will be the digital Signature of this request.

#### 9\. Add the digital Signature into the parameters of request path.

The final request sent to Server via API should be like:

`https://api.hbdm.com/api/v1/contract_order?AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx&order-
id=1234567890&SignatureMethod=HmacSHA256&SignatureVersion=2&Timestamp=2017-05-11T15%3A19%3A30&Signature=4F65x5A2bLyMWVQj3Aqp%2BB4w%2BivaA7n5Oi2SuYtCJ9o%3D`

  1. Add all the must authentication parameters into the parameters of request path;

  2. Add the digital Signature encoded with URL code into the path parameters with the parameter name of "Signature".

## API Rate Limit Illustration

Future, Coin Margined Swap,Option Swap and USDT Margined Swap are using
separate API rate limits.

Please note that, for both public interface and private interface, there are
rate limits, more details are as below:

  * Generally, the private interface rate limit of API key is at most 72 times every 3 seconds for each UID (Trade Interface: at most 36 times every 3 seconds. Read Interface: at most 36 times every 3 seconds) (this rate limit is shared by all the altcoins contracts delivered by different date). [ API Interface List ](https://docs.huobigroup.com/docs/dm/v1/en/#api-list)

  * For public interface used to get information of index, price limit, settlement, delivery, open positions and so on, the rate limit is 120 times every 3 seconds at most for each IP (this 120 times every 3 seconds public interface rate limit is shared by all the requests from that IP of non-marketing information, like above).

  * For public interface to get market data such as Get Kline data, Get Market Data Overview, Get Contract Information,Get market depth data, Get index kline, Get basis data, Get the last Trade of a Contract and so on：

(1) For restful interfaces：all products(futures, coin margined swap, usdt
margined swap and option) 800 times/second for one IP at most

（2）For websocket: The rate limit for “req” request is 50 times at once. No
limit for “sub” request as the data will be pushed by sever voluntarily.

  * WebSocket, the private order push interface, requires API KEY Verification:

Each UID can build at most create 30 WS connections for private order push at
the same time. For each account, contracts of the same underlying coin only
need to subscribe one WS order push, e.g. users only need to create one WS
order push connection for BTC Contract which will automatically push orders of
BTC weekly, BTC biweekly and BTC quarterly contracts. Please note that the
rate limit of WS order push and RESTFUL private interface are separated from
each other, with no relations.

  * Both read and trade interfaces will return the ratelimit info.You can refer to the following fields of "header" from api response. E.g.,you will get the total Read ratelimit("ratelimit-limit") and the remaining Read ratelimit("ratelimit-remaining") when you query the order info(/api/v1/contract_order_info) , and you will get the total Trade ratelimit("ratelimit-limit") and the remaining Trade ratelimit("ratelimit-remaining") when you place an order(/api/v1/contract_order)). [ API Interface List ](https://docs.huobigroup.com/docs/dm/v1/en/#api-list)

  * Will response following string for "header" via api:

ratelimit-limit: the upper limit of requests per time, unit: times

ratelimit-interval: reset interval (reset the number of request), unit: ms

ratelimit-remaining: the left available request number for this round, unit:
times

ratelimit-reset: upper limit of reset time used to reset request number, unit:
ms

When API Limitation on Order Cancellation Ratio is triggered,the following
string for "header" via api will also be returned:

recovery-time: recovery timestamp, whose unit is millisecond, showing the end
time of prohibition, or the access retrieval timestamp;

if you are not in the prohibition period, the field is not included in
returned header;

## API Limitation on Order Cancellation Ratio

  * The system will calculate the order cancellation ratio automatically when the total number of orders placed via certain order price types by the API user goes equal to or larger than 3,000 within 10 minutes. If the order cancellation ratio is greater than 99%, the user will be prohibited for 5 minutes from placing orders via certain API order price types which will be listed below (The response of placing orders will return: 1084 Your contract API is disabled, please try again after {0} (GMT+8).).
  * A 30-minute API order placement prohibition will be triggered if the user was prohibited for 3 times within an hour (The response of placing orders will return: 1084 Your contract API is disabled, please try again after {0} (GMT+8).). After resuming access, the total number of prohibited times will be cleared during the previous period and will not be counted into the total prohibited times in the new period.
  * Please note that the prohibition from placing orders will cause no effect on order cancellation via API as well as order placement and cancellation via other terminals. We’ll keep you notified on each prohibition via SMS and email.
  * Only four API order price types will be prohibited which are Limit order, Post_only, FOK and IOC. Please note that you can still use freely other order price types during the banned period, such as Flash Close, BBO, Optimal 5, Optimal 10 and Optimal 20, opponent_ioc, lightning_ioc, optimal_5_ioc, optimal_10_ioc，optimal_20_ioc，opponent_fok，lightning_fok，optimal_5_fok，optimal_10_fok，optimal_20_fok,etc.
  * The response header returned by HTTP request:

    * When placing order by using the four prohibited order price types during the prohibition period, the message header returned by interface will include the field: 
    * "recovery-time": recovery timestamp ,whose unit is millisecond, showing the end time of prohibition, or the access retrieval timestamp; 
    * if you are not in the prohibition period, the field is not included in returned header;
  * Please note that our system calculates order cancellation ratio according to UID and therefore, the master account UID and sub-accounts UIDs will be counted separately. The calculation period is 10 min/time(The start time starts at 00:00 and the end time is 00:10. Every 10 minutes is a cycle.).

  * Definition of Indicators：

    * Order Cancellation Ratio =Total number of invalid cancellation / Total number of placed orders (all types of orders placed via API) 
    * Total number of placed order: Total number of placed orders refers to all orders placed via API which meet these requirements:
    * 1.the order type is placing orders (Order Type = 1),
    * 2.order price types include Limit Order, Post_only, FOK and IOC.
    * 3.order creating time should be within the interval between 3 seconds before the start time of the calculation period and the end time of the calculation period.
    * Total number of invalid cancellation:Total number of invalid cancellation refers to all cancellation orders placed via API which meet the requirements.
    * the order type is placing orders (order Type=1),
    * the order price types are Limit Order, post_only, FOK and IOC.
    * the order status is “Orders cancelled” (status=7).
    * order with 0 fulfilled.
    * the interval between order cancellation and placement should be less than or equal to 3 seconds.
    * the order cancellation time should be within the calculation period.
  * In order to ensure stability and transaction performance of API, please try to reduce order cancellation rate and cancellation amount during peak periods to avoid frequent triggering of API restriction mechanism.Suggestions of reducing order cancellation rate are as below:

    * 1\. Set orders’ price to BBO prices as close as possible;
    * 2\. Prolong the interval properly between each order placement and cancellation;
    * 3\. Try to increase your amount for each order and reduce the frequency of order;
    * 4\. Try to improve your order fulfillment rate:
    * （1）Please try to use order prices types that help more on order fulfillment in preference such as BBO, Optimal 5, Optimal 10, Optimal 20, Flash Close, opponent_ioc, lightning_ioc, optimal_5_ioc, optimal_10_ioc，optimal_20_ioc，opponent_fok，lightning_fok，optimal_5_fok，optimal_10_fok，optimal_20_fok, etc.
    * （2）Try to use best bid/ask price when placing IOC orders, FOK orders and Post_only orders.
    * 5\. Please try to extend your request polling cycle when implementing your strategy.

## Maintenance with service suspended

During the maintenance of the business system, in addition to the below two
interfaces([Get system status](https://docs.huobigroup.com/docs/dm/v1/en/#get-
system-status), [Query whether the system is
available](https://docs.huobigroup.com/docs/dm/v1/en/#query-whether-the-
system-is-available)) for users to query the system status, all “rest”
interfaces of the API business will return this in a fixed manner::`{"status":
"maintain"}`. During maintenance with service suspended，all websocket notify
interfaces except subscribing system status updates(（[Subscribe system status
updates](https://docs.huobigroup.com/docs/dm/v1/en/#subscribe-system-status-
updates)）) can't work，and will push 1006 error code to clients.

> Response
    
    
    {
        "status": "maintain"
    }
    

### The two interfaces are:

  * Get system status: https://status-dm.huobigroup.com/api/v2/summary.json
  * Query whether the system is available: https://api.hbdm.com/heartbeat/

Besides the above two rest interfaces, for getting the infomation that system
maintenance with service suspended, could by subscribing system status updates
websocket interface.

## Get system status

This endpoint allows users to get system status, Incidents and planned
maintenance.

The system status can also be obtained through email, SMS, webhook, RSS/Atom
feed. Users can You can click [here](https://status-dm.huobigroup.com/) to
subscribe. The subscription function depends on Google services. Before you
subscribe, please ensure that you can access Google services normally.

    
    
    curl "https://status-dm.huobigroup.com/api/v2/summary.json"
    

### HTTP Request

  * GET `https://status-dm.huobigroup.com/api/v2/summary.json`

### Request Parameters

No parameter is available for this endpoint.

> Response:
    
    
    {
      "page": {  // Basic information of status page
        "id": "p0qjfl24znv5",  // page id
        "name": "Huobi",  // page name
        "url": "https://status-dm.huobigroup.com/", // page url
        "time_zone": "Etc/UTC", // time zone
        "updated_at": "2020-02-07T10:25:14.717Z" // page update time
      },
      "components": [  // System components and their status
        {
          "id": "h028tnzw1n5l",  // component id
          "name": "Deposit", // component name
          "status": "operational", // component status
          "created_at": "2019-12-05T02:07:12.372Z",  // component create time
          "updated_at": "2020-02-07T09:27:15.563Z", // component update time
          "position": 1,
          "description": null,
          "showcase": true,
          "group_id": "gtd0nyr3pf0k",  
          "page_id": "p0qjfl24znv5", 
          "group": false,
          "only_show_if_degraded": false
        }
      ],
      "incidents": [ // System fault incidents and their status
            {
                "id": "rclfxz2g21ly",  // incident id
                "name": "Market data is delayed",  // incident name
                "status": "investigating",  // incident stutus
                "created_at": "2020-02-11T03:15:01.913Z",  // incident create time
                "updated_at": "2020-02-11T03:15:02.003Z",   // incident update time
                "monitoring_at": null,
                "resolved_at": null,
                "impact": "minor",  // incident impact
                "shortlink": "http://stspg.io/pkvbwp8jppf9",
                "started_at": "2020-02-11T03:15:01.906Z",
                "page_id": "p0qjfl24znv5",
                "incident_updates": [ 
                    {
                        "id": "dwfsk5ttyvtb",   
                        "status": "investigating",   
                        "body": "Market data is delayed", 
                        "incident_id": "rclfxz2g21ly",   
                        "created_at": "2020-02-11T03:15:02.000Z",    
                        "updated_at": "2020-02-11T03:15:02.000Z",  
                        "display_at": "2020-02-11T03:15:02.000Z",   
                        "affected_components": [  
                            {
                                "code": "nctwm9tghxh6",  
                                "name": "Market data",  
                                "old_status": "operational",  
                                "new_status": "degraded_performance"  
                            }
                        ],
                        "deliver_notifications": true,
                        "custom_tweet": null,
                        "tweet_id": null
                    }
                ],
                "components": [  
                    {
                        "id": "nctwm9tghxh6",   
                        "name": "Market data",  
                        "status": "degraded_performance", 
                        "created_at": "2020-01-13T09:34:48.284Z", 
                        "updated_at": "2020-02-11T03:15:01.951Z", 
                        "position": 8,
                        "description": null,
                        "showcase": false,
                        "group_id": null,
                        "page_id": "p0qjfl24znv5",
                        "group": false,
                        "only_show_if_degraded": false
                    }
                ]
            }
        ],
          "scheduled_maintenances": [  // System scheduled maintenance events and their status
            {
                "id": "k7g299zl765l", // incident id
                "name": "Schedule maintenance", // incident name
                "status": "scheduled", // incident status
                "created_at": "2020-02-11T03:16:31.481Z",  // incident create time
                "updated_at": "2020-02-11T03:16:31.530Z",  // incident update time
                "monitoring_at": null,
                "resolved_at": null,
                "impact": "maintenance",  // incident impact
                "shortlink": "http://stspg.io/md4t4ym7nytd",
                "started_at": "2020-02-11T03:16:31.474Z",
                "page_id": "p0qjfl24znv5",
                "incident_updates": [  
                    {
                        "id": "8whgr3rlbld8",  
                        "status": "scheduled", 
                        "body": "We will be undergoing scheduled maintenance during this time.", 
                        "incident_id": "k7g299zl765l",  
                        "created_at": "2020-02-11T03:16:31.527Z",  
                        "updated_at": "2020-02-11T03:16:31.527Z",  
                        "display_at": "2020-02-11T03:16:31.527Z",  
                        "affected_components": [  
                            {
                                "code": "h028tnzw1n5l",  
                                "name": "Deposit And Withdraw - Deposit",  
                                "old_status": "operational",  
                                "new_status": "operational" 
                            }
                        ],
                        "deliver_notifications": true,
                        "custom_tweet": null,
                        "tweet_id": null
                    }
                ],
                "components": [  
                    {
                        "id": "h028tnzw1n5l",  
                        "name": "Deposit", 
                        "status": "operational", 
                        "created_at": "2019-12-05T02:07:12.372Z",  
                        "updated_at": "2020-02-10T12:34:52.970Z",  
                        "position": 1,
                        "description": null,
                        "showcase": false,
                        "group_id": "gtd0nyr3pf0k",
                        "page_id": "p0qjfl24znv5",
                        "group": false,
                        "only_show_if_degraded": false
                    }
                ],
                "scheduled_for": "2020-02-15T00:00:00.000Z",  // scheduled maintenance start time
                "scheduled_until": "2020-02-15T01:00:00.000Z"  // scheduled maintenance end time
            }
        ],
        "status": {  // The overall current status of the system
            "indicator": "minor",   // system indicator
            "description": "Partially Degraded Service"  // system description
        }
    }
    

### Response Content

Field | Data Type | Description  
---|---|---  
page |  | basic information of status page  
{id | string | page id  
name | string | page name  
url | string | page url  
time_zone | string | time zone  
updated_at} | string | page update time  
components |  | System components and their status  
[{id | string | component id  
name | string | component name, including Order submission, Order
cancellation, Deposit etc.  
status | string | component status, value range: operational,
degraded_performance, partial_outage, major_outage, under maintenance  
created_at | string | component create time  
updated_at | string | component update time  
.......}] |  | for details of other fields, please refer to the return example  
incidents |  | System fault incident and their status. If there is no fault at
present, it will return to null  
[{id | string | incident id  
name | string | incident name  
status | string | incident staus, value range: investigating, identified,
monitoring, resolved  
created_at | string | incident creat time  
updated_at | string | incident update time  
.......}] |  | for details of other fields, please refer to the return example  
scheduled_maintenances |  | System scheduled maintenance incident and status.
If there is no scheduled maintenance at present, it will return to null  
[{id | string | incident id  
name | string | incident name  
status | string | incident staus, value range: scheduled, in progress,
verifying, completed  
created_at | string | incident creat time  
updated_at | string | incident update time  
scheduled_for | string | scheduled maintenance start time  
scheduled_until | string | scheduled maintenance end time  
.......}] |  | for details of other fields, please refer to the return example  
status |  | The overall current status of the system  
{indicator | string | system indicator, value range: none, minor, major,
critical, maintenance  
description} | string | system description, value range: All Systems
Operational, Minor Service Outager, Partial System Outage, Partially Degraded
Service, Service Under Maintenance  
  
## Query whether the system is available

  * Interface `https://api.hbdm.com/heartbeat/`

### Returning Parameter

Parameter Name | Parameter Type | Desc  
---|---|---  
status | string | "ok" or "error"...  
<data> | dict object |  
heartbeat | int | future 1: avaiable 0: not available(maintenance with service
suspended)  
swap_heartbeat | int | coin margined swap 1: avaiable 0: not
available(maintenance with service suspended)  
estimated_recovery_time | long | null: normal. estimated recovery time
:millionseconds.  
swap_estimated_recovery_time | long | null: normal. coin margined swap
estimated recovery time millionseconds.  
option_heartbeat | int | option 1: avaiable 0: not available(maintenance with
service suspended)  
option_estimated_recovery_time | long | null: normal. option estimated
recovery time :millionseconds.  
linear_swap_heartbeat | long | USDT margined swap 1: avaiable 0: not
available(maintenance with service suspended)  
linear_swap_estimated_recovery_time | long | null: normal. USDT margined swap
estimated recovery time millionseconds.  
</data> |  |  
  
> Response:
    
    
    {
        "status":"ok",
        "data":{
            "heartbeat":1,
            "estimated_recovery_time":null,
            "swap_heartbeat":1,
            "swap_estimated_recovery_time":null,
            "option_heartbeat":1,
            "option_estimated_recovery_time":null,
            "linear_swap_heartbeat":1,
            "linear_swap_estimated_recovery_time":null
        },
        "ts":1557714418033
    }
    

  * Notice: Heartbeat is 1 is available, 0 is not available. 

## Get current system timestamp

get `https://api.hbdm.com/api/v1/timestamp`

### request

null

> response
    
    
    {
        "status": "ok",
        "ts": 1578124684692
    }
    
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result |  
ts | true | long | current system timestamp |  
  
#### Note:

  * It can be used for system time calibration.

## Details of Each Error Code

Error Code | Error Details Description  
---|---  
403 | invalid ID  
1000 | System error.  
1001 | System is unprepared.  
1002 | Query error.  
1003 | Abnormal redis operation.  
1004 | System busy. Please try again later.  
1010 | Account doesn't exist.  
1011 | The user's session doesn't exist.  
1012 | The user's account doesn't exist.  
1013 | This contract symbol doesn't exist.  
1014 | This contract doesn't exist.  
1015 | The index price does not exist.  
1016 | The bid offer does not exist. Please input the price.  
1017 | Order doesn't exist.  
1018 | Main account doesn't exist.  
1019 | Main account doesn't exist in the sub-account white list.  
1020 | The number of your sub-account exceeds the maximum. Please contact
customer service.  
1021 | Account open failed. Main account hasn’t opened contract trading
account yet.  
1030 | Input error.  
1031 | Incorrect form source.  
1032 | The number of access exceeded the limit.  
1033 | Incorrect field of contract period.  
1034 | Incorrect field of order price type.  
1035 | Incorrect field of form direction.  
1036 | Incorrect field of open long form.  
1037 | The leverage is invalid. Please contact the customer service.  
1038 | The order price exceeds the precision limit, please modify and order
again.  
1039 | Buy price must be lower than {0}{1}. Sell price must exceed {2}{3}.  
1040 | Invalid amount, please modify and order again.  
1041 | The order amount exceeds the limit ({0}Cont), please modify and order
again.  
1042 | Current positions have triggered position limits ({0}Cont). Please
order after changing the amount.  
1043 | Current positions have triggered position limits ({0}Cont). Please
order after changing the amount.  
1044 | Current positions have triggered position limits of our platform.
Please order after changing the amount.  
1045 | Unable to switch leverage due to open orders.  
1046 | Abnormal service. Please try again later.  
1047 | Insufficient margin available.  
1048 | Insufficient close amount available.  
1049 | Open a position with market price is not available.contracts  
1050 | Customer's order number is repeated. Please try again later.  
1051 | No orders to cancel.  
1052 | The number exceeds the batch limit.  
1053 | Unable to get the latest price range.  
1054 | Unable to get the latest price.  
1055 | The price is not reasonable, and the account equity will be less than 0
after placing this order. Please modify the price and place the order.  
1056 | In settlement. Your order can’t be placed/withdrew currently.  
1057 | Your order can’t be placed due to trading halt.  
1058 | Your order can’t be placed due to trade suspension.  
1059 | In delivery. Your order can’t be placed/withdrew currently.  
1060 | Your order can’t be placed currently due to abnormal contracts status.  
1061 | This order doesn't exist.  
1062 | Cancelling. Please be patient.  
1063 | The order has been executed.  
1064 | The main key of order conflicts.  
1065 | The form number of client isn't an integer.  
1066 | {0} cannot be empty.  
1067 | Illegal parameter {0}.  
1068 | Export error.  
1069 | The price is not reasonable.  
1070 | Empty data, cannot be exported.  
1071 | Repeated withdraw.  
1072 | Sell price must be lower than {0}{1}.  
1073 | Position abnormal. Please contact the customer service.  
1074 | Unable to order currently. Please contact the customer service.  
1075 | The price is not reasonable, and the margin rate will be less than 0
after placing this order. Please modify the price and place the order.  
1076 | No orders, please try again later.  
1077 | In settlement or delivery. Unable to get assets of current contract.  
1078 | In settlement or delivery. Unable to get assets of some contracts.  
1079 | In settlement or delivery. Unable to get positions of current contract.  
1080 | In settlement or delivery. Unable to get positions of some contracts.  
1081 | The number of your {0} contract trigger orders exceeds the limit {1}.  
1082 | Trigger type parameter error.  
1083 | Your position is in the process of forced liquidation. Unable to place
order temporarily.  
1084 | Your contract API is disabled, please try again after {0} (GMT+8).  
1085 | Trigger order failed, please modify the price and place the order again
or contact the customer service.  
1086 | {0} contract is restricted of opening positions on {1}. Please contact
customer service.  
1087 | {0} contract is restricted of closing positions on {1}. Please contact
customer service.  
1088 | {0} contract is restricted of withdraw order on {1}. Please contact
customer service.  
1089 | Transfer is temporarily restricted for {0} account, please contact
customer service support.  
1090 | Margin rate is lower than 0. Order can’t be placed.  
1091 | Equity is less than 0. Order can’t be placed.  
1092 | The Flash Closing Order takes the {0}th price at the order book. After
placing an order, the account equity will be less than 0. Please manually
enter the price or place an order with the counterparty price.  
1093 | The Flash Closing Order takes the {0}th price at the order book. The
margin rate will be less than 0 after placing an order. Please manually enter
the price or place an order with the counterparty price.  
1094 | The leverage cannot be empty, please switch the leverage or contact
customer service  
1095 | Non-trading state, unable to switch the leverage temporarily  
1100 | Unable to open a position currently. Please contact the customer
service.  
1101 | Unable to close a position currently. Please contact the customer
service.  
1102 | Unable to transfer in currently. Please contact customer service.  
1103 | Unable to transfer out currently. Please contact customer service.  
1104 | Trading is prohibited due to contracts trading constraints.  
1105 | Only Close is available due to contracts trading constraints.  
1106 | Delivery or settlement in progress, unable to transfer.  
1108 | Abnormal service. Please try again later.  
1109 | Sub-account doesn't own the permissions to open positions. Please
contact customer service.  
1110 | Sub-account doesn't own the permissions to close positions. Please
contact customer service.  
1111 | Sub-account doesn't own the permissions to transfer in. Please contact
customer service.  
1112 | Sub-account doesn't own the permissions to transfer out. Please contact
customer service.  
1113 | The sub-account does not have transaction permissions. Please login
main account to authorize.  
1114 | The sub-account does not have transfer permissions. Please login main
account to authorize.  
1115 | You have no access permissions of this sub-account.  
1200 | Login error. Please try again.  
1220 | You don’t have access permission as you have not opened contracts
trading.  
1221 | The total balances of Exchange Account can't meet the requirements for
opening contracts.  
1222 | The days of opening account can't meet the requirements for opening
contracts.  
1223 | The VIP level can't meet the requirements for opening contracts.  
1224 | Your country/region can't meet the requirements for opening contracts.  
1225 | Failed to open contracts.  
1226 | Repeated account.  
1227 | Huobi Contract does not support sub-accounts. Please log out sub-
account and log in again with primary account.  
1228 | You have not activated contract trading currently, please activate
first.  
1229 | Cannot agree twice.  
1230 | You haven't finished the risk verification.  
1231 | You haven't finished the ID Verification.  
1232 | The format/size of the image you uploaded does not meet the
requirements. Please re-upload.  
1233 | High leverage is not enabled (Please sign in the APP or web with your
main account to agree to the High-Leverage Agreement)  
1234 | {0} contract opening orders cannot exceed {1}  
1235 | {0} contract closing orders cannot exceed {1}  
1250 | Unable to get the HT_token.  
1251 | Unable to get BTC assets. Please try again later.  
1252 | Unable to get currency account assets. Please try again later.  
1253 | Error in signature verification.  
1254 | The sub-account has no permission to open futures, please go to the web
side to log in the main account and open.  
1300 | Transfer failed.  
1301 | Insufficient amount available.  
1302 | Transfer failed.  
1303 | The single transfer-out amount must be no less than {0}{1}.  
1304 | The single transfer-out amount must be no more than {0}{1}.  
1305 | The single transfer-in amount must be no less than {0}{1}.  
1306 | The single transfer-in amount must be no more than {0}{1}.  
1307 | Your accumulative transfer-out amount is over the daily maximum,
{0}{1}. You can't transfer out for the time being.  
1308 | Your accumulative transfer-in amount is over the daily maximum, {0}{1}.
You can't transfer in for the time being.  
1309 | Your accumulative net transfer-out amount is over the daily maximum,
{0}{1}. You can't transfer out for the time being.  
1310 | Your accumulative net transfer-in amount is over the daily maximum,
{0}{1}. You can't transfer in for the time being.  
1311 | The platform's accumulative transfer-out amount is over the daily
maximum. You can't transfer out for the time being.  
1312 | The platform's accumulative transfer-in amount is over the daily
maximum. You can't transfer in for the time being.  
1313 | The platform's accumulative net transfer-out amount is over the daily
maximum. You can't transfer out for the time being.  
1314 | The platform's accumulative net transfer-in amount is over the daily
maximum. You can't transfer in for the time being.  
1315 | Wrong transfer type.  
1316 | Failed to freeze the transfer.  
1317 | Failed to unfreeze the transfer.  
1318 | Failed to confirm the transfer.  
1319 | Failed to acquire the available transfer amount.  
1320 | The contract status is abnormal. Transfer is unavailable temporarily.  
1321 | Transfer failed. Please try again later or contact customer service.  
1322 | Invalid amount. Must be more than 0.  
1323 | Abnormal service, transfer failed. Please try again later.  
1325 | Failed to set trading unit  
1326 | Failed to obtain trading units  
1327 | No transfer permission, transfer failed, please contact customer
service  
1328 | No transfer permission, transfer failed, please contact customer
service  
1329 | No transfer permission, transfer failed, please contact customer
service  
1330 | No transfer permission, transfer failed, please contact customer
service  
1331 | Exceeds limit of transfer accuracy (8 digits). Please modify it  
1332 | The contract doesn't exist.  
1333 | Failed to open the Maker&Taker agreement  
1334 | Failed to check the Maker&Taker agreement  
1335 | Failed to check the second confirmation setting of Maker&Taker  
1336 | Failed to update the second confirmation setting of Maker&Taker  
1337 | Failed to check the settings of Maker&Taker  
1338 | Failed to update the settings of Maker&Taker  
1339 | Nickname contains illegal words, please modify it  
1340 | Nickname has been used, please modify it  
1341 | The enrollment has ended  
1342 | You cannot set nickname for sub-account  
1343 | Invalid indicator, please reset  
1344 | Sorry, {0} contracts can add market reminders currently at most  
1345 | Sorry, currently {0} can set up to {1} reminders  
1346 | The indicator already exists, please do not set it repeatedly  
1347 | {0} parameter is incorrect, please modify.  
1348 | This contract does not support cross margin mode.  
1349 | The leverage of the order does not match the leverage of the current
position, please switch the leverage first.  
1401 | order price shall be lower than the strike price.  
1403 | The number of take-profit and stop-loss orders for {0} contract shall
not exceed {1}  
1404 | Take-profit and stop-loss orders can only be bound with orders for
opening a position  
1405 | The take-profit price shall not be {0}{1}{2}  
1406 | Your chances of lucky draw have been used up  
1407 | The stop-loss price shall not be {0}{1}{2}  
12001 | Invalid submission time.  
12002 | Incorrect signature version.  
12003 | Incorrect signature method.  
12004 | Private key is expired.  
12005 | Incorrect IP address.  
12006 | The submission time can't be empty.  
12007 | Incorrect public key.  
12008 | Verification failed.  
12009 | The user is locked or doesn't exist.  
  
## API Best Practice

### 1\. Query contract history orders interface: /api/v1/contract_hisorders

  * To ensure timeliness and to reduce latency, users are highly recommended to get contract history orders information faster from server memory using interface “query contract order information” (URL: api/v1/contract_order_info).

  * For users who use interface “query contract history orders” (URL: /api/v1/contract_hisorders), please enter as many query conditions as possible (including symbol, trade_type（recommended to send “0” to query all）, type, status, create_date). Besides, try not to enter a big integer in parameter “create_date”. You are kindly suggested to query one-day data at a time.

### 2\. Query contract match results interface: /api/v1/contract_matchresults

  * To improve query performance and response speed, please enter as many querying conditions as possible (including symbol, trade_type（recommended to send “0” to query all）, contract_code, create_date). Besides, try not to enter a big integer in parameter “create_date”. You are kindly suggested to query one-day data at a time.

### 3\. Query contract financial record interface:
/api/v1/contract_financial_record

  * To improve query performance and response speed, please enter as many querying conditions as possible (including symbol, type(recommended to leave it blank to query all), create_date). Besides, try not to enter a big integer in parameter “create_date”. You are kindly suggested to query one-day data at a time.

### 4\. Query contract order detail interface: api/v1/contract_order_detail

  * When querying orders without parameter(such as the parameter: created_at), the query result data may be delayed. It is recommended to pass the two parameters of the interface: created_at (order timestamp) and order_type (order type, default 1), the database will be directly queried, and the query results data will be more timely.

  * Querying condition “created_at” uses 13-bit long type time stamp (including milliseconds). Querying performance will be improved when accurate time stamps are entered.

  * For example: the converted time stamp of "2019/10/18 10:26:22" is 1571365582123. The returned ts from interface “contract_order” can be used as time stamp to query corresponding order. 0 is not allowed in parameter “created_at”.

### 5\. Query contract trigger order history orders interface:

  * api/v1/contract_trigger_hisorders

  * To improve query performance and response speed, please enter as many parameters as possible (including symbol, contract_code, trade_type, status, create_date). Besides, try not to enter a big integer in parameter “create_date”. You are kindly suggested to query one-day data at a time.

### 6\. WebSocket subscription to Market Depth data:

  * For acquiring market depth data within 150 steps, you are kindly suggested to use step0, step1, step2, step3, step4, step5, step14, step15；

  * For acquiring market depth data within 20 steps, you are kindly suggested to use step6, step7, step8, step9, step10, step11, step12, step13；

  * Since the large volume of pushing 150 steps data every 100ms, WebSocket disconnection may occur frequently if client’s network bandwidth is insufficient or the processing is not in time; therefore, we highly recommend users using step6, step7, step8, step9, step10, step11, step12, step13 to acquire 20 steps data. For instance, subscribing 20 steps data.

`{`

`"sub": "market.BTC_CQ.depth.step6",`

`"id": "id5"`

`}`

  * We also suggest that you subscribe incremental market depth data.orderbook event will be checked every 30ms. If there is no orderbook event, you will not receive any orderbook data.you HAVE TO maintain local orderbook data,such as updating your local orderbook bids and asks data.You can subscribe 20 or 150 unmerged data.

`{`

`"sub": "market.BTC_CQ.depth.size_20.high_freq",`

`"data_type":"incremental",`

`"id": "id1"`

`}`

### 7\. Place order interface (URL: api/v1/contract_order) and place a batch
of orders interface (URL:api/v1/contract_batchorder):

  * We recommend to fill in the parameter “client_order_id”(should be unique from user-side),which can help users to acquire order status and other order information according to the parameter “client_order_id" from

  * query order information interface (URL: api/v1/contract_order_info ) when there is no returned information due to network or other problems.

## Code Demo

**REST**

  * [Java](https://github.com/huobiapi/Futures-Java-demo)

  * [Python](https://github.com/huobiapi/Futures-Python-demo)

  * [Golang](https://github.com/huobiapi/Futures-Go-demo)

  * [CSharp](https://github.com/huobiapi/Futures-CSharp-demo)

  * [PHP](https://github.com/huobiapi/Futures-PHP-demo)

  * [Node.js](https://github.com/huobiapi/Futures-Node.js-demo)

  * [Postman](https://github.com/hbdmapi/huobi_futures_Postman)

**Websocket**

  * [Java](https://github.com/huobiapi/Futures-Java-demo/tree/master/WebSocket-JAVA-demo)

  * [Python](https://github.com/huobiapi/Futures-Python-demo/tree/master/Websocket-Python3-demo)

  * [Node.js](https://github.com/huobiapi/Futures-Node.js-demo/tree/master/WebSocket-Node.js-demo)

**Contract sdk**

  * [Java](https://github.com/hbdmapi/huobi_future_Java)

**Asynchronous Library**

  * [Rust](https://github.com/hbdmapi/huobi_future_async)

# Future API FAQ

## Access and Authentication

### Q1: Is the API Key for future and spot the same ?

Yes. The future API key and spot API key are same. You can create API using
the following link.[ click here](https://www.hbg.com/zh-cn/apikey/)

### Q2: Why are APIs disconnected or timeout?

  1. The network connection is unstable if the server locates in China mainland,it is suggested to invoke APIS from a server located in 1c area of AWS Tokyo.

  2. You can use api.btcgateway.pro to debug for domestic network.

### Q3: Why is the websocket often disconnected?

It seems that most of the abnormal websocket issues (such as disconnect,
websocket close )(websocket: close 1006 (abnormal closure))are caused by
different network environment. The following measures can effectively reduce
websocket issues.

It would be better if the server is located in 1c area of AWS Tokyo with url
api.hbdm.vn and implement websocket re-connection mechanism. Both market
heartbeat and order heartbeat should response with Pong with different format,
following Websocket market heartbeat and account heartbeat
requirement.[here](https://docs.huobigroup.com/docs/dm/v1/en/#websocket-
heartbeat-and-authentication-interface)

### Q4: What is the difference between api.hbdm.com and api.hbdm.vn?

The api.hbdm.vn uses AWS's CDN service. it should be more stable and faster
for AWS users. The api.hbdm.com uses Cloudflare's CDN service.

### Q5: What is the colocation service ? which attention points should we know
?

Actually ,colo corresponds to a vpc node, which directly connects to private
network of huobi's future, so it will reduce the latency between the client
and the Huobi future server (bypassing the CDN)

huobi future and huobi swap have the same colo, so the domain name connecting
the swap api and the future api are the same.

Note : Colo needs to use api.hbdm.com for signature(authentication) to avoid
getting 403 error: Verification failure.

### Q6: Why does signature verification return failure (403: Verification
failure) ?

The signature process of future is similar to huobi Spot . In addition to the
following precautions,please refer to the swap or spot demo to verify whether
the signature is successful. Please check your own signature code after demo
verification is successful. The coin margined swap code demo is
[here](https://docs.huobigroup.com/docs/coin_margined_swap/v1/en/#code-demo).
The future code demo is
[here](https://docs.huobigroup.com/docs/dm/v1/en/#code-demo).The option code
demo is [here](https://docs.huobigroup.com/docs/option/v1/en/#code-demo). The
USDT Margined Swap code demo is
[here](https://docs.huobigroup.com/docs/usdt_swap/v1/en/#code-demo).

  1. Check if the API key is valid and copied correctly.
  2. Check if the IP is in whitelist
  3. Check if th timestamp is UTC time
  4. Check if parameters are sorted alphabetically
  5. Check if the encoding is UTF-8 
  6. Check if the signature has base64 encoding
  7. Any method with parameters for GET requests should be signed.
  8. Any method with parameters for POST requests don't need to be signed.
  9. Check if whether the signature is URI encoded and Hexadecimal characters must be capitalized, such as ":" should be encoded as "%3A", and the space should be encoded as "%20"
  10. The authorization of websocket is similar to the authorization of restful interface.Pls note that the json body of the websocket authorization shouldn't be URL encoded.
  11. The host in signature text should be the same as the host in your API request.The proxy may change the request host, you can try without proxy;Some http/websocket library may include port in the host, you can try to append port in signature host, like "api.hbdm.com:443"
  12. The hidden text in API Key and Secret Key may have impact on the signature.

### Q7: Is the ratelimit of public market based on IP ? Is the ratelimit of
interface with private key based on UID?

Yes. The ratelimit of interface with private key is based on the UID, not the
API key. The master and sub accounts are separately ratelimited and don't
affect each other.

### Q8: Is there any recommendation for third-party framework which integrates
Huobi future?

There is an open source asynchronous quantization framework which integrates
Huobi future and Huobi swap: [here](https://github.com/hbdmapi/hbdm_Python).
If you have any quetsions, please open a ticket in github issues.

## Market and Websocket

### Q1: How often are the snapshot orderbook subscription and incremental
orderbook subscription pushed?

The snapshot orderbook subscription(market.$symbol.depth.$type) is checked
once every 100MS.If there is an update,it will be pushed. It will be pushed at
least 1 second.The incremental orderbook subscription is checked once every
30MS.If there is an update,it will be pushed.If there is no update, it will
not be pushed.

### Q2: How often is the market trade subscription pushed?

The market trade subscription will be pushed when there is a transaction.

### Q3: Are there historical Kline data or historical market trade data?

Historical Kline data can be obtained through the API
interface:/market/history/kline.Only the from and to parameters need to be
filled in, and the size parameter is not needed.At most, only two consecutive
years of data can be obtained.

The historical market trade data is currently not available, you can store it
locally by subscribing to market trade: market.$symbol.trade.detail.

### Q4: How to get MACD and other technical indicators on Kline?

The API does not have interfaces to get technical indicators such as MACD. You
can refer to TradingView and other websites to calculate them.

### Q5: What is the definition of timestamp in the document?

The timestamp in the document refers to the total number of seconds or total
milliseconds from Greenwich Mean Time, January 1, 1970, 00:00:00 (Beijing
Time, January 1, 1970, 08:00:00) to the present.

### Q6: What is the definition of the 150 level and 20 level of MBP?

The Subscription of MBP data: market.$symbol.depth.$type.150 price level means
the current bids and asks splited into 150 level by price.20 price level means
the current bids and asks splited into 20 level by price.

### Q7: What is the meaning of merged depth when subscribing MBP data?

The subscrpition of MBP data:market.$symbol.depth.$type：

step1 and step7 are merged by 5 decimal places.bids down,asks up. step2 and
step8 are merged by 4 decimal places.bids down,asks up. step3 and step9 are
merged by 3 decimal places.bids down,asks up. step4 and step10 are merged by 2
decimal places.bids down,asks up. step5 and step11 are merged by 1 decimal
places.bids down,asks up. step12 and step14 are combined by single digit.bids
down,asks up. step13 and step15 are combined by tens.bids down,asks up.

Example:

step4(0.01):

bids price: 100.123, 100.245. The merged bids price are 100.12, 100.24.

asks price: 100.123, 100.245 The merged asks price are 100.13, 100.25.

("Down" and "Up" are rounded up or down, if the price is down, the asks price
is not rounded down, and the bids price is rounded up.)

150 price level: step0 to step5, step14, step15；

20 price level: step6 to step13;

More examples：

step1(0.00001):

price: 1.123456 The merged bid price is 1.12345. The merged ask price is
1.12346.

step7(0.00001):

price: 1.123456 The merged bid price is 1.12345. The merged ask price is
1.12346.

step6(0.000001)

price: 1.123456 The merged bid price is 1.123456. The merged ask price is
1.123456.

step11(0.1):

price: 1.123456 The merged bid price is 1.1. The merged ask price is 1.1.

### Q8:Does websocket's position channel push full data or incrementall data
each time?

Subscription of position event: "positions.btc".The latest position is
pushed,including the volumes, available volumes, frozen volumes.If there is no
update,it will not be pushed.

### Q9: Does websocket's position channel push data when the unrealized profit
is updated?

Subscription of position event: "positions.btc".It will not be pushed if only
unrealized profit is updated. It will be pushed only when position event is
updated.

### Q10: What is the difference between market detail and trade detail in WS?

Market Detail(market.$symbol.detail) is the merged market data. It will be
checked every 0.5s, pushed once trade event udpates,including the OHLCV
data,etc.Trade Detail(market.$symbol.trade.detail) is pushed once trade event
updates,including trade price, trade volume, trade direction,etc.

### Q11: What is the meaning of the two ts pushed by subscription of
incremental MBP ?

Subscription of incremental
MBP：market.$symbol.depth.size_${size}.high_freq，The outer ts is the timestamp
when the market server sends the data.The inner ts is the timestamp when the
orderbook is checked.

### Q12: What is the difference between websocket subscription of MBP and
incremental MBP? How often is the incremental MBP pushed?

market.$symbol.depth.$type is snapshot MBP
data，market.$symbol.depth.size_${size}.high_freq is incremental MBP
data.Snapshot MBP data is checked every 100ms,pushed at least every
1s.Incremental MBP data is checked every 30ms.It will not be pushed,if MBP has
no update.

### Q13: How to maintain local MBP data subscribing incremental
MBP:market.$symbol.depth.size_${size}.high_freq?

Snapshot MBP data will be pushed for the first time, and the incremental MBP
data will be pushed afterwards.

(1) Compare the incremental price with the previous full MBP data, and replace
the order amount with the same price;

(2) If the price is not in the local MBP data,add the price to the local MBP
data;

(3) If a price level is gone, data such as [8100, 0] will be pushed.You have
to remove the same price of local MBP data;

(4) For the same websocket connection, the incremental data version is
incremented; if the version is not incremented, you need to re-subscribe and
re-maintain the local full MBP data;

### Q14: Will the quarter contract of the delivery contract be converted to
the next week contract, will it be notified or changged by WS?

If a quarterly contract such as BTC_CQ is converted to the next week contract
BTC_NW, WS will not automatically notify you, you need to change the
subscription to BTC_NW.

## Order and Trade

### Q1: What is the future settlement cycle? Which interface can be used to
check the status when the future is settled?

一、Orders can't be placed or cancelled during settlement period, error code
"1056" will be returned if users place or cancel orders. You are recommended
to request contract information every few seconds during settlement period:
api/v1/contract_contract_info. It's in settlement time if there is any number
of 5, 6, 7, 8 included in the returned status code of contract_status, while
it indicates that settlement completed and users could place and cancel orders
as usual if the returned status code is 1.

二、 We warmly remind you that Huobi Futures is settled at 16:00 on each Friday
(GMT+8). When querying fund or position information during the settlement
period, error codes will be returned.

Error codes and their meaning are as following:

Error code "1077" indicates that "the fund query of current perpetual swap
trading pair failed during the settlement"; Error code "1078" indicates that
"the fund query of part of perpetual swap trading pairs failed during the
settlement"; Error code "1079" indicates that "the position query of current
perpetual swap trading pair failed during the settlement"; Error code "1080"
indicates that "the position query of part of perpetual swap trading pairs
failed during the settlement"; You are recommended to read the status code
from the returned message. If the above four types of status code appear, the
returned data is not accurate and couldn't be used as reference.

### Q2: What's the reason for 1004 error code?

We notice that the system is sometimes overloaded when the market suddenly
turns to be highly volatile. If the system is busy recently or the following
prompts appear:

{“status”: “error”, “err_code”: 1004, “err_msg”: “System busy. Please try
again later.”, “ts”:}

please be patient, and do not place or cancel order repeatedly during the
process to avoid repeated orders and additional pressure on system
performance. In the meanwhile, it is recommended to place and cancel orders
through Web and APP.

### Q3: The same order ID and match ID can have multiple trades. for example:
if a user take a large amount of maker orders, there will be multiple
corresponding trades . How to identify these different trades ?

The field ID returned by the information interface
api/v1/contract_order_detail is a globally unique transaction identifier. if a
maker order is matched multiple times, a trade will be pushed once there is a
transaction matched.

### Q4: What is the delay for the round trip of huobi future?

At present,it normally takes about 30-50ms from placing the order to getting
the status of the order.

### Q5: Why does the API return connection reset or Max retris or Timeout
error?

Most of the network connectivity problems ,(such as Connection reset or
network timeout ) are caused by network instability , you can use the server
in AWS Tokyo C area with api.hbdm.vn , which can effectively reduce network
timeout errors.

### Q6: How to check the order status without order_id not returned?

If the order_id couldn't be returned due to network problems, you can query
the status of the order by adding the custom order number(client_order_id ).

### Q7: What to do if it's diconnected after the websocket subscription of
account, order and positions for a while?

When subscribing private accounts, orders and positions, the heartbeat should
also be maintained regularly ,which is different from the market heartbeat
format . Please refer to the ["websocket Heartbeat and Authentication
Interface" ](https://docs.huobigroup.com/docs/dm/v1/en/#websocket-heartbeat-
and-authentication-interface). if the it is disconnected ,please try to
reconnect.

### Q8: What is the difference between order status 1 and 2 ? what is the
status 3 ?

Status 1 is the preparation for submission. status 2 is the sequential
submission of internal process, which can be considered that it has been
accepted by the system. Status 3 indicated that the order has been already
submitted to market.

### Q9: Is there an interface to get the total assets in BTC of my account ?

No.

### Q10: Why is the order filled after the order is withdrawed successfully by
placing API cancellation ?

The success return of order cancellation or placement only represents that the
command is excuted successfully and doesn't mean that the order has been
cancelled . You can check the order status through the interface
api/v1/contract_order_info.

### Q11: How long does it generally take for an API from withdrawing to
cancelling successfully ?

The order cancellation command generally takes several tens of ms. The actual
status of order cancellation can be obtained by invoking the interface:
api/v1/contract_order_info.

### Q12: How to get historical liquidation orders?

To obtain historical liquidation orders, you can access the one of four api
interfaces: Get History Orders (/api/v1/contract_hisorders), Get History Match
Results (/api/v1/contract_matchresults), Query history orders via multiple
fields (/api/v1/contract_hisorders_exact), Query history transactions via
multiple fields (/api/v1/contract_matchresults_exact), with the return field
order_source (order source) to judge. When order_source returns "risk", it
means that this order is a liquidated order.

## Error Codes

### Q1: What is the reason for 1030 error code?

If you encounter errors such as
{"status":"error","err_code":1030,"err_msg":"Abnormal service. Please try
again later.","ts":1588093883199},indicating that your input request parameter
is not correct, please print your request body and complete URL parameters,
and please check the corresponding API document interface one by one.The
common example is that the volume must be an integer, and the client_order_id
must be of type uint32 rather than type uint64.

### Q2: What is the reason for 1048 error code?

If you encounter errors such as {'index': 1, 'err_code': 1048, 'err_msg':
'Insufficient close amount available.'}, indicating that your available
position is not enough.You need to query the api api/v1/contract_position_info
to get your available position.

### Q3: What is the reason for 1032 error code?

1032 means that your request exceeds the ratelimit. The coin margined swap,
future, option swap and USDT margined swap limit the rate separately. Please
check the ratelimit in the api ratelimit instructions, and you can print the
current ratelimit in the header of the API response to check whether the
ratelimit is exceeded. It is recommended to increase the request interval
delay to avoid exceeding the ratelimit.

## How to solve problems more effectively?

When you report an API error, you need to attach your request URL, the
original complete body of the request and the complete request URL parameters,
and the original complete log of the server's response. If it is a websocket
subscription, you need to provide the address of the subscription, the topic
of the subscription, and the original complete log pushed by the server.

If it is an order-related issue, use the API order query interface
api/v1/contract_order_info to keep the complete log returned and provide your
UID and order number.

# Future Market Data interface

## Get Contract Info

### Example

  * GET `api/v1/contract_contract_info`

    
    
    curl "https://api.hbdm.com/api/v1/contract_contract_info"      
    

### Request Parameter

Parameter Name | Type | Mandatory | Description  
---|---|---|---  
symbol | string | false | Case-Insenstive.Both uppercase and lowercase are
supported.e.g. "BTC","ETH"...  
contract_type | string | false | "this_week","next_week", "quarter"
"next_quarter"  
contract_code | string | false | BTC180914  
  
### Note：

Note：If there is a number in the Contract Code row，inquiry with Contract_Code.
If there is no number，inquiry by Symbol + Contract Type. One of the query
conditions must be chosen.

> Response
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "BTC",
                "contract_code": "BTC201225",
                "contract_type": "quarter",
                "contract_size": 100,
                "price_tick": 0.01,
                "delivery_date": "20201225",
                "create_date": "20200605",
                "contract_status": 1
            }
        ],
        "ts": 1604296501822
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Description | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<list>(Attribute Name: data) |  |  |  |  
symbol | true | string | Product Code | "BTC","ETH"...  
contract_code | true | string | Contract Code | "BTC180914" ...  
contract_type | true | string | Contract Type | "this_week","next_week",
"quarter" ,"next_quarter"  
contract_size | true | decimal | Contract Value (USD of one contract) | 10,
100...  
price_tick | true | decimal | Minimum Variation of Contract Price | 0.001,
0.01...  
delivery_date | true | string | Contract Delivery Date | eg "20180720"  
create_date | true | string | Contract Listing Date | eg "20180706"  
contract_status | true | int | Contract Status | 0: Delisting,1: Listing,2:
Pending Listing,3: Suspension,4: Suspending of Listing,5: In Settlement,6:
Delivering,7: Settlement Completed,8: Delivered,9: Suspending of Trade  
</list> |  |  |  |  
ts | true | long | Time of Respond Generation，Unit：Millisecond |  
  
## Get Contract Index Price Information

### Example

  * GET `api/v1/contract_index`

    
    
    curl "https://api.hbdm.com/api/v1/contract_index?symbol=BTC" 
    

### Request Parameter

Parameter Name | Parameter Type | Mandatory | Desc  
---|---|---|---  
symbol | string | false | Case-Insenstive.Both uppercase and lowercase are
supported.e.g. "BTC","ETH"...  
  
> Response
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "BTC",
                "index_price": 13707.26,
                "index_ts": 1604296614010
            }
        ],
        "ts": 1604296620746
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<list>(Attribute Name: data) |  |  |  |  
symbol | true | string | symbol | "BTC","ETH"...  
index_price | true | decimal | Index Price |  
index_ts | true | long | Response generation time point, unit: millisecond |  
</list> |  |  |  |  
ts | true | long | Time of Respond Generation，Unit：Millisecond |  
  
## Get Contract Price Limitation

### Example

  * GET `api/v1/contract_price_limit`

    
    
    curl "https://api.hbdm.com/api/v1/contract_price_limit?symbol=BTC&contract_type=this_week"
    

### Request Parameter

Parameter Name | Parameter Type | Mandatory | Desc  
---|---|---|---  
symbol | string | false | Case-Insenstive.Both uppercase and lowercase are
supported.e.g."BTC","ETH"...  
contract_type | string | false | Contract Type
("this_week","next_week","quarter", "next_quarter")  
contract_code | string | false | BTC180914 ...  
  
### Note ：

If there is a number in the Contract Code row，inquiry with Contract_Code. If
there is no number，inquiry by Symbol + Contract Type. One of the query
conditions must be chosen.

> Response
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "BTC",
                "contract_code": "BTC201225",
                "contract_type": "quarter",
                "high_limit": 14724.88,
                "low_limit": 13057.92
            }
        ],
        "ts": 1604296680648
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" ,"error"  
<list>(Attribute Name: data) |  |  |  |  
symbol | true | string | Variety code | "BTC","ETH" ...  
high_limit | true | decimal | Highest Buying Price |  
low_limit | true | decimal | Lowest Selling Price |  
contract_code | true | string | Contract Code | eg "BTC180914" ...  
contract_type | true | string | Contract Type |
"this_week","next_week","quarter" ,"next_quarter"  
<list> |  |  |  |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
## Get Contract Open Interest Information

### Example

  * GET `api/v1/contract_open_interest`

    
    
    curl "https://api.hbdm.com/api/v1/contract_open_interest?symbol=BTC&contract_type=this_week"
    

### Request Parameter

Parameter Name | Parameter Type | Mandatory | Desc  
---|---|---|---  
symbol | string | false | Case-Insenstive.Both uppercase and lowercase are
supported.e.g."BTC","ETH"...  
contract_type | string | false | Contract Type
("this_week","next_week","quarter")  
contract_code | string | false | BTC180914  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "volume": 3057834,
                "amount": 22013.565930537597871378,
                "symbol": "BTC",
                "contract_type": "quarter",
                "contract_code": "BTC201225"
            }
        ],
        "ts": 1604296751272
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<list>(Attribute Name: data) |  |  |  |  
symbol | true | string | Variety code | "BTC", "ETH" ...  
contract_type | true | string | Contract Type |
"this_week","next_week","quarter", "next_quarter"  
volume | true | decimal | Position quantity(volume) |  
amount | true | decimal | Position quantity(Currency) |  
contract_code | true | string | Contract Code | eg "BTC180914" ...  
</list> |  |  |  |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
## Get the estimated delivery price

### Example

  * GET `api/v1/contract_delivery_price`

    
    
    curl "https://api.hbdm.com/api/v1/contract_delivery_price?symbol=BTC"
    

### Request Parameter

Parameter Name | Parameter Type | Mandatory | Desc  
---|---|---|---  
symbol | string | true | Case-Insenstive.Both uppercase and lowercase are
supported.e.g."BTC","ETH"...  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "delivery_price": 13212.3643864774624373956594
        },
        "ts": 1604296995036
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<list>(Attribute Name: data) |  |  |  |  
delivery_price | true | decimal | estimated delivery price |  
</list> |  |  |  |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
## Get Market Depth

### Example

  * GET `/market/depth`

    
    
    curl "https://api.hbdm.com/market/depth?symbol=BTC_CQ&type=step5"
    

### Request Parameter

Parameter Name | Parameter Type | Mandatory | Desc  
---|---|---|---  
symbol | string | true | Case-Insenstive.Both uppercase and lowercase are
supported..e.g. "BTC_CW" represents BTC “This Week”，"BTC_NW" represents BTC
“Next Week”，"BTC_CQ" represents BTC “Quarter”."BTC_NQ" represents BTC “Next
Quarter”. Contract code is supported to query data. e.g.: "BTC200918"(weekly),
"BTC200925"(Bi-weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
type | string | true | Get depth data within step 150, use step0, step1,
step2, step3, step4, step5, step14, step15（merged depth data 0-5,14-15）；when
step is 0，depth data will not be merged; Get depth data within step 20, use
step6, step7, step8, step9, step10, step11, step12, step13(merged depth data
7-13); when step is 6, depth data will not be merged.  
  
> tick illustration:
    
    
    "tick": {
        "id": Message id,
        "ts": Time of Message Generation, unit: millisecond,
        "bids": Buying, [price(hanging unit price), vol(this price represent single contract)], According to the descending order of Price,
        "asks": Selling, [price(hanging unit Price), vol(this price represent single contract)], According to the ascending order of Price,
        "ch": Data channel,
        "mrid": Order ID,
        "ts": Time of Respond Generation,
        "version": version ID 
    }
    
    

> Response:
    
    
    {
        "ch":"market.BTC_NQ.depth.step6",
        "status":"ok",
        "tick":{
            "asks":[
                [
                    14100.87,
                    163
                ],
                [
                    14100.88,
                    20
                ]
            ],
            "bids":[
                [
                    14098.09,
                    53
                ],
                [
                    14098.08,
                    75
                ]
            ],
            "ch":"market.BTC_NQ.depth.step6",
            "id":1604297395,
            "mrid":113765352864,
            "ts":1604297395012,
            "version":1604297395
        },
        "ts":1604297395085
    }
    

### Returning Parameter

Parameter Name | Mandatory | Data Type | Desc | Value Range  
---|---|---|---|---  
ch | true | string | Data belonged channel，Format： market.period |  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation，Unit：Millisecond |  
<tick> |  |  |  |  
mrid | true | long | Order ID |  
id | true | long | tick ID |  
asks | true | array | Sell,[price(Ask price), vol(Ask orders (cont.) )], price
in ascending sequence |  
bids | true | array | Buy,[price(Bid price), vol(Bid orders(Cont.))], Price in
descending sequence |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
version | true | long | version ID |  
ch | true | string | Data channel, Format： market.period |  
</tick> |  |  |  |  
  
## Get Kline Data

### Example

  * GET `/market/history/kline`

    
    
    curl "https://api.hbdm.com/market/history/kline?period=1min&size=200&symbol=BTC_CQ"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Contract Name |  | Case-Insenstive.Both uppercase and
lowercase are supported..e.g. "BTC_CW" represents BTC “This Week”，"BTC_NW"
represents BTC “Next Week”，"BTC_CQ" represents BTC “Quarter”."BTC_NQ"
represents BTC “Next Quarter”. Contract code is supported to query data. e.g.:
"BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
period | true | string | Kline Type |  | 1min, 5min, 15min, 30min, 60min,
1hour,4hour,1day, 1mon  
size | false | int | Acquisition Quantity | 150 | [1,2000]  
from | false | long | start timestamp seconds. |  |  
to | false | long | end timestamp seconds |  |  
  
### Note

  * Either `size` field or `from`/`to` fields need to be filled.
  * If `size` field and `from`/`to` fields are not filled, It will return error messages.
  * If `from` field is filled, `to` field need to filled too.
  * The api can mostly return the klines of last two years.

> Data Illustration：
    
    
    "data": [
      {
            "id": Kline id,
            "vol": Transaction Volume(amount),
            "count": transaction count
            "open": opening Price
            "close": Closing Price, when the Kline is the latest one，it means the latest price
            "low": Lowest price
            "high": highest price
            "amount": transaction volume(currency), sum(every transaction volume(amount)*every contract value/transaction price for this contract)
       }
    ]
    

> Response:
    
    
    {
        "ch": "market.BTC_NQ.kline.5min",
        "data": [
            {
                "amount": 4.30994018951037,
                "close": 14103.1,
                "count": 39,
                "high": 14110,
                "id": 1604297400,
                "low": 14098.29,
                "open": 14098.75,
                "vol": 608
            },
            {
                "amount": 0.19851299586596685,
                "close": 14104.87,
                "count": 1,
                "high": 14104.87,
                "id": 1604297700,
                "low": 14104.87,
                "open": 14104.87,
                "vol": 28
            }
        ],
        "status": "ok",
        "ts": 1604297729928
    }
    

### Returning Parameter

Parameter Name | Mandatory | Data Type | Desc | Value Range  
---|---|---|---|---  
ch | true | string | Data belonged channel，Format： market.period |  
data | true | object | Kline Data |  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
### data parameters

**parameter name** | **type** | **desc** |  
---|---|---|---  
id | int | kline id,the same as kline timestamp, kline start timestamp |  
vol | decimal | volume. |  
count | decimal | count. |  
open | decimal | open price |  
close | decimal | close price |  
low | decimal | lowest price |  
high | decimal | highest price |  
amount | decimal | amount based on coins. |  
  
## Get Market Data Overview

### Example

  * GET `/market/detail/merged`

    
    
    curl "https://api.hbdm.com/market/detail/merged?symbol=BTC_CQ"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Contract Name |  | Case-Insenstive.Both uppercase and
lowercase are supported..e.g. "BTC_CW" represents BTC “This Week”，"BTC_NW"
represents BTC “Next Week”，"BTC_CQ" represents BTC “Quarter”."BTC_NQ"
represents BTC “Next Quarter”. Contract code is supported to query data. e.g.:
"BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
  
> tick Illustration:
    
    
    "tick": {
        "id": Kline id,
        "vol": transaction volume（contract）,
        "count": transaction count
        "open": opening price,
        "close": Closing Price, when the Kline is the latest one，it means the latest price
        "low": Lowest price
        "high": highest price
        "amount": transaction volume(currency), sum(every transaction volume(amount)*every contract value/transaction price for this contract)
        "bid": [price of buying one (amount)],
        "ask": [price of selling one (amount)]
    
      }
    

> Response:
    
    
    {
        "ch": "market.BTC_NQ.detail.merged",
        "status": "ok",
        "tick": {
            "amount": "4478.2911316482577028620799060719867257944",
            "ask": [
                14114.01,
                177
            ],
            "bid": [
                14112.71,
                28
            ],
            "close": "14114",
            "count": 18805,
            "high": "14299.99",
            "id": 1604298319,
            "low": "14028.78",
            "open": "14229.47",
            "ts": 1604298319019,
            "vol": "633708"
        },
        "ts": 1604298319019
    }
    

### Returning Parameter

Parameter Name | Mandatory | Data Type | Desc | Value Range  
---|---|---|---|---  
ch | true | string | Data belonged channel，format：
market.$contract_code.detail.merged |  
status | true | string | Request Processing Result | "ok" , "error"  
tick | true | object | Kline Data |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
<tick> |  |  | kline data (Start at 00:00(UTC+8) of the day) |  
id | true | long | kline id,the same as kline timestamp |  
vol | true | string | Trade Volume(Cont.) |  
count | true | int | Order Quantity |  
open | true | string | Open Price |  
close | true | string | Clos Price, the price in the last kline is the latest
order price |  
low | true | string | Low Price |  
high | true | string | High Price |  
amount | true | string | Trade Amount(Coin), trade amount(coin)=sum(order
quantity of a single order * face value of the coin/order price) |  
ask | true | object | Sell,[price(Ask price), vol(Ask orders (cont.) )], price
in ascending sequence |  
bid | true | object | Buy,[price(Bid price), vol(Bid orders(Cont.))], Price in
descending sequence |  
</tick> |  |  |  |  
  
## Query The Last Trade of a Contract

### Example

  * GET `/market/trade`  

    
    
    curl "https://api.hbdm.com/market/trade?symbol=BTC_CQ"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Contract Name |  | Case-Insenstive.Both uppercase and
lowercase are supported.. e.g. "BTC_CW" represents BTC “This Week”，"BTC_NW"
represents BTC “Next Week”，"BTC_CQ" represents BTC “Quarter”."BTC_NQ"
represents BTC “Next Quarter”. Contract code is supported to query data. e.g.:
"BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
  
> Tick Illustration：
    
    
    "tick": {
      "id": Unique Order Id(symbol level),
      "ts": Latest Transaction time,
      "data": [
        {
          "id": Unique Transaction Id(symbol level),
          "price": Transaction price,
          "amount": transaction amount,
          "direction": Active transaction direction,
          "ts": transaction time
    
        }
      ]
    }
    

> Response:
    
    
    {
        "ch": "market.BTC_NQ.trade.detail",
        "status": "ok",
        "tick": {
            "data": [
                {
                    "amount": "4",
                    "ts": 1604298443540,
                    "id": 1137660004780000,
                    "price": "14117.98",
                    "direction": "sell"
                }
            ],
            "id": 1604298454352,
            "ts": 1604298454352
        },
        "ts": 1604298454352
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
ch | true | string | Data belonged channel，Format：
market.$contract_code.trade.detail |  |  
status | true | string |  |  | "ok","error"  
ts | true | long | Sending time |  |  
<dict> (attrs: tick) |  |  |  |  |  
id | true | long | Unique Order Id(symbol level) |  |  
ts | true | long | Latest Creation Time |  |  
<list> (attrs: data) |  |  |  |  |  
id | true | long | Unique Transaction Id(symbol level) |  |  
price | true | decimal | Price |  |  
amount | true | decimal | Quantity(Cont.) |  |  
direction | true | string | Order Direction |  |  
ts | true | long | Order Creation Time |  |  
</list> |  |  |  |  |  
</dict> |  |  |  |  |  
  
## Query a Batch of Trade Records of a Contract

### Example

  * GET `/market/history/trade`

    
    
    curl "https://api.hbdm.com/market/history/trade?symbol=BTC_CQ&size=100"
    

### Request Parameter

Parameter Name | Mandatory | Data Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Contract Name |  | Case-Insenstive.Both uppercase and
lowercase are supported.. e.g. "BTC_CW" represents BTC “This Week”，"BTC_NW"
represents BTC “Next Week”，"BTC_CQ" represents BTC “Quarter”."BTC_NQ"
represents BTC “Next Quarter”. Contract code is supported to query data. e.g.:
"BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
size | true | int | Number of Trading Records Acquisition | 1 | [1, 2000]  
  
> data Illustration：
    
    
    "data": {
      "id": Unique Order Id(symbol level),
      "ts": Latest transaction time,
      "data": [
        {
          "id": Unique Transaction Id(symbol level),
          "price": transaction price,
          "amount": transaction (amount),
          "direction": active transaction direction
          "ts": transaction time
          }
    }
    

> Response:
    
    
    {
        "ch": "market.BTC_NQ.trade.detail",
        "data": [
            {
                "data": [
                    {
                        "amount": 12,
                        "direction": "buy",
                        "id": 1137660361550000,
                        "price": 14119.84,
                        "ts": 1604298530920
                    }
                ],
                "id": 113766036155,
                "ts": 1604298530920
            },
            {
                "data": [
                    {
                        "amount": 4,
                        "direction": "sell",
                        "id": 1137660376740000,
                        "price": 14123.14,
                        "ts": 1604298531331
                    }
                ],
                "id": 113766037674,
                "ts": 1604298531331
            }
        ],
        "status": "ok",
        "ts": 1604298553734
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
ch | true | string | Data belonged channel，Format：
market.$contract_code.trade.detail |  |  
status | true | string |  |  | "ok","error"  
ts | true | long | Sending time |  |  
<dict> (attrs: tick) |  |  |  |  |  
id | true | long | Unique Order Id(symbol level) |  |  
ts | true | long | Latest Creation Time |  |  
<list> (attrs: data) |  |  |  |  |  
id | true | long | Unique Transaction Id(symbol level) |  |  
price | true | decimal | Price |  |  
amount | true | decimal | Quantity(Cont.) |  |  
direction | true | string | Order Direction |  |  
ts | true | long | Order Creation Time |  |  
</list> |  |  |  |  |  
</dict> |  |  |  |  |  
  
## Query information on contract insurance fund balance and estimated clawback
rate

  * GET `api/v1/contract_risk_info`

    
    
    curl "https://api.hbdm.com/api/v1/contract_risk_info"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | false | string | Contract Type | Case-Insenstive.Both uppercase and
lowercase are supported. "BTC","ETH"...，If no data detected, system will
return to all contracts by default.  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "BTC",
                "insurance_fund": 1909.852579486750035041,
                "estimated_clawback": 0
            }
        ],
        "ts": 1604298633195
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: milesecond |  
<data> |  |  |  |  
symbol | true | string | Contract Code | "BTC","ETH"...  
insurance_fund | true | decimal | Insurance Fund Balance |  
estimated_clawback | true | decimal | Estimated Clawback Rate |  
</data> |  |  |  |  
  
## Query history records of insurance fund balance

  * GET `api/v1/contract_insurance_fund`

    
    
    curl "https://api.hbdm.com/api/v1/contract_insurance_fund?symbol=BTC"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | true | string | Contract Code | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"...  
  
> Response:
    
    
    {
        "status":"ok",
        "data":{
            "symbol":"BTC",
            "tick":[
                {
                    "insurance_fund":1909.852579486750035041,
                    "ts":1604217600000
                },
                {
                    "insurance_fund":1907.646552903264189201,
                    "ts":1604131200000
                }
            ]
        },
        "ts":1604298695848
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: Milesecond |  
<data> |  |  |  | Dictionary Data  
symbol | true | string | Contract Code | "BTC","ETH"...  
<tick> |  |  |  |  
insurance_fund | true | decimal | Insurance Fund Balance |  
ts | true | long | Timestamp, Unit: Milesecond |  
</tick> |  |  |  |  
</data> |  |  |  |  
  
## Query information on Tiered Adjustment Factor

  * GET `api/v1/contract_adjustfactor`

    
    
    curl "https://api.hbdm.com/api/v1/contract_adjustfactor"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Data Value  
---|---|---|---|---  
symbol | false | string | Contract Code | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"...，If no data detected, system will return
to all contracts by default.  
  
> Response:
    
    
    {
        "status":"ok",
        "data":[
            {
                "symbol":"BTC",
                "list":[
                    {
                        "lever_rate":125,
                        "ladders":[
                            {
                                "ladder":0,
                                "min_size":0,
                                "max_size":1999,
                                "adjust_factor":0.65
                            },
                            {
                                "ladder":1,
                                "min_size":2000,
                                "max_size":14999,
                                "adjust_factor":0.8
                            },
                            {
                                "ladder":2,
                                "min_size":15000,
                                "max_size":null,
                                "adjust_factor":0.85
                            }
                        ]
                    }
                ]
            }
        ],
        "ts":1604298785020
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: Milesecond |  
<data> |  |  |  |  
symbol | true | string | Contract Code | "BTC","ETH"...  
<list> |  |  |  |  
lever_rate | true | decimal | Leverage |  
<ladderDetail> |  |  |  |  
min_size | true | decimal | Min net position limit |  
max_size | true | decimal | Max net position limit |  
ladder | true | int | Tier |  
adjust_factor | true | decimal | Adjustment Factor |  
</ladderDetail> |  |  |  |  
</list> |  |  |  |  
</data> |  |  |  |  
  
## Query information on open interest

  * GET `api/v1/contract_his_open_interest`

    
    
    curl "https://api.hbdm.com/api/v1/contract_his_open_interest?symbol=BTC&contract_type=this_week&period=60min&amount_type=1"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Data Range  
---|---|---|---|---  
symbol | true | string | Contract Code | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"...  
contract_type | true | string | Contract Type | Weekly:"this_week", Bi-
weekly:"next_week", Quarterly:"quarter" Next Quarterly Contract:
"next_quarter"  
period | true | string | Period Type | 1 hour:"60min"，4 hours:"4hour"，12
hours:"12hour"，1 day:"1day"  
size | false | int | Request Amount | Default：48，Data Range [1,200]  
amount_type | true | int | Open interest unit | 1:-cont，2:-cryptocurrenty  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "symbol": "BTC",
            "contract_type": "quarter",
            "tick": [
                {
                    "volume": "3058980.0000000000000000",
                    "amount_type": 1,
                    "ts": 1604296800000
                },
                {
                    "volume": "3049899.0000000000000000",
                    "amount_type": 1,
                    "ts": 1604293200000
                }
            ]
        },
        "ts": 1604298943494
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Data Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: Milesecond |  
<data> |  |  | Dictionary Data |  
symbol | true | string | Contract Code | "BTC","ETH"...  
contract_type | true | string | Contract Type | Weekly:"this_week", Bi-
weekly:"next_week", Quarterly:"quarter" Next Quarterly Contract:
"next_quarter"  
<tick> |  |  |  |  
volume | true | string | Open Interest |  
amount_type | true | int | Open Interest Unit | 1:-cont，2:- cryptocurrency  
ts | true | long | Recording Time |  
</tick> |  |  |  |  
</data> |  |  |  |  
  
### Notice

  * tick field：Tick data is arranged in reverse chronological order；

  * data field：Dictionary database.

## Query information on system status

  * GET `api/v1/contract_api_state`

    
    
    curl "https://api.hbdm.com/api/v1/contract_api_state"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | false | string | symbol | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"... If no data detected, system will return
to all symbols by default  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "BTC",
                "open": 1,
                "close": 1,
                "cancel": 1,
                "transfer_in": 1,
                "transfer_out": 1,
                "master_transfer_sub": 1,
                "sub_transfer_master": 1
            }
        ],
        "ts": 1604297099976
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: milesecond |  
<data> |  |  |  |  
symbol | true | string | symbol | "BTC","ETH"...  
open | true | int | open order access：when “1”, then access available; when
“0”, access unavailable"1" |  
close | true | int | close order access：when “1”, then access available; when
“0”, access unavailable "1" |  
cancel | true | int | order cancellation access：when “1”, then access
available; when “0”, access unavailable "1" |  
transfer_in | true | int | deposit access：when “1”, then access available;
when “0”, access unavailable "1" |  
transfer_out | true | int | withdraw access： when “1”, then access available;
when “0”, access unavailable "1" |  
master_transfer_sub | true | int | transfer from master to sub account："1" is
available，“0” is unavailable |  
sub_transfer_master | true | int | transfer from sub to master account："1" is
available，“0” is unavailable |  
</data> |  |  |  |  
  
### Notice

  * “open” is one of the trading access in “API-Open-Ordinary Order”. “On” stands for opening this access; “Off” stands for closing this access；

  * “close” is one of the trading access in “API-Close-Ordinary Order”. “On” stands for opening this access; “Off” stands for closing this access；

  * “cancel” is one of the trading access in “API-Cancel-Ordinary Order”. “On” stands for opening this access; “Off” stands for closing this access；

  * “transfer_in” is one of the trading access in “Others-Transfer-Deposit”. “On” stands for opening this access; “Off” stands for closing this access；

  * transfer_out，”transfer_out” is one of the trading access in “Others-Transfer-Withdraw”. “On” stands for opening this access; “Off” stands for closing this access；

## Query Top Trader Sentiment Index Function-Account

  * GET `api/v1/contract_elite_account_ratio`

    
    
    curl "https://api.hbdm.com/api/v1/contract_elite_account_ratio?symbol=BTC&period=60min"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | true | string | symbol | Case-Insenstive.Both uppercase and lowercase
are supported."BTC","ETH"...  
period | true | string | period | 5min, 15min, 30min, 60min,4hour,1day  
  
> Response:
    
    
    {
        "status":"ok",
        "data":{
            "list":[
                {
                    "buy_ratio":0.52,
                    "sell_ratio":0.45,
                    "locked_ratio":0.03,
                    "ts":1604290200000
                }
            ],
            "symbol":"BTC"
        },
        "ts":1604299070097
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Vaue Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: Milesecond |  
<data> |  |  |  |  
symbol | true | string | symbol | "BTC","ETH"...  
<list> |  |  |  |  
buy_ratio | true | decimal | net long accounts ratio |  
sell_ratio | true | decimal | net short accounts ratio |  
locked_ratio | true | decimal | locked accounts ratio |  
ts | true | long | Time of Respond Generation |  
</list> |  |  |  |  
</data> |  |  |  |  
  
## Query Top Trader Sentiment Index Function-Position

  * GET `api/v1/contract_elite_position_ratio`

    
    
    curl "https://api.hbdm.com/api/v1/contract_elite_position_ratio?symbol=BTC&period=60min"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | true | string | symbol | Case-Insenstive.Both uppercase and lowercase
are supported."BTC","ETH"...  
period | true | string | period | 5min, 15min, 30min, 60min,4hour,1day  
  
> Response:
    
    
    {
        "status":"ok",
        "data":{
            "list":[
                {
                    "buy_ratio":0.51,
                    "sell_ratio":0.49,
                    "ts":1604290500000
                },
                {
                    "buy_ratio":0.508,
                    "sell_ratio":0.492,
                    "ts":1604290800000
                }
            ],
            "symbol":"BTC"
        },
        "ts":1604299402211
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: Milesecond |  
<data> |  |  |  |  
symbol | true | string | symbol | "BTC","ETH"...  
<list> |  |  |  |  
buy_ratio | true | decimal | Net long position ratio |  
sell_ratio | true | decimal | Net short position ratio |  
ts | true | long | Time of Respond Generation |  
</list> |  |  |  |  
</data> |  |  |  |  
  
## Query Liquidation Order Information

  * GET `api/v1/contract_liquidation_orders`

    
    
    curl "https://api.hbdm.com/api/v1/contract_liquidation_orders?symbol=BTC&trade_type=0&create_date=7"
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | symbol |  | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"...  
trade_type | true | int | trading types |  | when “0”, request fully filled
liquidated orders; when “5’, request liquidated close orders; when “6”,
request liquidated open orders  
create_date | true | int | date |  | 7，90（ 7 days or 90 days）  
page_index | false | int | page, system sets page 1 by default without further
instruction |  |  
page_size | false | int | system sets page 20 by default without further
instruction. Max page size is 50. |  |  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "contract_code": "BTC201225",
                    "symbol": "BTC",
                    "direction": "buy",
                    "offset": "close",
                    "volume": 26,
                    "price": 19674.96,
                    "created_at": 1606293144641,
                    "amount": 0.132147663832607537
                }
            ],
            "total_page": 114,
            "current_page": 1,
            "total_size": 2264
        },
        "ts": 1604299610722
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result |  
<object>(object name: data) |  |  |  |  
<list>( object name: orders) |  |  |  |  
symbol | true | string | symbol |  
contract_code | true | string | contract code | "BTC180914" ...  
direction | true | string | "buy":buy"sell": sell |  
offset | true | string | "open":open "close": close |  
volume | true | decimal | liquidated volume(cont) |  
amount | true | decimal | liquidation amount (token) |  
price | true | decimal | bankruptcy price |  
created_at | true | long | liquidation time |  
</list> |  |  |  |  
total_page | true | int | total page |  
current_page | true | int | current page |  
total_size | true | int | total size |  
</object> |  |  |  |  
ts | true | long | timestamp |  
  
## Query historical settlement records of the platform interface

  * GET `/api/v1/contract_settlement_records`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | true | string | Token Code | "BTC","ETH"...  
start_time | false | long | Start time（timestamp，unit: millisecond） | Value
range: [(Current time minus 90 days), Current time] ，default current time
minus 90 days  
end_time | false | long | End time（timestamp，unit: millisecond） | Value range:
(start_time, current time]，default current time  
page_index | false | int | Page, default page 1 if not filled |  
page_size | false | int | Page items, default 20, shall not exceed 50 | [1-50]  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "total_page": 13,
            "current_page": 1,
            "total_size": 13,
            "settlement_record": [
                {
                    "symbol": "BTC",
                    "settlement_time": 1605859200000,
                    "clawback_ratio": 0,
                    "list": [
                        {
                            "contract_code": "BTC201120",
                            "settlement_price": 18217.62,
                            "settlement_type": "delivery"
                        },
                        {
                            "contract_code": "BTC201127",
                            "settlement_price": 18292.24,
                            "settlement_type": "settlement"
                        },
                        {
                            "contract_code": "BTC201225",
                            "settlement_price": 18490.42,
                            "settlement_type": "settlement"
                        },
                        {
                            "contract_code": "BTC210326",
                            "settlement_price": 18788.7,
                            "settlement_type": "settlement"
                        }
                    ]
                }
            ]
        },
        "ts": 1606295834648
    }
    
    

### Return Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Response generation time point, unit: millisecond |  
<data> | true | object array |  |  
<settlement_record> | true | object array |  |  
symbol | true | string | Token Code |  
settlement_time | true | long | Settlement Time（timestamp，unit:
millisecond）（when the settlement_type is delivery, the time is delivery time;
when the settlement_type is settlement, the time is settlement time） |  
clawback_ratio | true | decimal | Clawback Ratio |  
<list> | true | object array |  |  
contract_code | true | string | Contract Code | "BTC180914" ...  
settlement_price | true | decimal | Settlement Price（when the settlement_type
is delivery, the price is delivery price; when the settlement_type is
settlement, the price is settlement price；） |  
settlement_type | true | string | Settlement Type |
“delivery”：Delivery，“settlement”：Settlement  
</list> |  |  |  |  
</settlement_record> |  |  |  |  
total_page | true | int | Total Pages |  
current_page | true | int | Current Page |  
total_size | true | int | Total page items |  
</data> |  |  |  |  
  
## Query Index Kline Data

### example

  * GET `/index/market/history/index`

    
    
    curl "https://api.hbdm.com/index/market/history/index?symbol=BTC-USD&period=1min&size=150"
    

### request parameters

**Parameter Name** | **Mandatory** | **Type** | **Desc** | **Default** |
**Value Range**  
---|---|---|---|---|---  
symbol | true | string | index symbol |  | Case-Insenstive.Both uppercase and
lowercase are supported..e.g."BTC-USD","ETH-USD"...  
period | true | string | kline type |  | 1min, 5min, 15min, 30min,
60min,4hour,1day, 1mon  
size | true | integer | data size | 150 | [1,2000]  
  
> Response Example：
    
    
    {
        "ch": "market.BTC-USD.index.60min",
        "data": [
            {
                "amount": 0,
                "close": 13703.4175,
                "count": 0,
                "high": 13720.84,
                "id": 1604293200,
                "low": 13658.245,
                "open": 13709.6175,
                "vol": 0
            },
            {
                "amount": 0,
                "close": 13751.6,
                "count": 0,
                "high": 13771.21,
                "id": 1604296800,
                "low": 13693.16,
                "open": 13703.365,
                "vol": 0
            }
        ],
        "status": "ok",
        "ts": 1604299755097
    }
    

### response parameters：

**Parameter Name** | **Mandatory** | **Type** | **Desc** | **Default** |
**Value Range**  
---|---|---|---|---|---  
ch | true | string | data channel |  | eg： market.period  
<data> |  |  | object |  |  
id | true | decimal | index kline id,the same as kline timestamp, kline start
timestamp |  |  
vol | true | decimal | Trade Volume(Cont.) The value is 0 |  |  
count | true | decimal | Order Quantity The value is 0 |  |  
open | true | decimal | Opening Index Price |  |  
close | true | decimal | Closing Index Price, the price in the last kline is
the latest order price |  |  
low | true | decimal | Lowest Index Price |  |  
high | true | decimal | Highest Index Price |  |  
amount | true | decimal | Trade Amount(Coin), The value is 0. ) |  |  
</data> |  |  |  |  |  
status | true | string | process status |  | "ok" , "error"  
ts | true | long | timestamp of the response of the server |  |
unit：millionseconds  
  
## Query Basis Data

### example

  * GET `/index/market/history/basis`

    
    
    curl "https://api.hbdm.com/index/market/history/basis?symbol=BTC-USD&period=1min&size=150&basis_price_type=open"
    

### request parameters

**Parameter name** | **Mandatory** | **Type** | **Desc** | **Default** |
**Value Range**  
---|---|---|---|---|---  
symbol | true | string | symbol name |  | Case-Insenstive.Both uppercase and
lowercase are supported..e.g. "BTC_CW" represents BTC “This Week”，"BTC_NW"
represents BTC “Next Week”，"BTC_CQ" represents BTC “Quarter”."BTC_NQ"
represents BTC “Next Quarter”.  
period | true | string | kline period |  | 1min,5min, 15min, 30min,
60min,4hour,1day,1mon  
basis_price_type | false | string | use basis price type to calculate the
basis data | Using open price default | open price："open"，close
price："close"，highest price："high"，lowest price："low"，avg=（high price +low
price）/2："average"  
size | true | integer | data size | 150 | [1,2000]  
  
> Response example：
    
    
    {
        "ch": "market.BTC-USD.basis.5min.open",
        "data": [
            {
                "basis": "-2.1850000000013097",
                "basis_rate": "-0.00015880531885174013",
                "contract_price": "13756.8",
                "id": 1604299500,
                "index_price": "13758.985"
            },
            {
                "basis": "-4.235000000000582",
                "basis_rate": "-0.00030799697602973224",
                "contract_price": "13745.9",
                "id": 1604299800,
                "index_price": "13750.135"
            }
        ],
        "status": "ok",
        "ts": 1604299816352
    }
    

### response parameters

**parameter name** | **Mandatory** | **Type** | **Desc** | **Value Range**  
---|---|---|---|---  
ch | true | string | theme |  
status | true | string | status |  
<data> | true | object |  |  
id | true | long | unique id |  
contract_price | true | string | contract last price |  
index_price | true | string | index price |  
basis | true | string | basis=contract_price - index_price |  
basis_rate | true | string | basis_rate=basis/index_price |  
</data> |  |  |  |  
ts | true | long | the timestamp of generation |  
  
  * Note：

2000 size at most per request ；

The basis data of Next Quarterly Contract is available after 2020/6/15
14:00:00.

# Future Account Interface

## Query User’s Account Information

### Example

  * POST `api/v1/contract_account_info`  

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | false | string | Variety code |  | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"...if default, return to all types
defaulted  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "margin_balance": 453.151955780787465997,
                "margin_position": 0,
                "margin_frozen": 0,
                "margin_available": 453.151955780787465997,
                "profit_real": 16.35635155751274032,
                "profit_unreal": 0,
                "risk_rate": null,
                "withdraw_available": 436.795604223274725677,
                "liquidation_price": null,
                "lever_rate": 10,
                "adjust_factor": 0.2,
                "margin_static": 453.151955780787465997,
                "is_debit": 0
            }
        ],
        "ts": 1604300060777
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<list>(Attribute Name: data) |  |  |  |  
symbol | true | string | Variety code | "BTC","ETH"...  
margin_balance | true | decimal | Account rights |  
margin_position | true | decimal | Position Margin |  
margin_frozen | true | decimal | Freeze margin |  
margin_available | true | decimal | Available margin |  
profit_real | true | decimal | Realized profit |  
profit_unreal | true | decimal | Unrealized profit |  
risk_rate | true | decimal | risk rate |  
liquidation_price | true | decimal | Estimated liquidation price |  
withdraw_available | true | decimal | Available withdrawal |  
lever_rate | true | decimal | Leverage Rate |  
adjust_factor | true | decimal | Adjustment Factor |  
margin_static | true | decimal | Static Margin |  
</list> |  |  |  |  
ts | long | long | Time of Respond Generation, Unit: Millisecond |  
  
## Query User’s Position Information

### Example

  * POST `api/v1/contract_position_info`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | false | string | Variety code |  | Case-Insenstive.Both uppercase and
lowercase are supported. "BTC","ETH"...if default, return to all types
defaulted  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "contract_code": "ADA201225",
                "contract_type": "quarter",
                "volume": 1,
                "available": 1,
                "frozen": 0,
                "cost_open": 0.0991,
                "cost_hold": 0.0991,
                "profit_unreal": 0,
                "profit_rate": 0,
                "lever_rate": 10,
                "position_margin": 10.090817356205852674,
                "direction": "sell",
                "profit": 0,
                "last_price": 0.0991
            }
        ],
        "ts": 1604301441639
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<list>(Attribute Name: data) |  |  |  |  
symbol | true | string | Variety code | "BTC","ETH"...  
contract_code | true | string | Contract Code | "BTC180914" ...  
contract_type | true | string | Contract Type | "this_week", "next_week",
"quarter", "next_quarter"  
volume | true | decimal | Position quantity |  
available | true | decimal | Available position can be closed |  
frozen | true | decimal | frozen |  
cost_open | true | decimal | Opening average price |  
cost_hold | true | decimal | Average price of position |  
profit_unreal | true | decimal | Unrealized profit and loss |  
profit_rate | true | decimal | Profit rate |  
profit | true | decimal | profit |  
position_margin | true | decimal | Position margin |  
lever_rate | true | int | Leverage rate |  
direction | true | string | Transaction direction |  
last_price | true | decimal | Latest price |  
</list> |  |  |  |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
#### Note

  * If there are symbols in the settlement or delivery period,error code 1080(1080 In settlement or delivery. Unable to get positions of some contracts. ) will return without request parameters. It's suggested to query the position info with request parameters to avoid raising the error code and not being able to query the position.

## Query assets information of all sub-accounts under the master account

  * POST `api/v1/contract_sub_account_list`

### Request Parameters

**Parameter name** | **Must fill or not** | **Type** | **Description** |
**Default value** | **Value range**  
---|---|---|---|---|---  
symbol | false | string | type code |  | Case-Insenstive.Both uppercase and
lowercase are supported. "BTC","ETH"... ,if blank, it will return all contract
types by default  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "sub_uid": 123456789,
                "list": [
                    {
                        "symbol": "ADA",
                        "margin_balance": 50,
                        "liquidation_price": null,
                        "risk_rate": null
                    }
                ]
            }
        ],
        "ts": 1604301647427
    }
    

### Return parameters

**Parameter name** | **Must fill or not** | **Type** | **Description** |
**Value range**  
---|---|---|---|---  
status | true | string | the handling result of requests | "ok" , "error"  
ts | true | long | the create time point of response, unit: ms |  
<data> |  |  |  |  
sub_uid | true | long | sub-account UID |  
<list> |  |  |  |  
symbol | true | string | type code | "BTC","ETH"...  
margin_balance | true | decimal | account equity |  
liquidation_price | true | decimal | estimated liquidation price |  
risk_rate | true | decimal | margin rate |  
</list> |  |  |  |  
</data> |  |  |  |  
  
  * Notice

Only return data for activated contract sub-account (i.e. sub-accounts that
have gained contract trading permission).

## Query a single sub-account's assets information

  * POST `api/v1/contract_sub_account_info`

### Request Parameters

**Parameter name** | **Must fill or not** | **Type** | **Description** |
**Default value** | **Value range**  
---|---|---|---|---|---  
symbol | false | string | type code | Case-Insenstive.Both uppercase and
lowercase are supported. "BTC","ETH"...，if blank, it will return all contract
types by default |  
sub_uid | true | long | sub-account UID |  |  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "margin_balance": 50,
                "margin_position": 0,
                "margin_frozen": 0,
                "margin_available": 50,
                "profit_real": 0,
                "profit_unreal": 0,
                "risk_rate": null,
                "withdraw_available": 50,
                "liquidation_price": null,
                "lever_rate": 5,
                "adjust_factor": 0.1,
                "margin_static": 50,
                "is_debit": 0
            }
        ],
        "ts": 1604301730723
    }
    

### Return parameters

**Parameter name** | **Must fill or not** | **Type** | **Description** |
**Value range**  
---|---|---|---|---  
status | true | string | the handling result of requests | "ok" , "error"  
ts | true | long | the create time point of response, unit: ms |  
<data> |  |  |  |  
symbol | true | string | type code | "BTC","ETH"...when the$symbol value is
"*", it will subscribe all contract types  
margin_balance | true | decimal | account equity |  
margin_position | true | decimal | position margin (the margin used by current
positions) |  
margin_frozen | true | decimal | frozen margin |  
margin_available | true | decimal | available margin |  
profit_real | true | decimal | realized profits and losses |  
profit_unreal | true | decimal | unrealized profits and losses |  
risk_rate | true | decimal | margin rate |  
liquidation_price | true | decimal | estimated liquidation price |  
withdraw_available | true | decimal | available transfer amount |  
lever_rate | true | decimal | leverage ratios |  
adjust_factor | true | decimal | Adjustment Factor |  
margin_static | true | decimal | Static Margin |  
</data> |  |  |  |  
  
  * Notice

Only query account information for activated contract sub-account (i.e. sub-
accounts that have gained contract trading permission);

No data return for sub-accounts which has logged in hbdm but have not gained
trading permission/activated.

## Query a single sub-account's position information

  * POST `api/v1/contract_sub_position_info`

### Request Parameters

**Parameter name** | **Must fill or not** | **Type** | **Description** |
**Default value** | **Value range**  
---|---|---|---|---|---  
symbol | false | string | type code | Case-Insenstive.Both uppercase and
lowercase are supported. "BTC","ETH"...，if blank, it will return all contract
types by default |  
sub_uid | true | long | sub-account UID |  |  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "contract_code": "ADA201225",
                "contract_type": "quarter",
                "volume": 1,
                "available": 1,
                "frozen": 0,
                "cost_open": 0.0991,
                "cost_hold": 0.0991,
                "profit_unreal": -0.04686106551835051,
                "profit_rate": -0.002321965796434265,
                "lever_rate": 5,
                "position_margin": 20.191006925515375451,
                "direction": "buy",
                "profit": -0.04686106551835051,
                "last_price": 0.099054
            }
        ],
        "ts": 1604302891178
    }
    

### Return parameters

**Parameter name** | **Must fill or not** | **Type** | **Description** |
**Value range**  
---|---|---|---|---  
status | true | string | the handling result of requests | "ok" , "error"  
ts | true | long | the create time point of response, unit: ms |  
<data> |  |  |  |  
symbol | true | string | type code | "BTC","ETH"...  
contract_code | true | string | contract code | "BTC180914" ...  
contract_type | true | string | contract type | Weekly:"this_week",
Biweekly:"next_week", Quarterly:"quarter", Next Quarterly Contract:
"next_quarter"  
volume | true | decimal | open interest |  
available | true | decimal | available positions to close |  
frozen | true | decimal | amount of frozen positions |  
cost_open | true | decimal | average price of open positions |  
cost_hold | true | decimal | average price of positions |  
profit_unreal | true | decimal | unrealized profits and losses |  
profit_rate | true | decimal | profit rate |  
profit | true | decimal | profits |  
position_margin | true | decimal | position margin |  
lever_rate | true | int | leverage ratios |  
direction | true | string | transaction direction of positions | "buy":long
"sell":short  
last_price | true | decimal | Latest price |  
</data> |  |  |  |  
  
## Query account financial records

  * POST `api/v1/contract_financial_record`

### Request Parameters

**Parameter name** | **Must fill or not** | **Type** | **Description** |
**Value range**  
---|---|---|---|---  
symbol | true | string | contract type code | Case-Insenstive.Both uppercase
and lowercase are supported.e.g. "BTC","ETH"...  
type | false | string | if not fill this parameter, it will query all types
【please use "," to seperate multiple types】 | 3:close long; 4:close short;
5:fees for open positions-taker; 6:fees for open positions-maker; 7:fees for
close positions-taker; 8:fees for close positions-maker; 9:close long for
delivery; 10:close short for delivery; 11:delivery fee; 12:close long for
liquidation; 13:lose short for liquidation; 14:transfer from spot exchange to
contract exchange; 15:tranfer from contract exchange to spot exchange;
16:settle unrealized PnL-long positions; 17:settle unrealized PnL-short
positions; 19:clawback; 26:system; 28:activity prize rewards; 29:rebate;
34:transfer to sub; 35:transfer from sub; 36:transfer to master; 37:transfer
from master;  
create_date | false | int | any positive integer available. Requesting data
beyond 90 will not be supported, otherwise, system will return trigger history
data within the last 90 days by default. |  
page_index | false | int | which page, default value is "1st page" when not
fill this parameter |  
page_size | false | int | the default value is "20" when not fill this
parameter, should ≤50 |  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "total_page": 15,
            "current_page": 1,
            "total_size": 15,
            "financial_record": [
                {
                    "id": 3662498355,
                    "symbol": "ADA",
                    "type": 8,
                    "amount": -0.074766355140186915,
                    "ts": 1605014144415,
                    "contract_code": "ADA201225"
                }
            ]
        },
        "ts": 1604306015124
    }  
    

### Return parameters

**Parameter name** | **Must fill or not** | **Type** | **Description** |
**Value range**  
---|---|---|---|---  
status | true  | string | processing result of requests  | "ok" , "error"  
ts | true | long | response create time point，unit：ms |  
<data> |  |  | dicitionary type |  
<financial_record> |  |  |  |  
id | true | long |  |  
ts | true | long | create time |  
symbol | true | string | contract type code | "BTC","ETH"...  
type | true | int | transaction type | 3:close long; 4:close short; 5:fees for
open positions-taker; 6:fees for open positions-maker; 7:fees for close
positions-taker; 8:fees for close positions-maker; 9:close long for delivery;
10:close short for delivery; 11:delivery fee; 12:close long for liquidation;
13:lose short for liquidation; 14:transfer from spot exchange to contract
exchange; 15:tranfer from contract exchange to spot exchange; 16:settle
unrealized PnL-long positions; 17:settle unrealized PnL-short positions;
19:clawback; 26:system; 28:activity prize rewards; 29:rebate; 34:transfer to
sub; 35:transfer from sub; 36:transfer to master; 37:transfer from master;  
amount | true | decimal | amount |  
contract_code | true | string | contract code |  
</financial_record> |  |  |  |  
total_page | true | int | total page |  
current_page | true | int | current page |  
total_size | true | int | total size |  
</data> |  |  |  |  
  
## Query financial records via multiple fields

  * POST `api/v1/contract_financial_record_exact`

### Request Parameter

Parameter name | Mandatory | Type | Description | Value range  
---|---|---|---|---  
symbol | true | string | contract symbol | "BTC","ETH"...  
type | false | string | if not fill this parameter, it will query all types
【please use "," to seperate multiple types】 | 3:close long; 4:close short;
5:fees for open positions-taker; 6:fees for open positions-maker; 7:fees for
close positions-taker; 8:fees for close positions-maker; 9:close long for
delivery; 10:close short for delivery; 11:delivery fee; 12:close long for
liquidation; 13:lose short for liquidation; 14:transfer from spot exchange to
contract exchange; 15:tranfer from contract exchange to spot exchange;
16:settle unrealized PnL-long positions; 17:settle unrealized PnL-short
positions; 19:clawback; 26:system; 28:activity prize rewards; 29:rebate;
34:transfer to sub; 35:transfer from sub; 36:transfer to master; 37:transfer
from master;  
start_time | false | long | Start Time（Timestamp，Unit: Millisecond） | See Note  
end_time | false | long | End Time（Timestamp，Unit: Millisecond） | See Note  
from_id | false | long | Query start id（uses id of returned data） |  
size | false | int | number of data | it will be the default value of 20; the
number should ≤50  
direct | false | string | Query direction | prev ；next ；default value:prev  
  
#### Note:

  * Value range description of start_time and end_time: 
    * start_time: value range is [(current time - 90 days)，current time] ；default value is clamp（end_time - 10 days，current time -90 days，current time -10 days）which means the furthest time is the current time minus 90 days and the most recent time is current time minus 10 days.
    * end_time: value range is [(current day - 90 days)，above++)，if the end_time is greater than the current time, use current time; if start_time is filled，the end_time shall be greater than start_time. The system will use current time by default. 
  * if from_id is not filled and the query direction is prev, query from back to front from the end time; if from_id is not filled and the query direction is next, query from front to back from the start time. Query financial records with creation time greater than or equal to the start time but less than or equal to the end time. 
  * Regardless of whether the query direction is prev or next, the data returned is in reverse order of creation time. 
  * If the value of start_time or end_time filled in is not within the value range, the system will report that the parameter is invalid. 
  * Only data within 90 days are available to query.

#### Query cases are as below (special cases are not included)：

start_time | end_time | from_id | size | direct | Query Result  
---|---|---|---|---|---  
Default 10 days before the current time | Default current time | Default | 20
| prev | Query the data within the last 10 days; query 20 data from back to
front from the current time. The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
Default 60 days before the current time | 50 days before the current time |
Default | 20 | prev | Query data between 60 days ago and 50 days ago; query 20
data from back to front from 50 days ago. The data returned is in reverse
order based on creation time. The newer the data, the closer to the front.  
5 days before the current time | Default current time | Default | 20 | prev |
Query the data within the last 5 days; query 20 data from back to front from
the current time. The data returned is in reverse order based on creation
time. The newer the data, the closer to the front.  
20 days before the current time | 10 days before the current time | Default |
20 | prev | Query data between 20 days ago and 10 days ago; query 20 data from
back to front from 10 days ago.The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
Default 10 days before the current time | Default current time | Default | 20
| next | Query the data within the last 10 days; query 20 data from front to
back from 10 days ago. The data returned is in reverse order based on creation
time. The newer the data, the closer to the front.  
Default 60 days before the current time | 50 days before the current time |
Default | 20 | next | Query data between 60 days ago and 50 days ago, query 20
data from front to back from 60 days ago. The data returned is in reverse
order based on creation time. The newer the data, the closer to the front.  
5 days before the current time | Default current time | Default | 20 | next |
Query the data within the last 5 days; query 20 data from 5 days ago. query 20
data from front to back from 5 days ago. The data returned is in reverse order
based on creation time. The newer the data, the closer to the front.  
20 days before the current time | 10 days before the current time | Default |
20 | next | Query data between 20 days ago and 10 days ago; query 20 data from
front to back from 20 days ago. The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
Default 10 days before the current time | Default current time | 1000 | 20 |
prev | Query the data within the last 10 days; query 20 data from back to
front from the data with transaction id 1000 and the data with transaction id
1000 is in the first line. The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
20 days before the current time | 10 days before the current time | 1000 | 20
| next | Query data between 20 days ago and 10 days ago, query 20 data from
front to back from the data with transaction id 1000 and the data with
transaction id 1000 is in the last line. The data returned is in reverse order
based on creation time. The newer the data, the closer to the front.  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "financial_record": [
                {
                    "id": 3657420903,
                    "symbol": "ADA",
                    "type": 34,
                    "amount": -50,
                    "ts": 1604301623306,
                    "contract_code": "ADA"
                },
                {
                    "id": 3657420101,
                    "symbol": "ADA",
                    "type": 6,
                    "amount": -0.020181634712411705,
                    "ts": 1604301416067,
                    "contract_code": "ADA201225"
                }
            ],
            "remain_size": 22,
            "next_id": 3657309434
        },
        "ts": 1604305081144
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Description | Value Range  
---|---|---|---|---  
status  | true  | string | request handling result  | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
<data> | true | object | dicitionary type |  
<financial_record> | true | object array |  |  
id | true | long |  |  
ts | true | long | create time |  
symbol | true | string | Type Code | "BTC","ETH"...  
contract_code | true | string | Contract Code | "BTC200919"...  
type | true | int | order type | 3:close long; 4:close short; 5:fees for open
positions-taker; 6:fees for open positions-maker; 7:fees for close positions-
taker; 8:fees for close positions-maker; 9:close long for delivery; 10:close
short for delivery; 11:delivery fee; 12:close long for liquidation; 13:lose
short for liquidation; 14:transfer from spot exchange to contract exchange;
15:tranfer from contract exchange to spot exchange; 16:settle unrealized PnL-
long positions; 17:settle unrealized PnL-short positions; 19:clawback;
26:system; 28:activity prize rewards; 29:rebate; 34:transfer to sub;
35:transfer from sub; 36:transfer to master; 37:transfer from master;  
amount | true | decimal | amount |  
</financial_record> |  |  |  |  
remain_size | true | int | Remaining data number（the number of data that has
not been queried due to the limitation of data number in the time range） |  
next_id | true | long | id for next data (only has value when query result
exceeds data number limits） |  
</data> |  |  |  |  
  
#### Note:

  * if the query result exceeds the data limit, next_id is the id of next data. ( when the query direction is prev, next_id presents the first data on the next page; when the query direction is next, next_id presents the last data on the next page.)

## Query user’s settlement records

  * POST `api/v1/contract_user_settlement_records`

### Request Parameter

Parameter Name | Mandatory | Type | Description | Value Range  
---|---|---|---|---  
symbol | true | string | contract symbol | "BTC","ETH"...  
start_time | false | long | start time（Timestamp，Unit: Millisecond） | Value
Range: [(current time - 90 days), current time] ，default current day - 90 days  
end_time | false | long | end time（Timestamp，Unit: Millisecond） | Value Range:
(start_time, current time]，default current time  
page_index | false | int | Page | 1st page by default without given
instruction  
page_size | false | int | page size | Page 20 by default without given
instruction, ，no more than 50  
  
#### Note:

  * The data is queried in reverse order by default; the newer the data, the closer to the front.
  * If the start time or the end time is not within the value range, the system will report an error 1067 to indicate the parameter is invalid.  

  * Query users' settlement records with settlement start time behind the start_time but before the end_time. 

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "total_page": 13,
            "current_page": 1,
            "total_size": 13,
            "settlement_records": [
                {
                    "symbol": "ADA",
                    "margin_balance_init": 436.415907066107795161,
                    "margin_balance": 436.795604223274725677,
                    "settlement_profit_real": 0.379697157166930517,
                    "settlement_time": 1604044800130,
                    "clawback": 0,
                    "delivery_fee": 0,
                    "offset_profitloss": 13.25977319159553892,
                    "fee": -0.565357129977092573,
                    "fee_asset": "ADA",
                    "positions": [
                        {
                            "symbol": "ADA",
                            "contract_code": "ADA201225",
                            "direction": "buy",
                            "volume": 2,
                            "cost_open": 0.098,
                            "cost_hold_pre": 0.098,
                            "cost_hold": 0.092423,
                            "settlement_profit_unreal": -12.31471890445151583,
                            "settlement_price": 0.092423,
                            "settlement_type": "settlement"
                        }
                    ]
                }
            ]
        },
        "ts": 1604305358564
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Description | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result |  
<data> | true | object |  |  
<settlement_records> | true | object array |  |  
symbol | true | string | Contract Code | "BTC","ETH"...  
margin_balance_init | true | decimal | Initial account equity for this term |  
margin_balance | true | decimal | Account equity after settlement for this
term |  
settlement_profit_real | true | decimal | Realized PnL for this term |  
settlement_time | true | long | Settlement time for this term; delivery time
if at the delivery. |  
clawback | true | decimal | Clawback for this term |  
delivery_fee | true | decimal | Delivery fee for this term（total fee of long
and short positions）, the field has value only when the positions are at the
delivery |  
offset_profitloss | true | decimal | Current term PnL of positions closed |  
fee | true | decimal | Transaction fee for this term |  
fee_asset | true | string | Transaction Fee Coin |  
<positions> | true | object array |  |  
symbol | true | string | Coin Code | "BTC","ETH"...  
contract_code | true | string | Contract Code | "BTC200619" ...  
direction | true | string | Position Direction | [buy : sell ]  
volume | true | decimal | Position volume before the settlement of this
term（cont） |  
cost_open | true | decimal | Open price |  
cost_hold_pre | true | decimal | Average position price before the settlement
of this term |  
cost_hold | true | decimal | Average position price after the settlement of
this term |  
settlement_profit_unreal | true | decimal | Unrealized PnL for this term |  
settlement_price | true | decimal | Settlement price for this term; delivery
price if at the delivery. |  
settlement_type | true | string | Settlement Type | settlement:
settlement；delivery: delivery；  
</positions> |  |  |  |  
</settlement_records> |  |  |  |  
total_page | true | int | Total Pages |  
current_page | true | int | Current Page |  
total_size | true | int | Total Size |  
</data> |  |  |  |  
ts | true | long | Timestamp |  
  
#### Rule:

  * settlement_time for this term is the start time of the settlement.
  * As long as the user has had funds, there will be settlement records. If the user queried has no settlement record, no data will be returned. (data will be an empty array)

## Query contract information on order limit

  * POST `api/v1/contract_order_limit`

### Request Parameter

Parameter Name | Mandatory | Type | Description | Value Range  
---|---|---|---|---  
symbol | false | string | contract code | Case-Insenstive.Both uppercase and
lowercase are supported. "BTC","ETH"...，If no data detected, system will
return to all contracts by default  
order_price_type | true | string | Order Type | "limit": Limit
Order，"opponent":BBO，"lightning": Flash Close，"optimal_5": Optimal top 5
price，"optimal_10":Optimal top 10 price，"optimal_20":Optimal top 20
price,"fok":FOK order,"ioc":ioc order,"opponent_ioc"：IOC order using the BBO
price，"lightning_ioc"：lightning IOC，"optimal_5_ioc"：optimal_5
IOC，"optimal_10_ioc"：optimal_10 IOC， "optimal_20_ioc"：optimal_20 IOC,
"opponent_fok"：FOK order using the BBO price，"lightning_fok"：lightning
FOK，"optimal_5_fok"：optimal_5 FOK，"optimal_10_fok"：optimal_10
FOK，"optimal_20_fok"：optimal_20 FOK  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "order_price_type": "limit",
            "list": [
                {
                    "symbol": "ADA",
                    "types": [
                        {
                            "contract_type": "this_week",
                            "open_limit": 6000,
                            "close_limit": 12000
                        },
                        {
                            "contract_type": "next_week",
                            "open_limit": 6000,
                            "close_limit": 12000
                        },
                        {
                            "contract_type": "quarter",
                            "open_limit": 6000,
                            "close_limit": 12000
                        },
                        {
                            "contract_type": "next_quarter",
                            "open_limit": 6000,
                            "close_limit": 12000
                        }
                    ]
                }
            ]
        },
        "ts": 1604306946036
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range Í  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
<data> |  |  |  |  
order_price_type | true | string | Order Type | "limit": Limit
Order，"opponent":BBO，"lightning": Flash Close，"optimal_5": Optimal top 5
price，"optimal_10":Optimal top 10 price，"optimal_20":Optimal top 20
price,"fok":FOK order,"ioc":ioc order  
<list> |  |  |  |  
symbol | true | string | Contract Code | "BTC","ETH"...  
<types> |  |  |  |  
contract_type | true | string | Contract Type | Weekly:"this_week", Bi-
weekly:"next_week", Quarterly:"quarter". Next Quarterly Contract:
"next_quarter"  
open_limit | true | long | Max open order limit |  
close_limit | true | long | Max close order limit |  
</types> |  |  |  |  
</list> |  |  |  |  
</data> |  |  |  |  
  
## Query information on contract trading fee

  * POST `api/v1/contract_fee`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | false | string | Contract Code | Case-Insenstive.Both uppercase and
lowercase are supported. "BTC","ETH"...，If no data detected, system will
return to all contract by default  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "open_maker_fee": "0.0002",
                "open_taker_fee": "0.0004",
                "close_maker_fee": "0.0002",
                "close_taker_fee": "0.0004",
                "delivery_fee": "0.0005",
                "fee_asset": "ADA"
            }
        ],
        "ts": 1604307012954
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
<data> |  |  |  |  
symbol | true | string | Contract Code | "BTC","ETH"...  
open_maker_fee | true | string | Open maker order fee, decimal |  
open_taker_fee | true | string | Open taker order fee, decimal |  
close_maker_fee | true | string | Close maker order fee, decimal |  
close_taker_fee | true | string | Close taker order fee, decimal |  
delivery_fee | true | string | delivery fee, decimal |  
fee_asset | true | string | the corresponding cryptocurrency to the given fee
| "BTC","ETH"...  
</data> |  |  |  |  
  
## Query information on Transfer Limit

  * POST `api/v1/contract_transfer_limit`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | false | string | Contract Code | Case-Insenstive.Both uppercase and
lowercase are supported. "BTC","ETH"...，If no data detected, system will
return to all contracts by default.  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "transfer_in_max_each": 1500000000,
                "transfer_in_min_each": 16,
                "transfer_out_max_each": 150000000,
                "transfer_out_min_each": 0.000001,
                "transfer_in_max_daily": 15000000000,
                "transfer_out_max_daily": 3000000000,
                "net_transfer_in_max_daily": 7500000000,
                "net_transfer_out_max_daily": 1500000000
            }
        ],
        "ts": 1604307084954
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Respond Generation, Unit: Milesecond |  
<data> |  |  |  |  
symbol | true | string | Contract Code | "BTC","ETH"...  
transfer_in_max_each | true | decimal | Max limit of a single deposit |  
transfer_in_min_each | true | decimal | Min limit of a single deposit |  
transfer_out_max_each | true | decimal | Max limit of a single withdrawal |  
transfer_out_min_each | true | decimal | Min limit of a single withdrawal |  
transfer_in_max_daily | true | decimal | Max daily limit of total deposits |  
transfer_out_max_daily | true | decimal | Max daily limit of totally
withdrawals |  
net_transfer_in_max_daily | true | decimal | Max daily limit of net total
deposits |  
net_transfer_out_max_daily | true | decimal | Max daily limit of net total
withdrawals |  
</data> |  |  |  |  
  
## Query information on position limit

  * POST `api/v1/contract_position_limit`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | false | string | Contract Code | Case-Insenstive.Both uppercase and
lowercase are supported. "BTC","ETH"...，If no data detected, system will
return to all contracts by default.  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "list": [
                    {
                        "contract_type": "this_week",
                        "buy_limit": 60000,
                        "sell_limit": 60000
                    },
                    {
                        "contract_type": "next_week",
                        "buy_limit": 60000,
                        "sell_limit": 60000
                    },
                    {
                        "contract_type": "quarter",
                        "buy_limit": 60000,
                        "sell_limit": 60000
                    },
                    {
                        "contract_type": "next_quarter",
                        "buy_limit": 60000,
                        "sell_limit": 60000
                    },
                    {
                        "contract_type": "all",
                        "buy_limit": 240000,
                        "sell_limit": 240000
                    }
                ]
            }
        ],
        "ts": 1604307195501
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
ts | true | long | Time of Responding Generation, Unit: milesecond |  
<data> |  |  |  |  
symbol | true | string | Contract Code | "BTC","ETH"...  
<list> |  |  |  |  
contract_type | true | string | Contract Type | Weekly :"this_week", Bi-
weekly:"next_week", Quarterly:"quarter"， Next Quarterly Contract:
"next_quarter"  
buy_limit | true | decimal | Max long position limit, Unit: Cont |  
sell_limit | true | decimal | Max short position limit, Unit: Cont |  
</list> |  |  |  |  
</data> |  |  |  |  
  
## Query Assets And Positions

  * post `api/v1/contract_account_position_info`

### params

field | Mandatory | type | desc | range  
---|---|---|---|---  
symbol | true | string | symbol | Case-Insenstive.Both uppercase and lowercase
are supported. "BTC","ETH"....  
  
> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "margin_balance": 405.226124145843792312,
                "margin_position": 10.300252356182726476,
                "margin_frozen": 0,
                "margin_available": 394.925871789661065836,
                "profit_real": 16.336169922800328615,
                "profit_unreal": 2.09434999976873802,
                "risk_rate": 39.141378262699244579,
                "withdraw_available": 386.795604223274725677,
                "liquidation_price": null,
                "lever_rate": 10,
                "adjust_factor": 0.2,
                "margin_static": 403.131774146075054292,
                "positions": [
                    {
                        "symbol": "ADA",
                        "contract_code": "ADA201225",
                        "contract_type": "quarter",
                        "volume": 1,
                        "available": 1,
                        "frozen": 0,
                        "cost_open": 0.0991,
                        "cost_hold": 0.0991,
                        "profit_unreal": 2.09434999976873802,
                        "profit_rate": 0.20755008497708193,
                        "lever_rate": 10,
                        "position_margin": 10.300252356182726476,
                        "direction": "sell",
                        "profit": 2.09434999976873802,
                        "last_price": 0.097085
                    }
                ]
            }
        ],
        "ts": 1604307305267
    }
    

### response

attr | type | Mandatory | desc  
---|---|---|---  
status | string | true | Request Processing Result "ok" , "error"  
ts | long | true | Time of Respond Generation, Unit: Millisecond  
<data> | object array | true |  
symbol | string | true | contract type  
margin_balance | decimal | true | Balance Margin  
margin_position | decimal | true | Postion Margin  
margin_frozen | decimal | true | Frozen Margin  
margin_available | decimal | true | Available Margin  
profit_real | decimal | true | Realized Profit  
profit_unreal | decimal | true | Unreadlized Profit  
risk_rate | decimal | true | risk rate  
withdraw_available | decimal | true | Available Withdraw  
liquidation_price | decimal | true | Estimated Liquidation Price  
lever_rate | decimal | true | Leverage Rate  
adjust_factor | decimal | true | Adjustment Factor  
margin_static | decimal | true | Static Margin  
<positions> |  |  |  
symbol | string | true | Variety Code  
contract_code | string | true | Contract Code "BTC180914" ...  
contract_type | string | true | Contract Type "this_week", "next_week",
"quarter" "next_quarter"  
volume | decimal | true | Position Quantity  
available | decimal | true | Available position quatity can be closed  
frozen | decimal | true | forzen postion Quantity  
cost_open | decimal | true | Opening Average Price  
cost_hold | decimal | true | Average position price  
profit_unreal | decimal | true | Unrealized profit  
profit_rate | decimal | true | Profit Rate  
profit | decimal | true | Profit  
position_margin | decimal | true | Position Margin  
lever_rate | int | true | Leverage Rate  
direction | string | true | "buy" "sell"  
last_price | decimal | true | Last Price  
</positions> |  |  |  
</data> |  |  |  
  
## Transfer between master and sub account

  * post `api/v1/contract_master_sub_transfer`

> Request:
    
    
    {
        "sub_uid": "123456789",
        "symbol": "BTC",
        "amount": "123",
        "type": "master_to_sub"
    }
    

### params

attr | required | type | desc |  
---|---|---|---|---  
sub_uid | true | long | uid of sub account |  
symbol | true | string | symbol | Case-Insenstive.Both uppercase and lowercase
are supported."BTC","ETH"...  
amount | true | decimal | transfer amount |  
type | true | string | transfer type | "master_to_sub" or "sub_to_master"  
  
  * Note： the rate limit between the master account and each subaccount is 10 times/ minute

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "order_id": "772874532490125313"
        },
        "ts": 1604309247876
    }
    

### response

attr | required | type | desc |  
---|---|---|---|---  
status | true | string | status | "ok" , "error"  
ts | true | long | response timestamp，millionseconds |  
<data> | true | object |  |  
order_id | true | string | order id |  
</data> |  |  |  |  
  
## Get transfer records between master and sub account

  * post `api/v1/contract_master_sub_transfer_record`

### request

attr | required | type | desc |  
---|---|---|---|---  
symbol | true | string | symbol | Case-Insenstive.Both uppercase and lowercase
are supported."BTC","ETH"...  
transfer_type | false | string | All by default【multiple types need to be
joined with ';'】 | 34:transfer to sub account 35:transfer from sub account  
create_date | true | int | days | days need to be less than or equal to 90  
page_index | false | int | 1 by default | 1  
page_size | false | int | 20 by default.less than or equal to 50. | 20  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "total_page": 1,
            "current_page": 1,
            "total_size": 2,
            "transfer_record": [
                {
                    "id": 3657499070,
                    "symbol": "ADA",
                    "transfer_type": 34,
                    "amount": -1,
                    "ts": 1604309247860,
                    "sub_uid": "123456789",
                    "sub_account_name": "tom"
                },
                {
                    "id": 3657420904,
                    "symbol": "ADA",
                    "transfer_type": 34,
                    "amount": -50,
                    "ts": 1604301623314,
                    "sub_uid": "123456789",
                    "sub_account_name": "tom"
                }
            ]
        },
        "ts": 1604309883224
    }
    

### response

attr | required | type | desc |  
---|---|---|---|---  
status | true | string | respone status | "ok" , "error"  
ts | true | long | response millionseconds. |  
<data> | true | object |  |  
<transfer_record> | true | object array |  |  
id | true | long | transfer id |  
ts | true | long | create timestamp |  
symbol | true | string | symbol | "BTC","ETH"...  
sub_uid | true | string | subaccount uid |  
sub_account_name | true | string | subaccount name |  
transfer_type | true | int | transfer type | transfer from
subaccount：35，transfer to subaccount:34  
amount | true | decimal | amount |  
</transfer_record> |  |  |  |  
total_page | true | int | total page |  
current_page | true | int | current page |  
total_size | true | int | total size |  
</data> |  |  |  |  
  
## Query user's API indicator disable information

  * get `api/v1/contract_api_trading_status`

### request body

null

> eg：
    
    
      {
      "status": "ok",
      "data":
      [{
          "is_disable": 1,  
          "order_price_types": "limit,post_only,FOK,IOC", 
          "disable_reason":"COR", 
          "disable_interval": 5,
          "recovery_time": 1,
          "COR":
           {
               "orders_threshold": 150,
               "orders": 150,
               "invalid_cancel_orders": 150,
               "cancel_ratio_threshold": 0.98,
               "cancel_ratio": 0.98,
               "is_trigger": 1,
               "is_active": 1
          } ,
          "TDN":
           {
               "disables_threshold": 3,
               "disables": 3,
               "is_trigger": 1,
               "is_active": 1
          } 
       }],
     "ts": 158797866555
    }
    
    

### Response:

attr | required | type | desc |  
---|---|---|---|---  
status | true | string | response status | "ok" , "error"  
ts | true | long | response millionseconds |  
<data> | true | array object |  |  
is_disable | true | long |  | 1：is disabled，0：isn't disabled  
order_price_types | true | string | order price types,such
as：“limit,post_only,FOK,IOC” |  
disable_reason | true | string | disable reason | "COR":（Cancel Order
Ratio），“TDN”：（Total Disable Number）  
disable_interval | true | long | disable millionseconds |  
recovery_time | true | long | recovery millionseconds |  
<COR> | true | dict object | （Cancel Order Ratio） |  
orders_threshold | true | long | orders threshold |  
orders | true | long | total pending orders |  
invalid_cancel_orders | true | long | numbers of invalid cancel orders |  
cancel_ratio_threshold | true | decimal | cancel ratio threshold |  
cancel_ratio | true | decimal | cancel ratio |  
is_trigger | true | int |  | 1: triggered，0: not triggered  
is_active | true | int |  | 1: active，0：not active  
</COR> | true | dict object |  |  
<TDN> | true | dict object | Total Disable Number |  
disables_threshold | true | long | disable threshold |  
disables | true | long | total disable number |  
is_trigger | true | long |  | 1：triggered，0：not triggered  
is_active | true | long |  |  
</TDN> | true | dict object |  |  
</data> |  |  |  |  
  
## Query Available Leverage Rate

  * POST `api/v1/contract_available_level_rate`

### request body

attr | required | type | desc |  
---|---|---|---|---  
symbol | false | string | case-insensitive | "BTC" , "ETH"  
  
> eg:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "available_level_rate": "1,2,3,5,10,20,30,50,75"
            }
        ],
        "ts": 1604312615051
    }
    

### Response:

attr | required | type | desc |  
---|---|---|---|---  
status | true | string | response status | "ok" , "error"  
ts | true | long | response millionseconds |  
<data> | true | array object |  |  
symbol | false | string | case-insensitive | "BTC" , "ETH"  
available_level_rate | true | string | available level rate,splited by ',' |
"1,5,10"  
</data> |  |  |  |  
  
# Future Trade Interface

## Place an Order

### Example

  * POST `api/v1/contract_order`

> Request:
    
    
    {
        "client_order_id":11223344556677,
        "contract_code":"btc200925",
        "contract_type":"quarter",
        "direction":"BUY",
        "lever_rate":75,
        "offset":"OPEN",
        "order_price_type":"post_only",
        "price":2.5,
        "symbol":"btc",
        "volume":1
    }
    

### Request Parameter

Parameter Name | Parameter Type | Mandatory | Desc  
---|---|---|---  
symbol | string | false | Case-Insenstive.Both uppercase and lowercase are
supported. "BTC","ETH"...  
contract_type | string | false | Contract Type ("this_week": "next_week":
"quarter": "next_quarter")  
contract_code | string | false | BTC180914  
client_order_id | long | false | Clients fill and maintain themselves.must be
Less or Equal than 9223372036854775807  
price | decimal | false | Price  
volume | long | true | Numbers of orders (volume)  
direction | string | true | Transaction direction  
offset | string | true | "open", "close"  
lever_rate | int | true | Leverage rate [if“Open”is multiple orders in 10
rate, there will be not multiple orders in 20 rate. Using Leverage greater
than 20 times requires prior approval of high-leverage agreement for the first
time. ]  
order_price_type | string | true | "limit”: Limit Order "opponent":BBO
"post_only": Post-Only Order, No order limit but position limit for post-only
orders.,optimal_5： Optimal , optimal_10： Optimal 10, optimal_20：Optimal
20，ioc: IOC Order,，fok：FOK Order. "opponent_ioc"：IOC order using the BBO
price，"optimal_5_ioc"：optimal_5 IOC，"optimal_10_ioc"：optimal_10
IOC，"optimal_20_ioc"：optimal_20 IOC, "opponent_fok"：FOK order using the BBO
price，"optimal_5_fok"：optimal_5 FOK，"optimal_10_fok"：optimal_10
FOK，"optimal_20_fok"：optimal_20 FOK  
  
### Note ：

If there is a number in the Contract Code row，inquiry with Contract_Code.

If there is no number，inquiry by Symbol + Contract Type.

Post-Only orders are limit orders that will never take liquidity (also called
maker-only order). There are order limit and position for post-only orders
which the upper limit is 500,000 for open/close orders under weekly, bi-weekly
and quarterly contract respectively.

If you’re holding a position currently, the leverage you choose when placing
an order should be the same as the leverage of your current positions,
otherwise, the order will fail to be placed. If you need a new leverage to
place an order, you should switch the leverage of current positions first by
using the Switch Leverage interface.

Description of post_only: assure that the maker order remains as maker order,
it will not be filled immediately with the use of post_only, for the match
system will automatically check whether the price of the maker order is
higher/lower than the opponent first price, i.e. higher than bid price 1 or
lower than the ask price 1. If yes, the maker order will placed on the
orderbook, if not, the maker order will be cancelled.

open long: direction - buy、offset - open

close long: direction -sell、offset - close

open short: direction -sell、offset - open

close short: direction -buy、offset - close

No need to transfer BBO order price(ask 1and bid 1) parameter, optimal_5: top
5 optimal BBO price, optimal_10：top 10 optimal BBO price, optimal_20：top 20
optimal BBO price (No need to transfer price data) ，limit": limit order,
"post_only": maker order only (price data transfer is needed),IOC :Immediate-
Or-Cancel Order,FOK:Fill-Or-Kill Order.

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "order_id": 773119326353580033,
            "order_id_str": "773119326353580033"
        },
        "ts": 1604367611267
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<data> |  |  |  |  
order_id | true | long | Order ID |  
order_id_str | true | string | Order ID |  
client_order_id | true | int | the client ID that is filled in when the order
is placed, if it’s not filled, it won’t be returned |  
</data> |  |  |  |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
### Note

  * The return order_id is 18 bits, it will make mistake when nodejs and JavaScript analysed 18 bits. Because the Json.parse in nodejs and JavaScript is int by default. so the number over 18 bits need be parsed by jaso-bigint package.

## Place a Batch of Orders

### Example

  * POST `/v1/contract_batchorder`

> Request:
    
    
    {
        "orders_data":[
            {
                "clientOrderId":11223344556688,
                "contract_code":"btc200925",
                "contract_type":"quarter",
                "direction":"BUY",
                "leverRate":75,
                "offset":"OPEN",
                "order_price_type":"post_only",
                "price":2.5,
                "symbol":"btc",
                "volume":1
            },
            {
                "clientOrderId":11223344556699,
                "contract_code":"btc200925",
                "contract_type":"quarter",
                "direction":"BUY",
                "leverRate":75,
                "offset":"OPEN",
                "order_price_type":"post_only",
                "price":2.5,
                "symbol":"btc",
                "volume":1
            }
        ]
    }
    

### Request Parameter

Parameter Name | Parameter Type | Mandatory | Desc  
---|---|---|---  
orders_data | List<Object> |  | 10 orders most.  
  
  * orders_data object detail

Parameter Name | Parameter Type | Mandatory | Desc  
---|---|---|---  
symbol | string | false | Case-Insenstive.Both uppercase and lowercase are
supported. "BTC","ETH"...  
contract_type | string | false | Contract Type: "this_week": "next_week":
"quarter": "next_quarter"  
contract_code | string | false | BTC180914  
client_order_id | long | false | Clients fill and maintain themselves.Must be
Less or Equal than 9223372036854775807  
price | decimal | false | Price  
volume | long | true | Numbers of orders (volume)  
direction | string | true | Transaction direction  
offset | string | true | "open": "close"  
leverRate | int | true | Leverage rate [if “Open” is multiple orders in 10
rate, there will be not multiple orders in 20 rate.Using Leverage greater than
20 times requires prior approval of high-leverage agreement for the first
time. ]  
orderPriceType | string | true | "limit”: Limit Order "opponent":BBO
"post_only": Post-Only Order, No order limit but position limit for post-only
orders.,optimal_5： Optimal , optimal_10： Optimal 10, optimal_20：Optimal 20
,ioc: IOC Order,，fok：FOK Order ,"opponent_ioc"：IOC order using the BBO
price，"optimal_5_ioc"：optimal_5 IOC，"optimal_10_ioc"：optimal_10
IOC，"optimal_20_ioc"：optimal_20 IOC, "opponent_fok"：FOK order using the BBO
price，"optimal_5_fok"：optimal_5 FOK，"optimal_10_fok"：optimal_10
FOK，"optimal_20_fok"：optimal_20 FOK  
  
### Note ：

If there is a number in the Contract Code row,inquiry with Contract_Code.

If there is no number,inquiry by Symbol + Contract Type.

Description of post_only: assure that the maker order remains as maker order,
it will not be filled immediately with the use of post_only, for the match
system will automatically check whether the price of the maker order is
higher/lower than the opponent first price, i.e. higher than bid price 1 or
lower than the ask price 1. If yes, the maker order will placed on the
orderbook, if not, the maker order will be cancelled.

If you’re holding a position currently, the leverage you choose when placing
an order should be the same as the leverage of your current positions,
otherwise, the order will fail to be placed. If you need a new leverage to
place an order, you should switch the leverage of current positions first by
using the Switch Leverage interface.

No need to transfer BBO order price(ask 1and bid 1) parameter, optimal_5: top
5 optimal BBO price, optimal_10：top 10 optimal BBO price, optimal_20：top 20
optimal BBO price (No need to transfer price data) ，limit": limit order,
"post_only": maker order only (price data transfer is needed),IOC :Immediate-
Or-Cancel Order,FOK:Fill-Or-Kill Order

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "errors": [
                {
                    "index": 1,
                    "err_code": 1037,
                    "err_msg": "The leverage is invalid. Please contact the customer service."
                }
            ],
            "success": [
                {
                    "order_id": 773120304138219520,
                    "index": 2,
                    "order_id_str": "773120304138219520"
                }
            ]
        },
        "ts": 1604367844388
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<data> |  |  |  |  
<list>(Attribute Name: errors) |  |  |  |  
index | true | int | order Index |  
err_code | true | int | Error code |  
err_msg | true | string | Error information |  
</list> |  |  |  |  
<list>(Attribute Name: success) |  |  |  |  
index | true | int | order Index |  
order_id | true | long | Order ID |  
order_id_str | true | string | Order ID |  
client_order_id | true | long | the client ID that is filled in when the order
is placed, if it’s not filled, it won’t be returned |  
</list> |  |  |  |  
</data> |  |  |  |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
### Note

The return order_id is 18 bits, it will make mistake when nodejs and
JavaScript analysed 18 bits. Because the Json.parse in nodejs and JavaScript
is int by default. so the number over 18 bits need be parsed by jaso-bigint
package.

## Cancel an Order

### Example

  * POST `api/v1/contract_cancel`

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
order_id | false | string | Order ID（different IDs are separated by ",",
maximum 10 orders can be withdrew at one time）  
client_order_id | false | string | Client order ID (different IDs are
separated by ",", maximum 10 orders can be withdrew at one time)  
symbol | true | string | Case-Insenstive.Both uppercase and lowercase are
supported.."BTC","ETH"...  
  
### Note ：

Both order_id and client_order_id can be used for order withdrawl，one of them
needed at one time，if both of them are set，the default will be order id。

The return data from Cancel An Order Interface only means that order
cancelation designation is executed successfully. To check cancelation result,
please check your order status at Get Information Of An Order interface.

client_order_id, order status query is available for orders placed within 24
hours; Otherwise, clients cannot check orders placed beyond 24 hours.

> Response: result of multiple order withdraws (successful withdrew order ID,
> failed withdrew order ID)
    
    
    {
        "status": "ok",
        "data": {
            "errors": [
                {
                    "order_id": "769206471845261312",
                    "err_code": 1061,
                    "err_msg": "This order doesnt exist."
                }
            ],
            "successes": "773120304138219520"
        },
        "ts": 1604367997451
    } 
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<dict>(Key Name: data) |  |  |  |  
<list>(Attribute Name: errors) |  |  |  |  
order_id | true | string | Order ID |  
err_code | true | int | Error code |  
err_msg | true | string | Error information |  
</list> |  |  |  |  
successes | true | string | Successfully withdrew list of order_id or
client_order_id |  
</dict> |  |  |  |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
## Cancel All Orders

### Example

  * POST `api/v1/contract_cancelall`

> Request:
    
    
    {
        "symbol":"btc",
        "contract_code":"btc200925",
        "contract_type":"quarter"
    }
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
symbol | true | string | Case-Insenstive.Both uppercase and lowercase are
supported..Variety code，eg "BTC","ETH"...  
contract_code | false | string | contract_code  
contract_type | false | string | contract_type  
  
### Note

  1. Send symbol to cancel all the contracts of that kind of symbol, e.g. send “BTC” to cancel all BTC weekly, biweekly and quarterly contracts.

  2. Send contract_code to cancel the contracts of that code.

  3. Send symbol+contract_type to cancel the certain contracts under the symbol of that contract_type, e.g. send “BTC” and “this week”, then the BTC weekly contracts will be cancelled.

> Response:result of multiple order withdrawls (successful withdrew order ID,
> failed withdrew order ID)
    
    
    {
        "status": "ok",
        "data": {
            "errors": [],
            "successes": "773120045672095744,773120045684678656"
        },
        "ts": 1604369127577
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<dict>(Key Name: data) |  |  |  |  
<list>(Attribute Name: errors) |  |  |  |  
order_id | true | string | Order ID |  
err_code | true | int | failed order error messageError code |  
err_msg | true | string | failed order information |  
</list> |  |  |  |  
successes | true | string | Successful order |  
</dict> |  |  |  |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
## Switch Leverage

  * POST `api/v1/contract_switch_lever_rate`

#### Note

  * Only if a user has positions of a single token and has no open orders, the leverage is available to be switched flexibly.

  * The interface limits the number of requests to 1 time per 3 seconds.

### Request Parameter

**Parameter Name** | **Mandatory** | **Type** | **Desc** | **Value Range**  
---|---|---|---|---  
symbol | true | String | Variety code | "BTC","ETH"...  
lever_rate | true | int | Leverage to switch.[Using Leverage greater than 20
times requires prior approval of high-leverage agreement for the first time. ]
|  
  
> Response:
    
    
    OK：
    
    {
        "status": "ok",
        "data": {
            "symbol": "ada",
            "lever_rate": 20
        },
        "ts": 1604369902689
    }
    No：
    
    {
        "status": "error",
        "err_code": 1037,
        "err_msg": "The leverage is invalid. Please contact the customer service.",
        "ts": 1604369954194
    }
    
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | status: ok,error |  
<data> | false | object |  |  
symbol | false | string | Variety code |  
lever_rate | false | int | Switched leverage |  
</data> |  |  |  |  
err_code | false | int | error code |  
err_msg | false | string | error msg |  
ts | true | long | Timestamp |  
  
## Place Flash Close Order

  * POST `api/v1/lightning_close_position`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | false | string | Contract Code | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"...  
contract_type | false | string | Contract Type |
“this_week”:Weekly，“next_week”:Bi-weekly，“quarter”:Quarterly ,Next Quarterly
Contract: "next_quarter"  
contract_code | false | string | Contract Code | BTC190903  
volume | true | long | Order Quantity(volume) |  
direction | true | string | “buy”:Open，“sell”:Close |  
client_order_id | false | long | Client order ID.must be Less or Equal than
9223372036854775807 |  
order_price_type | false | string | "lightning" by default. "lightning_fok":
lightning FOK type,"lightning_ioc": lightning IOC type |  
  
### Note:

client_order_id, order status query is available for orders placed within 24
hours; Otherwise, clients cannot check orders placed beyond 24 hours.

> Response:
    
    
    {
      "status": "ok",
      "data": {
        "order_id": 633766664829804544,
        "order_id_str": "633766664829804544",
        "client_order_id": 9086
      },
         "ts": 158797866555
    }
    
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" :Order placed
successfully, "error"：Order failed  
ts | true | long | Time of Respond Generation, Unit: Milesecond |  
<data> |  |  |  | Dictionary  
order_id | true | long | Order ID [Different users may share the same order
ID] |  
order_id_str | true | string | Order ID |  
client_order_id | false | long | user’s own order ID |  
</data> |  |  |  |  
  
> Error：
    
    
    {
        "status": "error",
        "err_code": 1048,
        "err_msg": "Insufficient close amount available.",
        "ts": 1604372431440
    }
    

## Get Information of an Order

### Example

  * POST `api/v1/contract_order_info`

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
order_id | false | string | Order ID（different IDs are separated by ",",
maximum 50 orders can be withdrew at one time）  
client_order_id | false | string | Client order ID Order ID（different IDs are
separated by ",", maximum 50 orders can be withdrew at one time)  
symbol | true | string | Case-Insenstive.Both uppercase and lowercase are
supported.."BTC","ETH"...  
  
### Note ：

When getting information on order cancellation via get order information
interface, users can only query last 4-hour data

Both order_id and client_order_id can be used for order withdrawl，one of them
needed at one time，if both of them are set，the default will be order id. The
order completed( 5.partially fulfilled but cancelled by client; 6. Fully
fulfilled; 7. Cancelled; ) will be deleted after the settlement on Friday.

client_order_id，order status query is available for orders placed within 24
hours; Otherwise, clients cannot check orders placed beyond 24 hours.

> Response:
    
    
    {
        "status": "ok",
        "data": [
            {
                "symbol": "ADA",
                "contract_code": "ADA201225",
                "contract_type": "quarter",
                "volume": 1,
                "price": 0.0933,
                "order_price_type": "post_only",
                "order_type": 1,
                "direction": "sell",
                "offset": "open",
                "lever_rate": 10,
                "order_id": 773119326353580033,
                "client_order_id": null,
                "created_at": 1604367611263,
                "trade_volume": 1,
                "trade_turnover": 10,
                "fee": -0.021436227224008574,
                "trade_avg_price": 0.0933,
                "margin_frozen": 0,
                "profit": 0,
                "status": 6,
                "order_source": "api",
                "order_id_str": "773119326353580033",
                "fee_asset": "ADA",
                "liquidation_type": "0",
                "canceled_at": 0
            }
        ],
        "ts": 1604370179844
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<list>(Attribute Name: data) |  |  |  |  
symbol | true | string | Variety code |  
contract_type | true | string | Contract Type | "this_week", "next_week",
"quarter","next_quarter"  
contract_code | true | string | Contract Code | "BTC180914" ...  
volume | true | decimal | Numbers of order |  
price | true | decimal | Price committed |  
order_price_type | true | string | "limit", "opponent","post_only" Position
limit will be applied to post_only while order limit will not. |  
direction | true | string | Transaction direction |  
offset | true | string | "open": "close" |  
lever_rate | true | int | Leverage rate | 1\5\10\20  
order_id | true | long | Order ID |  
order_id_str | true | string | Order ID |  
order_type | true | int | Order type: 1. Quotation; 2. Cancelled order; 3.
Forced liquidation; 4. Delivery Order |  
client_order_id | true | long | Client order ID |  
created_at | true | long | Creation time |  
trade_volume | true | decimal | Transaction quantity |  
trade_turnover | true | decimal | Transaction aggregate amount |  
fee | true | decimal | Servicefee |  
trade_avg_price | true | decimal | Transaction average price |  
margin_frozen | true | decimal | Freeze margin |  
profit | true | decimal | profit |  
status | true | int | status: 1. Ready to submit the orders; 2. Ready to
submit the orders; 3. Have sumbmitted the orders; 4. Orders partially matched;
5. Orders cancelled with partially matched; 6. Orders fully matched; 7. Orders
cancelled; 11. Orders cancelling. |  
order_source | true | string | Order
source（system、web、api、m、risk、settlement、ios、android、windows、mac、trigger） |  
fee_asset | true | string | the corresponding cryptocurrency to the given fee
| "BTC","ETH"...  
canceled_at | true | long | Cancellation time |  
liquidation_type | true | string | 0:Not Forced Liquidation Type，1：Netting
Type， 2: Partial Takeover，3：All Takeover |  
</list> |  |  |  |  
ts | true | long | Timestamp |  
  
## Order details acquisition

### Example

  * POST `api/v1/contract_order_detail`

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
symbol | true | string | Case-Insenstive.Both uppercase and lowercase are
supported."BTC","ETH"...  
order_id | true | long | Order ID  
created_at | true | long | Timestamp  
order_type | true | int | Order type: 1. Quotation; 2. Cancelled order; 3.
Forced liquidation; 4. Delivery Order  
page_index | false | int | Page number, default 1st page  
page_size | false | int | Default 20，no more than 50  
  
### Note

When getting information on order cancellation via query order detail
interface, users who type in parameters “created_at” and “order_type” can
query last 24-hour data, while users who don’t type in parameters “created_at”
and “order_type” can only query last 2-hour data.

The return order_id is 18 bits, it will make mistake when nodejs and
JavaScript analysed 18 bits. Because the Json.parse in nodejs and JavaScript
is int by default. so the number over 18 bits need be parsed by jason-bigint
package.

created_at should use timestamp of long type as 13 bits (include Millisecond),
if send the accurate timestamp for "created_at", query performance will be
improved.

eg. the timestamp "2019/10/18 10:26:22" can be changed：1571365582123.It can
also directly obtain the timestamp（ts) from the returned ordering
interface(contract_order) to query the corresponding orders.

Please note that created_at can't send "0"

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "symbol": "ADA",
            "contract_code": "ADA201225",
            "contract_type": "quarter",
            "instrument_price": 0,
            "final_interest": 0,
            "adjust_value": 0,
            "lever_rate": 10,
            "direction": "sell",
            "offset": "open",
            "volume": 1,
            "price": 0.0933,
            "created_at": 1604367611263,
            "canceled_at": 0,
            "order_source": "api",
            "order_price_type": "post_only",
            "margin_frozen": 0,
            "profit": 0,
            "trades": [
                {
                    "trade_id": 113887800667,
                    "trade_price": 0.0933,
                    "trade_volume": 1,
                    "trade_turnover": 10,
                    "trade_fee": -0.021436227224008574,
                    "created_at": 1604368087894,
                    "role": "maker",
                    "id": "113887800667-773119326353580033-1"
                }
            ],
            "total_page": 1,
            "current_page": 1,
            "total_size": 1,
            "liquidation_type": "0",
            "fee_asset": "ADA",
            "order_id": 773119326353580033,
            "order_id_str": "773119326353580033",
            "client_order_id": null,
            "order_type": "1",
            "status": 6,
            "trade_avg_price": 0.0933,
            "trade_turnover": 10,
            "trade_volume": 1,
            "fee": -0.021436227224008574
        },
        "ts": 1604370259827
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
<object> (Attribute Name: data) |  |  |  |  
symbol | true | string | Variety code |  
contract_type | true | string | Contract Type |
"this_week","next_week","quarter","next_quarter"  
contract_code | true | string | Contract Code | "BTC180914" ...  
lever_rate | true | int | Leverage Rate | 1\5\10\20  
direction | true | string | Transaction direction |  
offset | true | string | "open": "close" |  
volume | true | decimal | Number of Order |  
price | true | decimal | Price committed |  
created_at | true | long | Creation time |  
canceled_at | true | long | Cancellation time |  
order_source | true | string | Order Source |  
order_price_type | true | string | "limit", "opponent","post_only" Position
limit will be applied to post_only while order limit will not. |  
margin_frozen | true | decimal | Freeze margin |  
profit | true | decimal | profit |  
order_id | true | long | Order ID |  
order_id_str | true | string | Order ID |  
order_type | true | int | Order type: 1. Quotation; 2. Cancelled order; 3.
Forced liquidation; 4. Delivery Order |  
client_order_id | true | long | Client order ID |  
trade_volume | true | decimal | Transaction quantity |  
trade_turnover | true | decimal | Transaction aggregate amount |  
fee | true | decimal | Servicefee |  
trade_avg_price | true | decimal | Transaction average price |  
status | true | int | status: 1. Ready to submit the orders; 2. Ready to
submit the orders; 3. Have sumbmitted the orders; 4. Orders partially matched;
5. Orders cancelled with partially matched; 6. Orders fully matched; 7. Orders
cancelled; 11. Orders cancelling. |  
total_page | true | int | Page in total |  
current_page | true | int | Current Page |  
total_size | true | int | Total Size |  
instrument_price | true | decimal | Liquidation price |  
final_interest | true | decimal | Account Balance After Liquidation |  
adjust_value | true | decimal | Adjustment Factor of Liquidating Order |  
fee_asset | true | string | the corresponding cryptocurrency to the given fee
| "BTC","ETH"...  
liquidation_type | true | string | 0:Not Forced Liquidation Type，1：Netting
Type， 2: Partial Takeover，3：All Takeover |  
<list> (Attribute Name: trades) |  |  |  |  
id | true | string | the global unique id of the trade. |  
trade_id | true | long | In this interface, trade_id is the same with match_id
of api/v1/contract_matchresults. trade_id is the result of sets of order
execution and trade confirmation. NOTE: trade_id is not unique, which includes
all trade records of a taker order and N maker orders. If the taker order
matches with N maker orders, it will create N trades with same trade_id. |  
trade_price | true | decimal | Match Price |  
trade_volume | true | decimal | Transaction quantity |  
trade_turnover | true | decimal | Transaction price |  
trade_fee | true | decimal | Transaction Service fee |  
role | true | string | taker or maker |  
created_at | true | long | Creation time |  
</list> |  |  |  |  
</object > |  |  |  |  
ts | true | long | Timestamp |  
  
## Query Open Orders

### Example

  * POST `api/v1/contract_openorders`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Variety code |  | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"...  
page_index | false | int | Page, default 1st page | 1 |  
page_size | false | int | Default 20，no more than 50 | 20 |  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "symbol": "ADA",
                    "contract_code": "ADA201225",
                    "contract_type": "quarter",
                    "volume": 1,
                    "price": 0.0925,
                    "order_price_type": "post_only",
                    "order_type": 1,
                    "direction": "buy",
                    "offset": "close",
                    "lever_rate": 20,
                    "order_id": 773131315209248768,
                    "client_order_id": null,
                    "created_at": 1604370469629,
                    "trade_volume": 0,
                    "trade_turnover": 0,
                    "fee": 0,
                    "trade_avg_price": null,
                    "margin_frozen": 0,
                    "profit": 0,
                    "status": 3,
                    "order_source": "web",
                    "order_id_str": "773131315209248768",
                    "fee_asset": "ADA",
                    "liquidation_type": null,
                    "canceled_at": null
                }
            ],
            "total_page": 1,
            "current_page": 1,
            "total_size": 1
        },
        "ts": 1604370488518
    }
    
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result |  
<list>(Attribute Name: data) |  |  |  |  
<orders> |  |  |  |  
symbol | true | string | Variety code |  
contract_type | true | string | Contract Type |
"this_week","next_week","quarter","next_quarter"  
contract_code | true | string | Contract Code | "BTC180914" ...  
volume | true | decimal | Number of Order |  
price | true | decimal | Price committed |  
order_price_type | true | string | "limit", "opponent","post_only" Position
limit will be applied to post_only while order limit will not. |  
order_type | true | int | Order type: 1. Quotation; 2. Cancelled order; 3.
Forced liquidation; 4. Delivery Order |  
direction | true | string | Transaction direction |  
offset | true | string | "open": "close" |  
lever_rate | true | int | Leverage Rate | 1\5\10\20  
order_id | true | long | Order ID |  
order_id_str | true | string | Order ID |  
client_order_id | true | long | Client order ID |  
created_at | true | long | Order Creation time |  
trade_volume | true | decimal | Transaction quantity |  
trade_turnover | true | decimal | Transaction aggregate amount |  
fee | true | decimal | Servicefee |  
trade_avg_price | true | decimal | Transaction average price |  
margin_frozen | true | decimal | Freeze margin |  
profit | true | decimal | profit |  
status | true | int | status: 1. Ready to submit the orders; 2. Ready to
submit the orders; 3. Have sumbmitted the orders; 4. Orders partially matched;
5. Orders cancelled with partially matched; 6. Orders fully matched; 7. Orders
cancelled; 11. Orders cancelling. |  
order_source | true | string | Order Source |  
fee_asset | true | string | the corresponding cryptocurrency to the given fee
| "BTC","ETH"...  
</orders> |  |  |  |  
total_page | true | int | Total Pages |  
current_page | true | int | Current Page |  
total_size | true | int | Total Size |  
</list> |  |  |  |  
ts | true | long | Timestamp |  
  
## Get History Orders

### Example

  * POST `api/v1/contract_hisorders`

> Request:
    
    
    {
        "symbol": "BTC",
        "trade_type": 0,
        "type": 1,
        "status": "0,3,4,5",
        "create_date": 1,
        "page_index": 1,
        "page_size": 20,
        "contract_code": "BTC180914",
        "order_type": "limit"
    }
    
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Variety code |  | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"...  
trade_type | true | int | Transaction type |  | 0:all,1: buy long,2: sell
short,3: buy short,4: sell long,5: sell liquidation,6: buy
liquidation,7:Delivery long,8: Delivery short 11:reduce positions to close
long，12:reduce positions to close short  
type | true | int | Type |  | 1:All Orders,2:Order in Finished Status  
status | true | string | Order Status |  | support multiple query seperated by
',',such as '3,4,5','0': all. 3. Have sumbmitted the orders; 4. Orders
partially matched; 5. Orders cancelled with partially matched; 6. Orders fully
matched; 7. Orders cancelled;  
create_date | true | int | Date |  | any positive integer available.
Requesting data beyond 90 will not be supported, otherwise, system will return
trigger history data within the last 90 days by default.  
page_index | false | int | Page, default 1st page | 1 |  
page_size | false | int | Default 20，no more than 50 | 20 |  
contract_code | false | string | Contract Code |  | "BTC180914" ...  
order_type | false | string | Order Type |  |
1:"limit"，3:"opponent"，4:"lightning",5:"Trigger
Order",6:"pst_only",7:"optimal_5"，8:"optimal_10"，9:"optimal_20",10:"fok":FOK
order,11:"ioc":ioc order  
  
### Note

When getting information on order cancellation via query history orders
interface, users can only query last 2-hour data.

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "order_id": 773131315209248768,
                    "contract_code": "ADA201225",
                    "symbol": "ADA",
                    "lever_rate": 20,
                    "direction": "buy",
                    "offset": "close",
                    "volume": 1,
                    "price": 0.0925,
                    "create_date": 1604370469629,
                    "order_source": "web",
                    "order_price_type": 6,
                    "order_type": 1,
                    "margin_frozen": 0,
                    "profit": 0,
                    "contract_type": "quarter",
                    "trade_volume": 0,
                    "trade_turnover": 0,
                    "fee": 0,
                    "trade_avg_price": 0,
                    "status": 3,
                    "order_id_str": "773131315209248768",
                    "fee_asset": "ADA",
                    "liquidation_type": "0"
                }
            ],
            "total_page": 19,
            "current_page": 1,
            "total_size": 19
        },
        "ts": 1604370617322
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result |  
<object>(Attribute Name: data) |  |  |  |  
<list>(Attribute Name: orders) |  |  |  |  
order_id | true | long | Order ID |  
order_id_str | true | string | Order ID |  
symbol | true | string | Variety code |  
contract_type | true | string | Contract Type |
"this_week","next_week","quarter","next_quarter"  
contract_code | true | string | Contract Code | "BTC180914" ...  
lever_rate | true | int | Leverage Rate | 1\5\10\20  
direction | true | string | Transaction direction |  
offset | true | string | "open": "close" |  
volume | true | decimal | Number of Order |  
price | true | decimal | Price committed |  
create_date | true | long | Creation time |  
order_source | true | string | Order Source |  
order_price_type | true | int |
1：limit，2：market，3：opponent，4：lightning，5：trigger，6：post_only ，7：optimal_5
，8：optimal_10 ，9：optimal_20，10：FOK ，11：IOC
，12：opponent_ioc，13：lightning_ioc，14：optimal_5_ioc，15：optimal_10_ioc，16：optimal_20_ioc，17：opponent_fok，18：lightning_fok，19：optimal_5_fok，40：optimal_10_fok，41：optimal_20_fok
. |  
margin_frozen | true | decimal | Freeze margin |  
profit | true | decimal | profit |  
trade_volume | true | decimal | Transaction quantity |  
trade_turnover | true | decimal | Transaction aggregate amount |  
fee | true | decimal | Servicefee |  
trade_avg_price | true | decimal | Transaction average price |  
status | true | int | status: 1. Ready to submit the orders; 2. Ready to
submit the orders; 3. Have sumbmitted the orders; 4. Orders partially matched;
5. Orders cancelled with partially matched; 6. Orders fully matched; 7. Orders
cancelled; 11. Orders cancelling. |  
order_type | true | string | Order type | 1\. Quotation; 2. Cancelled order;
3. Forced liquidation; 4. Delivery Order  
fee_asset | true | string | the corresponding cryptocurrency to the given fee
| "BTC","ETH"...  
liquidation_type | true | string | 0:Not Forced Liquidation Type，1：Netting
Type， 2: Partial Takeover，3：All Takeover |  
</list> |  |  |  |  
total_page | true | int | Total Pages |  
current_page | true | int | Current Page |  
total_size | true | int | Total Size |  
</object> |  |  |  |  
ts | true | long | Timestamp |  
  
### Note

The return order_id is 18 bits, it will make mistake when nodejs and
JavaScript analysed 18 bits. Because the Json.parse in nodejs and JavaScript
is int by default. so the number over 18 bits need be parsed by jaso-bigint
package.

## Query history orders via multiple fields

  * POST `api/v1/contract_hisorders_exact`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | true | string | Contract Symbol | "BTC","ETH"...  
trade_type | true | int | trading type | 0:all,1: buy long,2: sell short,3:
buy short,4: sell long,5: sell liquidation,6: buy liquidation,7:Delivery
long,8: Delivery short 11:reduce positions to close long，12:reduce positions
to close short  
type | true | int | Order Type | 1:All Orders,2:Order in Finished Status  
status | true | string | Order Status | support multiple query seperated by
',',such as '3,4,5','0': all. 3. Have sumbmitted the orders; 4. Orders
partially matched; 5. Orders cancelled with partially matched; 6. Orders fully
matched; 7. Orders cancelled;  
contract_code | false | string | Contract Code |  
order_price_type | false | string | order price types | "limit”: Limit Order
"opponent":BBO "post_only": Post-Only Order, No order limit but position limit
for post-only orders.,optimal_5： Optimal , optimal_10： Optimal 10,
optimal_20：Optimal 20，ioc: IOC Order,，fok：FOK Order. "opponent_ioc"：IOC order
using the BBO price，"optimal_5_ioc"：optimal_5 IOC，"optimal_10_ioc"：optimal_10
IOC，"optimal_20_ioc"：optimal_20 IOC, "opponent_fok"：FOK order using the BBO
price，"optimal_5_fok"：optimal_5 FOK，"optimal_10_fok"：optimal_10
FOK，"optimal_20_fok"：optimal_20 FOK  
start_time | false | long | start time（Timestamp，Unit: Millisecond） | See Note  
end_time | false | long | end time（Timestamp，Unit: Millisecond） | See Note  
from_id | false | long | Query start id（uses query_id of returned data） |  
size | false | int | number of data | it will be the default value of 20; the
number should ≤50  
direct | false | string | Query direction | prev ；next ；default value:prev  
  
#### Note：

  * Query history orders interface can only query the API order cancellation information within the last 2 hours.
  * Value range description of start_time and end_time: 
    * start_time: value range is [(current time - 90 days)，current time] ；default value is clamp（end_time - 10 days，current time -90 days，current time -10 days）which means the furthest time is the current time minus 90 days and the most recent time is current time minus 10 days.
    * end_time: value range is [(current day - 90 days)，above++)，if the end_time is greater than the current time, use current time; if start_time is filled，the end_time shall be greater than start_time. The system will use current time by default. 
  * if from_id is not filled and the query direction is prev, query from back to front from the end time; if from_id is not filled and the query direction is next, query from front to back from the start time. Query financial records with creation time greater than or equal to the start time but less than or equal to the end time. 
  * Regardless of whether the query direction is prev or next, the data returned is in reverse order of creation time. 
  * If the value of start_time or end_time filled in is not within the value range, the system will report that the parameter is invalid. 
  * Only data within 90 days are available to query.

#### Query cases are as below (special cases are not included)：

start_time | end_time | from_id | size | direct | Query Result  
---|---|---|---|---|---  
Default 10 days before the current time | Default current time | Default | 20
| prev | Query the data within the last 10 days; query 20 data from back to
front from the current time. The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
Default 60 days before the current time | 50 days before the current time |
Default | 20 | prev | Query data between 60 days ago and 50 days ago; query 20
data from back to front from 50 days ago. The data returned is in reverse
order based on creation time. The newer the data, the closer to the front.  
5 days before the current time | Default current time | Default | 20 | prev |
Query the data within the last 5 days; query 20 data from back to front from
the current time. The data returned is in reverse order based on creation
time. The newer the data, the closer to the front.  
20 days before the current time | 10 days before the current time | Default |
20 | prev | Query data between 20 days ago and 10 days ago; query 20 data from
back to front from 10 days ago.The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
Default 10 days before the current time | Default current time | Default | 20
| next | Query the data within the last 10 days; query 20 data from front to
back from 10 days ago. The data returned is in reverse order based on creation
time. The newer the data, the closer to the front.  
Default 60 days before the current time | 50 days before the current time |
Default | 20 | next | Query data between 60 days ago and 50 days ago, query 20
data from front to back from 60 days ago. The data returned is in reverse
order based on creation time. The newer the data, the closer to the front.  
5 days before the current time | Default current time | Default | 20 | next |
Query the data within the last 5 days; query 20 data from 5 days ago. query 20
data from front to back from 5 days ago. The data returned is in reverse order
based on creation time. The newer the data, the closer to the front.  
20 days before the current time | 10 days before the current time | Default |
20 | next | Query data between 20 days ago and 10 days ago; query 20 data from
front to back from 20 days ago. The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
Default 10 days before the current time | Default current time | 1000 | 20 |
prev | Query the data within the last 10 days; query 20 data from back to
front from the data with transaction id 1000 and the data with transaction id
1000 is in the first line. The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
20 days before the current time | 10 days before the current time | 1000 | 20
| next | Query data between 20 days ago and 10 days ago, query 20 data from
front to back from the data with transaction id 1000 and the data with
transaction id 1000 is in the last line. The data returned is in reverse order
based on creation time. The newer the data, the closer to the front.  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "query_id": 113957564277,
                    "order_id": 773135295142658048,
                    "contract_code": "ADA201225",
                    "symbol": "ADA",
                    "lever_rate": 20,
                    "direction": "buy",
                    "offset": "open",
                    "volume": 1,
                    "price": 0.092,
                    "create_date": 1604371418518,
                    "order_source": "web",
                    "order_price_type": "post_only",
                    "order_type": 1,
                    "margin_frozen": 0,
                    "profit": 0,
                    "contract_type": "quarter",
                    "trade_volume": 1,
                    "trade_turnover": 10,
                    "fee": -0.021739130434782608,
                    "trade_avg_price": 0.092,
                    "status": 6,
                    "order_id_str": "773135295142658048",
                    "fee_asset": "ADA",
                    "liquidation_type": "0"
                }
            ],
            "remain_size": 19,
            "next_id": 113956362239
        },
        "ts": 1604371805794
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result |  
<data> | true | object |  |  
<orders> | true | object array |  |  
query_id | true | long | Query id, which can be used as the from_id field for
the next query request. |  
order_id | true | long | Order ID |  
order_id_str | true | string | Order ID |  
symbol | true | string | Contract symbol |  
contract_type | true | string | Contract Type |
“this_week”:Weekly，“next_week”:Bi-weekly，“quarter”:Quarterly ,Next Quarterly
Contract: "next_quarter"  
contract_code | true | string | Contract Code | "BTC180914" ...  
lever_rate | true | int | Leverage Rate |  
direction | true | string | Transaction direction | 【buy : sell】  
offset | true | string | offset direction | 【open : close】  
volume | true | decimal | Number of Order |  
price | true | decimal | Price committed |  
create_date | true | long | Creation time |  
order_source | true | string | Order Source |  
order_price_type | true | string | order price types | "limit”: Limit Order
"opponent":BBO "post_only": Post-Only Order, No order limit but position limit
for post-only orders.,optimal_5： Optimal , optimal_10： Optimal 10,
optimal_20：Optimal 20，ioc: IOC Order,，fok：FOK Order. "opponent_ioc"：IOC order
using the BBO price，"optimal_5_ioc"：optimal_5 IOC，"optimal_10_ioc"：optimal_10
IOC，"optimal_20_ioc"：optimal_20 IOC, "opponent_fok"：FOK order using the BBO
price，"optimal_5_fok"：optimal_5 FOK，"optimal_10_fok"：optimal_10
FOK，"optimal_20_fok"：optimal_20 FOK  
margin_frozen | true | decimal | Freeze margin |  
profit | true | decimal | profit |  
trade_volume | true | decimal | Transaction quantity |  
trade_turnover | true | decimal | Transaction aggregate amount |  
fee | true | decimal | Servicefee |  
trade_avg_price | true | decimal | Transaction average price |  
status | true | int | status | 1\. Ready to submit the orders; 2. Ready to
submit the orders; 3. Have sumbmitted the orders; 4. Orders partially matched;
5. Orders cancelled with partially matched; 6. Orders fully matched; 7. Orders
cancelled; 11. Orders cancelling.  
order_type | true | int | Order type | 1\. Quotation; 2. Cancelled order; 3.
Forced liquidation; 4. Delivery Order  
fee_asset | true | string | the corresponding cryptocurrency to the given fee
| （"BTC","ETH"...）  
liquidation_type | true | string | liquidation type | 0:Not Forced Liquidation
Type，1：Netting Type， 2: Partial Takeover，3：All Takeover  
</orders> |  |  |  |  
remain_size | true | int | Remaining data number（the number of data that has
not been queried due to the limitation of data number in the time range） |  
next_id | true | long | query_id for next data (only has value when query
result exceeds data number limits） |  
</data> |  |  |  |  
ts | true | long | Timestamp |  
  
#### Note:

  * if the query result exceeds the data limit, next_id is the id of next data. ( when the query direction is prev, next_id presents the first data on the next page; when the query direction is next, next_id presents the last data on the next page.)

## Get History Match Results

### Example

  * POST `api/v1/contract_matchresults`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | symbol |  | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"...  
trade_type | true | int | trasanction types |  | 0:All; 1: Open long; 2: Open
short; 3: Close short; 4: Close long; 5: Liquidate long positions; 6:
Liquidate short positions  
create_date | true | int | date |  | any positive integer available.
Requesting data beyond 90 will not be supported, otherwise, system will return
trigger history data within the last 90 days by default.  
contract_code | false | string | contract code |  |  
page_index | false | int | page; if not enter, it will be the default value of
the 1st page. | 1 |  
page_size | false | int | if not enter, it will be the default value of 20;
the number should ≤50 | 20 |  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "trades": [
                {
                    "match_id": 113891764710,
                    "order_id": 773135295142658048,
                    "symbol": "ADA",
                    "contract_type": "quarter",
                    "contract_code": "ADA201225",
                    "direction": "buy",
                    "offset": "open",
                    "trade_volume": 1,
                    "trade_price": 0.092,
                    "trade_turnover": 10,
                    "trade_fee": -0.021739130434782608,
                    "offset_profitloss": 0,
                    "create_date": 1604371703183,
                    "role": "Maker",
                    "order_source": "web",
                    "order_id_str": "773135295142658048",
                    "fee_asset": "ADA",
                    "id": "113891764710-773135295142658048-1"
                }
            ],
            "total_page": 16,
            "current_page": 1,
            "total_size": 16
        },
        "ts": 1604371918571
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | request handling result |  
<object>(attribute name: data: data) |  |  |  |  
<list>(attribute name: data: trades) |  |  |  |  
id | true | string | the global unique ID of the trade. |  
match_id | true | long | match_id is the same with trade_id of the websocket
subscriptions: orders.$symbol and matchOrders.$symbol.match_id is the result
of sets of order execution and trade confirmation. NOTE: match_id is not
unique, which includes all trade records of a taker order and N maker orders.
If the taker order matches with N maker orders, it will create N trades with
same match_id. |  
order_id | true | long | order ID |  
order_id_str | true | string | order ID |  
symbol | true | string | contract type code |  
order_source | true | string | Order Source |  
contract_type | true | string | contract type | deliver on this Friday then
"this_week"; deliver on next Friday then "next_week"; for quarterly contract
then "quarter", Next Quarterly Contract: "next_quarter"  
contract_code | true | string | contract code | "BTC180914" ...  
direction | true | string | "buy": to bid/ go long; "sell": to ask/ go short.
|  
offset | true | string | "open": open positions; "close": close positions |  
trade_volume | true | decimal | the number of traded contract with unit of lot
|  
trade_price | true | decimal | the price at which orders get filled |  
trade_turnover | true | decimal | the number of total traded amout with number
of USD |  
create_date | true | long | the time when orders get filled |  
offset_profitloss | true | decimal | profits and losses generated from closing
positions |  
trade_fee | true | decimal | fees charged by platform |  
role | true | string | taker or maker |  
fee_asset | true | string | the corresponding cryptocurrency to the given fee
| "BTC","ETH"...  
</list> |  |  |  |  
total_page | true | int | total pages |  
current_page | true | int | current page |  
total_size | true | int | total size of the list |  
</object> |  |  |  |  
ts | true | long | timestamp |  
  
### Notice

  * If users don’t upload/fill the page_index or page_size, it will automatically be set as the default value of the top 20 data on the first page, for more details, please follow the parameters illustration.

  * The return order_id is 18 bits, it will make mistake when nodejs and JavaScript analysed 18 bits. Because the Json.parse in nodejs and JavaScript is int by default. so the number over 18 bits need be parsed by jaso-bigint package.

## Query history transactions via multiple fields

  * POST `api/v1/contract_matchresults_exact`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | true | string | Variety code | "BTC","ETH"...  
trade_type | true | int | Transaction type | 0:All; 1: Open long; 2: Open
short; 3: Close short; 4: Close long; 5: Liquidate long positions; 6:
Liquidate short positions  
contract_code | false | string | Contract Code |  
start_time | false | long | start time（Timestamp，Unit: Millisecond） | See Note  
end_time | false | long | end time（Timestamp，Unit: Millisecond） | See Note  
from_id | false | long | Query start id（uses query_id of returned data） |  
size | false | int | number of data | it will be the default value of 20; the
number should ≤50  
direct | false | string | Query direction | prev ；next ；Default value：prev  
  
#### Note:

  * Value range description of start_time and end_time: 
    * start_time: value range is [(current time - 90 days)，current time] ；default value is clamp（end_time - 10 days，current time -90 days，current time -10 days）which means the furthest time is the current time minus 90 days and the most recent time is current time minus 10 days.
    * end_time: value range is [(current day - 90 days)，above++)，if the end_time is greater than the current time, use current time; if start_time is filled，the end_time shall be greater than start_time. The system will use current time by default. 
  * if from_id is not filled and the query direction is prev, query from back to front from the end time; if from_id is not filled and the query direction is next, query from front to back from the start time. Query financial records with creation time greater than or equal to the start time but less than or equal to the end time. 
  * Regardless of whether the query direction is prev or next, the data returned is in reverse order of creation time. 
  * If the value of start_time or end_time filled in is not within the value range, the system will report that the parameter is invalid. 
  * Only data within 90 days are available to query.

#### Query cases are as below (special cases are not included)：

start_time | end_time | from_id | size | direct | Query Result  
---|---|---|---|---|---  
Default 10 days before the current time | Default current time | Default | 20
| prev | Query the data within the last 10 days; query 20 data from back to
front from the current time. The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
Default 60 days before the current time | 50 days before the current time |
Default | 20 | prev | Query data between 60 days ago and 50 days ago; query 20
data from back to front from 50 days ago. The data returned is in reverse
order based on creation time. The newer the data, the closer to the front.  
5 days before the current time | Default current time | Default | 20 | prev |
Query the data within the last 5 days; query 20 data from back to front from
the current time. The data returned is in reverse order based on creation
time. The newer the data, the closer to the front.  
20 days before the current time | 10 days before the current time | Default |
20 | prev | Query data between 20 days ago and 10 days ago; query 20 data from
back to front from 10 days ago.The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
Default 10 days before the current time | Default current time | Default | 20
| next | Query the data within the last 10 days; query 20 data from front to
back from 10 days ago. The data returned is in reverse order based on creation
time. The newer the data, the closer to the front.  
Default 60 days before the current time | 50 days before the current time |
Default | 20 | next | Query data between 60 days ago and 50 days ago, query 20
data from front to back from 60 days ago. The data returned is in reverse
order based on creation time. The newer the data, the closer to the front.  
5 days before the current time | Default current time | Default | 20 | next |
Query the data within the last 5 days; query 20 data from 5 days ago. query 20
data from front to back from 5 days ago. The data returned is in reverse order
based on creation time. The newer the data, the closer to the front.  
20 days before the current time | 10 days before the current time | Default |
20 | next | Query data between 20 days ago and 10 days ago; query 20 data from
front to back from 20 days ago. The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
Default 10 days before the current time | Default current time | 1000 | 20 |
prev | Query the data within the last 10 days; query 20 data from back to
front from the data with transaction id 1000 and the data with transaction id
1000 is in the first line. The data returned is in reverse order based on
creation time. The newer the data, the closer to the front.  
20 days before the current time | 10 days before the current time | 1000 | 20
| next | Query data between 20 days ago and 10 days ago, query 20 data from
front to back from the data with transaction id 1000 and the data with
transaction id 1000 is in the last line. The data returned is in reverse order
based on creation time. The newer the data, the closer to the front.  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "trades": [
                {
                    "query_id": 2424420723,
                    "match_id": 113891764710,
                    "order_id": 773135295142658048,
                    "symbol": "ADA",
                    "contract_type": "quarter",
                    "contract_code": "ADA201225",
                    "direction": "buy",
                    "offset": "open",
                    "trade_volume": 1,
                    "trade_price": 0.092,
                    "trade_turnover": 10,
                    "trade_fee": -0.021739130434782608,
                    "offset_profitloss": 0,
                    "create_date": 1604371703183,
                    "role": "Maker",
                    "order_source": "web",
                    "order_id_str": "773135295142658048",
                    "fee_asset": "ADA",
                    "id": "113891764710-773135295142658048-1"
                }
            ],
            "remain_size": 15,
            "next_id": 2424413094
        },
        "ts": 1604372202243
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | request handling result |  
<data> | true | object |  |  
<trades> | true | object array |  |  
id | true | string | the global unique ID of the trade. |  
query_id | true | long | Query id, which can be used as the from_id field for
the next query request. |  
match_id | true | long | match_id is the same with trade_id of the websocket
subscriptions: orders.$symbol and matchOrders.$symbol.match_id is the result
of sets of order execution and trade confirmation. NOTE: match_id is not
unique, which includes all trade records of a taker order and N maker orders.
If the taker order matches with N maker orders, it will create N trades with
same match_id. |  
order_id | true | long | order ID |  
order_id_str | true | string | order ID |  
symbol | true | string | Variety code |  
contract_type | true | string | contract type |
“this_week”:Weekly，“next_week”:Bi-weekly，“quarter”:Quarterly ,Next Quarterly
Contract: "next_quarter"  
contract_code | true | string | Contract Code | "BTC180914" ...  
direction | true | string | Transaction direction | [Buy (buy), Sell(sell)]  
offset | true | string | "open": "close" | [Open(open), Close(lose)]  
trade_volume | true | decimal | Transaction quantity |  
trade_price | true | decimal | the price at which orders get filled |  
trade_turnover | true | decimal | Transaction aggregate amount |  
create_date | true | long | Creation time |  
offset_profitloss | true | decimal | profits and losses generated from closing
positions |  
traded_fee | true | decimal | fees charged by platform |  
role | true | string | taker or maker |  
fee_asset | true | string | the corresponding cryptocurrency to the given fee
| （"BTC","ETH"...）  
order_source | true | string | Order Source |  
</trades> |  |  |  |  
remain_size | true | int | Remaining data number（the number of data that has
not been queried due to the limitation of data number in the time range） |  
next_id | true | long | query_id for next data (only has value when query
result exceeds data number limits） |  
</data> |  |  |  |  
ts | true | long | timestamp |  
  
#### Note

  * if the query result exceeds the data limit, next_id is the id of next data. ( when the query direction is prev, next_id presents the first data on the next page; when the query direction is next, next_id presents the last data on the next page.)

## Place Trigger Order

  * POST `api/v1/contract_trigger_order`

> Request:
    
    
    {
        "contract_code":"btc200925",
        "contract_type":"quarter",
        "direction":"BUY",
        "lever_rate":5,
        "offset":"OPEN",
        "order_price":10000,
        "order_price_type":"limit",
        "symbol":"btc",
        "trigger_price":10000,
        "trigger_type":"ge",
        "volume":1
    }
    

### body

Params | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
symbol | false | string | symbol | Case-Insenstive.Both uppercase and
lowercase are supported."BTC","ETH"...  
contract_type | false | string | contract type |
“this_week”，“next_week”，“quarter”,"next_quarter"  
contract_code | false | string | contract code | BTC190903  
trigger_type | true | string | trigger： `ge` Equal to or Greater than；`le`
Less than or Equal to |  
trigger_price | true | Decimal | Trigger Price |  
order_price | false | Decimal | Order Price |  
order_price_type | false |  | order price type： "limit" by
default;"optimal_5", "optimal_10"，"optimal_20" |  
volume | true | long | volume |  
direction | true | string | buy sell |  
offset | true | string | open close |  
lever_rate | true | int | Long leverage shall be equal to short
leverage.[Using Leverage greater than 20 times requires prior approval of
high-leverage agreement for the first time. ] |  
  
### Note

  * If the contract_code field is filled with a number, order will by placed by contract_code.

  * If the contract_code field is None, order will by placed by symbol and contract_type.

  * optimal_5: top 5 optimal BBO price. optimal_10: top 10 optimal BBO price. optimal_20: top 20 optimal BBO price. limit: the limit order, order_price needed.

  * If you’re holding a position currently, the leverage you choose when placing an order should be the same as the leverage of your current positions, otherwise, the order will fail to be placed. If you need a new leverage to place an order, you should switch the leverage of current positions first by using the Switch Leverage interface. 

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "order_id": 28312412,
            "order_id_str": "28312412"
        },
        "ts": 1604372634548
    }
    

### Response Desc

field | type | Mandatory | Desc  
---|---|---|---  
status | string | true | status: ok,error  
err_code | int | false | error code  
err_msg | string | false | error message  
data | List | false | list info  
ts | long | true | timestamp  
  
  * OrderInsertRspInfo

field | type | Mandatory | Desc  
---|---|---|---  
order_id | long | true | order id. order id may be same among different users  
order_id_str | string | true | order id str  
  
## Cancel Trigger Order

  * POST `api/v1/contract_trigger_cancel`

### request params

field | type | Mandatory | desc  
---|---|---|---  
symbol | string | true | Case-Insenstive.Both uppercase and lowercase are
supported.BTC,LTC...  
order_id | string | true | order id. multiple orderids need to be joined by
",".Max number of order ids is 10 once.  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "errors": [
                {
                    "order_id": "28312406",
                    "err_code": 1061,
                    "err_msg": "This order doesnt exist."
                }
            ],
            "successes": "28312412"
        },
        "ts": 1604372746401
    }
    

### response

field | Required | type | desc | value range  
---|---|---|---|---  
status | true | string | response status | "ok" , "error"  
<data> |  |  |  |  
successes | true | string | successful orders |  
<list>(field name: errors) |  |  |  |  
order_id | true | string | order id |  
err_code | true | int | error code |  
err_msg | true | string | error messages |  
</list> |  |  |  |  
</data> |  |  |  |  
ts | true | long | response timestamp millseconds |  
  
## Cancel All Trigger Orders

  * POST `api/v1/contract_trigger_cancelall`

### Params

field | type | Mandatory | desc  
---|---|---|---  
symbol | string | true | Case-Insenstive.Both uppercase and lowercase are
supported.BTC、LTC...  
contract_code | string | false | contract code,"BTC180914" ...  
contract_type | string | false | contract type "this_week" "next_week"
"quarter" "next_quarter"  
  
### Note

  * If only symbol is filled, cancel all trigger orders of this symbol

  * If contract_code is filled, cancel trigger orders of this contract code.

  * If symbol and contract_type are filled, cancel trigger orders of this symbol and contract code.

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "errors": [],
            "successes": "28312413,28312414"
        },
        "ts": 1604373863946
    }
    

### response params

field | Mandatory | type | desc | value range  
---|---|---|---|---  
status | true | string | status | "ok" , "error"  
<data> |  |  |  |  
<list>(data name: errors) |  |  |  |  
order_id | true | string | order id |  
err_code | true | int | error code |  
err_msg | true | string | error message |  
</list> |  |  |  |  
successes | true | string | successful orders |  
</data> |  |  |  |  
ts | true | long | response timestamp in millseconds |  
  
## Query Trigger Order Open Orders

  * POST `api/v1/contract_trigger_openorders`

### Request Parameter

Parameter Name | Type | Mandatory | Description  
---|---|---|---  
symbol | string | true | Case-Insenstive.Both uppercase and lowercase are
supported.BTC,LTC...  
contract_code | string | false | Case-Insenstive.Both uppercase and lowercase
are supported..contract code  
page_index | int | false | page number，default page 1 if no given instruction  
page_size | int | false | default 20 if no given instruction  
  
> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "symbol": "ADA",
                    "contract_code": "ADA201225",
                    "contract_type": "quarter",
                    "trigger_type": "le",
                    "volume": 1,
                    "order_type": 1,
                    "direction": "buy",
                    "offset": "open",
                    "lever_rate": 20,
                    "order_id": 28312415,
                    "order_id_str": "28312415",
                    "order_source": "api",
                    "trigger_price": 0.0895,
                    "order_price": 0.0895,
                    "created_at": 1604374041289,
                    "order_price_type": "limit",
                    "status": 2
                }
            ],
            "total_page": 1,
            "current_page": 1,
            "total_size": 1
        },
        "ts": 1604374215911
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Description | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
data | true | object | Returned data |  
ts | true | long | Time stamp of response, Unit: millisecond |  
  
  * data details

Parameter Name | Mandatory | Type | Description | Value Range  
---|---|---|---|---  
total_page | int | true | total page |  
current_page | int | true | current page |  
total_size | int | true | total size |  
<list> (Attribute Name: orders) |  |  |  |  
symbol | string | true | Cryptocurrency |  
contract_code | string | true | contract code |  
contract_type | string | true | contract type |  
trigger_type | string | true | trigger type： `ge`great than or equal
to；`le`less than or equal to |  
volume | decimal | true | trigger order volume |  
order_type | int | true | Transaction Type 1. Place orders 2. cancel orders |  
direction | string | true | order direction [buy,sell] |  
offset | string | true | offset direction [open,close] |  
lever_rate | int | true | Leverage 1\5\10\20 |  
order_id | long | true | trigger order ID |  
order_id_str | string | true | the order ID with string |  
order_source | string | true | source |  
trigger_price | decimal | true | trigger price |  
order_price | decimal | true | the preset price by the client |  
created_at | long | true | order creation time |  
order_price_type | string | true | order price type "limit": limit
order，"optimal_5":optimal 5，"optimal_10":optimal 10，"optimal_20":optimal 20 |  
status | int | true | order status：1:ready to submit、2:submited、3:order
accepted、7:wrong order、8：canceled orders but not found、9：canceling
order、10：failed' |  
</list> |  |  |  |  
  
## Query Trigger Order History

  * POST `api/v1/contract_trigger_hisorders`

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Cryptocurrency |  | Case-Insenstive.Both uppercase
and lowercase are supported."BTC","ETH"...  
contract_code | false | string | Contract Code |  | EOS190118  
trade_type | true | int | Transaction type |  | 0: All ,1: Open Long,2: Close
Short,3: Open Short,4: Close Long；the system will transfer these parameters
into offset and direction and query the requested data. Please note that no
data can be requested with parameter out of this range.  
status | true | string | Order Status |  | data divided with several commas,
trigger orders ready to be submitted：0: All (All filled orders),4: Trigger
orders successfully submitted,5: Trigger orders failed being submitted, 6:
Trigger orders cancelled  
create_date | true | int | Date |  | any positive integer available.
Requesting data beyond 90 will not be supported, otherwise, system will return
trigger history data within the last 90 days by default.  
page_index | false | int | Page, 1st page by default without given instruction
| 1 | page，1st page by default without given instruction  
page_size | false | int | Page 20 by default without given instruction, ，no
more than 50 | 20 | Page 20 by default without given instruction, ，no more
than 50  
  
### NOTE

  * System will query the filled trigger order history by default 

> Response:
    
    
    {
        "status": "ok",
        "data": {
            "orders": [
                {
                    "symbol": "ADA",
                    "contract_code": "ADA201225",
                    "contract_type": "quarter",
                    "trigger_type": "le",
                    "volume": 1,
                    "order_type": 1,
                    "direction": "buy",
                    "offset": "open",
                    "lever_rate": 20,
                    "order_id": 28312415,
                    "order_id_str": "28312415",
                    "relation_order_id": "773147284987842560",
                    "order_price_type": "limit",
                    "status": 4,
                    "order_source": "api",
                    "trigger_price": 0.0895,
                    "triggered_price": 0.089497,
                    "order_price": 0.0895,
                    "created_at": 1604374041289,
                    "triggered_at": 1604374277082,
                    "order_insert_at": 1604374277124,
                    "canceled_at": 0,
                    "fail_code": null,
                    "fail_reason": null
                }
            ],
            "total_page": 4,
            "current_page": 1,
            "total_size": 4
        },
        "ts": 1604374349086
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Request Processing Result | "ok" , "error"  
data | true | object | Return data |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
  * Data details：

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
total_page | int | true | Total page |  
current_page | int | true | Current page |  
total_size | int | true | Total Size |  
<list>(Attribute Name: orders) |  |  |  |  
symbol | string | true | Cryptocurrency |  
contract_code | string | true | Contract Code |  
contract_type | string | true | Contract Type |  
trigger_type | string | true | trigger： `ge` Equal to or Greater than；`le`
Less than or Equal to |  
volume | decimal | true | Numbers of order placed |  
order_type | int | true | Transaction type：1、Place orders 2、Cancel orders |  
direction | string | true | order direction, [Buy (buy), Sell(sell)] |  
offset | string | true | offset direction [Open(open), Close(lose)] |  
lever_rate | int | true | leverage 1\5\10\20 |  
order_id | int | true | Trigger order ID |  
order_id_str | string | true | the order ID with string |  
relation_order_id | string | true | Relation order ID is the string related to
the limit orders. The value is -1 before the trigger orders executed. |  
order_price_type | string | true | order type "limit": Limit order
price，"optimal_5": Optimal 5 price level，"optimal_10":Optimal 10 price
level，"optimal_20": the Optimal 20 price level |  
status | int | true | Order status (4:Orders accepted、5: Orders failing being
placed、6: Orders canceled ) |  
order_source | string | true | Order source |  
trigger_price | decimal | true | trigger price |  
triggered_price | decimal | true | the price when trigger orders executed |  
order_price | decimal | true | the order price preset by the client |  
created_at | long | true | the order creation time |  
triggered_at | long | true | the execution time when orders getting triggered.
|  
order_insert_at | long | true | the time when the triggered orders filled
successfully. |  
canceled_at | long | true | Order cancelation time |  
fail_code | int | true | the error code when the triggered orders failed to be
filled |  
fail_reason | string | true | the error message with failure reason when
triggered orders failed to filled. |  
</list> |  |  |  |  
  
# Future Transferring Interface

## Transfer margin between Spot account and Future account

### Example

  * POST `https://api.huobi.pro/v1/futures/transfer`

### Notice

This interface is used to transfer assets between Spot account and Future
account.

The type is “pro-to-futures” when transferring assets from Spot account to
Future; “futures-to-pro” when transferring from Future account to Spot
account.

API rate limit for this interface is 1 times/second.

Transferring margin between Spot account and Future account Interface, sets 8
decimal places for transferring amount of all coins.

### Request Parameter

Parameter Name | Mandatory | Type | Desc | Default | Value Range  
---|---|---|---|---|---  
currency | true | string | currency. Case insensitive |  | e.g. btc, BTC  
amount | true | Decimal | Transferring amount |  |  
type | true | string | type of the transfer |  | Transfer from Future account
to Spot account: “futures-to-pro” Transfer from Spot account to Future
account: "pro-to-futures"  
  
> Response:
    
    
    {
        "status": "ok",
        "data": 179697972
    }
    Error response:
    {
        "status": "error",
        "data": null,
        "err-code": "base-currency-error",
        "err-msg": "The current coin does not exist."
    }
    

### Returning Parameter

Parameter Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
status | true | string | Response status | ok, error  
data | true | long | Transfer ID | If status="error", data will be null.  
err-code | true | string | Error code |  
err-msg | true | string | Error code description |  
  
## Error Code Table

err-code | err-msg | Comments  
---|---|---  
base-msg |  | Other errors, please refer to err-msg list below for details。  
base-currency-error | The currency is invalid |  
frequent-invoke | the operation is too frequent. Please try again later |  
banned-by-blacklist | Blacklist restriction |  
dw-insufficient-balance | Insufficient balance. You can only transfer {0} at
most. |  
dw-account-transfer-unavailable | account transfer unavailable |  
dw-account-transfer-error | account transfer error |  
dw-account-transfer-failed | Failed to transfer. Please try again later. |  
dw-account-transfer-failed-account-abnormality | Account abnormality, failed
to transfer。Please try again later. |  
  
## Error message when err-code is ‘base-msg’.

err-msg | Comments  
---|---  
Unable to transfer in currently. Please contact customer service. |  
Unable to transfer out currently. Please contact customer service. |  
Abnormal contracts status. Can’t transfer. |  
Sub-account doesn't own the permissions to transfer in. Please contact
customer service. |  
Sub-account doesn't own the permissions to transfer out. Please contact
customer service. |  
The sub-account does not have transfer permissions. Please login main account
to authorize. |  
Insufficient amount available. | Insufficient amount of Future Contract
Account  
The single transfer-out amount must be no less than {0}{1}. |  
The single transfer-out amount must be no more than {0}{1}. |  
The single transfer-in amount must be no less than {0}{1}. |  
The single transfer-in amount must be no more than {0}{1}. |  
Your accumulative transfer-out amount is over the daily maximum, {0}{1}. You
can't transfer out for the time being. |  
Your accumulative transfer-in amount is over the daily maximum, {0}{1}. You
can't transfer in for the time being. |  
Your accumulative net transfer-out amount is over the daily maximum, {0}{1}.
You can't transfer out for the time being. |  
Your accumulative net transfer-in amount is over the daily maximum, {0}{1}.
You can't transfer in for the time being. |  
The platform's accumulative transfer-out amount is over the daily maximum. You
can't transfer out for the time being. |  
The platform's accumulative transfer-in amount is over the daily maximum. You
can't transfer in for the time being. |  
The platform's accumulative net transfer-out amount is over the daily maximum.
You can't transfer out for the time being. |  
The platform's accumulative net transfer-in amount is over the daily maximum.
You can't transfer in for the time being. |  
Transfer failed. Please try again later or contact customer service. |  
Abnormal service, transfer failed. Please try again later. |  
You don’t have access permission as you have not opened contracts trading. |  
This contract type doesn't exist. |  
  
# Future WebSocket Reference

## API List

Permission | Content Type | Request Method | Type | Description |
Authentication Required  
---|---|---|---|---|---  
Read | Market Data Interface | market.$symbol.kline.$period | sub | Subscribe
Kline data | No  
Read | Market Data Interface | market.$symbol.kline.$period | req | Request
Kline Data | Nos  
Read | Market Data Interface | market.$symbol.depth.$type | sub | Subscribe
Market Depth Data | No  
Read | Market Data Interface | market.$symbol.depth.size_${size}.high_freq |
sub | Subscribe Incremental Market Depth Data | No  
Read | Market Data Interface | market.$symbol.bbo | sub | Subscribe BBO Data |
No  
Read | Market Data Interface | market.$symbol.detail | sub | Subscribe Market
Detail Data | No  
Read | Market Data Interface | market.$symbol.trade.detail | req | Request
Trade Detail Data | No  
Read | Market Data Interface | market.$symbol.trade.detail | sub | Subscribe
Trade Detail Data | No  
Read | System Status Interface | public.$service.heartbeat | sub |
Subscription system status updates | No  
Trade | Trade Interface | orders.$symbol | sub | Subscribe Order Data | Yes  
Trade | Trade Interface | matchOrders.$symbol | sub | Subscribe Order Data |
Yes  
Read | Account Interface | accounts.$symbol | sub | Subscribe asset change
Information of a given coin | Yes  
Read | Account Interface | positions.$symbol | sub | Subscribe position change
Information of a given coin | Yes  
Read | Account Interface | trigger_order.$symbol | sub | Subscribe trigger
orders updates | Yes  
Read | Trade Interface | public.$symbol.liquidation_orders | sub | Subscribe
liquidation Order information of a given coin | Yes  
  
## Huobi Future WebSocket Subscription Address

Market Data Request and Subscription: wss://api.hbdm.com/ws

Order Push Subscription: wss://api.hbdm.com/notification

Index Kline Data and Basis Data Subscription: wss://api.hbdm.com/ws_index

System status updates subscription ：wss://api.hbdm.com/center-notification

If the url: api.hbdm.com can't be accessed, please use the url below:

Market Data Request and Subscription Address: wss://api.btcgateway.pro/ws;

Order Push Subscription：wss://api.btcgateway.pro/notification

Index Kline Data and Basis Data Subscription:
wss://api.btcgateway.pro/ws_index

System status updates subscription ：wss://api.btcgateway.pro/center-
notification

If you have further queries about Huobi Future order push subscription, please
refer to [Demo](https://github.com/huobiapi/Futures-Java-demo)

### Note:

If you can't connect "https://api.hbdm.com", please use
"https://api.btcgateway.pro" for debug purpose. If your server is deployed in
AWS, we recommend using "https://api.hbdm.vn".

## API Rate Limit Illustration

There is rate limit for both public and private interfaces. More details are
laid out as below:

  * Generally, the private interface rate limit of API key is at most 72 times every 3 seconds for each UID (Trade Interface: at most 36 times every 3 seconds. Read Interface: at most 36 times every 3 seconds) (this rate limit is shared by all the altcoins contracts delivered by different date).

  * For public interfaces used to get information of non-market data (such as request information of index, price limit, delivery and settlement, positions, etc.), the rate limit for each IP is 120 times every 3 seconds. (Please note that the 120 times/3s rate limit is shared by all the requests for non-market data under this UID)

  * For public interface to get market data such as Get Kline data, Get Market Data Overview, Get Contract Information,Get market depth data, Get index kline, Get basis data, Get the last Trade of a Contract and so on：

(1) For restful interfaces：all products(futures, coin margined swap, usdt
margined swap and option) 800 times/second for one IP at most

(2) The rate limit for “req” request is 50 times/s at most. No limit for “sub”
request as the data will be pushed by server voluntarily.

  * The order push private WebSocket interface requires API Key for authentication.

Each UID can create 30 WS connections at most for private order push at the
same time. The user under this UID only need to subscribe one WS order push
for the contracts of the same underlying coins. For example, users only need
to create one WS order push connection for BTC Contract, which our system will
automatically push orders of BTC weekly, BTC biweekly and BTC quarterly
contracts via this connection.

Note: The rate limit of WS order push and RESTFUL private interface are
separated from each other with no relations.

  * 40 subscriptions at most can be sent in one second in websocket connections.

Response the following strings for “Header” via API

  * ratelimit-limit： the upper request limit per time, unit: times

  * ratelimit-interval： reset interval(reset the number of request ), unit: ms

  * ratelimit-remaining： available request number left in this round, unit: times

  * ratelimit-reset： upper limit of reset time used to request number， unit: ms

# WebSocket Heartbeat and Authentication Interface

## Market Heartbeat

WebSocket API supports two-way heartbeat. Both Server and Client can send ping
message, which the opposite side can return with pong message.

  * WebSocket Server sends heartbeat：

`{"ping": 18212558000}`

  * WebSocket Client should respond:：

`{"pong": 18212558000}`

Note: Once the WebSocket Client and WebSocket Server get connected, the server
will send a heartbeat every 5 seconds (the frequency might change). The
connection will get disconnected automatically if the WebSocket Client ignores
the heartbeat message for 5 times. The server will remain connection if the
WebSocket Client responds one “ping” value within the latest 2 heartbeat
messages.

## Order Push Heartbeat

### WebSocket API supports one-way heartbeat. The Server initiates ping
message and the Client will return pong message. The Server sends back a
heartbeat:

`{`

`"op": "ping",`

`"ts": "1492420473058"`

`}`

  * WebSocket Client should return:

`{`

`"op": "pong",`

`"ts": "1492420473058"`

`}`

### Note

  * "ts" value in the return "pong" message is the "ts" value from "ping" push Once the WebSocket Client and WebSocket Server connected, Websocket Server will send a heartbeat every 5 seconds (the frequency might change) to Wesocket Client. If WebSocket Client ignores the heartbeat message for 5 times, it will get disconnected with Websocket Sever automatically. Under abnormal conditions, WebSocket Server will return error message like:

`{`

`"op": "pong"`

`"ts": "1492420473027",`

`"err-code": 2011,`

`"err-msg": “detailed error message”`

`}`

  * Websocket Server disconnects automatically During period of building connection and authentication, Websocket Server will disconnect automatically if there is any error. The data structure before closing pushing are as below:

`{`

`"op": "close", // indicate Websocket Server disconnected automatically`

`"ts": long // The local timestamp of Server push`

`}`

  * Server return error but remain connection After successful authentication, Server will return error but not disconnect if Client provides illegal Op or there is any internal error.

`{`

`"op": "error", // indicate that receive illegal Op or internal error`

`"ts": long// The local timestamp of Server push`

`}`

## Order Push Address

  * Huobi Future uses one official address:

`wss://api.hbdm.com/notification`

### Note:

If you can't connect "https://api.hbdm.com", please use
"https://api.btcgateway.pro" for debug purpose. If your server is deployed in
AWS, we recommend using "https://api.hbdm.vn".

Please note that the WS request connection should not go over 30 normally.

### Data Compression

All response data from WebSocket server are compressed into GZIP format.
Clients have to decompress them for further use.

### Illustration of Request(req and rep) Data

  * Character Encoding：UTF-8

  * Case sensitive，including parameter name and return parameter

  * Data type： use JSON to transmit data

-All request data has fixed format. Please note that Huobi Future API document will only focus on data illustration in non-fixed format.

> Request data format is laid out as below:
    
    
      {
      "op": string, // Required; Client requests operator name (Server will returns the same value), For detailed operator name list, please refer to the appendix
      "cid": string, // Optional;Request unique ID( Client generate a unique ID which server will return the same value)
      // Others required/ Optional string
      }
    
    

> All responses push data will be returned in fixed format，Huobi Future API
> document will only focus on data illustration， Response data format is laid
> out as below；
    
    
      {
      "op": string, // Required; Clients request operator name
      "cid": string, // optional; Client requests unique ID
      "ts": long, // required; Server responds local timestamp
      "err-code": integer, // required; return error code, “0” means successfully responded, others means error. For detailed return error code list, please refer to appendix
      "err-msg": string, only responds error message when error occurs, detailed error information. 
      "data": object // optional; return data object， request valid data after error removed 
      }
    
    

> Push Data Format is laid out as below:
    
    
      {
      "op": "string", // required;Server pushes operator name, For detailed operator type list, please refer to appendix
      "ts": long, // required; Server pushes local timestamp
      "data": object // required;返return data object
      }
    
    

## Server voluntarily disconnects connection

During making connection and authentication, server will disconnect connection
automatically when error occurs. Before disconnecting, server will send
notification below,

`{`

`"op": "close", // represents server disconnect connection voluntarily

`"ts": long // Server pushes local timestamp

`}`

## Server return error code but remain connection

After authentication, if clients encountered internal error or request data
out from Operator List, WebSocket server will return error message. But server
will remain connection

`{`

`"op": "error", // means server receive data out from Operator List or clients
got internal error`

`"ts": long// Server pushes local timestamp`

`}`

## Authentication

Clients can create Access Key and Secret Key on Huobi which Access Key is the
API access key kept by the client. The Secret Key is used to sign the request
(available only for request). To apply/change API key, please go to “Account-
API Management” on Huobi Futures. Make name for the API Key and click “create”
to finish. It’s optional to bind IP address to the API Key.

For the Trade WebSocket interface, server have to do authentication for topics
require authentication before making connection.

Note: These two keys are closely related to account security and should not be
disclosed to others at any time.

### Authentication Format Example:

`{`

`"op": "auth",`

`"type": "api",`

`"AccessKeyId": "e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx",`

`"SignatureMethod": "HmacSHA256",`

`"SignatureVersion": "2",`

`"Timestamp": "2017-05-11T15:19:30",`

`"Signature": "4F65x5A2bLyMWVQj3Aqp+B4w+ivaA7n5Oi2SuYtCJ9o=",`

`}`

### Illustration on Authentication Format Data

Field | type | Description  
---|---|---  
op | string | required； Operator type， Requested authentication operator type
is auth  
type | string | required； Signature method sign via API means API interface
signature, sign via ticket means terminal signature  
cid | string | Optional； Client requests the unique ID  
AccessKeyId | string | required if users use API signature； API Access key is
the API AccessKey you applied.  
SignatureMethod | string | required if users use API signature； Signature
method, user computes signature basing on the protocol of hash ,the API uses
HmacSHA256  
SignatureVersion | string | required if the users use API signature； the
signature protocol version, the API uses 2  
Timestamp | string | required if users use API signature； timestamp, the time
you request(UTC timezone) this value can help to avoid request data
interception by the third party for example ：2017-05-11T16:22:06 (UTC time
zone)  
Signature | string | required if the users use API signature； signature, the
value computed is ensure valid authentication without being tampered  
ticket | string | required if users use ticket signature ； return when logged
in  
  
#### Notice：

  * To decrease API access rate, the WebSocket server uses the same signature algorithm with that on REST API 

  * All data is case sensitive;

  * When type is api, In API authentication, parameter op, type, cid, Signature do not participate in operation.

  * The request method in signature's method is GET, the other parameter please refer to REST api document

#### Signature Illustration：

Example on Signature Computing Process:，

  * Request code requirement for signature computing. Because it can return to total different data with different content when using HMAC for signature computing; Before signature computing, clients need to sign by following the standard format.

  * Request Method (GET or POST), add newline character `\n` after URL

`GET\n`

  * add visit address with lowercase letters, add newline characters `\n` after URL

`api.hbdm.com\n`

  * Access path, adding newline character `\n` after URL

`/notification\n`

  * Sequence the parameter name according to ASCII code (use UTF-8 and transfer into URI encoding, capital letters for hexadecimal characters. E.G.: ‘:’ will be encoded into '%3A', blank will be encoded into '%20'). Here is an encoding example below for request parameters

`AccessKeyId=e2xxxxxx-99xxxxxx-84xxxxxx-7xxxx&SignatureMethod=HmacSHA256&SignatureVersion=2&Timestamp=2017-05-11T15%3A19%3A30`

  * Connect all parameters with ’&’ according to the sequence above.

  * The final strings for signature computing created by following the steps as below:

Signature Computing, transmit the two parameters below into cryptographic
hash: strings needed to be computed, API SecretKey. Get the signature
computing result and get it encoded with Base 64 code standard.

Add computed value into the Signature parameter in API request. Please note
the computed value SHOULD NOT be encoded into URL cdoe.

### Authentication Response Format Illustration

Field | type | description  
---|---|---  
op | string | required； Operator type， Authentication response type is auth  
type | string | required； Return data according to the requested parameters  
cid | string | optional； Return data when “cid” string requested  
err-code | integer | 0 means successfully response, others means response
failure成功返回 0 , For detailed Response code（Err-Code）, please refer to appendix  
err-msg | string | optional， response detailed error code when error occurs  
ts | long | server responds timestamp  
user-id | long | client ID  
  
> Example of A Success Authentication Response
    
    
    {
      "op": "auth",
      "type":"api",
      "ts": 1489474081631,
      "err-code": 0,
      "data": {
        "user-id": 12345678
      }
    }
    
    

> Example of Authentication Response with Error
    
    
    {
    "op": "auth",
    "type":"api",
    "ts": 1489474081631, 
    "err-code": xxxx， 
    "err-msg" : "Error details "
    }
    

# WebSocket Market Interface

## Subscribe Kline data

### To subscribe Kline data, clients have to connect WebSocket API server and
send subscribe request with the format below：

`{`

`"sub": "market.$symbol.kline.$period",`

`"id": "id generate by client"`

`}`

> Example of a successful subscription request：
    
    
        {
        "sub": "market.BTC_CQ.kline.1min",
        "id": "id1"
        }
    
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
sub | true | string | the themes that need to be subscribed; the interface is
fixed at: market.$symbol.kline.$period，For parameter details please check sub
Subscribe Parameter Rules  
id | false | string | id automatically generated by the business party  
  
### sub Subscribe Parameter Rules

Parameter Name | Mandatory | Type | Description | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Pairs |  | Case-Insenstive.Both uppercase and
lowercase are supported..E.G.: "BTC_CW" stands for BTC weekly contract,
"BTC_NW" stands for BTC Bi-weekly contract, "BTC_CQ" stands for BTC quarterly
contract."BTC_NQ" stands for BTC next quarterly contract. contract code is
supported too, e.g.: "BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
period | true | string | Kline Period |  | Case-Senstive.Only lowercase is
supported. 1min, 5min, 15min, 30min, 60min,4hour,1day,1week, 1mon  
  
> After subscription, clients can receive updates upon any change. Example:
    
    
    {
        "ch":"market.BTC_CW.kline.1min",
        "ts":1604385120328,
        "tick":{
            "id":1604385120,
            "mrid":113842458873,
            "open":13436.12,
            "close":13436.12,
            "high":13436.12,
            "low":13436.12,
            "amount":0,
            "vol":0,
            "count":0
        }
    }
    

### Return Parameter

Parameter Name | Mandatory | Type | Description  
---|---|---|---  
ch | true | string | Request Parameter  
ts | true | long | Time of Respond Generation，Unit：Millisecond  
<tick> |  |  |  
id | true | long | kline id,the same as kline timestamp, kline start timestamp  
mrid | true | long | Order ID  
vol | true | decimal | Trade Volume(Cont.)  
count | true | decimal | Order Quantity  
open | true | decimal | Open Price  
close | true | decimal | Clos Price, the price in the last kline is the latest
order price  
low | true | decimal | Low Price  
high | true | decimal | High Price  
amount | true | decimal | Trade Amount(Coin), trade amount(coin)=sum(order
quantity of a single order * face value of the coin/order price)  
</tick> |  |  |  
  
## Request Kline data

### To request Kline data, clients have to make connection to WebSocket API
Server and send subscribe request in the format below：

`{`

`"req": "market.$symbol.kline.$period",`

`"id": "id generated by client",`

`"from": " type: long, the time from 2017-07-28T00:00:00+08:00 to
2050-01-01T00:00:00+08:00, unit: s",`

`"to": "type: long, the time from 2017-07-28T00:00:00+08:00 to
2050-01-01T00:00:00+08:00, unit: s , the 'to' value should be larger than
'from' value"`

`}`

> Example of Kline Data Subscription Request：
    
    
    {
        "req": "market.BTC_CQ.kline.1min",
        "id": "id4",
        "from": 1571000000,
        "to": 1573106298
    }
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
req | true | string | the themes that need to be subscribed; the interface is
fixed at: market.$symbol.kline.$period，For parameter details please check req
Subscribe Parameter Rules  
id | false | string | id automatically generated by the business party  
from | true | long | Start Time  
to | true | long | End Time  
  
### req Subscribe Parameter Rules

Parameter Name | Mandatory | Type | Description | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Pairs |  | Case-Insenstive.Both uppercase and
lowercase are supported..E.g.: "BTC_CW" stands for BTC weekly contract,
"BTC_NW" stands for BTC bi-weekly contract, "BTC_CQ" stands for BTC quarterly
contract."BTC_NQ" stands for BTC next quarterly contract. contract code is
supported too, e.g.: "BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly).  
period | false | string | Kline Period |  | Case-Senstive.Only lowercase is
supported.1min, 5min, 15min, 30min, 60min,4hour,1day,1week, 1mon  
  
#### Note

If between time range [t1, t5], there are t1-t5 Klines in quantity.

from: t1, to: t5, return [t1, t5].

from: t5, to: t1, which t5 > t1, return [].

from: t5, return [t5].

from: t3, return [t3, t5].

to: t5, return [t1, t5].

from: t which t3 < t <t4, return [t4, t5].

to: t which t3 < t <t4, return [t1, t3].

from: t1 and to: t2, should satisfy 1325347200 < t1 < t2 < 2524579200.

Clients can request 2000 Klines at most in one request

> After subscription, Clients can receive the most recent data upon any
> update：
    
    
    {
        "id":"id4",
        "rep":"market.BTC_CQ.kline.15min",
        "wsid":498385304,
        "status":"ok",
        "data":[
            {
                "id":1599667200,
                "open":10262.31,
                "close":10244.93,
                "low":10234.84,
                "high":10282,
                "amount":1849.4984536479908439463088799853871134642,
                "vol":189634,
                "count":5342
            },
            {
                "id":1599668100,
                "open":10244.94,
                "close":10242.07,
                "low":10216.55,
                "high":10244.94,
                "amount":1586.9623024248859129381285787325037896282,
                "vol":162334,
                "count":4375
            }
        ]
    }
    

### Return Parameter

Parameter Name | Mandatory | Type | Description  
---|---|---|---  
rep | true | string | Request Parameter  
status | true | string | status  
id | true | string | Request ID  
wsid | true | long | wsid  
<data> |  |  |  
id | true | long | kline id,the same as kline timestamp, kline start timestamp  
vol | true | decimal | Trade Volume(Cont.)  
count | true | decimal | Order quantity  
open | true | decimal | Open Price  
close | true | decimal | Clos Price, the price in the latest Kline is the last
order price  
low | true | decimal | Low Price  
high | true | decimal | High Price  
amount | true | decimal | Trade Amount(Coin), trade amount(coins)=sum(order
quantity of a single order * face value of the coin/order price)  
</data> |  |  |  
  
## Subscribe Market Depth Data

### To subscribe market depth data, clients have to make connection to
WebSocket API Server and send subscribe request in the format below：

`{`

`"sub": "market.$symbol.depth.$type",`

`"id": "id generated by client"`

`}`

> Example of a successful request ：
    
    
        {
        "sub": "market.BTC_CQ.depth.step0",
        "id": "id5"
        }
    
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
sub | true | string | the themes that need to be subscribed; the interface is
fixed at: market.$symbol.depth.$type，For parameter details please check sub
Subscribe Parameter Rules  
id | false | string | id automatically generated by the business party  
  
### sub Subscribe Parameter Rules

Parameter Name | Mandatory | Type | Description | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Pairs |  | Case-Insenstive.Both uppercase and
lowercase are supported..E.g.: "BTC_CW" stands for BTC weekly contract,
"BTC_NW" stands for BTC bi-weekly contract, "BTC_CQ" stands for BTC quarterly
contract."BTC_NQ" stands for BTC next quarterly contract. contract code is
supported too, e.g.: "BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
type | true | string | Depth Type |  | Get depth data within step 150, use
step0, step1, step2, step3, step4, step5, step14, step15（merged depth data
0-5, 14-15）；when step is 0，depth data will not be merged; Get depth data
within step 20, use step6, step7, step8, step9, step10, step11, step12,
step13(merged depth data 7-13); when step is 6, depth data will not be merged.  
  
### Note:

  * When clients choose merged depth data, WebSocket server will only display the merged price within price steps in order book. Please note that the merged depth price will not make any change on the actual order price.

  * steps between step1 and step5, step14, step15 are merged orderbook data of step 150. steps between step7 and step13 are merged orderbook data of step 20. Details are below:

Depth | precision  
---|---  
step1、step7 | 0.00001  
step2、step8 | 0.0001  
step3、step9 | 0.001  
step4、step10 | 0.01  
step5、step11 | 0.1  
step14、step12 | 1  
step15、step13 | 10  
  
> Clients can receive data if there is any update upon market depth. Example：
    
    
    {
        "ch":"market.BTC_CQ.depth.step6",
        "ts":1604385453899,
        "tick":{
            "mrid":113842765361,
            "id":1604385453,
            "bids":[
                [
                    13584.33,
                    1483
                ],
                [
                    13584,
                    1
                ]
            ],
            "asks":[
                [
                    13584.34,
                    126
                ],
                [
                    13584.35,
                    24
                ]
            ],
            "ts":1604385453896,
            "version":1604385453,
            "ch":"market.BTC_CQ.depth.step6"
        }
    }
    

### Return Parameter

Parameter Name | Mandatory | Type | Description | Value Range  
---|---|---|---|---  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
ch | true | string | Data channel, Format： market.period |  
<tick> |  |  |  |  
mrid | true | long | Order ID |  
id | true | ling | tick ID |  
asks | true | object | Sell,[price(Ask price), vol(Ask orders (cont.) )],
price in ascending sequence |  
bids | true | object | Buy,[price(Bid price), vol(Bid orders(Cont.))], Price
in descending sequence |  
ts | true | long | Timestamp for depth generation; generated once every 100ms,
unit: millisecond |  
version | true | long | version ID |  
ch | true | string | Data channel, Format： market.period |  
</tick> |  |  |  |  
  
## Subscribe Incremental Market Depth Data

### To subscribe incremental market depth data, clients have to make
connection to WebSocket API Server and send subscribe request in the format
below：

{

"sub": "market.$symbol.depth.size_${size}.high_freq",

"data_type":"incremental",

"id": "id generated by client"

}

> Example of a successful request
    
    
    {
      "sub": "market.btc_cw.depth.size_20.high_freq",
      "data_type":"incremental",
      "id": "id generated by client"
    }
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
sub | true | string | the themes that need to be subscribed; the interface is
fixed at: market.$symbol.depth.size_${size}.high_freq，For parameter details
please check sub Subscribe Parameter Rules  
id | false | string | id automatically generated by the business party  
data_type | false | string | Depth size  
  
### sub Request Parameter Rules

Parameter Name | Mandatory | Type | Description | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Pairs |  | Case-Insenstive.Both uppercase and
lowercase are supported.. E.g.: "BTC_CW" stands for BTC weekly contract,
"BTC_NW" stands for BTC bi-weekly contract, "BTC_CQ" stands for BTC quarterly
contract."BTC_NQ" stands for BTC next quarterly contract. contract code is
supported too, e.g.: "BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
size | true | integer | Depth size. `20`: stands for 20 unmerged data.
`150`:stands for 150 unmerged data. |  |  
  
### Return Parameter

Parameter Name | Mandatory | Type | Description | Value Range  
---|---|---|---|---  
ts | true | int | Timestamp of Respond Generation, Unit: Millisecond |  
ch | true | string | Data channel,
Format：`market.$symbol.depth.size_${size}.high_freq` |  
<tick> |  |  |  |  
mrid | true | long | Order ID |  
id | true | long | tick ID |  
asks | true | object | Sell,[price(Ask price), vol(Ask orders (cont.) )],
price in ascending sequence |  
bids | true | object | Buy,[price(Bid price), vol(Bid orders(Cont.))], Price
in descending sequence |  
ts | true | int | Timepoint for system detecting orderbook, unit: millisecond
|  
version | true | long | version ID,auto increment ID. |  
event | true | string | event type: `update` or `snapshot` |  
ch | true | string | Data channel, Format：
`market.$symbol.depth.size_${size}.high_freq` |  
</tick> |  |  |  |  
  
### Note:

  * when `data_type` is `incremental`,`snapshot` data wil be pushed for the first time. When re-connection occurs, `snapshort` data will be pushed for the first time. 
  * `version`: auto increment in single websocket connection. `version` may be different among several websocket subscription connections.
  * orderbook will be pushed if orderbook is updated whenever `incremental` or `snapshot`.  

  * orderbook event will be checked every 30ms. If there is no orderbook event, you will not receive any orderbook data.
  * you HAVE TO maintain local orderbook data,such as updating your local orderbook bids and asks data.

> Response example:
    
    
    {
        "ch":"market.BTC_CQ.depth.size_20.high_freq",
        "tick":{
            "asks":[
                [
                    13576.41,
                    2627
                ],
                [
                    13576.53,
                    122
                ]
            ],
            "bids":[
                [
                    13576.4,
                    1648
                ],
                [
                    13574.17,
                    398
                ]
            ],
            "ch":"market.BTC_CQ.depth.size_20.high_freq",
            "event":"snapshot",
            "id":113842925649,
            "mrid":113842925649,
            "ts":1604385634838,
            "version":330099154
        },
        "ts":1604385634838
    }
    

## Subscribe Market BBO Data

### To subscribe market BBO data, clients have to make connection to WebSocket
API Server and send subscribe request in the format below：

`{`

`"sub": "market.$symbol.bbo",`

`"id": "id generated by client"`

`}`

> Example of a successful request
    
    
    {
      "sub": "market.$symbol.bbo",
      "id": "id generated by client"
    }
    
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
sub | true | string | the themes that need to be subscribed; the interface is
fixed at: market.$symbol.bbo，For parameter details please check sub Subscribe
Parameter Rules  
id | false | string | id automatically generated by the business party  
  
### Request Parameter

Parameter Name | Mandatory | Type | Description | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Pairs |  | Case-Insenstive.Both uppercase and
lowercase are supported.. E.g.: "BTC190412" stands for BTC contract with the
the delivery date of 20190412, "BTC_CW" stands for BTC weekly contract,
"BTC_NW" stands for BTC bi-weekly contract, "BTC_CQ" stands for BTC quarterly
contract."BTC_NQ" stands for BTC next quarterly contract. contract code is
supported too, e.g.: "BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
  
> Response:
    
    
    {
        "ch":"market.BTC_CQ.bbo",
        "ts":1604385767803,
        "tick":{
            "mrid":113843014986,
            "id":1604385767,
            "bid":[
                13579.06,
                1488
            ],
            "ask":[
                13579.07,
                1535
            ],
            "ts":1604385767803,
            "version":113843014986,
            "ch":"market.BTC_CQ.bbo"
        }
    }
    

### Return Parameter

Parameter Name | Mandatory | Type | Description | Value Range  
---|---|---|---|---  
ts | true | int | Timestamp of Respond Generation, Unit: Millisecond |  
ch | true | string | Data channel, Format：`market.$symbol.bbo` |  
<tick> |  |  |  |  
mrid | true | long | Order ID |  
id | true | long | tick ID |  
ask | true | object | Best Ask Quotation,[price(Ask price), vol(Ask order
(cont.) )] |  
bid | true | object | Best Bid Quotation,[price(Bid price), vol(Bid
order(Cont.))] |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
version | true | long | version ID. |  
ch | true | string | Data channel, Format： `market.$symbol.bbo` |  
</tick> |  |  |  |  
  
### Note:

  * Once Best Bid/Ask Quotations (price,volume) change, it will be pushed.

  * When the price and volume of Best Bid/Ask Quotations both change, only the latest BBO will be pushed. 

  * When the data received by the client is failed or delayed, the old data buffer in the server will be discarded.The latest BBO will be pushed.

  * version（version number). Use match id directly to ensure it is globally unique and the value of version number pushed is the largest.

## Subscribe Market Detail Data

### To subscribe market details, the clients have to make connection to
WebSocket Server and send subscribe request in the format below:

`{`

`"sub": "market.$symbol.detail",`

`"id": "id generated by client"`

`}`

> Example of Subscribe Market Detail Data：
    
    
        {
         "sub": "market.BTC_CQ.detail",
         "id": "id6"
        }
    
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
sub | true | string | the themes that need to be subscribed; the interface is
fixed at: market.$symbol.detail，For parameter details please check sub
Subscribe Parameter Rules  
id | false | string | id automatically generated by the business party  
  
### sub Subscribe Parameter Rules

Parameter Name | Mandatory | Type | Description | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | Pairs |  | Case-Insenstive.Both uppercase and
lowercase are supported..E.g.： "BTC_CW" stands for BTC Weekly contract,
"BTC_NW" stands for BTC Bi-weekly contract, "BTC_CQ" stands for BTC Quarterly
contract,"BTC_NQ" stands for BTC next quarterly contract. contract code is
supported too, e.g.: "BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
  
### Return Parameter

Parameter Name | Mandatory | Type | Description  
---|---|---|---  
ch | true | string | Data channel，Format： market.$symbol.detail.merged  
ts | true | long | Time of Respond Generation, Unit: Millisecond  
<tick> |  |  |  
id | true | long | ID  
mrid | true | long | Order ID  
open | true | decimal | Open Price  
close | true | decimal | Clos Price, the price from the latest kline is the
last order price  
high | true | decimal | High Price  
low | true | decimal | Low Price  
amount | true | decimal | Trade amount(Coins), Trade
amount(Coin)=SUM(quantity(cont.)*face value/ order price  
vol | true | decimal | Trade amount(Cont.)， the sum volume of both buy and
sell sides  
count | true | decimal | fulfilled order quantity  
</tick> |  |  |  
  
> Example of a successful return data：
    
    
    {
        "ch":"market.BTC_CQ.detail",
        "ts":1604385863717,
        "tick":{
            "id":1604385840,
            "mrid":113843084999,
            "open":13607.17,
            "close":13589,
            "high":13830.63,
            "low":13411.89,
            "amount":261417.4288915740193389700120854767791857974,
            "vol":35572590,
            "count":586972
        }
    }
    

## Request Trade Detail Data

### To request Trade detail data, Clients have to make connection to the
WebSocket Server and send request data in the format below：

`{`

`"req": "market.$symbol.trade.detail",`

`"id": "id generated by client"` // “id” string is optional currently. Server
will return with null because client ID is not necessary

`}`

Return to the current trade detail data only

> Example of requesting market detail data：
    
    
    
        {
         "req": "market.BTC_CQ.trade.detail",
         "size": 10,
         "id": "id8"
        }
    
    

### Subscribe Parameter

Parameter Name | Mandatory | Type | Description | Default  
---|---|---|---|---  
req | true | string | Theme for Requesting Data; the interface is fixed at:
market.$symbol.trade.detail; for details of the parameter please check req
Request Parameter Rules |  
id | false | string | id automatically generated by the business party |  
size | false | int | number of data; no more than 50; default 50 if not filled
| [1,50]  
  
### req Request Parameter Rules

Parameter Name | Mandatory | Type | Description | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | contract type |  | Case-Insenstive.Both uppercase and
lowercase are supported..E.g.: "BTC_CW" stands for BTC weekly contract,
"BTC_NW" stands for BTC bi-weekly contract, "BTC_CQ" stands for BTC quarterly
contract."BTC_NQ" stands for BTC next quarterly contract. contract code is
supported too, e.g.: "BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
  
> Example of a successful return data：
    
    
    {
        "data":[
            {
                "amount":"4",
                "ts":1604386167285,
                "id":1138433247400000,
                "price":"13586.25",
                "direction":"buy"
            },
            {
                "amount":"20",
                "ts":1604386167469,
                "id":1138433248730000,
                "price":"13586.25",
                "direction":"buy"
            }
        ],
        "id":"id8",
        "rep":"market.BTC_CQ.trade.detail",
        "status":"ok",
        "ts":1604386202755
    }
    

### Return Parameter

Parameter Name | Mandatory | Type | Description | Default  
---|---|---|---|---  
rep | true | string | Data Channel，Format： market.$symbol.trade.detail |  
status | true | string | Request Status |  
id | true | string | Request ID |  
<data> |  |  |  |  
id | true | long | Unique Transaction Id(symbol level) |  
price | true | string | Price |  
amount | true | string | Trade amount(Coin), trade amount(coin)=sum(order
quantity of a single order * face value of the coin/order price) |  
direction | true | string | Active transaction direction |  
ts | true | long | Order Creation Time |  
</data> |  |  |  |  
ts | true | long | server response time |  
  
## Subscribe Trade Detail Data

### To subscribe trade detail data, the Client has to make connection to the
Server and send subscribe request in the format below：

`{`

`"sub": "market.$symbol.trade.detail",`

`"id": "id generated by client"`

`}`

> Example of a successful subscribe request：
    
    
        {
         "sub": "market.BTC_CQ.trade.detail",
         "id": "id7"
        }
    
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
sub | true | string | the themes that need to be subscribed; the interface is
fixed at:market.$symbol.trade.detail，For parameter details please check sub
Subscribe Parameter Rules  
id | false | string | id automatically generated by the business party  
  
### sub Subscribe Parameter Rules

Parameter Name | Mandatory | Type | Description | Default | Value Range  
---|---|---|---|---|---  
symbol | true | string | contract type |  | Case-Insenstive.Both uppercase and
lowercase are supported..E.g.: "BTC_CW" stands for BTC weekly contract,
"BTC_NW" stands for BTC bi-weekly contract, "BTC_CQ" stands for BTC quarterly
contract."BTC_NQ" stands for BTC next quarterly contract. contract code is
supported too, e.g.: "BTC200918"(weekly), "BTC200925"(Bi-
weekly),"BTC201225"(quarterly),"BTC210326"(next quarterly)  
  
### Return Parameter

Parameter Name | Mandatory | Type | Description | Default  
---|---|---|---|---  
ch | true | string | Data channel,format: market.$symbol.trade.detail |  
ts | true | long | server response time |  
<tick> |  |  |  |  
id | true | long | Unique Order Id(symbol level). |  
ts | true | long | tick time |  
<data> |  |  |  |  
amount | true | decimal | quantity(Cont.) |  
ts | true | long | trade timestamp |  
id | true | long | Unique Transaction Id(symbol level) |  
price | true | decimal | Price |  
direction | true | string | Order direction |  
</data> |  |  |  |  
</tick> |  |  |  |  
  
> When there is any update upon trade detail data, clients will receive
> notification from server. Example：
    
    
    {
        "ch":"market.BTC_CQ.trade.detail",
        "ts":1604386599136,
        "tick":{
            "id":113843672389,
            "ts":1604386599123,
            "data":[
                {
                    "amount":120,
                    "ts":1604386599123,
                    "id":1138436723890000,
                    "price":13562.5,
                    "direction":"sell"
                },
                {
                    "amount":2,
                    "ts":1604386599123,
                    "id":1138436723890001,
                    "price":13562.5,
                    "direction":"sell"
                }
            ]
        }
    }
    

# WebSocket Index and Basis Interface

### The websocket url of Index and Basis Data is：wss://api.hbdm.com/ws_index

## Subscribe Index Kline Data

### To subscribe index kline data, the Client has to make connection to the
Server and send subscribe request in the format below:

`{`

`"sub": "market.$symbol.index.$period",`

`"id": "id generate by client"`

`}`

> example of the subscription of index kline data：
    
    
        {
        "sub": "market.BTC-USD.index.1min",
        "id": "id1"
        }
    
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
sub | true | string | the themes that need to be subscribed; the interface is
fixed at: market.$symbol.index.$period，For parameter details please check sub
Subscribe Parameter Rules  
id | false | string | id automatically generated by the business party  
  
### sub Subscribe Parameter Rules

**Parameter Name** | **Mandatory** | **Type** | **Desc** | **Default** |
**Value Range**  
---|---|---|---|---|---  
symbol | true | string | index symbol |  | Case-Insenstive.Both uppercase and
lowercase are supported.."BTC-USD","ETH-USD"...  
period | true | string | kline type |  | 1min, 5min, 15min, 30min,
60min,4hour,1day, 1mon  
  
### Note

  * Pushed once the index data is changed.

  * Periodical Push when the index data hasn't changed according to the kline period.

> results pushed by the server
    
    
    {
        "ch":"market.BTC-USD.index.1min",
        "ts":1604387688243,
        "tick":{
            "id":1604387640,
            "open":"13419.4325",
            "close":"13420.3325",
            "high":"13424.4925",
            "low":"13419.4325",
            "amount":"0",
            "vol":"0",
            "count":0
        }
    }
    

### Returning Parameter

**parameter name** | **Mandatory** | **type** | **desc** | **Value Range**  
---|---|---|---|---  
ch | true | string | Data channel，Format：market.$symbol.index.$period |  
tick | true | object array | Details：tick parameters |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
### tick parameters

**parameter name** | **type** | **desc** |  
---|---|---|---  
id | string | index kline id,the same as kline timestamp,kline start timestamp
|  
vol | string | Trade Volume. The value is 0. |  
count | decimal | count. The value is 0. |  
open | string | open index price |  
close | string | close index price |  
low | string | lowest index price |  
high | string | highest index price |  
amount | string | amount based on coins. |  
  
## Request Index Kline Data

### To subscribe index kline data, the Client has to make connection to the
Server and send subscribe request in the format below:

`{`

`"req": "market.$symbol.index.$period",`

`"id": "id generated by client",`

`"from": "type: long, from 2017-07-28T00:00:00+08:00 to
2050-01-01T00:00:00+08:00",`

`"to": "type: long, from 2017-07-28T00:00:00+08:00 to
2050-01-01T00:00:00+08:00 .Larger than 'from' value. ",`

`}`

> example of the subscription of index kline data：
    
    
      {
        "req": "market.bct-usd.index.1min",
        "id": "id4",
        "from":1571000000,
        "to":1573098606
      }
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
req | true | string | the themes that need to be subscribed; the interface is
fixed at: market.$symbol.index.$period，For parameter details please check req
Subscribe Parameter Rules  
id | false | string | id automatically generated by the business party  
from | true | long | start time, from 2017-07-28T00:00:00+08:00 to
2050-01-01T00:00:00+08:00. timestamp unit：seconds  
to | true | long | end time, from 2017-07-28T00:00:00+08:00 to
2050-01-01T00:00:00+08:00. timestamp unit：seconds. larger than 'from' value  
  
### req Subscribe Parameter Rules：

**Parameter Name** | **Mandotary** | **Type** | **Desc** | **Default** |
**Value Range**  
---|---|---|---|---|---  
symbol | true | string | symbol |  | Case-Insenstive.Both uppercase and
lowercase are supported.."BTC-USD","ETH-USD"...  
period | true | string | kline type |  | 1min, 5min, 15min, 30min,
60min,4hour,1day, 1mon  
  
### Note：

  * Pushed once the index data is changed.

> response example：
    
    
    {
        "id":"id4",
        "rep":"market.BTC-USD.index.60min",
        "wsid":915217437,
        "status":"ok",
        "data":[
            {
                "id":1604160000,
                "open":13862.65,
                "close":13832.615,
                "low":13822.41,
                "high":13890.2225,
                "amount":0,
                "vol":0,
                "count":0
            },
            {
                "id":1604163600,
                "open":13832.7725,
                "close":13788.6625,
                "low":13751.9075,
                "high":13833.41,
                "amount":0,
                "vol":0,
                "count":0
            }
        ]
    }
    

### Returning Parameter

**parameter name** | **Mandatory** | **type** | **desc** | **Value Range**  
---|---|---|---|---  
req | true | string | Data channel，Format：market.$symbol.index.$period |  
status | true | string | Request processing result | "ok" , "error"  
id | true | string | ID |  
wsid | true | long | wsid |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
data | true | object array | Details：data parameters |  
  
### data parameters

**parameter name** | **type** | **desc** |  
---|---|---|---  
id | int | index kline id,the same as kline timestamp,kline start timestamp |  
vol | decimal | Trade Volume. The value is 0. |  
count | decimal | count. The value is 0. |  
open | decimal | open index price |  
close | decimal | close index price |  
low | decimal | lowest index price |  
high | decimal | highest index price |  
amount | decimal | amount based on coins. |  
  
## Subscribe Basis Data

### To subscribe basis data, the Client has to make connection to the Server
and send subscribe request in the format below:

`{`

`"sub": "market.$symbol.basis.$period.$basis_price_type",`

`"id": "id generate by client"`

`}`

> example of the subscription of basis data：
    
    
        {
        "sub": "market.BTC_CW.basis.1min.open",
        "id": "id1"
        }
    
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
sub | true | string | the themes that need to be subscribed; the interface is
fixed at: market.$symbol.basis.$period.$basis_price_type，For parameter details
please check sub Subscribe Parameter Rules  
id | false | string | id automatically generated by the business party  
  
### sub Subscribe Parameter Rules：

**Parameter Name** | **Mandotary** | **Type** | **Desc** | **Default** |
**Value Range**  
---|---|---|---|---|---  
symbol | true | string | symbol name |  | Case-Insenstive.Both uppercase and
lowercase are supported..e.g. "BTC_CW" represents BTC “This Week”，"BTC_NW"
represents BTC “Next Week”，"BTC_CQ" represents BTC “Quarter”."BTC_NQ"
represents BTC “Next Quarter”.  
period | true | string | kline period |  | 1min,5min, 15min, 30min,
60min,4hour,1day,1mon  
basis_price_type | false | string | use basis price type to calculate the
basis data | Using open price default | open price："open"，close
price："close"，highest price："high"，lowest price："low"，avg=（high price +low
price）/2："average"  
  
#### Note:

  * The basis data of Next Quarterly Contract is available after 2020/6/15 14:00:00.

> Response Example
    
    
    {
        "ch":"market.BTC_CW.basis.5min.close",
        "ts":1604387856115,
        "tick":{
            "id":1604387700,
            "index_price":"13434.5075",
            "contract_price":"13454.01",
            "basis":"19.5025",
            "basis_rate":"0.0014516721212147151654052074480586653"
        }
    }
    

### Returning Parameter

**parameter name** | **Mandatory** | **type** | **desc** | **Value Range**  
---|---|---|---|---  
ch | true | string | Data
channel，Format：market.$symbol.basis.$period.$basis_price_type |  
tick | true | object array | Details：tick parameters |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
  
### tick Parameters

**parameter name** | **Mandatory** | **Type** | **Desc** | **Value Range**  
---|---|---|---|---  
id | true | long | unique id |  
contract_price | true | string | contract last price |  
index_price | true | string | index price |  
basis | true | string | basis=contract_price - index_price |  
basis_rate | true | string | basis_rate=basis/index_price |  
  
## Request Basis Data

### To subscribe basis data, the Client has to make connection to the Server
and send subscribe request in the format below:

`{`

`"req": "market.$symbol.basis.$period.$basis_price_type",`

`"id": "id generated by client",`

`"from": "type: long, from 2017-07-28T00:00:00+08:00 to
2050-01-01T00:00:00+08:00",`

`"to": "type: long, from 2017-07-28T00:00:00+08:00 to
2050-01-01T00:00:00+08:00 .Larger than 'from' value. "`

`}`

> example of the subscription of basis data：
    
    
      {
        "req": "market.btc_cw.basis.1min.open",
        "id": "id4",
        "from":1571000000,
        "to":1573098606
      }
    

### Request Parameter

Parameter Name | Mandatory | Type | Desc  
---|---|---|---  
req | true | string | the themes that need to be subscribed; the interface is
fixed at: market.$symbol.basis.$period.$basis_price_type，For parameter details
please check req Subscribe Parameter Rules  
id | false | string | id automatically generated by the business party  
from | true | long | start time, from 2017-07-28T00:00:00+08:00 to
2050-01-01T00:00:00+08:00. timestamp unit：seconds  
to | true | long | end time, from 2017-07-28T00:00:00+08:00 to
2050-01-01T00:00:00+08:00. timestamp unit：seconds. larger than 'from' value  
  
### req Subscribe Parameter Rules：

**Parameter Name** | **Mandotary** | **Type** | **Desc** | **Default** |
**Value Range**  
---|---|---|---|---|---  
symbol | true | string | symbol name |  | Case-Insenstive.Both uppercase and
lowercase are supported..e.g. "BTC_CW" represents BTC “This Week”，"BTC_NW"
represents BTC “Next Week”，"BTC_CQ" represents BTC “Quarter”."BTC_NQ"
represents BTC “Next Quarter”.  
period | true | string | kline type |  | 1min, 5min, 15min, 30min,
60min,4hour,1day, 1mon  
basis_price_type | false | string | use basis price type to calculate the
basis data | Using open price default | open price："open"，close
price："close"，highest price："high"，lowest price："low"，avg=（high price +low
price）/2："average"  
  
### Note：

  * 2000 data at most per request.

> response example：
    
    
    {
        "data":[
            {
                "basis":"20.357500000000073",
                "basis_rate":"0.0014671752201438544",
                "contract_price":"13895.66",
                "id":1604160000,
                "index_price":"13875.3025"
            },
            {
                "basis":"20.13249999999971",
                "basis_rate":"0.001454177342461542",
                "contract_price":"13864.73",
                "id":1604160300,
                "index_price":"13844.5975"
            }
        ],
        "id":"id4",
        "rep":"market.BTC_CW.basis.5min.close",
        "status":"ok",
        "ts":1604387965575,
        "wsid":3823737955
    }
    

### Returning Parameter

**parameter name** | **Mandatory** | **type** | **desc** | **Value Range**  
---|---|---|---|---  
req | true | string | Data
channel，Format：market.$symbol.basis.$period.$basis_price_type |  
status | true | string | Request processing result | "ok" , "error"  
id | true | string | ID |  
wsid | true | long | wsid |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
tick | true | object array | Details：tick parameters |  
  
### tick Parameters

**parameter name** | **Mandatory** | **Type** | **Desc** | **Value Range**  
---|---|---|---|---  
id | true | long | unique id |  
contract_price | true | string | contract last price |  
index_price | true | string | index price |  
basis | true | string | basis=contract_price - index_price |  
basis_rate | true | string | basis_rate=basis/index_price |  
  
# Orders and Accounts WebSocket Interfaces

## Subscribe Order Data(sub)

To subscribe order data, Clients have to make connection to the Server and
send subscribe request in the format below:

### Subscribe Request Format

`{`

`“op”: “sub”,`

`"cid": "id generated by client”,`

`“topic": "orders.$symbol”`

`}`

> Example of a successful subscribe request:
    
    
    {
      "op": "sub",
      "cid": "40sG903yz80oDFWr",
      "topic": "orders.btc"
    }
    
    

### Data format illustration of orders subscription

Field Name | Type | Description  
---|---|---  
op | string | Required； Operator Name，required subscribe value is sub  
cid | string | Optional; ID Client requests unique ID  
topic | string | Required；Topic name format: orders.$symbol; symbol is case-
insenstive.Both uppercase and lowercase are supported. e.g.:"BTC,ETH"  
  
#### Note:

  * The order status of 'post_only' type pushed by ws is ethier '7:canceled' or '3:submitted'.

> Illustration on detailed data format of orders Notification
    
    
    {
        "op":"notify",
        "topic":"orders.ada",
        "ts":1604388667226,
        "symbol":"ADA",
        "contract_type":"quarter",
        "contract_code":"ADA201225",
        "volume":1,
        "price":0.0905,
        "order_price_type":"post_only",
        "direction":"sell",
        "offset":"open",
        "status":6,
        "lever_rate":20,
        "order_id":773207641127878656,
        "order_id_str":"773207641127878656",
        "client_order_id":null,
        "order_source":"web",
        "order_type":1,
        "created_at":1604388667146,
        "trade_volume":1,
        "trade_turnover":10,
        "fee":-0.022099447513812154,
        "trade_avg_price":0.0905,
        "margin_frozen":0,
        "profit":0,
        "trade":[
            {
                "trade_fee":-0.022099447513812154,
                "fee_asset":"ADA",
                "trade_id":113913755890,
                "id":"113913755890-773207641127878656-1",
                "trade_volume":1,
                "trade_price":0.0905,
                "trade_turnover":10,
                "created_at":1604388667194,
                "role":"maker"
            }
        ],
        "canceled_at":0,
        "fee_asset":"ADA",
        "uid":"123456789",
        "liquidation_type":"0"
    }
    

### Format Illustration on return data of order push

Filed Name | Type | Description  
---|---|---  
op | string | Required;Operator Name，Order push value is notify ;  
topic | string | Required; Order push topic  
uid | string | account uid  
ts | long | Server responses timestamp  
symbol | string | Coin  
contract_type | string | Contract Type  
contract_code | string | Contract Code  
volume | decimal | Order quantity  
price | decimal | Order price  
order_price_type | string | Order price type
"limit":Limit,"opponent":opponent,"post_only":Post-Only Order, No order limit
but position limit for post-only orders.，"lightning":lightning,
"optimal_5":optimal 5，"optimal_10":optimal 10，"optimal_20":optimal
20，"fok":FOK Order，"ioc":IOC Order, "opponent_ioc": opponent
ioc，"lightning_ioc": lightning ioc，"optimal_5_ioc": optimal_5
ioc，"optimal_10_ioc": optimal_10 ioc，"optimal_20_ioc"：optimal_20
ioc，"opponent_fok"： opponent fok，"lightning_fok"：lightning
fok，"optimal_5_fok"：optimal_5 fok，"optimal_10_fok"：optimal_10
fok，"optimal_20_fok"：optimal_20 fok  
direction | string | "buy" Long "sell": Short  
offset | string | "open": Open "close": Close  
status | int | Order status(1. Placing orders to order book; 2 Placing orders
to order book; 3. Placed to order book 4. Partially fulfilled; 5 partially
fulfilled but cancelled by client; 6. Fully fulfilled; 7. Cancelled;)  
lever_rate | int | Leverage  
order_id | long | Order ID  
order_id_str | string | Order ID  
client_order_id | long | Client ID  
order_source | string | Order
source(system、web、api、m、risk、settlement、ios、android、windows、mac、trigger)  
order_type | int | Order type 1Requested orders; 2. Cancelled orders; 3.
Liquidated orders; 4. Delivered orders  
created_at | long | order creation time  
canceled_at | long | order canceled time  
trade_volume | decimal | trade volume(volume)  
trade_turnover | decimal | Turnover  
fee | decimal | Fees  
trade_avg_price | decimal | Average order price  
margin_frozen | decimal | Frozen Margin  
profit | decimal | Profits&Losses  
fee_asset | string | the corresponding cryptocurrency to the given fee  
liquidation_type | string | 0:Not Forced Liquidation Type，1：Netting Type， 2:
Partial Takeover，3：All Takeover  
<trade> |  |  
id | string | the global unique id of the trade.。  
trade_id | long | In this interface, trade_id is the same with match_id of
api/v1/contract_matchresults. trade_id is the result of sets of order
execution and trade confirmation. NOTE: trade_id is not unique, which includes
all trade records of a taker order and N maker orders. If the taker order
matches with N maker orders, it will create N trades with same trade_id.  
trade_volume | decimal | trade volume  
trade_price | decimal | trade price  
trade_fee | decimal | trading fees  
trade_turnover | decimal | turnover  
created_at | long | trade creation time  
role | string | taker or maker  
fee_asset | string | fee asset  
</trade> |  |  
  
## Unsubscribe Order Data（unsub）

To unsubscribe order data, the clients have to make connection to the server
and send unsubscribe request in the format below:

### Format of Unsubscribe order data

`{`

`“op”: “unsub”,`

`“topic": "orders.$symbol”,`

`"cid": "id generated by client”,`

`}`

> Example of a successful unsubscribe request：
    
    
    {
      "op": "unsub",
      "topic": "orders.btc",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### Format illustration of unsubscribe order data

Filed | Type | Description  
---|---|---  
op | string | Required;Operator Name，value for unsubscribe is unsub;  
cid | string | Optional; Client requests unique ID  
topic | string | Required；Unsubscribe topic name: orders.$symbol; symbol is
case-insenstive.Both uppercase and lowercase are supported.e.g: "BTC,ETH" ;
when $symbol value is *, it stands for unsubscribing the data of all coins;  
  
### Rules on Subscribe and Unsubscribe

Subscribe(sub) | Unsubscribe( unsub) ) | Rule  
---|---|---  
orders.* | orders.* | Allowed  
orders.symbol1 | orders.* | Not Allowed  
orders.symbol1 | orders.symbol1 | Allowed  
orders.symbol1 | orders.symbol2 | Not Allowed  
orders.* | orders.symbol1 | Not Allowed  
  
## Subscribe Match Order Data（sub）

To subscribe order data, Clients have to make connection to the Server and
send subscribe request in the format below:

### Subscribe Request Format

`{`

`“op”: “sub”,`

`"cid": "cid”,`

`“topic": "matchOrders.$symbol”`

`}`

> sub example:
    
    
    {
      "op": "sub",
      "cid": "40sG903yz80oDFWr",
      "topic": "matchOrders.btc"
    }
    
    

### Format of subscribe match order data

attr | type | desc  
---|---|---  
op | string | Required； Operator Name，required subscribe value is sub  
cid | string | Optional; ID Client requests unique ID  
topic | string | Required；Topic name format: matchOrders.$symbol; symbol is
case-insenstive.Both uppercase and lowercase are supported. e.g.:"BTC,ETH"  
  
> Illustration on detailed data format of orders Notification

#### Note:

  * The order status of 'post_only' type pushed by ws is ethier '7:canceled' or '3:submitted'.
  * The orders will be pushed when matched by matching engine.
  * The delivery orders will not be pushed.
  * The orders transfered from future or to future will not be pushed.
  * The netting and forced liquidation orders will not be pushed.
  * The orders will generally be pushed faster than the normal orders subscription.But It's not guranted.
  * If there is an order with N trades,including 1 taker and N maker,it will push N+1 trades at most.
  * If there is a status with 9 or 10,pls ignore it.

> response
    
    
    {
        "op":"notify",
        "topic":"matchOrders.ada",
        "ts":1604388667219,
        "symbol":"ADA",
        "contract_code":"ADA201225",
        "contract_type":"quarter",
        "status":6,
        "order_id":773207641127878656,
        "order_id_str":"773207641127878656",
        "client_order_id":null,
        "order_type":1,
        "created_at":1604388667146,
        "trade":[
            {
                "trade_id":113913755890,
                "id":"113913755890-773207641127878656-1",
                "trade_volume":1,
                "trade_price":0.0905,
                "trade_turnover":10,
                "created_at":1604388667194,
                "role":"maker"
            }
        ],
        "uid":"123456789",
        "volume":1,
        "trade_volume":1,
        "direction":"sell",
        "offset":"open",
        "lever_rate":20,
        "price":0.0905,
        "order_source":"web",
        "order_price_type":"post_only"
    }
    

### format of order data pushed

Parameter Name | Type | Desc  
---|---|---  
op | string | notify;  
topic | string | topic  
uid | string | account uid  
ts | long | Time of Respond Generation  
symbol | string | symbol  
contract_type | string | contract type  
contract_code | string | contract code  
status | int | 1\. Ready to submit the orders; 2. Ready to submit the orders;
3. Have sumbmitted the orders; 4. Orders partially matched; 5. Orders
cancelled with partially matched; 6. Orders fully matched; 7. Orders
cancelled;  
order_id | bigint | order id  
order_id_str | string | order id  
client_order_id | long | the client ID that is filled in when the order is
placed  
order_type | int | Order type: 1. Quotation; 2. Cancelled order; 3. Forced
liquidation; 4. Delivery Order  
trade_volume | decimal | total filled volume of the order  
volume | decimal | total volume of the order  
<trade> |  |  
id | string | the global unique id of the trade.  
trade_id | long | In this interface, trade_id is the same with match_id of
api/v1/contract_matchresults. trade_id is the result of sets of order
execution and trade confirmation. NOTE: trade_id is not unique, which includes
all trade records of a taker order and N maker orders. If the taker order
matches with N maker orders, it will create N trades with same trade_id.  
trade_volume | decimal | trade volume  
trade_price | decimal | trade price  
trade_turnover | decimal | trade turnover  
created_at | long | created at  
role | string | taker or maker  
</trade> |  |  
direction | string | direction "buy" or "sell"  
offset | string | offset: "open" or "close"  
lever_rate | int | lever rate  
price | decimal | trigger price  
created_at | long | created at  
order_source | string | order source  
order_price_type | string | order price type:
"limit":Limit,"opponent":opponent,"post_only":Post-Only Order, No order limit
but position limit for post-only orders.，"lightning":lightning,
"optimal_5":optimal 5，"optimal_10":optimal 10，"optimal_20":optimal
20，"fok":FOK Order，"ioc":IOC Order, "opponent_ioc": opponent
ioc，"lightning_ioc": lightning ioc，"optimal_5_ioc": optimal_5
ioc，"optimal_10_ioc": optimal_10 ioc，"optimal_20_ioc"：optimal_20
ioc，"opponent_fok"： opponent fok，"lightning_fok"：lightning
fok，"optimal_5_fok"：optimal_5 fok，"optimal_10_fok"：optimal_10
fok，"optimal_20_fok"：optimal_20 fok  
  
## Unsubscribe Match Order Data（unsub）

To unsubscribe order data, the clients have to make connection to the server
and send unsubscribe request in the format below:

### Format of Unsubscribe order data

`{`

`“op”: “unsub”,`

`“topic": "matchOrders.$symbol”,`

`"cid": "id generated by client”,`

`}`

> Example of a successful unsubscribe request：
    
    
    {
      "op": "unsub",
      "topic": "matchOrders.btc",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### Format illustration of unsubscribe order data

Filed | Type | Description  
---|---|---  
op | string | Required;Operator Name，value for unsubscribe is unsub;  
cid | string | Optional; Client requests unique ID  
topic | string | Required；Unsubscribe topic name: matchOrders.$symbol; symbol
is case-insenstive.Both uppercase and lowercase are supported.e.g: "BTC,ETH" ;
when $symbol value is *, it stands for unsubscribing the data of all coins;  
  
### Rules on Subscribe and Unsubscribe

Subscribe(sub) | Unsubscribe( unsub) ) | Rule  
---|---|---  
matchOrders.* | matchOrders.* | allowed  
matchOrders.symbol1 | matchOrders.* | Not Allowed  
matchOrders.symbol1 | matchOrders.symbol1 | allowed  
matchOrders.symbol1 | matchOrders.symbol2 | Not Allowed  
matchOrders.* | matchOrders.symbol1 | Not Allowed  
  
## Subscribe Account Equity Updates Data(sub)

To subscribe accounts equity data updates, the client has to make connection
to the server and send subscribe request in the format below:

### Request Format for Subscribe Account Equity Updates Data

`{`

`"op": "sub",`

`"cid": "id generated by client”,`

`“topic": "accounts.$symbol”`

`}`

> Example of a successful subscribe request:
    
    
    {
      "op": "sub",
      "cid": "40sG903yz80oDFWr",
      "topic": "accounts.btc"
    }
    
    

### Format illustration on request subscribe account equity updates data

Field Name | Type | Description  
---|---|---  
op | string | Required； Operator Name，Subscribe value is sub  
cid | string | Optional; Client requests unique ID  
topic | string | Required；Topic name format: accounts.$symbol; symbol is case-
insenstive.Both uppercase and lowercase are supported. e.g.:"BTC,ETH"  
  
> When there is any balance change, the Server will send a notification with
> the return parameter. For example:
    
    
    {
        "op":"notify",
        "topic":"accounts.ada",
        "ts":1604388667226,
        "event":"order.match",
        "data":[
            {
                "symbol":"ADA",
                "margin_balance":446.417641681222726716,
                "margin_static":445.554085945257745136,
                "margin_position":11.049723756906077348,
                "margin_frozen":0,
                "margin_available":435.367917924316649368,
                "profit_real":21.627049781983019459,
                "profit_unreal":0.86355573596498158,
                "risk_rate":40.000796572150656768,
                "liquidation_price":0.018674308027108984,
                "withdraw_available":423.927036163274725677,
                "lever_rate":20,
                "adjust_factor":0.4
            }
        ],
        "uid":"123456789"
    }
    

### Format Illustration of Notification

Field Name | Type | Description  
---|---|---  
op | string | notify;  
topic | string | topic  
uid | string | account uid  
ts | long | Time of Respond Generation, Unit: Millisecond  
event | string | notification on account asset change such as commit
order(order.open), fulfill order(order.match)(excluding liquidated order and
settled orders), settlement and delivery(settlement), fulfill liquidation
order(order.liquidation)(including voluntarily fulfilled liquidation order and
the fulfilled liquidation order taken over by system ) , cancel
order(order.cancel), asset transfer（contract.transfer) (including withdraw and
deposit), system (contract.system), other asset change(other), switch
leverages(switch_lever_rate), initial margin(init)  
<data> |  |  
symbol | string | Coins. When the $symbol value is “*”, it stands for
subscribing data of all coins  
margin_balance | decimal | Account Equity  
margin_static | decimal | Static Equity  
margin_position | decimal | Position Margi(the margin for holding currenty
positions)  
margin_frozen | decimal | Frozen Margin  
margin_available | decimal | Available Margin  
profit_real | decimal | Realized Profits&Losses  
profit_unreal | decimal | Unrealized Profits&Losses  
risk_rate | decimal | Margin Ratio  
liquidation_price | decimal | Liquidation Price  
withdraw_available | decimal | Assets available to withdraw  
lever_rate | decimal | Leverage  
adjust_factor | decimal | Adjustment Factor  
</data> |  |  
  
### Note

  * A regular push of account is performed every 5 sedconds.The event field of the reponse is "snapshot".If there is a push in 5 seconds, snapshot push will be skipped.

## Unsubscribe Account Equity Updates Data (ubsub)

To unsubscribe account equity updates data, the client has to make connection
to the server and send unsubscribe request in the format below:

### Request Format of Unsubscribe Account Equity Updates Data

`{`

`“op”: “unsub”,`

`“topic": "accounts.$symbol”,`

`"cid": "id generated by client”,`

`}`

> Example of a successful subscription request
    
    
    {
      "op": "unsub",
      "topic": "accounts.btc",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### Format Illustration on Unsubscribe Account Equity Updates

Filed Name | Type | Description  
---|---|---  
op | string | Required; Operator Name，Subscribe value is unsub;  
cid | string | Optional; Client requests unique ID  
topic | string | Required；Unsubscribe topic name: accounts.$symbol; symbol is
case-insenstive.Both uppercase and lowercase are supported.e.g: "BTC,ETH" ;
when $symbol value is *, it stands for unsubscribing the data of all coins;  
  
### Rules on Subscribe and Unsubscribe

Subscribe(sub) | Unsubscribe(unsub) | Rule  
---|---|---  
accounts.* | accounts.* | Allowed  
accounts.symbol1 | accounts.* | Allowed  
accounts.symbol1 | accounts.symbol1 | Allowed  
accounts.symbol1 | accounts.symbol2 | Not Allowed  
accounts.* | accounts.symbol1 | Not Allowed  
  
## Subscribe Position Updates(sub)

To subscribe position updates data, the client has to make connection to the
server and send subscribe request in the format below:

### Subscribe Request Format

`{`

`“op”: “sub”,`

`"cid": "id generated by client”,`

`“topic": "positions.$symbol”`

`}`

> Example of a successful subscribe request:
    
    
    {
      "op": "sub",
      "cid": "40sG903yz80oDFWr",
      "topic": "positions.btc"
    }
    
    

### Format Illustration of Subscribe Position Updates

Filed Name | Type | Description  
---|---|---  
op | string | Required；Operator Name，Subscribe value is sub  
cid | string | Optional ; Client requests unique ID  
topic | string | Required；Topic name format: positions.$symbol; symbol is
case-insenstive.Both uppercase and lowercase are supported. e.g.:"BTC,ETH"  
  
> When there is any position update, the server will send notification with
> return parameter. For example:
    
    
    {
        "op":"notify",
        "topic":"positions.ada",
        "ts":1604388667226,
        "event":"order.match",
        "data":[
            {
                "symbol":"ADA",
                "contract_code":"ADA201225",
                "contract_type":"quarter",
                "volume":1,
                "available":1,
                "frozen":0,
                "cost_open":0.0905,
                "cost_hold":0.0905,
                "profit_unreal":0,
                "profit_rate":0,
                "profit":0,
                "position_margin":5.524861878453038674,
                "lever_rate":20,
                "direction":"sell",
                "last_price":0.0905
            }
        ],
        "uid":"123456789"
    }
    

### Return Parameter Illustration

Filed Name | Type | Description  
---|---|---  
op | string | notify;  
topic | string | topic  
uid | string | account uid  
ts | long | Time of Respond Generation, Unit: Millisecond  
event | string | Related events of position change notification, such as order
creation and position closing (order.close), order filled (order.match)
(except for liquidation, settlement and delivery), settlement and delivery
(settlement), order liquidation (order.liquidation), order cancellation
(order.cancel),switch leverage（switch_lever_rate）, initial positions (init),
triggered by system periodic push (snapshot).  
<data> |  |  
symbol | string | Coin, when $symbol value is *, it stands for subscribing the
data of all coins  
contract_code | string | Contract Code  
contract_type | string | Contract Type, Weekly contract: "this_week", Bi-
weeklycontract: "next_week", Quarterly Contract: "quarter", Next Quarterly
Contract: "next_quarter"“delivered”  
volume | decimal | Open Interest  
available | decimal | Positions available to close  
frozen | decimal | Frozen Margin  
cost_open | decimal | Open price  
cost_hold | decimal | Position Price  
profit_unreal | decimal | Unrealized Profits&Losses  
profit_rate | decimal | Profit/Losses Ratio  
profit | decimal | Profits/Losses  
position_margin | decimal | Position Margin  
lever_rate | decimal | Leverage  
direction | string | Position direction "buy":Long "sell":Short  
last_price | decimal | Last Price  
</data> |  |  
  
### Note

  * A regular push of position is performed every 5 sedconds.The event field of the reponse is "snapshot".If there is a push in 5 seconds, snapshot push will be skipped.

  * When switching leverage with no positions, the event "switch_lever_rate" will not be pushed by the position topic.

## Unsubscribe Position Updates Data(unsub)

To unsubscribe, the client has to make connection to the server and send
unsubscribe request in the format below:

### Request Format of Unsubscribe Position Updates

`{`

`“op”: “unsub”,`

`“topic": "positions.$symbol”,`

`"cid": "id generated by client”,`

`}`

> Example of a successful unsubscribe request:
    
    
    {
      "op": "unsub",
      "topic": "positions.btc",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### Format Illustration of Unsubscribe Position Updates

Field Name | Type | Description  
---|---|---  
op | string | Required; Operator Name，Subscribe value is unsub;  
cid | string | Optional; Client requests unique ID  
topic | string | Required；Unsubscribe topic name: positions.$symbol; symbol is
case-insenstive.Both uppercase and lowercase are supported.e.g: "BTC,ETH" ;
when $symbol value is *, it stands for unsubscribing the data of all coins;  
  
### Rules on Subscribe and Unsubscribe

Subscribe(sub) | Unsubscribe(unsub) | Rule  
---|---|---  
positions.* | positions.* | Allowed  
positions.symbol1 | positions.* | Allowed  
positions.symbol1 | positions.symbol1 | Allowed  
positions.symbol1 | positions.symbol2 | Not Allowed  
positions.* | positions.symbol1 | Not Allowed  
  
## Subscribe Liquidation Order Data(No authentication) (sub)

### Subscription Request Format of Liquidation order data

`{`

`“op”: “sub”,`

`“topic": "public.$symbol.liquidation_orders”,`

`"cid": "id generated by client”,`

`}`

> Example of a successful subscription request:
    
    
    {
      "op": "sub",
      "cid": "40sG903yz80oDFWr",
      "topic": "public.BTC.liquidation_orders"
    }
    
    

### Data format illustration of orders subscription

Field Name | Type | Description  
---|---|---  
op | string | Required； Operator Name，required subscribe value is sub  
cid | string | Optional; ID Client requests unique ID  
topic | string | Required；Topic name format:
public.$symbol.liquidation_orders. symbol is case-insenstive.Both uppercase
and lowercase are supported. e.g:"BTC"  
  
### Return Parameter

Field Name | Type | Description  
---|---|---  
op | string | value:"notify"  
topic | string | topic subscribed  
ts | long | Time of Respond Generation，Unit：Millisecond  
<data> | array object |  
symbol | string | Coin  
contract_code | string | contract code  
direction | string | Long or short  
offset | string | Open or close  
volume | decimal | liquidated volume(cont)  
amount | decimal | liquidation amount (token)  
price | decimal | bankruptcy price  
created_at | long | Order Creation Time  
<\data> |  |  
  
> When there commences any liquidation order, the server will send
> notification with return parameter. For example：
    
    
    {
        "op":"notify",
        "topic":"public.BTC.liquidation_orders",
        "ts":1606293144641,
        "data":[
            {
                "contract_code": "BTC201225",
                "symbol": "BTC",
                "direction": "buy",
                "offset": "close",
                "volume": 26,
                "price": 19674.96,
                "created_at": 1606293144641,
                "amount": 0.132147663832607537
            }
        ]
    }
    

## Unsubscribe Liquidation Order Data(no authentication)(unsub)

### Unsubscribe Request Format

`{`

`“op”: “unsub”,`

`“topic": "public.$symbol.liquidation_orders”,`

`"cid": "id generated by client”,`

`}`

> Example of a successful unsubscribe request :
    
    
    {
      "op": "unsub",
      "topic": "public.BTC.liquidation_orders",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### Data format illustration of orders subscription

Field Name | Type | Description  
---|---|---  
op | string | Required； Operator Name，required subscribe value is sub  
cid | string | Optional; ID Client requests unique ID  
topic | string | Required；Unsubscribe topic name:
public.$symbol.liquidation_orders; symbol is case-insenstive.Both uppercase
and lowercase are supported.e.g: "BTC,ETH" ; when $symbol value is *, it
stands for unsubscribing the data of all coins;  
  
### Rules on Subscribe and Unsubscribe

Subscribe(sub) | Unsubscribe(unsub) | Rule  
---|---|---  
public.*.liquidation_orders | public.*.liquidation_orders | Allowed  
public.symbol1.liquidation_orders | public.*.liquidation_orders | Allowed  
public.symbol1.liquidation_orders | public.symbol1.liquidation_orders |
Allowed  
public.symbol1.liquidation_orders | public.symbol2.liquidation_orders | Not
Allowed  
public.*.liquidation_orders | public.symbol1.liquidation_orders | Not Allowed  
  
## Subscribe Contract Info (no authentication)（sub）

To subscribe contract info, the client has to make connection to the server
and send subscribe request in the format below:

`{`

`"op": "sub",`

`"cid": "40sG903yz80oDFWr",`

`"topic": "public.$symbol.contract_info"`

`}`

> Example of a successful request:
    
    
    {
      "op": "sub",
      "topic": "public.btc.contract_info",
      "cid": "40sG903yz80oDFWr"
    }
    
    

### Data format illustration of orders subscription

Field Name | Type | Description  
---|---|---  
op | string | Required； Operator Name，required subscribe value is sub  
cid | string | Optional; ID Client requests unique ID  
topic | string | Required；Topic name format: public.$symbol.contract_info.;
symbol is case-insenstive.Both uppercase and lowercase are supported.
e.g:"BTC,ETH"  
  
> Response example：
    
    
    {
        "op":"notify",
        "topic":"public.btc.contract_info",
        "ts":1604389592693,
        "event":"snapshot",
        "data":[
            {
                "symbol":"BTC",
                "contract_code":"BTC201106",
                "contract_type":"this_week",
                "contract_size":100,
                "price_tick":0.01,
                "delivery_date":"20201106",
                "create_date":"20201016",
                "contract_status":1
            },
            {
                "symbol":"BTC",
                "contract_code":"BTC201113",
                "contract_type":"next_week",
                "contract_size":100,
                "price_tick":0.01,
                "delivery_date":"20201113",
                "create_date":"20201023",
                "contract_status":1
            },
            {
                "symbol":"BTC",
                "contract_code":"BTC201225",
                "contract_type":"quarter",
                "contract_size":100,
                "price_tick":0.01,
                "delivery_date":"20201225",
                "create_date":"20200612",
                "contract_status":1
            },
            {
                "symbol":"BTC",
                "contract_code":"BTC210326",
                "contract_type":"next_quarter",
                "contract_size":100,
                "price_tick":0.01,
                "delivery_date":"20210326",
                "create_date":"20200904",
                "contract_status":1
            }
        ]
    }
    

### Response data fields

Field Name | Type | Description | Value Range  
---|---|---|---  
op | string | value: "notify"; |  
topic | string | topic subscribed |  
ts | long | timestamp of server response.unit: millionseconds |  
event | string | event | "init", "update", "snapshot"  
<data> | object array |  |  
symbol | string | symbol,"BTC","ETH"... |  
contract_code | string | contract code | "EOS200113"  
contract_type | string | contract type | "this_week","next_week", "quarter",
"next_quarter", Next Quarterly Contract: "next_quarter"  
contract_size | decimal | Contract Value (USD of one contract). such as 10,100
| 10, 100...  
price_tick | decimal | Minimum Variation of Contract Price | 0.001, 0.01...  
delivery_date | string | delivery date | such as "20200327"  
create_date | string | Contract Listing Date | such as "20180706"  
contract_status | int | contract status | 0: Delisting,1: Listing,2: Pending
Listing,3: Suspension,4: Suspending of Listing,5: In Settlement,6:
Delivering,7: Settlement Completed,8: Delivered, 9: Suspending of Trade  
</data> |  |  |  
  
### Note：

  * The websocket subscription of contract info event is pushed every 60 seconds, and the event is "snapshot". 
  * When the subscription is successful, the latest contract information will be pushed immediately, and the event is "init".
  * Only when the status is 1(Listing), can it be traded normally, other statuses are not tradable;

## Unsubscribe Contract Info Data(no authentication)(unsub)

To unsubscribe contract info data, the client has to make connection to the
server and send subscribe request in the format below:

### request format of unsubscribing contract info

`{`

`"op": "unsub",`

`"topic": "public.$symbol.contract_info",`

`"cid": "id generated by client",`

`}`

> example of unsubscribing contract info::
    
    
    {                                    
      "op": "unsub",                     
      "topic": "public.BTC.contract_info",   
      "cid": "40sG903yz80oDFWr"          
    }                                    
    

### request field desc of unsubscrbing contract info

field | datatype | desc  
---|---|---  
op | string | Required; Operator Name，subscribe value is unsub;  
cid | string | Optional; Client requests unique ID  
topic | string | Required；Unsubscribe topic name:
public.$symbol.contract_info; symbol is case-insenstive.Both uppercase and
lowercase are supported.e.g: "BTC,ETH" ; when $symbol value is *, it stands
for unsubscribing the data of all coins;  
  
### Data format of subscription and unsubscription of contract info

subscribe(sub) | unsubscribe(unsub) | rules  
---|---|---  
public.*.contract_info | pubic.*.contract_info | Allowed  
public.symbol1.contract_info | public.*.contract_info | Allowed  
public.symbol1.contract_info | public.symbol1.contract_info | Allowed  
public.symbol1.contract_info | public.symbol2.contract_info | Not Allowed  
public.*.contract_info | public.symbol1.contract_info | Not Allowed  
  
## Subscribe trigger orders updates

### To subscribe basis data, the Client has to make connection to the Server
and send subscribe request in the format below:

`{`

`"op": "sub",`

`"cid": "id generated by client",`

`"topic": "trigger_order.$symbol"`

`}`

> request
    
    
    {                                    
      "op": "sub",                     
      "topic": "trigger_order.BTC",   
      "cid": "40sG903yz80oDFWr"          
    }                                    
    

### Request Parameter

Parameter Name | Mandotary | Type | Desc | Value Range  
---|---|---|---|---  
op | true | string | Required； Operator Name，required subscribe value is sub |  
cid | false | string | Optional; ID Client requests unique ID |  
topic | true | string | Required；format: trigger_order.$symbol; symbol is
case-insenstive.Both uppercase and lowercase are supported.e.g.:"BTC,ETH"
;when $symbol value is *, it stands for subscribing the data of all coins; |  
  
> Return example：
    
    
    {
        "op":"notify",
        "topic":"trigger_order.ADA",
        "ts":1604390110568,
        "event":"order",
        "uid":"123456789",
        "data":[
            {
                "symbol":"ADA",
                "contract_code":"ADA201225",
                "contract_type":"quarter",
                "trigger_type":"le",
                "volume":1,
                "order_type":1,
                "direction":"buy",
                "offset":"close",
                "lever_rate":20,
                "order_id":28312417,
                "order_id_str":"28312417",
                "relation_order_id":"-1",
                "order_price_type":"limit",
                "status":2,
                "order_source":"web",
                "trigger_price":0.09,
                "triggered_price":null,
                "order_price":0.09,
                "created_at":1604390110565,
                "triggered_at":0,
                "order_insert_at":0,
                "canceled_at":0,
                "fail_code":null,
                "fail_reason":null
            }
        ]
    }
    

### Format Illustration on return data of order push：

Parameter Name | Mandotary | Type | Desc | Value Range  
---|---|---|---|---  
op | true | string | Required;Operator Name，Order push value is notify |  
topic | true | string | Required; Order push topic |  
ts | true | long | Time of Respond Generation, Unit: Millisecond |  
uid | true | string | account uid |  
event | true | string | Event notification description | trigger order placed
successfully（order），trigger order canceled successfully（cancel），order
triggered successfully（trigger_success），order failed to be
triggered（trigger_fail）  
<data> | true | object array |  |  
symbol | true | string | Variety code |  
contract_type | true | string | contract type | Weekly:"this_week", Bi-
weekly:"next_week", Quarterly:"quarter" Next Quarterly Contract:
"next_quarter"：“next_quarter”  
contract_code | true | string | contract code | "BTC180914" ...  
trigger_type | true | string | trigger type | `ge`great than or equal
to；`le`less than or equal to  
volume | true | decimal | trigger order volume |  
order_type | true | int | Transaction Type | 1\. Place orders  
direction | true | string | order direction | [buy,sell]  
offset | true | string | offset direction | [open,close]  
lever_rate | true | int | Leverage |  
order_id | true | long | trigger order ID |  
order_id_str | true | string | the order ID with string |  
relation_order_id | true | string | Relation order ID is the string related to
the limit orders , The value is -1 before the trigger orders executed. |  
order_price_type | true | string | Order price type | "limit": limit
order，"optimal_5":optimal 5，"optimal_10":optimal 10，"optimal_20":optimal 20  
status | true | int | order status | 2\. Ready to submit the orders; 4. Orders
partially matched; 5. Orders cancelled with partially matched; 6. Orders fully
matched;  
order_source | true | string | Order Source |  
trigger_price | true | decimal | trigger price |  
triggered_price | true | decimal | the price when trigger orders executed |  
order_price | true | decimal | the preset price by the client |  
created_at | true | long | order creation time |  
triggered_at | true | long | the execution time when orders getting triggered
|  
order_insert_at | true | long | the time when the triggered orders filled
successfully |  
canceled_at | true | long | Order cancelation time |  
fail_code | true | int | the error code when the triggered orders failed to be
filled |  
fail_reason | true | string | the error message with failure reason when
triggered orders failed to filled |  
</data> |  |  |  |  
  
#### Rule：

  * The intermediate states processed by the order status system will not be pushed, such as in the progress of placing an order, The descriptions of specific event notifications are as below: 
    * when the order status is 2（Submitted），event notification is order（trigger order placed successfully）；
    * when the order status is 4（Order placed successfully），event notification is trigger_success（trigger order triggered successfully）；
    * when the order status is 6（Canceled），event notification is cancel（trigger order canceled successfully）；
    * when the order status is 5（Order failed to be placed），event notification is trigger_fail（trigger order failed to be triggered）；
  * Single coin cannot be re-suscribed, and all coins subscription can cover single coin subscription; single coin cannot be subscribed after subscribing all coins. 

## Unsubscribe trigger orders updates（unsub）

To subscribe basis data, the Client has to make connection to the Server and
send subscribe request in the format below:

### Format of Unsubscribe order data

`{`

`"op": "unsub",`

`"topic": "trigger_order.$symbol",`

`"cid": "id generated by client",`

`}`

> Example of a successful unsubscribe request:
    
    
    {                                    
      "op": "unsub",                     
      "topic": "trigger_order.*",   
      "cid": "40sG903yz80oDFWr"          
    }                                    
    

### Format illustration of unsubscribe order data

Field Name | Type | Description  
---|---|---  
op | string | Required; Operator Name，subscribe value is unsub;  
cid | string | Optional; Client requests unique ID  
topic | string | Required；Unsubscribe topic name: trigger_order.$symbol;
symbol is case-insenstive.Both uppercase and lowercase are supported.e.g:
"BTC,ETH" ; when $symbol value is *, it stands for unsubscribing the data of
all coins;  
  
### Rules on Subscribe and Unsubscribe

Subscribe(sub) | Unsubscribe( unsub) | Rule  
---|---|---  
trigger_order.* | trigger_order.* | allowed  
trigger_order.symbol1 | trigger_order.* | allowed  
trigger_order.symbol1 | trigger_order.symbol1 | allowed  
trigger_order.symbol1 | trigger_order.symbol2 | Not Allowed  
trigger_order.* | trigger_order.symbol1 | Not Allowed  
  
# WebSocket interface for system status updates

  * The websocket url of system status updates is : wss://api.hbdm.com/center-notification

## Subscribe system status updates

### After successfully establishing a connection with the WebSocket API, users
could send data in the following format to the server to request data:

`{`

`"op": "sub",`

`"cid": "id generated by client",`

`"topic ": "public.$service.heartbeat"`

`}`

> Example on using parameters to request data:
    
    
    {
        "op": "sub",
        "cid": "id generated by client",
        "topic ": "public.futures.heartbeat"
    }
    

### **Request Parameter** :

Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
op | true | string | The fixed value of subscription is sub |  
cid | false | string | Client requests a unique ID |  
topic | true | string | Subscription topic name is required
(public.$service.heartbeat), Subscribe system status information of a certain
business |  
  
### **subscription parameter description** :

Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
service | true | string | Business Code | futures  
  
> **Return Parameter Example** :
    
    
    {
        "op": "notify",
        "topic": "public.futures.heartbeat",
        "event": "init",
        "ts":1580815422403,
        "data":{
            "heartbeat": 0,
            "estimated_recovery_time": 1408076414000
        }
    }
    
    

### **Return Parameter Rules** ：

Name | Mandatory | Type | Desc | Value Range  
---|---|---|---|---  
op | true | string | Operation name, the fixed value of push is notify; |  
topic | true | string | Push topic |  
event | true | string | Description on notification related event | The
initial system status information returned by a successful subscription
(init), triggered by system status change (update)  
ts | true | long | Server response timestamp |  
<data> |  |  |  |  
heartbeat | true | int | System Status | 1 is available, 0 is not
available(maintenance with service suspended)  
estimated_recovery_time | true | long | Estimated system recovery time, unit:
millisecond | When the system status is available, return NULL  
</data> |  |  |  |  
  
### Note

  * Since this push is a poll query status, there may be a delay of 1-2 seconds.

# Appendix

## Operator Type(OP)

Type | Description  
---|---  
ping | Server sends heatbeat with a Ping  
pong | Clients responds heatbeat with a Pong  
auth | Authentication  
sub | Subscribe Message  
unsub | Unsubscribe Message  
notify | Server pushes subscribe message  
  
## Topic Type

Type | applicative operator type | Description  
---|---|---  
orders.$symbol | sub,ubsub | Subscribe/unsubscribe the order data of a given
pair; when the $symbol value is *, it stands for subscribing/unsubscribing the
data of all pairs  
  
## Response code（Err-Code）

Return Error Code | Return description  
---|---  
0 | Request successfully.  
2001 | Invalid authentication.  
2002 | Authentication required.  
2003 | Authentication failed.  
2004 | Number of visits exceeds limit.  
2005 | Connection has been authenticated.  
2010 | Topic error.  
2011 | Contract doesn't exist.  
2012 | Topic not subscribed.  
2013 | Authentication type doesn't exist.  
2014 | Repeated subscription.  
2030 | Exceeds connection limit of single user.  
2040 | Missing required parameter.  
  
shell

