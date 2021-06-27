# robotarm-servo-motor-design

//the code used

#include <Servo.h>

Servo servo1;
Servo servo2;
Servo servo3;
Servo servo4;
Servo servo5;

int potpin1 = A1;
int potpin2 = A2;
int potpin3 = A3;
int potpin4 = A4;
int potpin5 = A5;

int valpotpin1;
int valpotpin2;
int valpotpin3;
int valpotpin4;
int valpotpin5;


void setup() {
  
  servo1.attach(3);
  servo2.attach(5);
  servo3.attach(6);
  servo4.attach(9);
  servo5.attach(10);
  

}

void loop(){

  valpotpin1 = analogRead (potpin1);
  valpotpin1 = map(valpotpin1, 0, 1023, 0, 180);
  servo1.write(valpotpin1);
  delay(10);
  
  
  valpotpin2 = analogRead (potpin2);
  valpotpin2 = map(valpotpin2, 0, 1023, 0, 180);
  servo2.write(valpotpin2);
  delay(10);
  
  valpotpin3 = analogRead (potpin3);
  valpotpin3 = map(valpotpin3, 0, 1023, 0, 180);
  servo3.write(valpotpin3);
  delay(10);
  
  valpotpin4 = analogRead (potpin4);
  valpotpin4 = map(valpotpin4, 0, 1023, 0, 180);
  servo4.write(valpotpin4);
  delay(10);
  
  valpotpin5 = analogRead (potpin5);
  valpotpin5 = map(valpotpin5, 0, 1023, 0, 180);
  servo5.write(valpotpin5);
  delay(10);



}
