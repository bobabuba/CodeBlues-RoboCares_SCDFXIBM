# Robocares inhouse central smart system

## Main Component
A central cloud (idk if this term is used correctly) system 
+ multiple (decide range of number? Can do like a minimum __ devices) small devices placed around the house 
(compulsory: Toilet(s), Bedroom(s), living room, kitchen)

## How it works

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

### Stage 2: Using analytics to make sense of the situation
- Data analysis of past cases of fire, falls, cardiac arrest on indicators like: volume, tone, temperature, etc
- Trained model based on database to accurately categorize cases and level of emergency

### Stage 3: Mobilization of CFRs for effective early intervention
Main idea: Leveraging on existing technologies (MyResponders App) , (Dog, UAV) and giving existing technologies new uses. 

#### 3A 1a - Suspected Minor Fire Case
- Activate UAV (Carry smaller size fire extinguisher + First Aid Kit to the scene)
- Activate CFRs on MyResponder App - “Minor Fire’
- Eg. Unattended Cooking Fire
- HFAD: Drastic increase in temperature in localized area
- Motion Sensor, Volume Sensor and Tone Sensor: Can be no abnormalities detected

#### 3B Suspected Major Fire Case
- Activate CFRs on MyResponder App - “Major Incident”
- Eg. Explosion 
- Device may detect sharp spike in temperature before being disconnected (damaged)

#### 3C Suspected Fall/Cardiac Case
- Any abnormalities in the motion, volume or tone sensor will automatically activate the Voice Chatbot.
- Motion Sensor: Abnormal patterns of motion detected or 
- Volume Sensor: Spike in volume (Scream for help) or 
- Tone Sensor: Distressed sensed in tone of person
- HFAD: Can be no abnormalities detected

### Stage 4: Using analytics to refine the system
- Data analysis of incidents like: accuracy of prediction, time taken for CFR to arrive, required items to gelp the situation, etc
- Collate areas of improvement and effective areas, and improve future deployments accordingly
- i.e. make first aid kit more accessible, etc


