MIT License

Copyright (c) 2021, All Rights Reserved, Sudhir Kshirsagar, Steve Mylroie

Permission is hereby granted, free of charge, to any person obtaining a copy
of this Data and associated documentation files (the "Data"), to deal
in the Data without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Data, and to permit persons to whom the Data is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Data.

THE DATA IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
DATA.

**CHARIoT Challenge: Flood Scenario**

Team SmartIoT flood scenario was intended to create data for PSCR AR teams and other types of IoT research for First Responder sensor and Smart City Innovations programs.  The data corresponds to the "TEEX" location where the data was meant to be used with AR/VR headsets.


**Scenario Defnition:**

The flood scenario provided eight data streams from eight types of sensors. Each stream was provided as a CSV file and was transmitted as an MQTT based json string by the IoT gateway simulator hardware.

The eight sensor types were:
E Coli
Heart Rate
Radio Chat
Oil Slick Detection
Oil Well Spill Monitor
Vehicle OnStar System Alarms
pH 
Road Closure Violation Count

**Data Dictionary**

**Introduction:**
This Section provides a data dictionary for all sensor types.
**Attributes:**
ID,name,time,latitude,longitude,value,units,range

**ID**: Sensor Identifier (optional)
**name/type**: Name or type of the sensor
**time** A standardized UTC date and time. 
**latitude** 
**longitude**
**value** sensor measurement
**units** measurement system
**range** intensity of the measurement


**Example Sensor Messages:**
name,time,latitude,longitude,value,units,range
Wastewater Treatment Plant E Coli,2020-05-19 14:06:24.589692Z,30.566435,-96.370411,300,count,MEDIUM

type, ID, time, latitude, longitude,value,units,,range
First Responder Heart Rate,first_responder_1,2020-05-19 14:06:24.589692Z,37.544235,-77.44859,117,beats per minute,,HIGH

name,ID, time,latitude,longitude,value,units,range
First Responder Group Leader,leader_1,2020-05-19 14:06:24.589692Z,37.544235,-77.44859,"I see 10 people, Over",text,MEDIUM

ID,name,time,latitude,longitude,value,units,range
oilslick_1,Oil slick,2020-05-19 07:09:24.589692Z,30.531331,-96.384816,100,sq feet,LOW

ID,name,time,latitude,longitude,value,units,range
well_3976,Oil Well Spill,2020-05-19 07:10:24.589692Z,30.533216,-96.36529,100,gallons/hr,LOW

id,name,time,latitude,longitude,value,units,range
DisabledVehicle_1,buick special Texas AC1G321,2020-05-19 14:09:54.589692Z,30.592165,-96.385775,AC1G321,License Plate,LOW

name,time,latitude,longitude,value,units,range
Wastewater Treatment Plant pH,2020-05-19 14:06:24.589692Z,30.566435,-96.370411,6.5,pH,MEDIUM

ID,name,time,latitude,longitude,value,units,range
Road Closure 1 Violations,Road Closure Violations,2020-05-19 07:09:24.589692Z,30.593347,-96.377192,1,Count,LOW





