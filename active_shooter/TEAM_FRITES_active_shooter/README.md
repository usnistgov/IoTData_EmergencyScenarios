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

**CHARIoT Challenge: Active Shooter Scenario**

Team Frites scenarios are intended to create data for PSCR AR teams and other types of IoT research for First Responder sensor and Smart City Innovations programs.  This section provided an overview of the scenarios including the following information for each scenario:
•	Sensor Type and Names
•	Relative Start Time of major state changes for sensors within each of 5 scenario versions
•	Sensor Behavior 
Where possible, the names of sensors in Team Frites scenarios match the names of PSCR sensors provided to challenge competitors.

Many Team Frites Sensors contain selectable properties which support multiple selection options.  Sensor properties including: locations, sex, race, and other have multiple options. Options are randomly selected each time scenarios execute making each scenario run unique. For example, location names found in maps provided by PSCR are options for sensor locations. Each time the simulator executes a scenario, different locations are selected for sensor locations. 

Our designated team Point of Contact (Gary Mazzaferro) garym <AT> oedata <DOT> com is available for questions.

In this folder includes five (5) different excutions of the scenario data. 

**Scenario Defnition:**

The data generated for each of the five (5) instaniations of the scenation is define by the table below:

| **Sensor Name** | **Start Time** | **End Time** | **Update Interval** | **Behavior** |
|-------------|------------|----------|-----------------|----------|
| **Building Electrical Sensor** |
| buildingelectrical_shooter_frites              | 0s         | 6m       | 30s             | HVAC set to Open, Electrical Panel random, locations set to EOTC floor map, 30 second transmit time |
| **Computer Aided Dispatch** |
| cadems_shooter_frites                          | 0s         | 5s       | 5s              | EMS CAD. static data, transmit once, Time On Scene is current clock time, Time Received and Time Dispatched are negative offsets from start of scenario |
| cadfire_shooter_frites                         | 0s         | 5s       | 5s              | FIRE Dept. CAD. static data, transmit once, Time On Scene is current clock time, Time Received and Time Dispatched are negative offsets from start of scenario |
| cadlaw_shooter_frites                          | 0s         | 5s       | 5s              | POLICE CAD. static data, transmit once, Time On Scene is current clock time, Time Received and Time Dispatched are negative offsets from start of scenario |
| **Cognitive Monitor** |
| cognitivemonitor_shooter_frites_a              | 0s         | N/A      | 5s              | Cognitive level set to Red. Begins transmitting data at start of scenario. Continues data transmission until end of scenario. Numeric/level data is pseudo-randomly varies during across the durations of the scenario.  Alarm and alert levels are static though out the scenarios.                                                                             |
| cognitivemonitor_shooter_frites_b_002  to _023 | 0s         | N/A      | 5s              | Cognitive levels set to Yellow. Begins transmitting data at start of scenario. Continues data transmission until end of scenario. Numeric/level data is pseudo-randomly varies during across the durations of the scenario.  Alarm and alert levels are static though out the scenarios.                                                                         |
| **Door Sensors** |
| door_shooter_add_frites                        | 0s         | 4m       | 30s             | Emergency Exit Door and Door Forced Open set to alarm value, doors set to EOTC floor plan: EOTC_Floor1_Emergency_Exit_North_Room15, EOTC_Floor1_Emergency_Exit_South_Door7, EOTC_Floor1_Emergency_Exit_South_Door6, EOTC_Floor1_Emergency_Exit_East_Door5, EOTC_Floor1_Emergency_Exit_North_Room15, EOTC_Floor1_Emergency_Exit_North_Room15, DCT_Floor1_DR15_RM1 |
| **Fire Alarms** |
| firealarm_shooter_frites                       | 0s         | 4m       | 20s             | manual pull station set to alarm, alarm placement set to EOTC floor plan, 4 minutes of alarms @ 20 seconds: EOTC_Floor1_NorthEast_Corridor_Door41, EOTC_Floor1_West_Corridor_Door27, EOTC_Floor1_Main_Entry_Door1, OTC_Floor1_South_West_Corridor_Door10, EOTC_Floor1_East_Exit_Stairwell_Door5, EOTC_Floor2_Elevator                                            |
| **Gunshot Detector** |
| gunfire_shooter_add_frites                     | 0s         | 3m       | 30s             | detector set to random type single/multi-shot, regular and automatic for alert, locations set to EOTC floor plan: EOTC_Floor1_North_Corridor__Rooms14_17, EOTC_Floor1_West_Corridor_Rooms4_11, EOTC_Floor1_Main_Entry |
| **Shooter Detection Camera** |
| interiorcamera_shooter_frites_a                | 0s         | N/A      | 30s             | camera alert set to mass exit detected, floor plan based on EOTC, multiple camera locations: Floor1_North_Hallway, Floor1_Main_Entry, Floor1_South_Emergency_Exit |
| interiorcamera_shooter_frites_a_002            | 0s         | N/A      | 30s             | weapon detected alert value, EOTC Floor Plan, multicamera: Floor1_North_Hallway, Floor1_Main_Entry, Floor1_South_Emergency_Exit |
| **Safety Monitor** |
| officersafety_shooter_frites_a_001             | 4m         | N/A      | 11s             | Officer 1 with Emergency Button automatic alert at 4 minutes  |
| officersafety_shooter_frites_a_001 to _023     | 0s         | N/A      | 11s             | No alerts. Continues data transmission until end of scenario. Numeric/level data is pseudorandomly varies during  across the durations of the scenario.  Alarm and alert levels are static though out the scenarios. |
| safetymonitor_shooter_frites_a                 | 0s         | N/A      | 5s              | motionless for 60 seconds, alert |
| safetymonitor_shooter_frites_b_002 to _023     | 0s         | N/A      | 5s              | no alerts. Continues data transmission until end of scenario. Numeric/level data is pseudorandomly varies during  across the durations of the scenario.  Alarm and alert levels are static though out the scenarios. |
| **Officer Vitals** |
| officer_vitals_monitor_frites_a                | 0s         | N/A      | 2s              | Respiratory rate set to alert level for sensor |
| officervitals_fire_add_frites_b_002  to _023   | 0s         | N/A      | 2s              | Respiratory rate set to alert level for sensor |
| **Triage Tag**  |
| triagetag_shooter_frites_a_001                 | 0s         | N/A      | 10s             | all vitals set to critical values for alert |
| triagetag_shooter_frites_a_002                 | 0s         | N/A      | 10s             | all vitals set to critical values for alert |
| triagetag_shooter_frites_c_003                 | 0s         | N/A      | 10s             | "Vitals set to Yellow for Patient c, Adult WM, Tag 003 |
| triagetag_shooter_frites_d_004                 |  0s         | N/A      | 10s             | Vitals set to Yellow |
| triagetag_shooter_frites_e_005                 | 0s         | N/A      | 10s             | all vitals set to Yellow |
| triagetag_shooter_frites_e_006                 | 0s         | N/A      | 10s             | all vitals set to critical values for alert |

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

