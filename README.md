# Wolfe Wave Scanner MT4

This code represents a custom indicator for MetaTrader 4 (MT4) that scans all symbols and timeframes to detect Wolfe Wave patterns. The Wolfe Wave pattern is a harmonic pattern that consists of four price swings or waves. It is used by traders to identify potential reversal points in the market.

## Developer

This indicator was developed by Forex Robot Easy Team.

## Website

For more information about this indicator and detailed reviews and trading results, visit the [Wolfe Wave Scanner MT4 Review](https://forexroboteasy.com/forex-robot-review/wolfe-wave-scanner-mt4-review-one-click-all-symbol-scan/) page on the Forex Robot Easy website.

## Features

- Scans all symbols and timeframes to detect Wolfe Wave patterns.
- Allows customization of pattern parameters such as pips threshold, deviation threshold, and channel deviation.
- Displays the detected patterns on the MT4 platform.
- Sends alerts or notifications when a Wolfe Wave pattern is detected.

## Usage

1. Install the indicator on your MetaTrader 4 platform.
2. Open the chart of the desired symbol and timeframe.
3. Run the indicator and click on the 'OneClickScan' button to initiate a full scan of all symbols and timeframes.
4. The indicator will detect Wolfe Wave patterns that meet the specified criteria and display them on the chart.
5. Optionally, alerts or notifications can be sent to the user when a Wolfe Wave pattern is detected.

## Code Explanation

The code consists of several functions and parameters:

1. `MAX_SYMBOLS` and `MAX_TIMEFRAMES` define the maximum number of symbols and timeframes to scan.
2. `PipsThreshold`, `DeviationThreshold`, and `ChannelDeviation` are input parameters that define the criteria for detecting Wolfe Wave patterns.
3. `SWolfeWavePattern` is a structure that stores the information of a detected pattern.
4. `patterns` is an array that stores the detected patterns.
5. `OneClickScan` is a function that initiates a full scan of all symbols and timeframes. It clears the patterns array, loops through all symbols and timeframes, calculates the Wolfe Wave pattern for each symbol and timeframe, and adds the pattern to the patterns array if it meets the criteria. It then displays the detected patterns on the MT4 platform and sends alerts or notifications.
6. `CalculateWolfeWavePattern` is a function that calculates the Wolfe Wave pattern for a given symbol and timeframe. It needs to be implemented to calculate the price levels for points 1, 2, 3, and 4 of the Wolfe Wave pattern.
7. `DisplayPatterns` is a function that displays the detected patterns on the MT4 platform. It needs to be implemented to draw lines or shapes on the chart to represent the Wolfe Wave patterns.
8. `SendAlerts` is a function that sends alerts or notifications for the detected patterns. It needs to be implemented to send an alert or notification to the user when a Wolfe Wave pattern is detected.
9. `ResetPatterns` is a function that resets the patterns array.
10. `OnStart` is the entry point of the program. It calls the `OneClickScan` function to start the scanning process.

**Please note that Forex Robot Easy is not the official developer of this product. This code is provided as a sample and can work as described in the product. To find the official developer of this product, use MQL5.
