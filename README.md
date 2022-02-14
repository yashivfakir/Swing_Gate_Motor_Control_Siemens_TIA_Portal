# Double Swing Gate Motor Contol

The double swing gate motor control was implemented using Siemens TIA Portal V13 and Step 7.
An S7300 specifically the CPU 314 and a I/O module.

## Basic Overview of Gate Operation

The gate consists of two motors and two swing gates that open/close in sync with each other. The open/close actions are controlled from a single button remote transmitter where the time that the button is engaged determines the operation tat is to be performed.
If the remote is pressed once:
- The gate motors begin opening/closing
If the remote is pressed again before the motors have been fully open/closed:
- The gate motors are stopped and the gate remains in the current position
- When pressed again the gates move in the opposite direction to prior being stopped until completely open/closed
If the remote is not pressed during the duration of opening/closing:
- The gate completes the opening/closing action
Once the gate operation has been completed the gate waits for the next signal to begin opening or closing the gates.


