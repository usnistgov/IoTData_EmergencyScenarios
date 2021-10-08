MIT License

Copyright (c) 2020, All Rights Reserved, Michael Behrens, Barry Luke, Gary Mazzaferro

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

**CHARIoT Challenge: Mass Transit Scenario**

Team Frites scenarios are intended to create data for PSCR AR teams and other types of IoT research for First Responder sensor and Smart City Innovations programs.  This section provided an overview of the scenarios including the following information for each scenario:
•	Sensor Type and Names
•	Relative Start Time of major state changes for sensors within each of 5 scenario versions
•	Sensor Behavior 
Where possible, the names of sensors in Team Frites scenarios match the names of PSCR sensors provided to challenge competitors.

Many Team Frites Sensors contain selectable properties which support multiple selection options.  Sensor properties including: locations, sex, race, and other have multiple options. Options are randomly selected each time scenarios execute making each scenario run unique. For example, location names found in maps provided by PSCR are options for sensor locations. Each time the simulator executes a scenario, different locations are selected for sensor locations. 

Our designated team Point of Contact (Gary Mazzaferro) garym AT oedata DOT com is available for questions.

In this folder includes five (5) different excutions of the scenario data. 

**Scenario Defnition:**

The data generated for each of the five (5) instaniations of the scenation is define by the table below:

| Sensor Name | Start Time | End Time | Update Freq | Behavior |
|---------|---------|---------|---------|---------|
| **Air Quality Monitor** |
| airquality_transit_add_frites_m_001 to _0019    | 0s          | N/A        | 1s       | HVAC set to Open, Electrical Panel random, locations set to EOTC floor map, 30 second transmit time: EOTC_Floor1_North_East_Corridor_Room16, EOTC_Floor1_West_Entry_Doors, EOTC_Floor1_Corridor_Room9, EOTC_Floor2_North_Stairwell, EOTC_Floor1_Corridor_Room40, EOTC_Floor1_North_Stairwell |
| **Computer Aided Dispatch**                               |
| cadfire_transit_frites                              | 0s          | 2s         | 1s       | FIRE Dept. CAD. static data, transmit once, Time On Scene is current clock time, Time Received and Time Dispatched are negative offsets from start of scenario |
| **Fire Alarms**                                           |
| firealarm_transit_frites                            | 0s          | N/A        | 30s      | fire alarm type float: Platform_East_Stairwell, EB_Green_Tunnel_Entrance, Platform_Central_EB, Platform_Central_WB, Platform_East_Stairwell_Plaza_Level, Platform_West_EB, Platform_West_WB, Platform_West_Stairwell, WB_Green_Tunnel_Entrance |
|  **Intelligent Camera**                                   |
| interiorcamera_transit_frites                       | 0s          | N/A        | 30s      | alerts for smoke detected. Multiple camera locations: Platform_East_Stairwell, Platform_West_Stairwell, Platform_Central, Platform_North, Platform_South, Platform_Central_Stairwell  |
| **Officer Vitals**                                        |
| officervitals_transit_add_frites_b_001           | 0s          | N/A        | 11s      | Officer A has alert level for high respiratory rate |
| officervitals_transit_add_frites_b_002  to _045 | 0s          | N/A        | 11s      | Sensors 2 through 45 have no alert levels set |
| **Safety Monitor** |
| safetymonitor_transit_frites_a                     | 0s          | N/A        | 11s      | Officer 1 with Emergency Button automatic alert at 4 minutes |
| safetymonitor_transit_frites_b_002 to _045       | 11s         | N/A        | 11s |         no alerts for sensors 2-45, area oxygen, area temperature set to fire levels for tunnel,  motionless time floats between 2 and 5 |
| **Security Sensor** |
| security_transit_frites                             | 0s          | N/A        | 30s      | Emergency Exit and forced open, removed normal: East_Stairwell_Emergency_Exit, South_Stairwell_Emergency_Exit, Platform_East_Stairwell, EB_Green_Tunnel_Entrance, Platform_Central_EB, Platform_Central_WB, Platform_East_Stairwell_Plaza_Level, Platform_West_EB, Platform_West_WB, Platform_West_Stairwell, WB_Green_Tunnel_Entrance, EB_Central_Corridor_Emergency_Exit |
| **Smart Building Sensor** |
| building_transit_frites                             | 0s          | N/A        | 30s      | smart building, HVAC alert, Electrical Panel Main Off: Platform_East_Stairwell, Platform_Central, Corridor_SB_3, Platform_East_Stairwell, Platform_West_Stairwell, Platform_Central, Platform_North, Platform_South, Platform_Central_Stairwell |
| **Tunnel Structural Integrity Sensor**                    |
| structuralintegrity_transit_frites                  | 0s          | N/A        | 60s      | consolidated risk set to high, cracking set: MP_2_WestBound_Tunnel, MP_1_WestBound_Tunnel, MP_2_EastBound_Tunnel, MP_1_EastBound_Tunnel |
| **Subway Car Status**                                     |
| subwaycarstatus_transit_frites                      | 3s          | 16s        | 3s       | emergency exit alert: Car_001, Car_002, Car_003, Car_004, Car_005 |
| **Triage Tag**                                            |
| triagetag_transit_frites_a_001                    | 0s          | N/A        | 10s      | all vitals set to critical values for alert, WM Difficulty Breathing, patient 1 and 2 |
| triagetag_transit_frites_b_002                    | 0s          | N/A        | 10s      | WF Adult, all vitals set to critical values for alert, WF Fall, patients 1 and 2 |
| triagetag_transit_frites_c_003                    | 0s          | N/A        | 10s      | all vitals set to values for alert, patients 3 & 4, Shock Index High, Traige Yellow, BM difficulty breathing |
| triagetag_transit_frites_d_004                    | 0s          | N/A        | 10s      | all vitals set to alert values, BF Fall, Patient Yellow | 0s          | N/A        | 10s      | all vitals set to alert, Asian Male, Fall, Patient Yellow |
| triagetag_transit_frites_f_006                    | 0s          | N/A        | 10s      | all vitals set to critical values for alert, WM difficulty breathing, yellow  |
| **Voltage Sensors**                                       |
| voltage_transit_add_frites                         | 0s          | N/A        | 44s      | electrical integrity, heat detection alert set, 15 sensor locations: MP_2_Tunnel_Eastbound_Section_331, MP_2_Tunnel_Eastbound_Section_332, MP_2_Tunnel_Eastbound_Section_333, MP_2_Tunnel_Eastbound_Section_334, MP_2_Tunnel_Eastbound_Section_335, MP_2_Tunnel_Westbound_Section_331, MP_2_Tunnel_Westbound_Section_332, MP_2_Tunnel_Westbound_Section_333, MP_2_Tunnel_Westbound_Section_334, MP_2_Tunnel_Westbound_Section_335, MP_1_Tunnel_Eastbound_Section_331, MP_1_Tunnel_Eastbound_Section_332, MP_1_Tunnel_Eastbound_Section_333, MP_1_Tunnel_Eastbound_Section_334, MP_1_Tunnel_Eastbound_Section_335 |

