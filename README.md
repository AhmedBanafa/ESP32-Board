Wasdom ESP32 خوارزمية تشغيل قطعة 

1-In your Arduino IDE, go to File> Preferences

2-Enter the following into the “Additional Board Manager URLs” field:

https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json
Then, click the “OK” button:

3-Open the Boards Manager. Go to Tools > Board > Boards Manager…

4-Search for ESP32 and press install button for the “ESP32 by Espressif Systems“:

____________________________________________________________________
الاكواد المستخدمة


#include <Arduino.h>

#define LED 2

void setup() {
  // put your setup code here, to run once:
  Serial.begin(115200);
  pinMode(LED, OUTPUT);
}

void loop() {
  // put your main code here, to run repeatedly:
  digitalWrite(LED, HIGH);
  Serial.println("LED is on");
  delay(1000);
  digitalWrite(LED, LOW);
  Serial.println("LED is off");
  delay(1000);
}


