# Push-button-counter
int i;
void setup()
{
  Serial.begin(9600);
  pinMode(3,INPUT);
}

void loop()
{
  int x = digitalRead(3);
  if (x==1)
  {
    i=i+1;
  Serial.println(i);
  delay(300);
  }
  else{
    i=0;
  }
  
    
}