**Data Dictionary**

**Introduction:**
This Section provides a data dictionary for all sensor devices in the active shooter secnarionprovided by Team FRITES. It includes an overview of our approach to data structure as well as describing the value that each sensor provides to public safety. JSON file structures provide detailed information on each attribute, including severity levels, transmission rates, and data ranges. The JSON data displayed in the Data Dictionary represent values specific to a single scenario. Each sensor has been customized to display scenario specific data. For example, the Air Quality sensor has been programmed to display environmental data that is appropriate for the Mass Transit Accident and different data for the Wildland Fire scenario.
The sensor devices are easily configurable and can be modified to transmit a virtually unlimited amount of data. Our public safety Subject Matter Experts created and configured all of the sensors used in our submission. All sensor devices have a set of standard attributes.

**Common Attributes:**

**Device ID**: The name of the sensor device. The suffix “add” at the end of a sensor name indicates that it provides supplemental information to a NIST sensor of the same name. Each device id also ends in a 3 digit number, i.e.: 001. This indicates the sensor instance number. 
**Time:** A standardized UTC date and time stamp. 
**Location:** Many devices transmit a street address and additional information on the specific sensor placement within the location (e.g. 3rd floor, north hallway). NOTE: GPS data was not used because of an inability to sync the coordinate data to the locations that PSCR will be using. 
**Value & Units:** Consistent with PSCR data structures, some sensor values are followed by a data field labeled “unit” which specifies the unit of measurement (bpm, ppm, %, degrees F, etc.) 
**Device Data Range:** Some sensors transmit the minimum and maximum value that the device is capable of measuring. This data should not be confused with the severity alert levels and is intended to allow detection of a malfunctioning sensor (in cases where a transmitted value was beyond the allowable range of the device).

