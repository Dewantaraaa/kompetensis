![image](https://github.com/user-attachments/assets/8d687ed3-0aea-44a6-91cd-a4a31f3aecb3)# kompetensis

import time
import RPi.GPIO as GPIO
GPIO.setmode(GPIO.BOARD)
GPIO.setwarnings(False)

LED_Red = 7
LED_Green = 11
LED_Yellow = 12
LED_Blue = 13

GPIO.setup(LED_Red,GPIO.OUT)
GPIO.setup(LED_Green,GPIO.OUT)
GPIO.setup(LED_Yellow,GPIO.OUT)
GPIO.setup(LED_Blue,GPIO.OUT)

while 1:
   GPIO.output(LED_Red, True)
   time.sleep(1)
   GPIO.output(LED_Red, False)
   time.sleep(1)
   GPIO.output(LED_Green, True)
   time.sleep(1)
   GPIO.output(LED_Green, False)
   time.sleep(1)
   GPIO.output(LED_Yellow, True)
   time.sleep(1)
   GPIO.output(LED_Yellow, False)
   time.sleep(1)
   GPIO.output(LED_Blue, True)
   time.sleep(1)
   GPIO.output(LED_Blue, False)
   time.sleep(1)
   time.sleep(1)
   GPIO.output(LED_Yellow, True)
   time.sleep(1)
   GPIO.output(LED_Yellow, False)
   time.sleep(1)
   GPIO.output(LED_Green, True)
   time.sleep(1)
   GPIO.output(LED_Green, False)
   time.sleep(1)
   

  
