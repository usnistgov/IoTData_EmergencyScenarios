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

**CHARIoT Challenge: Wildfire Scenario**

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

| Sensor Name | Start Time | End Time | Update Interval | Behavior |
|-------------|------------|----------|-----------------|----------|
| **Air Quality** |
| air_quality_0xx                              | 0s         | N/A      | 1s              | Begins transmitting data at start of scenario. Continues data transmission until end of scenario. Numeric/level data is pseudo-randomly varies during across the durations of the scenario.  Alarm and alert levels are static though out the scenarios. air_quality_001_S to air_quality_019_S randomly picked |
| **Computer Aided Dispatch** |
| cadfire_fire_frites                          | 0s         | 2s       | 1s              | static data, transmit once, Time On Scene is current clock time, Time Received and Time Dispatched are negative offsets from start of scenario |
| **Evacuation Analytics** |
| evacuationanalytics_fire_frites              | 0s         | N/A      | 30s             | provides evacuation details and status each 30 seconds |
| **Officer Vitals** |
| officervitals_fire_add_frites_a_001          | 0s         | N/A      | 2s              | Police officer 1's Respiratory rate set to alert level, body temperature to alert random |
| officervitals_fire_add_frites_b_002  to _023 | 0s         | N/A      | 2s              | No Alarms set. Numeric/level data is pseudo-randomly varies during across the durations of the scenario.  Alarm and alert levels are static though out the scenarios. |
| **Safety Monitor** |
| safetymonitor_wildfire_frites_a_001          | 0s         | N/A      | 5s              | motionless for 60 seconds, alert |
| safetymonitor_wildfire_frites_a_001 to _023  | 0s         | N/A      | 5s              | No Alarms set. Numeric/level data is pseudo-randomly varies during across the durations of the scenario.  Alarm and alert levels are static though out the scenarios. |
| **Weather Conditions** |
| wind_generated_fire_add_frites               | 0s         | N/A      | 1s              | winds set to 19-24 random, lightning strikes set to 2, rainfall set to 2 inches |
| wind_generated_fire_add_frites_002 to _0019  | 0s         | N/A      | 1s              | winds set to 19-24 random, lightning strikes set to 2, rainfall set to 2 inches |


**Note: ** Sensors named officervitals_fire_add_frites_a_001 through vitals_fire_add_frites_a_023 and sensors named safetymonitor_wildfire_frites_a_001 through safetymonitor_wildfire_frites_a_023 are intended to be integrated using operations command software and AR devices.

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

**Evacuation Analytics:** This device simulates the harvesting of data from other sources and provides the incident commander with a dynamic list of evacuation priority areas. The incident commander receives information associated to a smaller geographic area comprising a Zip+4 postal code and associated street name. The data stream identifies the priority order of the evacuation, the number of critical infrastructure assets are in the target zone, the number of minutes until the hazard impact begins, and the number of minutes until peak impact is realized. This type of device helps organize evacuation priorities in situations like wildfires and flooding where conditions are dynamic. This sensor is highlighted in the Wildfire scenario.

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
	"deviceid":"air_quality_frites_001",
	"time":"2020-10-23 04:37:04.973792Z",
	"air_quality_level":"Orange",
	"air_quality_level_alert_high":"very_unhealthy",
	"air_quality_level_alert_critical_high":"hazardous",
	"air_quality_level_pscr_alert_low":"red",
	"air_quality_level_pscr_alert_medium":"very_unhealthy",
	"air_quality_level_pscr_alert_high":"hazardous",
	"ozone_level":"Increasing",
	"ozone_level_alert_high":"Increasing",
	"ozone_level_alert_critical_high":"High",
	"ozone_level_pscr_alert_medium":"Increasing",
	"ozone_level_pscr_alert_high":"High",
	"sulfer_dioxide_level":"High",
	"sulfer_dioxide_level_alert_low":"Trace",
	"sulfer_dioxide_level_alert_high":"Increasing",
	"sulfer_dioxide_level_alert_critical_high":"High",
	"sulfer_dioxide_level_pscr_alert_low":"Trace",
	"sulfer_dioxide_level_pscr_alert_medium":"Increasing",
	"sulfer_dioxide_level_pscr_alert_high":"High",
	"nitrogen_dioxide_level":"Trace",
	"nitrogen_dioxide_level_alert_low":"Trace",
	"nitrogen_dioxide_level_alert_high":"Increasing",
	"nitrogen_dioxide_level_alert_critical_high":"High",
	"nitrogen_dioxide_level_pscr_alert_low":"Trace",
	"nitrogen_dioxide_level_pscr_alert_medium":"Increasing",
	"nitrogen_dioxide_level_pscr_alert_high":"High",
	"sensor_id":"air quality_018_S",
	"parent":"Point 18",
	"coords":{"longitude":-96.3491697,"latitude":30.579711}
}
```
**CAD FIRE:**

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
	"deviceid":"cadfire_fire_frites_001",
	"time":"2020-10-23 04:37:04.983766Z",
	"incident_number":"F201114",
	"incident_type":"BRUSH_FIRE_LEVEL_3",
	"incident_location":"1595 Nuclear Science Road, College Station",
	"location_name":"TEEX Brayton Fire Training Field",
	"comments_911_caller":"Caller reports hot spots flaring up near homes, along State Road 47",
	"units_responding":"['E171', 'E172', 'E174', 'BC17', 'TA170', 'TA171', 'AIR1']",
	"time_received":"2020-10-23 04:26:33.983766Z",
	"time_dispatched":"2020-10-23 04:31:10.983766Z",
	"time_onscene":"2020-10-23 04:37:04.983766Z",
	"total_units_onscene":"11"
}
```
**Evacuation Analytics**

