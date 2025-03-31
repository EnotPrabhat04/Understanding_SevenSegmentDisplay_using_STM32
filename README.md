**STM32 Seven Segment Display Control**

**Overview**

This project demonstrates how to control a common cathode seven-segment display using an STM32 microcontroller. The code initializes the GPIO pins, configures the clock, and displays digits from 0 to 9 using segment control logic. 
The primary function of this project is to provide a clear understanding of GPIO manipulation using HAL (Hardware Abstraction Layer) in STM32CubeIDE.

**Features**

1.Display digits 0 to 9 on a seven-segment display

2.Efficient use of GPIO pins for segment control

3.Clear demonstration of STM32 GPIO initialization and control using HAL functions

4.Simple error handling using Error_Handler()

**Components Used**

STM32 Microcontroller (e.g., STM32F103C8T6),Common Cathode Seven Segment Display,Connecting Wires,Power Supply,

**CODE EXPLANATION**

**Initialization:**

The system clock is configured using the High-Speed Internal (HSI) oscillator.

GPIO pins (PA0 to PA6) are initialized as output pins using HAL.

**Display Function:**

displayDigit() takes a digit (0-9) as input and sets the corresponding segment values using the segment data stored in an array.

The GPIO pins are controlled using HAL_GPIO_WritePin() to display the correct number.

**Error Handling:**

The Error_Handler() function is used to stop the system and disable interrupts in case of an error.

**How to Use**

1.Connect the seven-segment display to GPIO pins PA0 to PA6 on the STM32 board.

2.Upload the code using STM32CubeIDE.

3.Monitor the display as it shows digits from 0 to 9.

4.Use the Serial Monitor to debug using the available printf() statements.

**Future Enhancements**

1.Implement a counter to cycle through digits automatically.

2.Add support for multiple displays using multiplexing.

3.Interface with sensors to display real-time data.
