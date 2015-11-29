# 09.29: Simple LED Blink
## Blink LED on arduino board

```arduino 
int thePin = 13;
int delayTime = 3000;
// Global variables useful since it helps to repeat yourself less

void setup() 
{
 // void: means do not have to return anything (e.g. integer, etc). 
// put your setup code here, to run once:

pinMode(thePin, OUTPUT); 
  // pinMode: (function) tells a pin what to do.
  // output: (macro) rip out text and put something in its place. 
  delayTime = delayTime / 2; 
}

void loop() 
{
  // put your main code here, to run repeatedly:
  
  digitalWrite(thePin, HIGH); 
  delay(delayTime);
  digitalWrite(thePin, LOW);
  delay(delayTime);
  // digitalWrite: (function) allows you to set digital pin; HIGH = on & LOW = off.
  // delay: (function) time in miliseconds.
}
```
