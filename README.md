# Smart-street-lightning
smart street lightning project based on IoT.
 This project is based on [IoT].The basic idea behind this project is that whenever a vehicle passes over an LDR, the intensity of light falling on it reduces and as a result the corresponding LEDs turns on. The main advantage of the project is energy saving. We can send this data over the cloud to calculate how much energy is conserved. It is done with the help of LDR[light dependent resistor]. It is implemented on [Arduino]. The code used is :- 
int sensorPin1 = A0;
int sensorPin2 = A1;
int sensorPin3 = A2;
int sensorValue1 = 0;
int sensorValue2 = 0;
int sensorValue3 = 0;
void setup(){ 
 pinMode(5,OUTPUT);
 pinMode(6,OUTPUT);
 pinMode(7,OUTPUT);
 pinMode(8,OUTPUT);
 pinMode(9,OUTPUT);
 pinMode(10,OUTPUT);
 pinMode(11,OUTPUT);
 pinMode(12,OUTPUT);
 pinMode(13,OUTPUT);
 Serial.begin(9600);
 } 
  void loop(){
  sensorValue1 = analogRead(sensorPin1);
  Serial.print("Reading of LDR1=");
  Serial.println(sensorValue1);
  delay(200);
 }

