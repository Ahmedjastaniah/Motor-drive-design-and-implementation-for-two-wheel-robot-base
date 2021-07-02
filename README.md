# Motor-drive-design-and-implementation-for-two-wheel-robot-base
controlling two DC motors using H bridge L298D for two wheel robot base.Each motor can rotate either for clockwise or counter-clockwise.

 ## Components
 - 2 DC motors
 - H bridge L298D
 - 1 Arduino Uno R3
 - Breadbaourd
 - 21 wires
 - 9V battery
 
 ## C++ Code 
  the code that used in the circuit is:
  ```javascript
// C++ code
//
void setup()
{
  pinMode(11, INPUT);
  pinMode(10, INPUT);
  pinMode(9, INPUT);
  pinMode(11, OUTPUT);
  pinMode(10, OUTPUT);
  pinMode(9, OUTPUT);
  pinMode(3, INPUT);
  pinMode(5, INPUT);
  pinMode(6, INPUT);
  pinMode(5, OUTPUT);
  pinMode(3, OUTPUT);
  pinMode(6, OUTPUT);
}

void loop()
{
  digitalRead(11);

  digitalRead(10);

  digitalRead(9);

  digitalWrite(11, HIGH);
  digitalWrite(10, LOW);
  analogWrite(9, 100);

  digitalRead(3);

  digitalRead(5);

  digitalRead(6);

  digitalWrite(5, HIGH);
  digitalWrite(3, LOW);
  analogWrite(6, 100);
  delay(10); // Delay a little bit to improve simulation performance
}

```
## Program
The program that used to do the circuit and the code is TINKERCAD.
