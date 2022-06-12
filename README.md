# SECOND-CLASS

## TOPIC
- RGB LED
- SERIAL CODE
### RGB LED
![image](https://user-images.githubusercontent.com/102523600/173243366-6ca67404-17ba-4ede-9278-65598a33e2e6.png)
### CODE
1. int redPin = 9;      
2. int greenPin = 10;       
3. int bluePin = 11; //Use pwm pins marked with wavy shapes.
4. void setup() {
5. pinMode(redPin, OUTPUT);         
6. pinMode(greenPin, OUTPUT);           
7. pinMode(bluePin, OUTPUT); 
8. }
9. void loop(){   
10. setColor(255, 0, 0); delay(1000); // red
11. setColor(0, 255, 0); delay(1000);  // green
12. setColor(0,0,255); delay(1000);   // blue
13. setColor(0,100,100); delay(1000);     // aqua(You can use values from 0 to 255 to make your favorite color.)
14. setColor(130,50,0); delay(1000);   // yellow
15. setColor(0,100,100); delay(1000);    // yellow
16. setColor(80,0,80); delay(1000);    // yellow
17. }
18. void setColor(int red, int green, int blue){
19. analogWrite(redPin, red);
20. analogWrite(greenPin, green);
21. analogWrite(bluePin, blue); 
22. }
### RGB color code
![image](https://user-images.githubusercontent.com/102523600/173242909-ea0cfb03-bb03-4b50-9993-1530673899c4.png)
#### PWM pin
![image](https://user-images.githubusercontent.com/102523600/173243065-b1e70332-9a36-4a37-b918-f3217d830dc1.png)
### SERIAL CODE
1. void setup() {
2. Serial.begin(9600);                // start SERIAL communication with 9600 baud rate
3. Serial.println("Goodnight moon!"); // set the data rate for the SoftwareSerial port
4. Serial.begin(9600);
5. Serial.println("Hello, world?");    //print Hello, world? at serial monitor
6. }
7. void loop() {}
