# Cybersecurity 150 Lab

## Name of Project
ESP32: Messages to WhatsApp

## Purpose
To send messages from the ESP32 to send messages to WhatsApp using CallMeBot

## Equipment
* [ESP32Cam](https://www.amazon.com/Aideepen-ESP32-CAM-Bluetooth-ESP32-CAM-MB-Arduino/dp/B08P2578LV/ref=sr_1_3?crid=4FY0ECFW0ZX7&keywords=ESP32+Cam&qid=1678902050&sprefix=esp32+cam%2Caps%2C240&sr=8-3)

* [USB Micro Data Cable](https://www.amazon.com/AmazonBasics-Male-Micro-Cable-Black/dp/B0711PVX6Z/ref=sr_1_1_sspa?keywords=micro+usb+data+cable&qid=1678902214&sprefix=Micro+USB+data+%2Caps%2C89&sr=8-1-spons&psc=1&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUFaU0NaUVZHU1RFUlAmZW5jcnlwdGVkSWQ9QTA3NTA4MDVFVERCS01HVlgxM1YmZW5jcnlwdGVkQWRJZD1BMDE4NTE1NTIwWUdONkdWSzU1M1Amd2lkZ2V0TmFtZT1zcF9hdGYmYWN0aW9uPWNsaWNrUmVkaXJlY3QmZG9Ob3RMb2dDbGljaz10cnVl)

## Link to Documentation Followed
-(https://randomnerdtutorials.com/esp32-send-messages-whatsapp/)

##### Youtube Video 1: 
https://www.youtube.com/watch?v=1CWIgxkviuU
##### Youtube Video 2: 
https://www.youtube.com/watch?v=Tp8CTeV5j1Q&t=183s 

## Steps I followed
1. Add this phone number +34 621 331 709 to your Phone Contacts. This is the number of the Api Bot
2. Send the authorization message: “I allow callmebot to send me messages”, to the Api Bot contact. 
3. Wait until you receive the message “API Activated for your phone number", and the Api key from the Bot
4. Now you need to prepare the ESP32 code. Open the Arduino IDE. Go to Sketch > Include Library > Manage Libraries and Search for URLEncode library by Masayuki Sugahara and install it.
5. Next copy and paste the example code from "random nerd tutorials", and insert your network SSID and password, phone number, and API key.
6. Select your board and port, and upload the code to your ESP32.
7. Open the Serial Monitor in Arduino and set the baud rate to 115200.
8. Press the reset (RST) button on the ESP32 board, and wait for the successful network connection message.
9. Finally, Look at your phone for your message!

## Pictures of Project
![230D9614-0BC2-4E40-A1F8-2834A5D72CEA](https://github.com/Domhubb/CSN150-Documentation-Template/assets/166040147/d27069a9-d265-409e-b68a-7a2409f32314)
![midterm pic](https://github.com/Domhubb/CSN150-Documentation-Template/assets/166040147/56a0d5c4-d6be-4a8e-8c04-b79570bb43a9)


