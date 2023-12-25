# ATR Keltner Channels Multi TF Real Value for MT5

This is a custom indicator for MetaTrader 5 (MT5) that calculates and displays Keltner Channels on the chart. Keltner Channels are a volatility-based trend indicator that consists of an upper band, a middle line (exponential moving average), and a lower band. The indicator uses the Average True Range (ATR) as a measure of volatility to calculate the width of the bands.

## Input Parameters

The indicator has the following input parameters:

- `emaPeriod`: Exponential Moving Average period (default: 20)
- `upperBandMultiplier`: Multiplier for the upper band (default: 3.0)
- `lowerBandMultiplier`: Multiplier for the lower band (default: 3.0)

## Indicator Initialization

The `OnInit()` function is called when the indicator is initialized. In this function, the Keltner Channels indicator is created using the `iCustom` function. The indicator name, input parameters, and symbol and timeframe are passed to the `iCustom` function to create the indicator handle. If the indicator creation fails, an error message is printed and the initialization fails. 

The indicator line styles and colors are set using the `SetIndexStyle` and `SetIndexBuffer` functions. The upper band, middle line (EMA), and lower band values are set using the `SetIndexValue` function. The labels for the indicator lines are also set using the `SetIndexLabel` function.

## Indicator Calculation

The `OnCalculate()` function is called for each new bar on the chart. In this function, the Keltner Channels values are calculated using the `iCustom` function with the appropriate parameters. The calculated values are then plotted on the chart using the `SetIndexValue` function.

## Product Description

This code provides a sample implementation of the ATR Keltner Channels indicator for MetaTrader 5. The indicator calculates and displays Keltner Channels on the chart, which can be used to identify trends and potential trading opportunities.

The ATR Keltner Channels indicator is a popular technical analysis tool that combines volatility and trend analysis. It consists of three lines - an upper band, a middle line (exponential moving average), and a lower band. The width of the bands is determined by the Average True Range (ATR), which is a measure of volatility.

By using the ATR Keltner Channels indicator, traders can identify periods of high volatility and potential trend reversals. When the price moves above the upper band, it indicates that the market is overbought and a reversal may be imminent. Conversely, when the price moves below the lower band, it indicates that the market is oversold and a reversal may be imminent.

This code is provided as a sample implementation and is not the official product developed by Forex Robot Easy. To find the official developer of this product, please refer to the MQL5 website.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/atr-keltner-channels-mt5-software-review-volatility-based-trend-indicator/).
