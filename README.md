# electrical-task
![2022-08-07](https://user-images.githubusercontent.com/109479248/183304856-10aa6ab2-d619-4a18-88f3-b5f37889fa46.png)

#include <Servo.h>

Servo myservo;  


int pos = 0;   

void setup() {
  myservo.attach(7);  
}

void loop() {
  for (pos = 0; pos <= 180; pos += 1) { 
    myservo.write(pos);             
    delay(15);                       
  }
  for (pos = 180; pos >= 0; pos -= 1) { 
    myservo.write(pos);              
    delay(15);         
  }
}
