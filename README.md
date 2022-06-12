# SECOND-CLASS

## TOPIC
- RGB LED
- SERIAL CODE
### RGB LED

### CODE
1.int redPin = 8;      
2.int greenPin = 9;       
3.int bluePin = 10; //Use pwm pins marked with wavy shapes.
4.void setup() {
5.pinMode(redPin, OUTPUT);         
6.pinMode(greenPin, OUTPUT);           
7.pinMode(bluePin, OUTPUT); 
8.}
9.void loop(){   
10.setColor(255, 0, 0); delay(1000); // red
11.setColor(0, 255, 0); delay(1000);  // green
12.setColor(0,0,255); delay(1000);   // blue
13.setColor(0,100,100); delay(1000);     // aqua(You can use values from 0 to 255 to make your favorite color.)
14.setColor(130,50,0); delay(1000);   // yellow
15.setColor(0,100,100); delay(1000);    // yellow
16.setColor(80,0,80); delay(1000);    // yellow
17.}
18.void setColor(int red, int green, int blue){
19.analogWrite(redPin, red);
20.analogWrite(greenPin, green);
21.analogWrite(bluePin, blue); 
22.}
### RGB color code
![image](https://user-images.githubusercontent.com/102523600/173242909-ea0cfb03-bb03-4b50-9993-1530673899c4.png)
#### PWM pin
