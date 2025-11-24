Electricity Bill Generator GUI
This program is a simple electricity bill calculator with a graphical user interface (GUI) built using the Guietta library in Python. It allows users to input electricity units consumed and calculates the total bill based on slab rates.

Features
User-friendly GUI to input electricity consumption units.

Calculates bill using predefined slab rates and base prices.

Displays details of consumption, base unit, base price, extra units, price per extra unit, and total amount.

Easy-to-use with simple button click to generate bills.

Installation
Ensure you have Python installed. Then install Guietta for the GUI:

text
pip install guietta
How to Use
Run the program.

Enter the number of electricity units consumed.

Click the "Generate" button.

View the bill details including units consumed, base price, extra units, extra unit price, and total amount payable.

Click "Quit" to exit the program.

Billing Logic
The electricity bill is calculated using multiple consumption slabs:

For less than 150 units: ₹3 per unit.

Between 151 and 300 units: ₹100 base price + ₹3.75 for each unit above 150.

Between 301 and 450 units: ₹250 base price + ₹4 per extra unit.

Between 451 and 600 units: ₹300 base price + ₹4.25 per extra unit.

Above 600 units: ₹400 base price + ₹5 per extra unit.

The program calculates and displays relevant billing details accordingly.

Code Overview
The GUI is created using Guietta with fields for input and outputs.

The calculate_bill() function is called when the "Generate" button is clicked.

It computes the bill based on the units entered and updates the GUI with detailed billing info.

Example
Input: 250 units
Output:

Base unit: 150

Base price: ₹100

Extra units: 100

Price per extra unit: ₹3.75

Total amount: ₹475

License
This is a simple educational project. Feel free to modify and use it as needed.