**Cognitive Monitor:** This device monitors the cognitive load of the first responder using industry accepted criteria and provides a set of warning indicators that trigger reductions in the amount of data presented. As the first responder comes under increasing stress, the sensor will activate an Alert Display Reduction algorithm that reduces voice and data flowing to the individual. This action will increasingly limit the type of incoming data from the Situational Awareness level to Urgent Tactical information ending with data that only impacts Life Safety aspects of the operation. This type of device not only alerts the incident commander and/or communications center of an emergency event but also increases first responder safety by dynamically reducing the amount of data that needs to be processed. This allows the first responder to focus on data that is either mission critical or survival critical. This sensor is featured in the Active Shooter scenario.
   
**Computer Aided Dispatch (CAD):** Three sensor devices have been created to simulate information flowing to the incident commander or first responder from the communications center. Each device represents incident data for law enforcement, fire or EMS. The data stream is customized for each scenario and identifies the location of the emergency, which units are responding, and the total number of units currently on scene. CAD system data is used by many public safety agencies during simulation exercises. This data stream is highlighted in the Mass Transit Accident scenario.

**Scenario Sensor List:**

|Type  |Message ID  | Comment |
|---------|---------|---------|
|X Building Electrical System | buildingelectrical_shooter_frites        |
|Computer Aided Dispatch | cadems_shooter_frites |
|Computer Aided Dispatch | cadfire_shooter_frites |
|Computer Aided Dispatch | cadlaw_shooter_frites |
|Cognitive Monitor  | cognitivemonitor_shooter_frites |
|Building Security Emergency Exits | door_shooter_add_frites | (supplements NIST sensor) |
|Building Fire Alarm | firealarm_shooter_frites |
|Interior Gunshot Detection     | gunfire_shooter_add_frites | (supplements NIST sensor) |
|X Interior Security Camera Analytics  | interiorcamera_shooter_frites_1 |
|X Interior Security Camera Analytics  | interiorcamera_shooter_frites_2 |
|X Officer Safety Monitor     | officersafety_shooter_frites |
|Officer Vital Signs Monitor     | officer_vitals_shooter_add_frites | (supplements NIST sensor) |
|First Responder Safety Monitor     | safetymonitor_shooter_frites |
|X Triage Tag Vital Signs Monitor     | triagetag_shooter_frites |

