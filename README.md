# Golden Weasle Professional ReadMe

This ReadMe file provides an overview of the code for the Golden Weasle Professional forex robot, developed by the Forex Robot Easy Team. Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in the product.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/golden-weasle-pro-a-detailed-review-of-mt5-forex-software/).

## Code Description

The code for Golden Weasle Professional is an expert advisor written in MQL4 programming language. It is designed to execute trading algorithms based on specified time frames and trade signals.

### Input Parameters

The code contains the following input parameters:

- `TimeFrame1`: Specifies the first time frame (default value: 5).
- `TimeFrame2`: Specifies the second time frame (default value: 15).
- `TimeFrame3`: Specifies the third time frame (default value: 30).
- `SignalType`: Specifies the type of trade signals (default value: SIGNAL_TYPE_1).

### Global Variables

The code includes the following global variable:

- `SignalTime`: Represents the time of the trading signal.

### Initialization Function

The `OnInit()` function is called during the expert initialization. It checks the compatibility with MetaTrader 5 and sets the time frames using the `SetTimeframes()` function.

### Deinitialization Function

The `OnDeinit()` function is called during the expert deinitialization. It cleans up the `SignalTime` variable.

### Tick Function

The `OnTick()` function is called on each tick of the chart. It checks for a new trading signal using the `isNewSignal()` function and executes the trading algorithm using the `ExecuteTradingAlgorithm()` function.

### Check for New Signal

The `isNewSignal()` function checks if a new signal has occurred by comparing the current time with the `SignalTime` variable. If a new signal is detected, it updates the `SignalTime` variable and returns true.

### Set Time Frames

The `SetTimeframes()` function sets the specified time frames using the `SetTimeframe()` function. It returns true if all time frames are successfully set.

### Set Individual Time Frame

The `SetTimeframe()` function sets an individual time frame using the `ChartSetInteger()` function. It returns true if the time frame is successfully set.

### Execute Trading Algorithm

The `ExecuteTradingAlgorithm()` function represents the trading algorithm. In the provided code, it only prints a message indicating the reception of a new trading signal.

### Entry Point

The `OnStart()` function is the entry point of the program. In the provided code, it does nothing.

## Product Description

Golden Weasle Professional is a forex robot developed by the Forex Robot Easy Team. It is designed to execute trading algorithms based on specified time frames and trade signals. The robot aims to provide automated trading solutions to forex traders, allowing them to take advantage of market opportunities.

Please note that this code is only a sample and not the official product developed by the Forex Robot Easy Team. For the official product and more information, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/golden-weasle-pro-a-detailed-review-of-mt5-forex-software/).
