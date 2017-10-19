{\rtf1\ansi\ansicpg1252\cocoartf1504\cocoasubrtf760
{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\margl1440\margr1440\vieww10800\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 BSE Owen Balloon Project (2017)\
\
Combines code from MAX7456 (On-Screen-Display (OSD) shield), \
SFE_BMP180 (Altitude/Temperature sensor) and SD libraries. Reads data from \
BMP180 sensor, overlays temperature and altitude text onto video stream,\
and writes data to an SD card. \
\
NOTE: \
When run on an Arduino UNO, this sketch functions with very low available memory. \
Take note of RAM capacity issues when changing/adding additional variables. \
Commented out is a library and println to display available RAM.\
\
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0
\cf0 Arduino Shields:\
OSD Shield (http://www.tinyosshop.com/arduino-osd-shield)\
W5200 Ethernet Shield v2.2 (www.seeedstudios.com)\
\
Sensors:\
BMP180 Barometric Pressure Sensor (https://www.sparkfun.com/products/11824)\
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0
\cf0 \
Arduino Libraries:\
MAX7456 (On-Screen-Display (OSD) shield):\
	This library is used to display text (in this case temperature and altitude data) \
	over the live video feed. OSD communicates with Arduino via Serial, using \
	pin 10 as chip select. Adjust position of text on screen with \
	OSD.setCursor(< x >, < y >) and display with OSD.print(< variable >).  \
\
	Retrieved from http://www.tinyosshop.com/datasheet/MAX7456.rar\
\
SFE_BMP180 (Altitude/Temperature sensor):\
	This library is used to retrieve measurements from the temp/alt sensor. Sensor\
	communicates with Arduino via I2C. In this code, formatted to produce \
	temperature in Fahrenheit and altitude in meters above sea level (where\
	sea level is approximated by 1013.25 mbar).\
\
	Retrieved from https://github.com/sparkfun/BMP180_Breakout_Arduino_Library/archive/master.zip \
	\
MemoryFree:\
	Commented out. Used to check amount of available RAM.\
\
	Retrieved from http://github.com/maniacbug/MemoryFree}