**FRITES Sensor Message Output:**

**EMS Computer Aided Dispatch**

This sensor simulates EMS incident data transmitted by a public safety agency communications center to first responders and incident commanders. This information represents the initial data that flows to first responders regarding an incident and establishes early situational awareness.

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
	"deviceid":"cadems_shooter_frites_001",
	"time":"2020-10-07 06:25:41.221248Z",
	"incident_number":"E201247",
	"incident_type":"SHOOTING_MCI",
    "incident_location":"10096 Stillwater Rd, College Station","location_name":"TEEX Financial Center",
    "comments_911_caller":"PD reports man with gun in lobby, multiple perons shot, stage for pd clearnance. ",
    "units_responding":"['Medic3', 'Medic4', 'Medic7', 'Medic9', 'Aid21', 'Aid25', 'MS91', 'MS96']",
    "time_received":"2020-10-07 06:20:52.221827Z",
    "time_dispatched":"2020-10-07 06:21:32.221927Z",
    "time_onscene":"2020-10-07 06:25:41.221966Z",
    "total_units_onscene":"3"
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
	"deviceid":"cadfire_shooter_frites_001",
	"time":"2020-10-07 06:25:41.224237Z",
	"incident_number":"F201113","incident_type":"SOV_MCI",
	"incident_location":"10096 Stillwater Rd, College Station",
	"location_name":"TEEX Financial Center",
	"comments_911_caller":"PD advises multiple persons shot at this location, shooter is active, stage for PD",
	"units_responding":"['E73', 'E51', 'E45', 'R1', 'R2', 'B4', 'B5', 'D1']",
	"time_received":"2020-10-07 06:20:34.224654Z",
	"time_dispatched":"2020-10-07 06:20:45.224766Z",
	"time_onscene":"2020-10-07 06:25:41.224807Z",
	"total_units_onscene":"4"
}
```
**Law Enforcement Computer Aided Dispatch**

This sensor simulates Law Enforcement incident data transmitted by a public safety agency communications center to first responders and incident commanders. This information represents the initial data that flows to first responders regarding an incident and establishes early situational awareness.

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
	"deviceid":"cadlaw_shooter_frites_001",
	"time":"2020-10-07 06:25:41.215161Z",
	"incident_number":"L2087232",
	"incident_type":"ACTIVE_SHOOTER",
	"incident_location":"10096 Stillwater Rd, College Station",
	"location_name":"TEEX Financial Center",
	"comments_911_caller":"Male suspect in lobby with gun, shots fired, multiple victims reported down",
	"units_responding":"['1A21', '1A22', '1A31', '1A15', '1K50', '1L81', '1L90']",
	"units_onscene":"1A20, 1A23",
	"time_received":"2020-10-07 06:20:47.215334Z",
	"time_dispatched":"2020-10-07 06:21:22.215403Z",
	"time_onscene_first_unit":"2020-10-07 06:25:41.215441Z",
	"total_units_onscene":"2"
}
```
**Cognitive Monitor**

