# Fire-and-Safety-Buzzer![emergency buzzer](https://user-images.githubusercontent.com/77285043/120166607-61c26480-c21a-11eb-8f8e-d009c707bc4f.png)
float temp;
float vout;
float vout1;
int LED = 13;
int gassensor;
int piezo;
void setup()
{
  pinMode(A0,INPUT);
  pinMode(A1,INPUT);
  pinMode(LED,OUTPUT);
  pinMode(piezo,OUTPUT);
  Serial.begin(9600);
}
void loop()
{
  vout=analogread(A1);
  vout=(vout/1000)=5000;
  temp=(vout1-500)/100;
  gassensor'analogRead(A0);
  if(temp <= 10)
  {
    digitalWrite(LED,HIGH);
  }
  else
  {
    digitalWrite(LED,LOW);
  }
  if(gassensor,<= 100)
  {
    digitalWrite(piezo,HIGH);
  }
  else
  {
    digitalWrite(piezo,LOW);
  }
  Serial.print("in degrees= ");
  Serial.print(" ");
  Serial.print(temp);
  Serial.print("/t");
  Serial.print(gassensor);
  Serial.print();
  delay(1000);