**Long Form Data Field Descriptors:**
Our sensors use Long Form Data Descriptors to provide maximum ease of readability. Each attribute is clearly defined and easily understood. For example, the weather station sensor uses data fields labeled “temperature”, “humidity”, wind_speed”, and “peak_wind_speed” instead of displaying short form abbreviations for these values. While short form field descriptors, using industry accepted abbreviations, may be preferred to reduce the bandwidth requirements we elected to provide more information to help AR teams who may not have experience working with these types of data. If PSCR desires, we can convert to a smaller form.

**Data Field Values**
Each sensor is designed to provide actionable information to the incident commander by providing easily understood numbers or descriptive words. In some cases, the use of descriptive text is preferred to the display of numeric values. For example, Carbon Monoxide levels are presented as None, Trace, Increasing, and High instead of providing specific numeric values. This type of display reduces cognitive load and allows for rapid analysis of the presented data and its impact to emergency operations. Our public safety Subject Matter Experts determined the type of data and the manner in which it was presented.

**Severity Level Indicators:**
Our devices transmit two different sets of severity indicators. Each sensor will provide a Low, Medium and High severity threshold as prescribed by PSCR. The sensors will also transmit four additional severity thresholds that were designed by our public safety Subject Matter Experts. These include Low, Critical Low, High, and Critical High. This allows severity levels to be set for values that are below the acceptable range and above the acceptable range. For example, a first responders heart rate may be too fast or too slow. The use of the Low, Critical Low, High and Critical High provides flexibility to address these issues. They also allow for an easier distinction of whether the alert value is below the normal range or above the normal range. For example, using PSCR values, a very low heart rate would trigger a high severity alert, possibly confusing the incident commander who may think that the firefighters heart rate is too fast because they see an alert value coded “high”. Each sensor is customized with alert values and some sensors do not require all severity levels.

PSCR severity levels are noted in the data stream using a standardized format in which “xxx” represents the name of the sensor (e.g. “heart_rate”) xxx_pscr_alert_low xxx_pscr_alert_medium xxx_pscr_alert_high
Team FRITES severity levels are noted using the following format, in which “xxx” also refers to the name of the sensor (e.g. “heart rate”).

xxx_alert_low xxx_alert_critical_low xxx_alert_high xxx_alert_critical_high
AR teams are free to use either set of severity indicators that best meet their needs. We understand that AR teams may have already programmed their appliances to accept the three PSCR designated levels.

**Data Stream:** 

NIST will manage the flow of prebuilt messages to the AR Teams. Sensor data messages will not be generated by Team FRITES devices.

Multiple instances of the same sensor are noted with the placement of a three-digit number at the end of the sensor name (e.g., xxx_001, xxx_002, xxx_023). This will allow AR teams to logically associated a group of sensors to the same first responder. For example, in the Active Shooter scenario, a single police officer would be assigned the following sensors if they were the second officer in the overall response group: officer_vitals_002 (NIST sensor) officer_vitals_add_002 (Team FRITES sensor) cognitive_monitor_002 (Team FRITES sensor) officer_safety_002 (Team FRITES sensor) safety_monitor_002 (Team FRITES sensor).

AR teams must take steps to associate the data as it may not be correlated for them by PSCR.
Unique Sensor Devices The following sensors were developed to enhance situational awareness and maximize first responder safety. We believe that these innovative sensors highlight the “art of the possible” and further demonstrate the importance of leveraging data to support public safety.

**Structural Integrity Sensor:** This device monitors the integrity of critical infrastructure sites which include bridges, subway tunnels, radio communications towers and hospitals. It can signal the imminent collapse of building or allow the ongoing monitoring of a structure that has been damaged or is being compromised. This information provides vital life safety information to the incident commander on the status of a bridge being used for evacuation, but which is impacted by rising flood waters. Incident commanders can also continuously monitor the integrity of a structure during other emergency operations including fire, earthquake, or tornado. The device provides specific data points for ongoing monitoring of 6 factors used in civil engineering while also providing an easy to read Consolidated Failure Risk assessment. This sensor is highlighted in the Flood scenario.

**Computer Aided Dispatch (CAD):** Three sensor devices have been created to simulate information flowing to the incident commander or first responder from the communications center. Each device represents incident data for law enforcement, fire or EMS. The data stream is customized for each scenario and identifies the location of the emergency, which units are responding, and the total number of units currently on scene. CAD system data is used by many public safety agencies during simulation exercises. This data stream is highlighted in the Mass Transit Accident scenario.

**Scenario Sensor List:**

**Air Quality Add**

This sensor supplements NIST sensor Air Quality