This device monitors the cognitive load of the first responder using industry accepted criteria and provides a set of warning indicators that trigger reductions in the amount of data presented on first responder devices. As the first responder comes under increasing stress, the sensor will activate an Alert Display Reduction algorithm that reduces voice and data flowing to the individual. This action will increasingly limit the type of incoming data from a Normal Level to a Situational Awareness level to Urgent Tactical information and ending with data that only relates to Life Safety controls. This type of device not only alerts the incident commander and/or communications center of an emergency event but also increases first responder safety by dynamically reducing the amount of data that needs to be processed. This allows the first responder to focus on data that is either mission critical or survival critical.

This sensor reports the following data:
First Responder Profile ID 
EEG Beta (uv) 
Electrodermal Activity (us) 
Ambient Light (lux) 
Pupil Diameter (mm) 
Eye Track Average Fixation Duration (ms) 
Eye Track Microsaccade Magnitude (deg) 
Cognitive Level (current reading) 
Alert Display Reduction (current level activated) 
Alert Interface Body Camera (auto “on” feature) 
Alert Interface Emergency Button (auto “on” feature) 
Alert Interface GPS (auto transmit feature)

**Example Sensor Message:**
```json
{
	"deviceid":"cognitivemonitor_shooter_frites_b_020",
	"reference_id":"officer_002",
	"time":"2020-10-07 06:25:41.855882Z",
	"first_responder_profile_id":"Law_Enforcement",
	"sensor_eeg_beta_uv":{"value":6,"unit":"uv"},
	"sensor_electrodermal_activity_us":{"value":77,"unit":"us"},
	"sensor_ambient_light_lux":{"value":45687,"unit":"lux"},
	"sensor_pupil_diameter_mm":{"value":8,"unit":"mm"},
	"sensor_eye_track_avg_fix_duration_ms":{"value":240,"unit":"ms"},
	"sensor_eye_track_microsaccade_magnitude_deg":{"value":1,"unit":"deg"},
	"cognitive_level":"Yellow","cognitive_monitor_alert_low":"Yellow",
	"cognitive_monitor_alert_high":"Orange",
	"cognitive_monitor_alert_critical_high":"Red",
	"cognitive_monitor_pscr_alert_low":"Yellow",
	"cognitive_monitor_pscr_alert_medium":"Orange",
	"cognitive_monitor_pscr_alert_high":"Red",
	"alert_display_reduction":"Situational_Awareness",
	"alert_interface_bodycam":"Auto_On_Orange",
	"alert_interface_emergency_button":"Auto_Alert_Red",
	"alert_interface_gps":"Auto_Transmit_Orange"
}
```
**Smart Security: Door Shooter Add**

This sensor supplements NIST Sensor: Door

This device is the third of three Smart City sensor systems. The Smart Security sensors simulate the transmission of information from a buildings safety and security system. This includes information on breaches to secure areas and opening of doors and emergency exits. These sensors may be customized to match the unique needs of each scenario. Security System information provides important data to the incident commander such as which exits are being used for evacuation by persons fleeing an emergency or the location of a suspect (based on door access data). 

This sensor reports the following data:
- Event Type (Normal, Emergency Exit Open, Door Forced Open, Failed PIN, Glass Break) 
- Event Location 
- Building Street Address

