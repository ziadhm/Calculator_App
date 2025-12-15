# Calculator App

## Overview
The Calculator App is a Java application that provides a graphical user interface (GUI) for performing basic arithmetic calculations. It uses Swing components for the GUI and includes features such as number input, arithmetic operations, and result display.

Checkout the full tutorial [here](https://www.youtube.com/watch?v=IuGh1pXLfhc)

## Files

1. **CalculatorApp.java**: This file contains the main class `CalculatorApp`, which serves as the entry point for the application. It creates an instance of the `CalculatorGui` class and makes the GUI visible.

2. **CalculatorGui.java**: This file contains the `CalculatorGui` class, which extends `JFrame` and represents the main GUI window of the application. It sets up the GUI components, including a display field for showing the numbers and results, and buttons for number input and arithmetic operations. It also handles button click events to perform the calculations.

3. **CalculatorService.java**: This file contains the `CalculatorService` class, which provides the actual arithmetic calculations for the application. It includes methods for addition, subtraction, multiplication, and division.

4. **CommonConstants.java**: This file contains the `CommonConstants` class, which defines common constants used in the application, such as the application name, the size of the GUI window, and the configurations for the display field and buttons.

## Usage

To use the Calculator App, follow these steps:

1. Compile the Java files:
```bash
javac -d . src\CalculatorApp.java src\gui\CalculatorGui.java src\service\CalculatorService.java src\constants\CommonConstants.java
```

2. Run the compiled Java program:
```bash
java CalculatorApp
```

3. The Calculator App GUI window will appear. You can enter numbers and perform arithmetic operations using the buttons.

4. To enter numbers, click the respective number buttons (0-9).

5. To perform arithmetic operations, click the corresponding operator buttons (+, -, x, /). The current number in the display field will be used as the first operand.

6. To calculate the result, click the "=" button. The result will be displayed in the display field.

## Class Details

### 1. CalculatorApp.java

This class contains the `CalculatorApp` class, which serves as the entry point for the application.

#### Methods
- `main(String[] args)`: The main method creates an instance of `CalculatorGui` and makes the GUI visible.

### 2. CalculatorGui.java

This class represents the main GUI window of the application.

#### Constructors
- `CalculatorGui()`: Constructs a new `CalculatorGui` object. It sets up the JFrame with the application name, size, and close operation. It then calls the `addGuiComponents()` method to add the GUI components.

#### Methods
- `addGuiComponents()`: This method sets up the GUI components, including a display field for showing numbers and results, and buttons for number input and arithmetic operations. It also sets up the layout using `SpringLayout` and adds event handling for button clicks.

- `getButtonLabel(int buttonIndex)`: This method returns the label for the buttons based on the button index.

- `actionPerformed(ActionEvent e)`: This method handles button click events and performs the corresponding arithmetic calculations.

### 3. CalculatorService.java

This class provides the actual arithmetic calculations for the application.

#### Methods
- `setMathSymbol(char mathSymbol)`: Sets the mathematical symbol for the arithmetic operation.

- `setNum1(double num1)`: Sets the first operand for the arithmetic operation.

- `setNum2(double num2)`: Sets the second operand for the arithmetic operation.

- `add()`: Performs addition and returns the result.

- `subtract()`: Performs subtraction and returns the result.

- `multiply()`: Performs multiplication and returns the result.

- `divide()`: Performs division and returns the result.

### 4. CommonConstants.java

This class contains common constants used in the application.

#### Constants
- `APP_NAME`: Represents the name of the application.
- `APP_SIZE`: Represents the size of the main GUI window as an array of two integers: width and height.
- `TEXTFIELD_LENGTH`: Represents the length of the display field.
- `TEXTFIELD_FONTSIZE`: Represents the font size of the display field.
- `TEXTFIELD_SPRINGLAYOUT_NORTHPAD`: Represents the north padding of the display field in the layout.
- `TEXTFIELD_SPRINGLAYOUT_WESTPAD`: Represents the west padding of the display field in the layout.
- `BUTTON_ROWCOUNT`: Represents the number of rows for the button grid.
- `BUTTON_COLCOUNT`: Represents the number of columns for the button grid.
- `BUTTON_COUNT`: Represents the total number of buttons.
- `BUTTON_FONTSIZE`: Represents the font size of the buttons.
- `BUTTON_SPRINGLAYOUT_NORTHPAD`: Represents the north padding of the button panel in the layout.
- `BUTTON_SPRINGLAYOUT_WESTPAD`: Represents the west padding of the button panel in the layout.
- `BUTTON_HGAP`: Represents the horizontal gap between buttons in the grid layout.
- `BUTTON_VGAP`: Represents the vertical gap between buttons in the grid layout.
