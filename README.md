# Super Fibo - Fibonacci Levels

Super Fibo is a custom indicator that calculates and plots Fibonacci levels on the chart. It is designed to help traders optimize their forex trades using Fibonacci ratios.

## Input Parameters

- HighPrice: The high price point used for calculating the Fibonacci levels.
- LowPrice: The low price point used for calculating the Fibonacci levels.

## Custom Fibonacci Levels

The indicator uses a custom array `fibLevels` to store the calculated Fibonacci levels.

## Custom Fibonacci Ratios

The indicator uses a custom array `fibRatios` to store the Fibonacci ratios. The default ratios are 0.0, 0.236, 0.382, 0.5, 0.618, 0.786, and 1.0.

## Custom Fibonacci Colors

The indicator uses a custom array `fibColors` to store the colors for each Fibonacci level. The default colors are Red, Green, Blue, Yellow, Orange, Violet, Brown, and Pink.

## Custom Fibonacci Level Calculation

The `CalculateFibLevels()` function calculates the Fibonacci levels based on the input parameters. It uses the high and low price points to calculate the Fibonacci range, and then applies the Fibonacci ratios to determine the levels.

## Custom Chart Drawing

The `DrawFibLevels()` function draws the Fibonacci levels on the chart using horizontal lines. It creates a separate object for each level and sets the color and style of the lines.

## Custom Initialization

The `OnInit()` function is called when the indicator is initialized. It calculates the Fibonacci levels using the `CalculateFibLevels()` function and draws them on the chart using the `DrawFibLevels()` function.

## Custom Deinitialization

The `OnDeinit()` function is called when the indicator is removed from the chart. It deletes the Fibonacci level objects from the chart.

## Custom Entry

The `OnTick()` function is called on each tick. This is where the entry logic for trading should be implemented.

## Custom Exit

The `ShouldExit()` function is called to determine if the trading position should be closed. This is where the exit logic for trading should be implemented.

## Custom Money Management

The `ManageMoney()` function is called to manage the money for trading. This is where the money management logic should be implemented.

## Custom Trading

The `SuperFibo()` function is the main function that controls the trading process. It calls the `OnInit()` function to initialize the indicator, then enters a loop where it calls the `OnTick()` function, the `ManageMoney()` function, and sleeps for a delay of 1000 milliseconds. This loop continues until the `ShouldExit()` function returns true. Finally, the `OnDeinit()` function is called to deinitialize the indicator.

## Program Start

The `OnStart()` function is the entry point of the program. It calls the `SuperFibo()` function to start the trading process.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Super Fibo Review](https://forexroboteasy.com/forex-robot-review/super-fibo-review-optimize-forex-trades-with-fibonacci-levels/).

Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work as described in this product. To find the official developer of this product, please use MQL5.
