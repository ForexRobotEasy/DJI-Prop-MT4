# DJI Prop MT4 - ReadMe

This is a ReadMe file for the DJI Prop MT4 code, developed by the Forex Robot Easy Team. This code is intended for optimizing Dow Jones trading with prop firms. For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/dji-prop-mt4-review-optimize-dow-jones-trading-with-prop-firms/). 

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in this product. To find the official developer of this product, please refer to MQL5.

## Code Description

The DJI Prop MT4 code is an Expert Advisor (EA) that operates on the MetaTrader 4 (MT4) platform. It makes use of various input parameters and global variables to perform trading operations. 

### Input Parameters

- RiskLevel: This parameter determines the risk level for calculating the lot size.
- MaximumDrawdownPerDay: Specifies the maximum drawdown allowed per day.
- OverallDrawdown: Defines the overall drawdown limit.
- MinimumProfitPerMonth: Sets the minimum profit required per month.
- LeverageRatio: Specifies the leverage ratio for trading.
- NewsFilterEnabled: Enables or disables the news filter.

### Global Variables

- AccountEquity: Stores the current account equity.
- AccountBalance: Stores the current account balance.
- AccountProfit: Stores the current account profit.
- AccountLeverage: Stores the current account leverage.
- MarketInfoInteger: Stores the market information integer for the news filter.
- NewsEventTime: Stores the time of the news event.

### Initialization Function (OnInit)

The OnInit function is called when the EA is initialized. It retrieves the initial account information and sets the news filter if enabled.

### Tick Function (OnTick)

The OnTick function is called on each tick of the market. It checks if the news filter is enabled and if the current time is after the news event time. Based on this, it performs trading operations with or without the news filter. It also checks for maximum drawdown per day, overall drawdown, lot size calculation based on risk level, minimum profit per month, and leverage ratio. It then performs trading operations based on the calculated lot size.

### Deinitialization Function (OnDeinit)

The OnDeinit function is called when the EA is deinitialized. It performs actions before deinitialization.

## Disclaimer

Please note that the DJI Prop MT4 code provided here is a sample code and does not guarantee any specific trading results. The actual performance of the EA may vary based on market conditions and trading strategies. It is recommended to thoroughly test the code and make necessary modifications before using it in a live trading environment.

For detailed reviews and trading results of the official DJI Prop MT4 product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/dji-prop-mt4-review-optimize-dow-jones-trading-with-prop-firms/).
