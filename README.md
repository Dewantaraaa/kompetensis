import time
import RPi.GPIO as GPIO
GPIO.setmode(GPIO.BOARD)
GPIO.setwarnings(False)

LED_Red = 7
LED_Green = 11
LED_Yellow = 33
LED_Blue = 13

GPIO.setup(LED_Red,GPIO.OUT)
GPIO.setup(LED_Green,GPIO.OUT)
GPIO.setup(LED_Yellow,GPIO.OUT)
GPIO.setup(LED_Blue,GPIO.OUT)

while 1:
   GPIO.output(LED_Green, False)
   GPIO.output(LED_Red, True)
   time.sleep(1)
   GPIO.output(LED_Red, False)
   GPIO.output(LED_Green, True)
   time.sleep(1)
   GPIO.output(LED_Green, False)
   GPIO.output(LED_Yellow, True)
   time.sleep(1)
   GPIO.output(LED_Yellow, False)
   GPIO.output(LED_Blue, True)
   time.sleep(1)
   GPIO.output(LED_Blue, False)
   GPIO.output(LED_Yellow, True)
   time.sleep(1)
   GPIO.output(LED_Yellow, False)
   GPIO.output(LED_Green, True)
   time.sleep(1)

  
