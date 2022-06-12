# SECOND-CLASS

## TOPIC
- RGB LED
- SERIAL CODE
### RGB LED

### CODE
1.int redPin = 3;      
2.int greenPin = 4;       
3.int bluePin = 5;
4.void setup() {
5.pinMode(redPin, OUTPUT);         
6.pinMode(greenPin, OUTPUT);           
7.pinMode(bluePin, OUTPUT); 
8.}
 
void loop()
     {   setColor(255, 0, 0); delay(1000); // red
         setColor(0, 255, 0); delay(1000);  // green
         setColor(0,0,255); delay(1000);   // blue
         setColor(0,100,100); delay(1000);     // aqua
         setColor(130,50,0); delay(1000);   // yellow
         setColor(0,100,100); delay(1000);    // yellow
         setColor(80,0,80); delay(1000);    // yellow
       }

void setColor(int red, int green, int blue)
     {
       analogWrite(redPin, red);
       analogWrite(greenPin, green);
       analogWrite(bluePin, blue); 
     }
