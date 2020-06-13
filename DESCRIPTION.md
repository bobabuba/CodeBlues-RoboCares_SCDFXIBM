# ROBOCARES Home Monitoring System

## Content
- [Background](#background)
- [Why Robocares?](#why-robocares)
- [What is it?](#what-is-it)
- [How it works?](#how-it-works)
- [Who it helps?](#who-it-helps)

## Background
With Singapore facing an increasingly silver population, there is a larger vulnerable elderly population. These include elderly living alone, those with no next of kin, and those who are mostly alone at home. As Singapore pushes to be a smart nation, important agencies such as the SCDF can better harness the power of technology to respond more effectively to emergencies (e.g. cardiac arrests, falls, unattended cooking fires etc.). Moreover, SCDF can leverage on enhancing and streamlining the process for mobilising CFRs for early intervention. These improvements will greatly enhance SCDF's capabilities to save lives.  

## Why Robocares?
### Problems to tackle
1. Distinguishing an incident from a false alarm to reduce wastage of precious resources
2. Timely discovery of incidents, especially for vulnerable populations who spend most of their time at home alone
3. Analysis and tracking of situation while waiting for the emergency services to come
4. Mobilization of CFRs for effective early and effective intervention, especially for vulnerable populations

### Solution
1. ROBOCARES Home Monitoring System can help to determine if the resident is in an emergency situation
2. ROBOCARES Home Monitoring System can help to assess the severity of the situation with the use of sensors and a voice chatbot
3. Real-time information continues to be uploaded and analyzed by the relevant personnel while help is being deployed to location of incident
4. CFRs are mobilized early on so that they can provide timely help or resolve any minor issues quickly
5. Utilizing technology to get important resources to the scene more quickly, allowing for more timely response from CFRs as they reduce their journey time to the house as they do not have to worry about getting the resources

### Technology involved
- Use of existing technology like the MyResponder App and Home Fire Alarm Device (HFAD).
- Use of IoT to obtain readings like motion, , voice to make sense of the situation
- Use of AI to develop Voice Chatbot to further analyse the situation and obtain details from victim
- Use of Data Analytics and Machine Learning to develop a model to predict whether there is an event, as well as type and severity of event, based on readings collected
- Use of IoT to notify and mobilise CFRs
- Use of Data Analytics to record past incidents (accuracy of prediction of events, time taken for help to arrive etc) for future enhancements

## What is it?
ROBOCARES Home monitoring system consists of a central cloud system linked to multiple devices (ROBOCARES) which are placed around the house.  The system utilises IoT, AI, Data Analytics and Machine Learning. Each ROBOCARE consist of 3 types of sensors and have the HFAD incorporated. These devices are recommended to be placed in locations where the elderly frequent such as the toilets, bedrooms, living room and kitchen. 

Using the sensors, the ROBOCARES Home Monitoring System tells us 3 important pieces of information: (1) Whether there is truly an emergency (2) Type of emergency [if any] (3) Severity of emergency. This allows for better sense-making at the onset of the incident.

The ROBOCARES Home Monitoring System is linked to the MyResponder app, and will activate CFRs depending on the type of event detected. This will be elaborated on further in the later parts of the explanation.

Additionally, two types of Unmanned Aerial Vehicles (UAVs) will be stationed at the void deck of HDB blocks to complement ROBOCARES. The number of UAVs found in each neighbourhood depends on the population density of vulnerable groups in that location. 

The first type of UAV is the AED UAV, while the second type of UAV is the Fire Extinguisher UAV. As the name suggests, the former will carry around an AED, while the latter carries with it an small portable fire extinguisher. Both UAVs will also be equipped with first aid kits. 

Depending on the type of event suspected, the type of UAV deployed will differ. This allows the CFRs to head directly to the location and have the necessary equipment and/or first aid supplies to help the resident more effectively and quickly. 

## How it works?
### Component 1: ROBOCARES
####  Sensors
##### Workings of sensors
1. Volume + Frequency (Tone)
- Differentiate between person’s voice and others’ voice (Eg. from technological devices - TV, phone, radio)
- Voice match
- Abnormalities: Sudden, loud bang sound, sound of person collapsing, loud sounds, clashes, shouts, screams, words like ‘help’ (in different languages)
2. Motion sensor
- AI: Track usual time spent in various parts of the house (toilet), detect any abnormalities
- Track whether movement is present
3. HFAD (heat and smoke detector)
- Using existing SCDF technology detect fires
- Siren
- Will be placed in kitchen, but given 1 minute to disarm before we activate uav and myresponder app
##### Voice Chatbot
It will then first ring for 5 seconds (like an alarm)
then ask in dialect/malay/the selected language: Is there anything wrong? Do you need help?
Flowchart
1. ‘No’ -> the chatbot will then say ‘okay’ and then -end-
2. ‘Yes, help’/’Help me’
- UAV (Carrying AED and First Aid Kit) activated 
- Notification sent to the MyResponders App - ‘Injury/Cardiac Case suspected’ (new category)
3. No response → after 20 seconds, the robot will ring again and then prompt ‘is there anything wrong? Do you need help? If you do not need help, please say no.’ just to remind the elderly that a negative response is needed. After 40 seconds (2 reminder rings), 
- UAV (Carrying AED and First Aid Kit) activated 
- Notification sent to the MyResponders App - ‘Cardiac Case suspected’
#### Step 1C: Data Analytics and event prediction
- Data analysis of past cases of fire, falls, cardiac arrest on indicators like: volume, tone, temperature, etc
- Trained model based on database to accurately categorize cases and level of emergency

### Stage 2: Mobilization of CFRs for effective early intervention
Main idea: Leveraging on existing technologies (MyResponders App) , (Dog, UAV) and giving existing technologies new uses. 
1. Suspected Minor Fire Case
- Activate UAV (Carry smaller size fire extinguisher + First Aid Kit to the scene)
- Activate CFRs on MyResponder App - “Minor Fire’
- Eg. Unattended Cooking Fire
- HFAD: Drastic increase in temperature in localized area
- Motion Sensor, Volume Sensor and Tone Sensor: Can be no abnormalities detected
2. Suspected Major Fire Case
- Activate CFRs on MyResponder App - “Major Incident”
- Eg. Explosion 
- Device may detect sharp spike in temperature before being disconnected (damaged)
3. Suspected Fall/Cardiac Case
- Any abnormalities in the motion, volume or tone sensor will automatically activate the Voice Chatbot.
- Motion Sensor: Abnormal patterns of motion detected or 
- Volume Sensor: Spike in volume (Scream for help) or 
- Tone Sensor: Distressed sensed in tone of person
- HFAD: Can be no abnormalities detected

### Stage 3: Using analytics to refine the system
- Data analysis of incidents like: accuracy of prediction, time taken for CFR to arrive, required items to gelp the situation, etc
- Collate areas of improvement and effective areas, and improve future deployments accordingly
- i.e. make first aid kit more accessible, etc

## Who it helps?
Examples of vulnerable populations include:
- Elderly with no next of kin, living alone
- People with dementia
– Elderly who are alone at home most of the time (eg. their children are working)
