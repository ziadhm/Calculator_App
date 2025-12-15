# Calculator App

A simple Java Swing-based calculator application with a graphical user interface for performing basic arithmetic operations.

## Features

- ✨ Clean and intuitive GUI built with Java Swing
- ➕ Basic arithmetic operations: Addition, Subtraction, Multiplication, Division
- 🔢 Number input via clickable buttons (0-9)
- 🎯 Real-time result display
- 📐 Organized code structure with service and constant layers

## Quick Start

### Prerequisites

- Java Development Kit (JDK) 8 or higher

### How to Run

1. Clone the repository:
```bash
git clone https://github.com/ziadhm/Calculator.git
cd Calculator
```

2. Compile all Java files:
```bash
javac -d . src/CalculatorApp.java src/gui/CalculatorGui.java src/service/CalculatorService.java src/constants/CommonConstants.java
```

3. Run the application:
```bash
java CalculatorApp
```

The Calculator GUI window will appear, and you can start performing calculations!

## Project Structure

```
Calculator/
├── src/
│   ├── CalculatorApp.java          # Main entry point
│   ├── gui/
│   │   └── CalculatorGui.java      # GUI implementation
│   ├── service/
│   │   └── CalculatorService.java  # Calculation logic
│   └── constants/
│       └── CommonConstants.java    # Application constants
└── README.md
```

## Usage

1. **Enter Numbers**: Click the number buttons (0-9) to input values
2. **Select Operation**: Click an operator button (+, -, ×, ÷)
3. **Calculate Result**: Click the "=" button to display the result
4. **Continue Calculating**: Use the result for further operations or start fresh

## Technical Details

<details>
<summary>Click to expand class documentation</summary>

### CalculatorApp.java

Main entry point for the application.

**Methods:**
- `main(String[] args)`: Creates and displays the calculator GUI

### CalculatorGui.java

GUI implementation using Java Swing components.

**Constructor:**
- `CalculatorGui()`: Initializes the JFrame with title, size, and components

**Methods:**
- `addGuiComponents()`: Sets up display field, buttons, and layout using SpringLayout
- `getButtonLabel(int buttonIndex)`: Returns button labels based on index
- `actionPerformed(ActionEvent e)`: Handles button click events and calculations

### CalculatorService.java

Handles arithmetic calculations.

**Methods:**
- `setMathSymbol(char mathSymbol)`: Sets the operation symbol
- `setNum1(double num1)`: Sets first operand
- `setNum2(double num2)`: Sets second operand
- `add()`: Returns sum of operands
- `subtract()`: Returns difference of operands
- `multiply()`: Returns product of operands
- `divide()`: Returns quotient of operands

### CommonConstants.java

Application-wide constants.

**Constants:**
- `APP_NAME`: Application window title
- `APP_SIZE`: Window dimensions [width, height]
- `TEXTFIELD_LENGTH`: Display field length
- `TEXTFIELD_FONTSIZE`: Display field font size
- `TEXTFIELD_SPRINGLAYOUT_NORTHPAD`: Display field top padding
- `TEXTFIELD_SPRINGLAYOUT_WESTPAD`: Display field left padding
- `BUTTON_ROWCOUNT`: Number of button rows
- `BUTTON_COLCOUNT`: Number of button columns
- `BUTTON_COUNT`: Total button count
- `BUTTON_FONTSIZE`: Button font size
- `BUTTON_SPRINGLAYOUT_NORTHPAD`: Button panel top padding
- `BUTTON_SPRINGLAYOUT_WESTPAD`: Button panel left padding
- `BUTTON_HGAP`: Horizontal gap between buttons
- `BUTTON_VGAP`: Vertical gap between buttons

</details>

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

## License

This project is open source and available for educational purposes.
