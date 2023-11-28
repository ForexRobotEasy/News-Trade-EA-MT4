# News Trade EA MT4

This code is an Expert Advisor (EA) for MetaTrader 4 (MT4) developed by the Forex Robot Easy Team. It is designed to trade news events specifically for GBP pairs. The EA includes functions to check for the availability of GBP pairs, retrieve economic news for GBP pairs from an economic calendar, determine the trading direction based on the news impact, and place market orders automatically or with user confirmation.

## Features
- Trade GBP pairs: The EA checks if GBP pairs (GBPUSD, EURGBP, GBPJPY, GBPCAD, GBPAUD, GBPCHF) are available for trading.
- Economic calendar integration: The EA uses the CCalendar class to retrieve the next economic event for GBP pairs on the daily timeframe.
- Trading modes: The EA supports two trading modes - SEMI_AUTOMATIC and FULLY_AUTOMATIC.
- User confirmation: In SEMI_AUTOMATIC mode, the EA prompts the user to confirm the trade before placing market orders.
- Customizable parameters: The EA allows customization of trading parameters such as lot size, stop loss, and take profit.

## Usage
1. Include the necessary libraries: The EA requires the Trade, Timeseries, and Calendar libraries.
2. Define constants: SYMBOL_GBPUSD, SYMBOL_EURGBP, SYMBOL_GBPJPY, SYMBOL_GBPCAD, SYMBOL_GBPAUD, and SYMBOL_GBPCHF are defined as constants representing the GBP pairs.
3. Define trading modes: The TradingMode enum defines two modes - SEMI_AUTOMATIC and FULLY_AUTOMATIC. Specify the desired mode using the 'mode' input variable.
4. Define trading parameters: Specify the desired lot size, stop loss, and take profit using the 'lotSize', 'stopLoss', and 'takeProfit' input variables.
5. Initialize objects: Initialize the CCalendar, CTrade, and CTimeseries objects for economic calendar, trading, and timeseries functionalities respectively.
6. Implement the tradeGBP() function: This function checks for the availability of GBP pairs, retrieves the next economic event for GBP pairs, determines the trading direction based on the news impact, and places market orders.
7. Implement the OnTick() function: This function is the entry point of the program and calls the tradeGBP() function.
8. Implement the GetUserConfirmation() function: This function prompts the user for input to confirm or skip the trade.
9. Implement the GetStringFromTerminal() function: This function reads a string input from the terminal.

## Product Description
Forex Robot Easy presents the News Trade EA MT4, an Expert Advisor specifically designed to trade news events for GBP pairs on MetaTrader 4. With its integration of an economic calendar and customizable trading parameters, this EA provides a reliable and automated solution for trading news events.

The News Trade EA MT4 allows traders to take advantage of market volatility during news releases by automatically placing market orders based on the trading mode selected. In SEMI_AUTOMATIC mode, the EA prompts the user for confirmation before placing trades, ensuring full control over the trading decisions. In FULLY_AUTOMATIC mode, the EA automatically executes trades without any user intervention.

Key Features:
- Trade GBP pairs: The EA supports trading of popular GBP pairs including GBPUSD, EURGBP, GBPJPY, GBPCAD, GBPAUD, and GBPCHF.
- Economic calendar integration: The EA retrieves the next economic news event for GBP pairs on the daily timeframe, allowing traders to stay updated on market-moving events.
- Customizable parameters: Traders can customize the lot size, stop loss, and take profit according to their risk appetite and trading strategy.
- User confirmation: In SEMI_AUTOMATIC mode, the EA prompts the user to confirm trades, ensuring complete control over trading decisions.
- Easy to use: The EA is designed to be user-friendly and can be easily integrated into existing trading setups.

Please note that ForexRobotEasy is not the official developer of this product. We provide this sample code to showcase the functionality of the News Trade EA MT4. To find the official developer of this product and access detailed reviews and trading results, please visit [Forex Robot Easy - News Trade EA MT4 Review](https://forexroboteasy.com/forex-robot-review/news-trade-ea-mt4-review-a-reliable-forex-trading-robot/). For additional support and updates, we recommend using the MQL5 platform.
