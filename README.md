// C++ code
int distancia = 0;
int i = 0;
long readUltrasonicDistance (int triggerPin, int echopin)
{
pinMode (trigger Pin, OUTPUT);
digitalWrite(triggerPin, LOW);
delayMicroseconds (2);
digitalWrite(triggerPin, HIGH);
delayMicroseconds (10);
digitalWrite(triggerPin, LOW);
pinMode (echopin, INPUT);
return pulse In (echoPin, HIGH);
void setup()
{
pinMode (8, OUTPUT);
pinMode (12, OUTPUT);
pinMode (13, OUTPUT);
pinMode (5, OUTPUT);
}
void loop()
{
distancia = 0.01723 readultrasonicDistance (11, 10);
if (distancia > 10) (
digitalWrite(8, HIGH);
digitalWrite(12, LOW);
digitalWrite(13, LOW);
digitalWrite(5, LOW);
delay(200);
digitalWrite(5, LOW);
delay(200);
} else {
digitalWrite(8, LOW);
digitalWrite(5, LOW);
}
distancia = 0.01723 readUltrasonicDistance (11, 10);
if (distancia <= 10) {
digitalWrite(8, LOW);
digitalWrite(12, HIGH);
digitalWrite(13, LOW);
digitalWrite(5, HIGH);
delay(200);
digitalWrite(5, LOW);
delay (200);
} else {
digitalWrite(12, LOW);
digitalWrite(5, LOW);
}
distancia = 0.01723) readUltrasonicDistance (11, 10);
if (distancia <= 5) {
digitalWrite(8, LOW);
digitalWrite(12, LOW);
digitalWrite(13, HIGH);
digitalWrite(5, HIGH);
delay(100);
digitalWrite(5, Low);
delay(100);
} else {
digitalWrite(13, LOW);
digitalWrite(5, LOW);
}