**Example Sensor Message:**
```json
{
	"deviceid":"door_shooter_add_frites_001",
    "time":"2020-10-07 06:25:40.989423Z",
    "event_type":"Door_Forced_Open",
    "event_type_alert_high":"Emergency_Exit_Open",
    "event_type_alert_critical_high":"Door_Forced_Open",
    "event_type_pscr_alert_medium":"Emergency_Exit_Open",
    "event_type_pscr_alert_high":"Door_Forced_Open",
	"event_location":"EOTC_Floor1_Emergency_Exit_North_Room15",
    "event_address":"10096 Stillwater Rd, College Station",
    "location_name":"TEEX Financial Center"
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
	"deviceid":"firealarm_shooter_frites_001",
	"time":"2020-10-07 06:25:45.988674Z",
	"alarm_type":"Manual_Pull_Station",
	"alarm_type_alert_high":"Manual_Pull_Station",
	"alarm_type_critical_high":"Detector",
	"alarm_type_pscr_alert_medium":"Manual_Pull_Station",
	"alarm_type_pscr_alert_high":"Detector",
	"event_location":"10096 Stillwater Rd, College Station",
	"location_name":"TEEX Financial Center",
	"alarm_placement":"EOTC_Floor1_South_West_Corridor_Door10"
}
```
Gunfire Shooter Add

This sensor supplements NIST sensor Gunfire Shooter

This device simulates the transmission of data from an indoor gunshot detection system. These devices may be installed in schools, government buildings or other high-risk locations. The sensor detects the acoustic signature of a firearm discharge, identifies the caliber of the weapon, the number of shots fired, and the location. This data provides public safety agencies with early notification of a life threatening situation and can provide substantial intelligence information that helps rapidly determine how many shooters may be present, what type of firearms are being used, and the movement of the suspect through the facility. 

This sensor reports the following data:
- Detection Type (Single Shot, Multi Shot) 
- Building Address 
- Detector Location 
- Detector Confidence 
- Analytics Weapon Caliber