This sensor provides the incident commander with important information on the quality of the air at the scene of the emergency event. Multiple Air Quality sensors may be deployed at an incident scene. For example, in the Mass Transit Accident, Air Quality sensors are used on the subway station platform and inside the tunnel near the accident scene.

The “Add” designation for this sensor indicate additional information augmenting Air Quality sensors provided by PSCR. PSCR has requested longitude and latitude information to the FRITES Air Quality Add sensors for the wild fire scenario allowing easier synchronization to PSCR sensors. Additionally, a “parent” field’s been added to directly associate PSCR sensors with FRITES parent Air Quality sensors.

This sensor reports the following data:
- Overall Air Quality 
- Ozone Level 
- Sulfur Dioxide Level 
- Nitrogen Dioxide Level

**Example Sensor Message:**
```json
{
	"deviceid":"airquality_transit_add_frites_m_001",
    "time":"2020-10-07 07:44:28.199064Z",
    "air_quality_level":"Hazardous",
    "air_quality_level_alert_high":"very_unhealthy",
    "air_quality_level_alert_critical_high":"hazardous",
    "air_quality_level_pscr_alert_low":"red",
    "air_quality_level_pscr_alert_medium":"very_unhealthy",
    "air_quality_level_pscr_alert_high":"hazardous",
    "ozone_level":"Normal",
    "ozone_level_alert_high":"Increasing",
    "ozone_level_alert_critical_high":"High",
    "ozone_level_pscr_alert_medium":"Increasing",
    "ozone_level_pscr_alert_high":"High",
    "sulfer_dioxide_level":"Increasing",
    "sulfer_dioxide_level_alert_low":"Trace",
    "sulfer_dioxide_level_alert_high":"Increasing",
    "sulfer_dioxide_level_alert_critical_high":"High",
    "sulfer_dioxide_level_pscr_alert_low":"Trace",
    "sulfer_dioxide_level_pscr_alert_medium":"Increasing",
    "sulfer_dioxide_level_pscr_alert_high":"High",
    "nitrogen_dioxide_level":"High",
    "nitrogen_dioxide_level_alert_low":"Trace",
    "nitrogen_dioxide_level_alert_high":"Increasing",
    "nitrogen_dioxide_level_alert_critical_high":"High",
    "nitrogen_dioxide_level_pscr_alert_low":"Trace",
    "nitrogen_dioxide_level_pscr_alert_medium":"Increasing",
    "nitrogen_dioxide_level_pscr_alert_high":"High",
    "incident_location":"100 North Main Street",
    "location_name":"Green Line Station Eastbound",
    "sensor_placement":"station_platform_west_tunnel_exit"
}
```
**Fire Computer Aided Dispatch**

This sensor simulates Fire incident data transmitted by a public safety agency communications center to first responders and incident commanders. This information represents the initial data that flows to first responders regarding an incident and establishes early situational awareness.

This sensor reports the following data:
- Incident Number 
- Incident Type 
- Incident Location 
- 911 Caller Comments 
- Units Responding 
- Time Received 
- Time Dispatched 
- Time On-Scene 
- Total Number of Units On-Scene

**Example Sensor Message:**
```json
{
	"deviceid":"cadfire_transit_frites_001",
	"time":"2020-10-07 07:44:44.886358Z",
	"incident_number":"F201114",
	"incident_type":"SUBWAY_CRASH_LOADED",
	"incident_location":"100 North Main Street",
	"location_name":"Green Line Station Eastbound",
	"comments_911_caller":"Multiple callers report subway crash, several cars off the tracks, power out, possible injuries, PD and EMS also responding",
	"units_responding":"['E21', 'E22', 'E23', 'E24', 'E25', 'L1', 'L2', 'B1', 'B2', 'B3', 'R1']",
	"time_received":"2020-10-07 07:39:44.886487Z",
	"time_dispatched":"2020-10-07 07:39:58.886544Z",
	"time_onscene":"2020-10-07 07:44:44.886581Z",
	"total_units_onscene":"11"
}
```
**Smart Fire Alarm: Fire Alarm**

This device is the second of three Smart City sensor systems. The Smart Fire Alarm sensor monitors the status of the building’s fire detection and suppression system. These sensors may be customized to match the unique needs of each scenario. Fire Alarm panel information provides important system status messages to the incident commander and provides situational awareness on the location and scope of a fire emergency. 

This sensor reports the following data:
- Alarm Type (Normal, Detector, Manual Pull Station) 
- Alarm Street Address 
- Alarm Placement

