//*SunGlass-Bot an automatic sunglass by ashraf minhaj.
//full tutorial on youtube: www.youtube.com/c/fusebatti
//Contact if necessary ashraf_minhaj@yahoo.com

#include<Servo.h>
Servo sglass; //servo name
int ldr= 0;   //connect LDR to A0
int value= 0; //define value 0

void setup() 
{
  Serial.begin(9600); //this is not necessary-but to show value to pc
  sglass.attach(9);   //declare in which pin the servo you attach
}
void loop()
{
  value = analogRead(ldr);  //read value-analog from A0
  Serial.println(value);    
  delay(100);
  if(value<100)  //change the value as you wish
  {
    sglass.write(155); //black glass down
    delay(100);     //a bit delay for the servo to move there
  }
  else
  {
    sglass.write(80);  //black glass up
    delay(100);
  }
}