**Example Sensor Message:**
```json
{
	"deviceid":"gunfire_shooter_add_frites_001",
	"time":"2020-10-07 06:25:41.031130Z",
	"detection_type":"Single_Shot",
	"detection_type_alert_high":"Single_Shot",
	"detection_type_alert_critical_high":"Multi_Shot",
	"detection_type_pscr_alert_medium":"Single_Shot",
	"detection_type_pscr_alert_high":"Multi_Shot",
	"detector_location":"EOTC_Floor1_Main_Entry",
	"detector_confidence":{"value":97,"unit":"%"},
	"incident_location":"10096 Stillwater Rd, College Station",
	"location_name":"TEEX Financial Center",
	"detector_confidence_device_range_low":"0",
	"detector_confidence_device_range_high":"100",
	"detector_confidence_alert_low":"90",
	"detector_confidence_alert_critical_low":"85",
	"detector_confidence_pscr_alert_medium":"90",
	"detector_confidence_pscr_alert_high":"85",
	"analytics_weapon_caliber":"45_Calibre_Automatic"
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
	"deviceid":"officer_vitals_monitor_frites_002",
	"time":"2020-10-07 06:25:41.043032Z",
	"ecg_heart_rhythm":"Sinus_Tachycardia",
	"ecg_heart_rhythm_alert_low":"Ectopy_Detected",
	"ecg_heart_rhythm_alert_high":"Ventricular_Tachycardia",
	"ecg_heart_rhythm_alert_critical_high":"Ventricular_Fibrillation",
	"respiratory_rate":{"value":17,"unit":"rpm"},
	"respiratory_rate_device_range_low":"0",
	"respiratory_rate_device_range_high":"100",
	"respiratory_rate_alert_low":"6",
	"respiratory_rate_alert_critical_low":"4",
	"respiratory_rate_alert_high":"20",
	"respiratory_rate_alert_critical_high":"50",
	"body_temperature":{"value":99,"unit":"Degrees F"},
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
	"body_temperature_pscr_alert_high":"105"
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
	"deviceid":"safetymonitor_shooter_frites_a_001",
	"time":"2020-10-07 06:25:40.835638Z",
	"area-temperature":{"value":75,"unit":"Degrees F"},
	"area_temperature_device_range_low":"-50",
	"area_temperature_device_range_high":"200",
	"area_temperature_alert_low":"40",
	"area_temperature_alert_critical_low":"32",
	"area_temperature_alert_high":"100",
	"area_temperature_alert_critical_high":"105",
	"fall_impact_intensity":{"value":0,"unit":"10 Point Scale"},
	"fall_impact_intensity_device_range_low":"0",
	"fall_impact_intensity_device_range_high":"10",
	"fall_impact_intensity_alert_high":"6",
	"fall_impact_intensity_alert_critical_high":"8",
	"fall_impact_intensity_pscr_alert_low":"4",
	"fall_impact_intensity_pscr_alert_medium":"6",
	"fall_impact_intensity_pscr_alert_high":"10",
	"motionless_time_seconds":{"value":60,"unit":"seconds"},
	"motionless_time_seconds_device_range_low":"0",
	"motionless_time_seconds_device_range_high":"3600",
	"motionless_time_seconds_alert_high":"15",
	"motionless_time_seconds_alert_critical_high":"30",
	"motionless_time_seconds_pscr_alert_low":"10",
	"motionless_time_seconds_pscr_alert_medium":"15",
	"motionless_time_seconds_pscr_alert_high":"30",
	"area_temperature_pscr_alert_medium":"105",
	"area_temperature_pscr_alert_high":"110",
	"area_oxygen":{"value":19,"unit":"%"},
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
	"deviceid": "triagetag_shooter_frites_e_005", 
	"time": "2020-10-05 14:04:26.000000Z", 
	"category": "Yellow", 
	"category_alert_low": "Green", 
	"category_alert_high": "Yellow", "category_alert_critical_high": "Red", 
	"category_pscr_alert_low": "Green", "category_pscr_alert_medium": "Yellow", 
	"category_pscr_alert_high": "Red", 
	"heart_rate": { "value": 120, "unit": "bpm" }, 
	"heart_rate_device_range_low": "0", 
	"heart_rate_device_range_high": "300", 
	"heart_rate_alert_low": "40", 
	"heart_rate_alert_critical_low": "30", 
	"heart_rate_alert_high": "140", "heart_rate_alert_critical_high": "160", 
	"heart_rate_pscr_alert_low": "30", "heart_rate_pscr_alert_medium": "140", 
	"heart_rate_pscr_alert_high": "160", 
	"resp_rate": { "value": 21, "unit": "rpm" }, 
	"resp_rate_device_range_low": "0", 
	"resp_rate_device_range_high": "50", "resp_rate_alert_low": "6", 
	"resp_rate_alert_critical_low": "4", 
	"resp_rate_alert_high": "20", "resp_rate_alert_critical_high": "30", 
	"resp_rate_pscr_alert_low": "6", "resp_rate_pscr_alert_medium": "20", 
	"resp_rate_pscr_alert_high": "30", 
	"oxysat": { "value": 96, "unit": "%" }, "oxysat_device_range_low": "0", 
	"oxysat_device_range_high": "100", 
	"oxysat_alert_low": "95", 
	"oxysat_alert_critical_low": "90", 
	"oxysat_pscr_alert_medium": "95", 
	"oxysat_pscr_alert_high": "90", 
	"body_temp_f": { "value": 97, "unit": "Degrees F" }, 
	"body_temp_f_device_range_low": "0", "body_temp_f_device_range_high": "120", 
	"body_temp_f_alert_low": "95"
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
	"deviceid": "buildingelectrical_shooter_frites_001", 
	"time": "2020-10-05 14:04:26.000000Z", 
	"hvac_type": "Air_Handler", 
	"hvac_status": "Open", 
	"hvac_status_alert_high": "Fault", 
	"hvac_status_alert_critical_high": "Alert", 
	"hvac_status_pscr_alert_low": "Fault", 
	"hvac_status_pscr_alert_high": "Alert", 
	"electrical_panel_status": "Unknown_Status", 
	"electrical_panel_status_alert_low": "Open", 
	"electrical_panel_status_alert_high": "Main_Off", 
	"electrical_panel_status_alert_critical_high": "Main_Failure",
	"electrical_panel_status_pscr_alert_low": "Open", 
	"electrical_panel_status_pscr_alert_medium": "Main_Off", 
	"electrical_panel_status_pscr_alert_high": "Main_Failure", 
	"electrical_panel_location": "EOTC_Floor1_West_Entry_Doors", 
	"sensor_address": "10096 Stillwater Rd, College Station" 
}
```