**Example Sensor Message:**
```json
{
	"deviceid":"firealarm_transit_frites_001",
	"time":"2020-10-07 07:44:53.049483Z",
	"alarm_type":"Manual_Pull_Station",
	"alarm_type_alert_high":"Manual_Pull_Station",
	"alarm_type_critical_high":"Detector",
	"alarm_type_pscr_alert_medium":"Manual_Pull_Station",
	"alarm_type_pscr_alert_high":"Detector",
	"incident_location":"100 North Main Street",
	"location_name":"Green Line Station Eastbound",
	"alarm_placement":"WB_Green_Tunnel_Entrance"
}
```
**Interior Camera**

This device simulates the transmission of video analytics data from building security cameras or from cameras placed by public safety personnel to monitor wildfires and flooding. Video and video analytics data is critically important and guides the incident commander’s decision making. The use of computer vision to analyze objects and transmit small, easy to interpret alerts helps first responders manage an emergency scene and avoids “video fatigue” caused by constant watching of live video. 

This sensor reports the following data:
- Camera Placement 
- Camera Facing Direction 
- Camera Analytics (Mass Exit, Weapon Detected, Smoke, Fire) 
- Building Address

**Example Sensor Message:**
```json
{
	"deviceid":"interiorcamera_transit_frites_001",
	"time":"2020-10-07 07:44:53.240539Z",
	"camera_location":"Platform_West_Stairwell",
	"camera_facing":"West",
	"camera_analytics":"Smoke",
	"camera_analytics_alert_high":"Mass_Exit",
	"camera_analytics_alert_critical_high":"Smoke",
	"camera_analytics_pscr_alert_medium":"Mass_Exit",
	"camera_analytics_pscr_alert_high":"Smoke",
	"incident_location":"100 North Main Street",
	"location_name":"Green Line Station Eastbound"
}
```
**Officer Vital Signs Add**

This sensor supplements NIST Sensor: Officer Vitals

This sensor provides the incident commander and first responders with important health information that allows for real time monitoring of personnel during tactical situations. Physiologic data can be used to determine when a first responder is nearing exhaustion and allow them to be removed from the incident for rehab prior to their collapse. This data is also an important for safety since it will provide alerts on sudden changes in a first responder’s medical status.

This sensor reports the following data:
- Heart Rate 
- ECG Rhythm 
- Respiratory Rate 
- Oxygen Saturation 
- Body Temperature

**Example Sensor Message:**
```json
{
	"deviceid":"officervitals_transit_add_frites_a_001",
	"time":"2020-10-07 07:44:53.030394Z",
	"ecg_heart_rhythm":"Sinus_Tachycardia",
	"ecg_heart_rhythm_alert_low":"Ectopy_Detected",
	"ecg_heart_rhythm_alert_high":"Ventricular_Tachycardia",
	"ecg_heart_rhythm_alert_critical_high":"Ventricular_Fibrillation",
	"respiratory_rate":{"value":14,"unit":"rpm"},
	"respiratory_rate_device_range_low":"0",
	"respiratory_rate_device_range_high":"100",
	"respiratory_rate_alert_low":"6",
	"respiratory_rate_alert_critical_low":"4",
	"respiratory_rate_alert_high":"20",
	"respiratory_rate_alert_critical_high":"50",
	"body_temperature":{"value":98,"unit":"degrees F"},
	"body_temperature_device_range_low":"50",
	"body_temperature_device_range_high":"115",
	"body_temperature_alert_low":"95",
	"body_temperature_alert_critical_low":"90",
	"body_temperature_alert_high":"102",
	"body_temperature_alert_critical_high":"105",
	"respiratory_rate_pscr_alert_low":"30",
	"respiratory_rate_pscr_alert_medium":"40",
	"respiratory_rate_pscr_alert_high":"50",
	"body_temperature_pscr_alert_low":"100",
	"body_temperature_pscr_alert_medium":"102",
	"body_temperature_pscr_alert_high":"10
}
```
**Safety Monitor:**

This device simulates the transmission of environmental and injury data from first responders who are engaged in high risk activities. The Safety Monitor is designed to be carried by all public safety personnel (law enforcement, fire, and EMS). It may be supplemented with an additional Officer Safety module which provides additional sensor monitoring of law enforcement personnel. The Safety Monitor identifies a severity of a fall injury and if the first responder is motionless. It also monitors the atmosphere to determine the oxygen level and has a Submersion Alert feature that immediately detects if a first responder is in the water. 

This sensor reports the following data:

- Area Temperature 
- Fall Impact Intensity 
- Motionless (Time in Seconds) 
- Area Oxygen (%) 
- Submersion Alert (OK, ALERT) 
- Location (GPS)

