![WhatsApp Image 2025-12-03 at 22 01 40_e1c5a8c9](https://github.com/user-attachments/assets/7f3d6821-af29-4956-afa8-cf1cef658f86)📐 DSA-Based Calculator (C++ & Qt)

A modern desktop calculator built using C++, Qt, and core Data Structures & Algorithms (DSA) principles.
This project demonstrates how structured algorithmic logic and custom data structures can power a clean, efficient, and extensible GUI application.


🚀 Features
Core Calculator Functions

Basic arithmetic: Addition, Subtraction, Multiplication, Division

Expression evaluation using a DSA-based algorithm


Supports:

Multi-digit inputs

Operator precedence

Parentheses

Unary operations (optional, if implemented)

DSA Components

Stack-based expression evaluation (Infix → Postfix → Evaluation)

Custom Stack / Node implementation (if applicable)

Efficient parsing algorithms

Time & space complexity awareness in core modules


Qt UI

Clean and responsive interface

Custom buttons, display screen, and layout control

Error handling and input validation in UI (e.g., division by zero, invalid expressions)


🧠 Technologies & Concepts
Layer	Technology / Concept
Front-end GUI	Qt Widgets (QPushButton, QLineEdit, QGridLayout, etc.)
Back-end Logic	C++17+
DSA	Stacks, Parsing Algorithms, Expression Trees (optional)
Architecture	Modular class-based design with separated UI and logic layers
📁 Project Structure (Example)
├── src/
│   ├── main.cpp
│   ├── calculator.cpp
│   ├── calculator.h
│   ├── expression_parser.cpp
│   ├── expression_parser.h
│   ├── stack.h
│   └── ui/
│       └── calculator.ui
├── assets/
│   └── screenshots/
├── README.md
└── CMakeLists.txt or .pro file

⚙️ How It Works (DSA-Focused)
1. Tokenization

Breaks user input into:

numbers

operators

parentheses

2. Infix → Postfix Conversion (Shunting-Yard Algorithm)

Uses two stacks:

Operator stack

Output queue

Ensures correct operator precedence and associativity.

3. Postfix Evaluation

A stack is used to evaluate postfix expressions efficiently.

4. Integration With Qt

UI sends expression string

Parser converts & evaluates

Result is returned to UI display

🛠️ Build & Run
Prerequisites

Qt 5/6 (Qt Creator recommended)

C++17 or later

CMake or qmake (depending on your project setup)

Building

Using Qt Creator:

Open the .pro / CMakeLists.txt file

Configure the kit

Build & Run

Using command line (CMake example):

mkdir build && cd build
cmake ..
make
./Calculator


🧪 Testing

Unit tests for expression evaluation

Boundary cases:

malformed input

division by zero

nested parentheses

long expressions

📌 Future Improvements

Scientific calculator functions (sin, cos, log, etc.)

History panel using a queue or list

Expression tree visualization

Theming (light/dark mode)

🤝 Contributing

Pull requests are welcome!
For major changes, please open an issue first to discuss what you’d like to modify.
