INTERACTIVE SYSTEMS - PROJECT BY TEAM #53 (Joe Arens & Marcel Niedballa) lol
-------------------------------------------------------------------------------------------------------------------------------------
In this project we are going to implement a local pipeline, consisting of a input, given by an input (Morse Code and button), a 
processing unit (WeMos D1 mini) and an output (hex-code and servo motor).

PREREQUISITIES
-------------------------------------------------------------------------------------------------------------------------------------
- Microcontroller
- Jumper wires
- Breadboard
- LED's
- Buttons
- Resistors
- Servo Motors
- Shift Register
- Aluminum foil
- paper notes

CONCEPT
--------------------------------------------------------------------------------------------------------------------------------------
-First step: Implement default Input
 For the mandatory part, we connect a button to the microcontroller, which acts as the input method to use the morse code in order to
 implement the characters. A function decides how long a “long” and “short” signal is, whilst the button is pressed. It will also
 determine the length of the break between two signals to ease the input.

             Implement alternative Input
 For the alternative method, we are planning on including a FSR using aluminum foil, wires and resistors to build a touch button. 
 It is basically used the same way as the button method. We will use a function, that defines the state of the FSR by connecting 
 the applied pressure on the foil to the length of the signal, characterized by “short” or “long”. 

-Second step: Implement default output
 For the mandatory part, we are going to use the given, to the microcontroller connected  servo motor, that is supposed to point at 
 the hexadecimal-number given by the input. We will use a function, which determines the necessary degree, the pointer needs to 
 circle to. Additionally, we will include an equation to calculate the time the servo motor needs to do a full 360° turn. 
 This information will eventually be used to calculate the next output and so on. The function will end with either a “time-out” or 
 as mentioned above a specified end-signal.

              Implement alternative output
 As for the alternative output method, we are going to utilize a similar method to the default one, but changed in a way, that people,
 who do not know the hexadecimal-system also understand the given output. Our plan is to build a circle, consisting of the servo motor 
 and 13 units, on which the motor can eventually point at (right side of the picture above). Regarding the microcontroller, two LED’s 
 will be added to define the range of characters. 
 When the input is given, a function decides, if it is a letter from A to M, M to Z, a number from 0 up to 9 or 3 freely chosen special
 characters, such as “+”,”-“ and “/” for example and lets, in the first case, the first LED blink and in the second case, the second LED
 blink. If no lamp shines, the latter case is selected (left side in picture above). Summarized, instead of using a hexadecimal-system, 
 we are using the alphabet as an alternative.

RUNNING THE TESTS
----------------------------------------------------------------------------------------------------------------------------------------
The idea for the code of the tests will be implemented here

CODING STYLE
----------------------------------------------------------------------------------------------------------------------------------------
The idea fo the main code will be implemented here