**Example Sensor Message:**
```json
{
	"deviceid":"safetymonitor_transit_frites_a_001",
	"time":"2020-10-07 07:44:53.045017Z",
	"area-temperature":{"value":98,"unit":"Degrees F"},
	"area_temperature_device_range_low":"-50",
	"area_temperature_device_range_high":"200",
	"area_temperature_alert_low":"40",
	"area_temperature_alert_critical_low":"32",
	"area_temperature_alert_high":"100",
	"area_temperature_alert_critical_high":"105",
	"fall_impact_intensity":{"value":0,"unit":"10 Point Scale"},"fall_impact_intensity_device_range_low":"0",
	"fall_impact_intensity_device_range_high":"10",
	"fall_impact_intensity_alert_high":"6",
	"fall_impact_intensity_alert_critical_high":"8",
	"fall_impact_intensity_pscr_alert_low":"4",
	"fall_impact_intensity_pscr_alert_medium":"6",
	"fall_impact_intensity_pscr_alert_high":"10",
	"motionless_time_seconds":{"value":60,"unit":"seconds"},"motionless_time_seconds_device_range_low":"0",
	"motionless_time_seconds_device_range_high":"3600",
	"motionless_time_seconds_alert_high":"15",
	"motionless_time_seconds_alert_critical_high":"30",
	"motionless_time_seconds_pscr_alert_low":"10",
	"motionless_time_seconds_pscr_alert_medium":"15",
	"motionless_time_seconds_pscr_alert_high":"30",
	"area_temperature_pscr_alert_medium":"105",
	"area_temperature_pscr_alert_high":"110",
	"area_oxygen":{"value":17,"unit":"%"},
	"area_oxygen_device_range_low":"0",
	"area_oxygen_device_range_high":"25",
	"area_oxygen_alert_low":"17",
	"area_oxygen_alert_critical_low":"15",
	"area_oxygen_pscr_alert_low":"18",
	"area_oxygen_pscr_alert_medium":"17",
	"area_oxygen_pscr_alert_high":"15",
	"water_submersion":"OK",
	"water_submersion_alert_critical_high":"ALERT_Submersion",
	"water_submersion_pscr_alert_high":"ALERT_Submersion"
}
```
**Smart Security: Door Mass Transit Add**

This sensor supplements NIST Sensor: Door

This device is the third of three Smart City sensor systems. The Smart Security sensors simulate the transmission of information from a buildings safety and security system. This includes information on breaches to secure areas and opening of doors and emergency exits. These sensors may be customized to match the unique needs of each scenario. Security System information provides important data to the incident commander such as which exits are being used for evacuation by persons fleeing an emergency or the location of a suspect (based on door access data). 

This sensor reports the following data:
- Event Type (Normal, Emergency Exit Open, Door Forced Open, Failed PIN, Glass Break) 
- Event Location 
- Building Street Address

**Example Sensor Message:**
```json
{
	"deviceid":"security_transit_frites_001",
	"time":"2020-10-07 07:45:01.521390Z",
	"event_type":"Glass_Break",
	"event_type_alert_high":"Emergency_Exit_Open",
	"event_type_alert_critical_high":"Door_Forced_Open",
	"event_type_pscr_alert_medium":"Emergency_Exit_Open",
	"event_type_pscr_alert_high":"Door_Forced_Open",
	"event_location":"EB_Green_Tunnel_Entrance",
	"sensor_address":"100 North Main Street",
	"location_name":"Green Line Station Eastbound"
}
```
**Smart Building: Building Electrical**

This device is one of three Smart City sensor systems. The Smart Building sensors monitor the status of HVAC and electrical systems and provide a variety of status and alert messages. These sensors highly customized to match the unique needs of each scenario. Building system information is important to provide enhanced situational awareness to the incident commander. For example, they can confirm that the building’s electrical system is off or that a damper vent has been closed to stop the spread of smoke during a fire. 

This sensor reports the following data:
- HVAC Type (Air Handler, Smoke Damper) 
- HVAC Status (Open, Closed, Fault, Alert) 
- Electrical Panel Status (Normal, Open, Main Off, Main Failure) 
- Electrical Panel Location 
- Building Street Address

