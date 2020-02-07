////////////////////////////////////////
// Created with a lot of love         //
// By - Ashutosh Deshwal              //
// Website: www.ashutoshdeshwal.com   //
////////////////////////////////////////
#include <ESP8266WiFi.h>

#include <ThingSpeak.h>

WiFiClient client;

void setup()
{
  Serial.begin(9600);
ThingSpeak.begin(client);

  WiFi.disconnect();
  delay(300);
  Serial.println("START");
   WiFi.begin("ssid","password");
  while ((!(WiFi.status() == WL_CONNECTED))){
    delay(300);
    Serial.print("");

  }
  Serial.println("Connected");
  Serial.println("Your IP is");
  Serial.println((WiFi.localIP().toString()));

}


void loop()
{

    Serial.println((ThingSpeak.readIntField(channel id,1,"your read key")));
    delay(15000);

}
