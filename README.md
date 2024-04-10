# Cybersecurity 150 Lab

## Name of Project
ESP32 Whatsapp Message Sender

## Purpose
Create an ESP32 project using the ESP32CAM to communicate with Whatsapp

## Equipment
* [ESP32Cam](https://www.amazon.com/Aideepen-ESP32-CAM-Bluetooth-ESP32-CAM-MB-Arduino/dp/B08P2578LV/ref=sr_1_3?crid=4FY0ECFW0ZX7&keywords=ESP32+Cam&qid=1678902050&sprefix=esp32+cam%2Caps%2C240&sr=8-3)

* USB C to USB C Cable
## Link to Documentation Followed
- [[Random Nerd Tutorials - ](https://randomnerdtutorials.com/esp32-send-messages-whatsapp/)](https://randomnerdtutorials.com/esp32-send-messages-whatsapp/)
- (https://www.youtube.com/watch?v=1CWIgxkviuU)

## Steps I followed
1. The first step I did was to test if my board even worked so I tried to do the camera project again, found out the board worked and not the camera.

2. Then I tested the lights on the board.
   
3. The third step I did was setting up the callmebot api before even writing the code. It is pretty easy to setup you just need to send a text to the bot on whatsapp, and it'll give you a link to insert into the esp32 code.

4. Writing the code and troubleshooting the API (Instead of copy pasting it I wrote it manually from the site so I could understand how the code worked.)

5. Adding light functionality to my code for it to blink when connecting and stop when it connected.(I essentially looked for a flashing light function somewhere, the one I found was done in the loop but it just makes it flash forever.
   So I took the blinking code and made some tweaks so it blinks slower, and moved it so it doesn't blink forever into the while loop.

6. After that I used the verify option to find any errors in the code which some I found are listed below. The main errors where just with the lighting.

7. So when all of these are completed, you should be able to send messages to yourself on whatsapp or anyone else who allows that bot to send messages. Or make your own Bot and spam people if you want.

## Problems
1. First problem I had is that I was on the wrong serial, I just changed the port and it fixed that issue. (On Mac its serial port 10 instead of 110, and for windows I believe its Com3)

2. Second problem I had was with connecting to the wifi, problem was mitagated but not removed by changing hotspot to 4G instead of 5G, this will only be a problem if you are using a phone hotspot.

3. The third is when I tried to add the indicator lights to blink untill it successfully connected to the internet. At first I tried to do it in the loop part but that just makes it infinitely loop.
   So then I put it in the while connecting, under the main which is a while loop so the light blinks untill it has successfully connected to the internet.