**Example Sensor Message:**
```json
{
	"deviceid":"building_transit_frites_001",
	"time":"2020-10-07 07:45:01.640667Z",
	"hvac_type":"Air_Handler",
	"hvac_status":"Alert",
	"hvac_status_alert_high":"Fault",
	"hvac_status_alert_critical_high":"Alert",
	"hvac_status_pscr_alert_low":"Fault",
	"hvac_status_pscr_alert_high":"Alert",
	"electrical_panel_status":"Main_Failure",
	"electrical_panel_status_alert_low":"Open",
	"electrical_panel_status_alert_high":"Main_Off",
	"electrical_panel_status_alert_critical_high":"Main_Failure",
	"electrical_panel_status_pscr_alert_low":"Open",
	"electrical_panel_status_pscr_alert_medium":"Main_Off",
	"electrical_panel_status_pscr_alert_high":"Main_Failure",
	"electrical_panel_location":"Platform_East_Stairwell",
	"sensor_location":"100 North Main Street",
	"location_name":"Green Line Station Eastbound"
}
```
**Structural Integrity**

This device monitors the integrity of critical infrastructure sites which include bridges, subway tunnels, radio communications towers and hospitals. It can signal the imminent collapse of building or allow the ongoing monitoring of a structure that has been damaged or is being compromised. This information provides vital life safety information to the incident commander on the status of a bridge being used for evacuation, but which is impacted by rising flood waters. Incident commanders can also continuously monitor the integrity of a structure during emergency operations during or following a fire, earthquake or other emergency. The device provides specific data points for ongoing monitoring of 6 factors while also providing an easy to read Consolidated Failure Risk assessment.

This sensor reports the following data:
- Strain 
- Vibration 
- Tilt 
- Acceleration 
- Deformation 
- Cracking 
- Sensor Street Address 
- Sensor Placement 
- Consolidated Failure Risk

**Example Sensor Message:**
```json
{
	"deviceid":"structuralintegrity_transit_frites_001",
	"time":"2020-10-07 07:45:09.971204Z",
	"strain":{"value":0,"unit":"Points"},
	"strain_device_range_low":"0",
	"strain_device_range_high":"10",
	"vibration":{"value":0,"unit":"Points"},
	"vibration_device_range_low":"0",
	"vibration_device_range_high":"10",
	"tilt":{"value":0,"unit":"Points"},
	"tilt_device_range_low":"0",
	"tilt_device_range_high":"10",
	"acceleration":{"value":0,"unit":"Points"},
	"acceleration_device_range_low":"0",
	"acceleration_device_range_high":"10",
	"deformation":{"value":0,"unit":"Points"},
	"deformation_device_range_low":"0",
	"deformation_device_range_high":"10",
	"cracking":{"value":2,"unit":"Points"},
	"cracking_device_range_low":"0",
	"cracking_device_range_high":"10",
	"sensor_location":"100 North Main Street",
	"location_name":"Green Line Station Eastbound",
	"sensor_placement":"MP_2_WestBound_Tunnel",
	"consolidated_failure_risk":"Medium_Risk",
	"consolidated_failure_risk_alert_high":"High_Risk",
	"consolidated_failure_risk_alert_critical_high":"Collapse_Imminent",
	"consolidated_failure_risk_pscr_alert_medium":"High_Risk",
	"consolidated_failure_risk_pscr_alert_high":"Collapse_Imminent"
}
```
**Subway Car Status**

This device monitors the status of mass transit subway cars to estimate passenger counts and the integrity of safety systems. While this data is used daily by the transit organization, subway car data can be vitally important to first responders and can provide an early indication to the severity of an incident. Since response times to subway emergencies are prolonged, due to access issues, the availability of data early in the incident can ensure that appropriate resources are assigned. Specifically, the passenger count is a lead indicator to the number of persons who may be injured. This information drives the number of EMS units assigned to the incident.

This sensor reports the following data:
- Car ID 
- Door Status (Open, Closed, Emergency Open, Malfunction Closed) 
- Emergency Exit (Secure, Activated)

**Example Sensor Message:**
```json
{
	"deviceid":"subwaycarstatus_transit_frites_001",
	"time":"2020-10-07 07:45:10.027036Z",
	"subway_car_id":"Car_005",
	"door_status":"Closed",
	"emergency_exit":"Secure"
}
```
**Triage Tag**

This device simulates patient data transmitted from a Smart Triage Tag. These devices are attached to ill and injured persons at the scene of a Mass Casualty Incident. The sensors monitor each patient’s vital signs and provide an analysis of injury severity. Additional data may be entered by a first responder to include the patients age category, race, sex and chief complaint. Location data is also transmitted allowing first responders to quickly navigate to the most critically injured patients first.