This device simulates the harvesting of data from other sources and provides the incident commander with a dynamic list of evacuation priority areas. The incident commander receives information associated to a smaller geographic area comprising a Zip+4 postal code. The data stream identifies the priority order of the evacuation, the number of critical infrastructure assets are in the target zone, the number of minutes until the impact starts, and the number of minutes until peak impact is realized. This type of device helps organize evacuation priorities in situations like wildfires and flooding where conditions are dynamic. US Postal Service Zip+4 areas are designed to be small and have efficiently designed delivery routes that are suitable for managing evacuation.

This sensor reports the following data:
- Evacuation Priority Evacuation Cause (Fire, Flood, Smoke, Hazmat, Life Safety Hazard) 
- Evacuation Zip Code & Street Name 
- Number of Critical Infrastructure Facilities in zone 
- Hazard arriving in ___ Minutes 
- Peak Hazard impact in ___ Minutes

**Example Sensor Message:**
```json
{
	"deviceid":"evacuationanalytics_fire_frites_001",
	"time":"2020-10-23 04:37:34.981950Z",
	"evacuation_priority":"2",
	"evacuation_priority_alert_high":"2",
	"evacuation_priority_alert_critical_high":"1",
	"evacuation_priority_pscr_alert_medium":"2",
	"evacuation_priority_pscr_alert_high":"1",
	"evacuation_cause":"Fire",
	"evacuation_zip_code":"77845-3404, State Highway 47",
	"number_cii_facilities":"0",
	"hazard_arrival_in":"52_minutes",
	"peak_hazard_impact_in":"63_minutes",
	"number_cii_facilities_alert_high":"2",
	"number_cii_facilities_alert_critical_high":"4",
	"number_cii_facilities_pscr_alert_medium":"2",
	"number_cii_facilities_pscr_alert_high":"4"
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
	"deviceid":"officervitals_fire_add_frites_a_001",
	"time":"2020-10-23 04:37:35.017675Z",
	"ecg_heart_rhythm":"Sinus_Tachycardia",
	"ecg_heart_rhythm_alert_low":"Ectopy_Detected",
	"ecg_heart_rhythm_alert_high":"Ventricular_Tachycardia",
	"ecg_heart_rhythm_alert_critical_high":"Ventricular_Fibrillation",
	"respiratory_rate":{"value":23,"unit":"rpm"},
	"respiratory_rate_device_range_low":"0",
	"respiratory_rate_device_range_high":"100",
	"respiratory_rate_alert_low":"6",
	"respiratory_rate_alert_critical_low":"4",
	"respiratory_rate_alert_high":"20",
	"respiratory_rate_alert_critical_high":"50",
	"body_temperature":{"value":101,"unit":"Degrees F"},
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
	"deviceid":"safetymonitor_wildfire_frites_a_001",
	"time":"2020-10-23 04:37:34.996060Z",
	"area-temperature":{"value":91,"unit":"degrees F"},
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

**Weather Station:** Wind Generated Fire Add

This sensor supplements NIST sensor: Wind Generated

This device simulates data from a fixed or portable weather station. Weather data, including forecast modeling, is a critical component of many emergencies. The ability to access real time data on wind speed, rain fall, temperature and humidity impact an incident commander’s decision making regarding the safe deployment and withdrawal of personnel.

This sensor reports the following data:

- Temperature
- Humidity 
- Rainfall 
- Rainfall 24 Hour 
- Lightning Strikes (past 30 minutes) 
- Sensor Street Address
- Sensor Location GPS

**Example Sensor Message:**
```json
{
	"deviceid":"wind_generated_fire_add_frites_m_001",
	"time":"2020-10-23 04:37:35.553752Z",
	"temperature":{"value":95,"unit":"Degrees F"},
	"temperature_device_range_low":"-50",
	"temperature_device_range_high":"200",
	"temperature_alert_low":"40",
	"temperature_alert_critical_low":"32",
	"temperature_alert_high":"105",
	"temperature_alert_critical_high":"110",
	"humidity":{"value":38,"unit":"%"},
	"humidity_device_range_low":"0",
	"humidity_device_range_high":"100",
	"humidity_alert_low":"40",
	"barometric_pressure":{"value":29.92,"unit":"inches Hg"},
	"barometric_pressure_device_range_low":"2500",
	"barometric_pressure_device_range_high":"3500",
	"rainfall":{"value":1,"unit":"inches per hour"},
	"rainfall_device_range_low":"0",
	"rainfall_device_range_high":"35",
	"rainfall_alert_high":"2","rainfall_alert_critical_high":"5",
	"rainfall_24hour":{"value":2,"unit":"inches per 24 hours"},
	"temperature_pscr_alert_low":"102",
	"temperature_pscr_alert_medium":"105",
	"temperature_pscr_alert_high":"110",
	"humidity_pscr_alert_high":"40",
	"rainfall_pscr_alert_low":"1",
	"rainfall_pscr_alert_medium":"2",
	"rainfall_pscr_alert_high":"5",
	"lightning_strikes_past_30_minutes":{"value":2,"unit":"strikes 30 minutes"},
	"lightning_strikes_past_30_minutes_alert_low":"1",
	"lightning_strikes_past_30_minutes_alert_high":"4",
	"lightning_strikes_past_30_minutes_alert_critical_high":"10",
	"lightning_strikes_past_30_minutes_pscr_alert_low":"1 ",
	"lightning_strikes_past_30_minutes_pscr_alert_medium":"4",
	"lightning_strikes_past_30_minutes_pscr_alert_high":"10 "
}


