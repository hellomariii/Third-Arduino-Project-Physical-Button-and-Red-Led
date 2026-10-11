# Third-Arduino-Project-Physical-Button-and-Red-Led
Using a physical button to turn on a red LED

## COLOR KeyWords from now own
Gr = Green,
Y = Yellow,  
O = Orange,
Bl = Black,
Br = Brown,
Blu = Blue,
R = Red,
P = Purple,
G = Grey,

## Goal
Make an LED light by pressing a button.

## Ideal Pathway
My finger --> button --> Arduino input pin --> code --> LED

## Materials 
-RLED
-4 jumper wires
-Button 
-330 Ohm resistor
-Mega 2560 control board
-breadboard
-USB

## Circuit
RLED
Pin 9 --> 330 Ohm --> RLED --> GND
Button
Pin 2 --> Button --> GND

## Workflow
Red LED
Arduino Pin 9 --> YJW --> 330 Ohm --> RLED --> BlJW --> Arduino GND
Button(B)
Arduino Pin 2 --> GJW --> B --> 

## BreadBoard Position
RLED
Pin 9-40d-YWJ-40e-330-40f-40g-anode-41g-cathode-41h-BlJW-GND
Button(B)
Pin 2-50g-GrJW-50f/52f-button-50e/52e-52d-OJW-GND

## Results 
When the physical button is pressed the RLED lights up; LED does not light up when button is not pressed

## Code

```cpp
const int buttonPin = 2;
const int redLedPin = 9;

void setup() {
  pinMode(buttonPin, INPUT_PULLUP);
  pinMode(redLedPin, OUTPUT);
}

void loop() {
  int buttonState = digitalRead(buttonPin);

  if (buttonState == LOW) {
    digitalWrite(redLedPin, HIGH);
  } else {
    digitalWrite(redLedPin, LOW);
  }
}

```
## Troubleshooting 
Orientation of wires were incorrect on breadboard; OJW,button and GrJW were all in a row on the breadboard (row 50 d,e,f,g and row 52 e,f), thus not being a complete circuit vs a complete circuit (row 50 e,f,g and row d,e,f)

## Lesson
Dont be afraid to try something without the guidance of the internet

## What I Learned
-Learned how to combine LED and a physical button 
- Created a circuit pathway that could put my idea into reality
- Had to troubleshoot and debug but I was able to troubleshoot completely on my own.
- Proud of myself

## Photos
<img width="3024" height="4032" alt="IMG_1360" src="https://github.com/user-attachments/assets/cdc31b89-90f2-4572-aba8-ffded4effc05" />
<img width="3024" height="4032" alt="IMG_1361" src="https://github.com/user-attachments/assets/6266d9fb-2bce-4763-b39d-86e9842dee25" />
<img width="3024" height="4032" alt="IMG_1362" src="https://github.com/user-attachments/assets/663c78f7-bbaa-4830-b861-4372f3eff8e3" />




