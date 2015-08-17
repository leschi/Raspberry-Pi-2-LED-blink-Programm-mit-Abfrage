import os
import time
import RPi.GPIO as GPIO
GPIO.setmode(GPIO.BOARD)
GPIO.setwarnings(False)
GPIO.setup(7,GPIO.OUT)
GPIO.setup(11,GPIO.OUT)
GPIO.setup(13,GPIO.OUT)
led_choice = 0
count = 0

os.system('clear')
print "Dieses Skrip wurde von Leopold Pöchinger erstellt."
print "Welche LED soll blinken?"
print "1: Rot? (Pin 7)"
print "2: Gruen? (Pin 11)"
print "3: Gelb? (Pin 13)"
print "4: Alle? (Pins 7, 11 & 13)"
led_choice = input("Waehle aus: ")

if led_choice == 1:
	os.system('clear')
	print "Du hast die rote LED ausgewaehlt"
	count = input("Wie oft soll sie blinken?: ")
	while count > 0:
		GPIO.output(7,GPIO.HIGH)
		time.sleep(1)
		GPIO.output(7,GPIO.LOW)
		time.sleep(1)
		count = count - 1
		
if led_choice == 2:
	os.system('clear')
	print "Du hast die gruene LED ausgewaehlt"
	count = input("Wie oft soll sie blinken?: ")
	while count > 0:
		GPIO.output(11,GPIO.HIGH)
		time.sleep(1)
		GPIO.output(11,GPIO.LOW)
		time.sleep(1)
		count = count - 1
if led_choice == 3:
        os.system('clear')
        print "Du hast die gelbe LED ausgewaehlt"
        count = input("Wie oft soll sie blinken?: ")
        while count > 0:
                GPIO.output(13,GPIO.HIGH)
                time.sleep(1)
                GPIO.output(13,GPIO.LOW)
                time.sleep(1)
                count = count - 1

if led_choice == 4:
	os.system('clear')
	print "Du hast alle LEDs ausgewaehlt"
	count = input("Wie oft soll sie blinken?: ")
	while count > 0:
		GPIO.output(7,GPIO.HIGH)
		GPIO.output(11,GPIO.HIGH)
	        GPIO.output(13,GPIO.HIGH)
		time.sleep(1)
		GPIO.output(7,GPIO.LOW)
                GPIO.output(11,GPIO.LOW)
                GPIO.output(13,GPIO.LOW)
                time.sleep(1)
                count = count - 1
                

GPIO.cleanup()
