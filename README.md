# LED-code3
import RPi.GPIO as GPIO
import time

LedGpio=18
waitTime=1

GPIO.setwarnings(False)
GPIO.setmode(GPIO.BCM)
GPIO.setup(LedGpio,GPIO.OUT)

for i in range(20):
    GPIO.output(LedGpio, True)
    time.sleep(WaitTime)
    Gpio.output(LedGpio, False)
    time.sleep(WaitTime)
    
GPIO.cleanup()