This sensor reports the following data:
- Category (Green, Yellow, Red, Black) 
- Heart Rate 
- Respiratory Rate 
- Oxygen Saturation 
- Body Temperature 
- Blood Pressure 
- Shock Index (Low, Medium, High) 
- Patient ID Number 
- Patient Age (Infant, Pediatric, Adult) 
- Patient Sex 
- Patient Race 
- Medical or Trauma 
- Chief Complaint 
- Patient Location (GPS)

**Example Sensor Message:**
```json
{
	"deviceid":"triagetag_transit_frites_b_002",
	"time":"2020-10-07 07:57:03.617513Z",
	"category":"Red",
	"category_alert_low":"Green",
	"category_alert_high":"Yellow",
	"category_alert_critical_high":"Red",
	"category_pscr_alert_low":"Green",
	"category_pscr_alert_medium":"Yellow",
	"category_pscr_alert_high":"Red",
	"heart_rate":{"value":126,"unit":"bpm"},
	"heart_rate_device_range_low":"0",
	"heart_rate_device_range_high":"300",
	"heart_rate_alert_low":"40",
	"heart_rate_alert_critical_low":"30",
	"heart_rate_alert_high":"140",
	"heart_rate_alert_critical_high":"160",
	"heart_rate_pscr_alert_low":"30",
	"heart_rate_pscr_alert_medium":"140",
	"heart_rate_pscr_alert_high":"160",
	"resp_rate":{"value":23,"unit":"rpm"},
	"resp_rate_device_range_low":"0",
	"resp_rate_device_range_high":"50",
	"resp_rate_alert_low":"6",
	"resp_rate_alert_critical_low":"4",
	"resp_rate_alert_high":"20",
	"resp_rate_alert_critical_high":"30",
	"resp_rate_pscr_alert_low":"6",
	"resp_rate_pscr_alert_medium":"20",
	"resp_rate_pscr_alert_high":"30",
	"oxysat":{"value":95,"unit":"%"},
	"oxysat_device_range_low":"0",
	"oxysat_device_range_high":"100",
	"oxysat_alert_low":"95",
	"oxysat_alert_critical_low":"90",
	"oxysat_pscr_alert_medium":"95",
	"oxysat_pscr_alert_high":"90",
	"body_temp_f":{"value":96,"unit":"Degrees F"},
	"body_temp_f_device_range_low":"0",
	"body_temp_f_device_range_high":"120",
	"body_temp_f_alert_low":"95",
	"body_temp_f_alert_critical_low":"90",
	"body_temp_f_alert_high":"102",
	"body_temp_f_alert_critical_high":"105",
	"body_temp_f_pscr_alert_low":"95",
	"body_temp_f_pscr_alert_medium":"102",
	"body_temp_f_pscr_alert_high":"105",
	"blood_pressure":{"value":"80/40","unit":"mmHg"},
	"blood_pressure_device_range_low":"0",
	"blood_pressure_device_range_high":"250",
	"blood_pressure_alert_low":"90/50",
	"blood_pressure_alert_critical_low":"80/40",
	"blood_pressure_alert_high":"150/90",
	"blood_pressure_alert_critical_high":"170/100",
	"blood_pressure_pscr_alert_low":"80/40",
	"blood_pressure_pscr_alert_medium":"150/90",
	"blood_pressure_pscr_alert_high":"170/100",
	"shock_Index":"High",
	"shock_index_alert_high":"Medium",
	"shock_index_alert_critical_high":"High",
	"shock_index_pscr_alert_medium":"Medium",
	"shock_index_pscr_alert_high":"High",
	"patient_id":"MCI202000002",
	"patient_age":"Adult",
	"patient_sex":"F",
	"patient_race":"W",
	"medical_trauma":"Medical",
	"chief_complaint":"Fall"
}
```
**Subway Track Status: Voltage Add**

This sensor supplements NIST Sensor: Voltage

This device actively monitors the status of each subway rail line and provides information on the integrity of the “3rd Rail” electrical system. Information is provided for each segment of track and indicates if the electrical system components are intact, if the rail is energized and if there is any indication of a safety risk (e.g. heat).

This sensor reports the following data:
- Sensor Street Address 
- Sensor Placement 
- Electrical Integrity 
- Track Safety

**Example Sensor Message:**
```json
{
	"deviceid":"voltage_transit_add_frites_001",
	"time":"2020-10-07 07:57:03.778363Z",
	"sensor_location":"100 North Main Street",
	"location_name":"Green Line Station Eastbound",
	"sensor_placement":"MP_1_Tunnel_Eastbound_Section_333",
	"electrical_integrity":"Unknown",
	"track_safety":"Heat_Detected"
}


