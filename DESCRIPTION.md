# Robocares inhouse central smart system

## Content
- [Background](#background)
- [Why Robocares](#why-robocares)
- [What is Robocares?](#what-is-robocares)
- [How it works?](#how-it-works)
- [Who it helps?](#who-it-helps)

## Background
With Singapore facing an increasingly silver population, there is a growing segment of vulnerable elderly population. These include elderly living alone, those with no next of kin, and those who are mostly alone at home. As Singapore pushes to be a smart nation, important agencies such as the SCDF can better harness the power of technology to respond more effectively to emergencies (e.g. cardiac arrests, falls, unattended cooking fires etc.). Moreover, SCDF can leverage on enhancing and streamlining the process for mobilising CFRs for early intervention. These improvements will greatly enhance SCDF's capabilities to save lives.  

## Why Robocares?
### Problems to tackle
1. Timely discovery of incidents, especially for vulnerable populations with no one near them
2. Analysis and tracking of current situation while waiting for help to come
3. Mobilization of CFRs for effective early and effective intervention, especially for vulnerable populations

### Solution
1. Home monitoring system to detect potential cardiac arrests, falls, unattended cooking fires, etc, and seek help from SCDF quickly
2. Live feedback of readings continues as help is being deployed to incident location
3. "Check on your neighbour" feature, perhaps with clearer instructions on incident details and possible items they need to bring along (i.e. AED, first aid kit, fire extinguisher, etc)

### Technology involved
- Use of IoT to obtain readings like motion, temperature and humidity, voice to make sense of the situation
- Use of AI to develop Voice Chatbot to further analyse the situation and obtain details from victim
- Use of Data Analytics and Machine Learning to develop a model to predict whether there is an event, as well as type and severity of event, based on readings collected
- Use of IoT to notify and mobilise CFRs
- Use of Data Analytics to record past incidents (accuracy of prediction of events, time taken for help to arrive etc) for future enhancements

## What is Robocares?
A central cloud (idk if this term is used correctly) system 
+ multiple (decide range of number? Can do like a minimum __ devices) small devices placed around the house 
(compulsory: Toilet(s), Bedroom(s), living room, kitchen)

## How it works?
### Stage 1: Making sense of the situation
#### Step 1A: Sensors (real-time information fed to central cloud system which is not placed in the household) 
in multiple smaller devices to determin 
- Whether there is an event
- Type of event
- Severity of event
##### Workings of sensor
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
#### Step 1B: Voice chatbot (assessment of situation and casualty)
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

## Who it help?
Examples of vulnerable populations include:
- Elderly with no next of kin
- People with dementia
