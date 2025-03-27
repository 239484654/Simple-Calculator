# Simple Calculator for Windows

## Introduction
This calculator is a simple desktop application designed to provide users with basic calculation functions. It draws on the design concepts and ideas of some open - source projects and features simplicity and ease of use.

[Chinese version](./README_zhs.md)

## Function Overview
This calculator has the following main functions:
1. **Basic Arithmetic Operations**: Supports basic mathematical operations such as addition, subtraction, multiplication, and division.
2. **Decimal Handling**: Can handle the input and calculation of numbers containing decimal points.
3. **Number Input**: Users can input numbers by clicking the number buttons on the interface.
4. **Clear Operations**: Provides functions to clear all inputs, clear the current input, and delete the last digit.
5. **System Color Adaptation**: Can automatically adjust the interface color according to the system's theme color (dark or light).

## Interface Description

### Color Mode
The calculator will automatically switch the interface color according to the system's color theme. If the system is in dark mode, the calculator will use a dark color scheme; if it is in light mode, it will use a light color scheme. If the `darkdetect` library is not installed on the system, the calculator will default to the light mode.

### Display Area
- **Current Display**: Used to show the numbers input by the user and the calculation results. The maximum display length is 10 digits.

### Button Area
- **Number Buttons**: From 0 to 9, used to input numbers.
- **Decimal Point Button**: Used to input decimal points.
- **Operator Buttons**: Include operators such as addition (+), subtraction (-), multiplication (×), and division (÷) for mathematical operations.
- **Clear Buttons**:
  - **Clear All**: Clears all inputs and calculation results, resetting the display area to 0.
  - **Clear Current**: Clears the currently input number.
  - **Delete One**: Deletes the last digit in the display area.

## Usage Instructions

### Number Input
Click the number buttons (0 - 9) to input numbers. If you need to input a decimal, click the decimal point button.

### Basic Arithmetic Operations
After inputting the first number, click an operator button to select the operation to be performed. Then input the second number and finally click the equal sign (=) button to perform the calculation. The calculation result will be displayed in the display area.

### Clear Operations
- To clear all inputs and calculation results, click the "Clear All" button.
- To clear only the currently input number, click the "Clear Current" button.
- To delete the last digit in the display area, click the "Delete One" button.

## Technical Details

### Dependencies
This calculator uses the following Python libraries:
- `math`: For mathematical calculations.
- `tkinter`: For creating the graphical user interface (GUI).
- `cmath`: For complex number calculations.
- `fractions`: For fraction processing.
- `decimal`: For high - precision decimal calculations.
- `threading`: For starting a thread to check the system color.
- `time`: For time - related operations.
- `darkdetect`: For detecting the system's color theme (dark or light).

### Code Structure
- `add_fraction`: Handles the addition operation of fractions.
- `calculate_expression`: Calculates the input expression.
- `Int`: Performs integer conversion.
- `pressNumber`: Handles the click events of number buttons.
- `pressDP`: Handles the click event of the decimal point button.
- `clearAll`: Clears all inputs and calculation results.
- `clearCurrent`: Clears the currently input number.
- `delOne`: Deletes the last digit in the display area.
- `pressOperator`: Handles the click events of operator buttons.
- `Demo`: Used for demonstration.
- `check_system_color`: Starts a thread to check the system's color theme and adjusts the interface color accordingly.

## References
This project refers to the following open - source projects:
- [Cascadia Code](https://github.com/microsoft/cascadia-code/releases)
- [Microsoft Calculator](https://github.com/Microsoft/calculator)

These projects have provided us with valuable inspiration and references. We would like to express our gratitude here.

## Notes
- The maximum display length of the display area is 10 digits. Numbers that are too long may not be fully displayed.

We hope this instruction manual will help you use this calculator better. If you have any questions or suggestions, please feel free to provide feedback.