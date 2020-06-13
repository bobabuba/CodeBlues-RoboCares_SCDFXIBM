# ROBOCARES Home Monitoring System

## Content
- [Background](#background)
- [Why Robocares?](#why-robocares)
- [What is it?](#what-is-it)
- [How it works?](#how-it-works)
- [Who it helps?](#who-it-helps)

## Background
With Singapore facing an increasingly silver population, there is a larger vulnerable elderly population. These include elderly living alone, those with no next of kin, and those who are mostly alone at home. As Singapore pushes to be a smart nation, important agencies such as the SCDF can better harness the power of technology to respond more effectively to emergencies (e.g. cardiac arrests, falls, unattended cooking fires etc.). Moreover, SCDF can leverage on enhancing and streamlining the process for mobilising Community First Responders (CFRs) for early intervention. These improvements will greatly enhance SCDF's capabilities to save lives.  

## Why Robocares?
### Problems to tackle
1. Distinguishing an emergency from a false alarm to reduce wastage of precious resources.
2. Timely discovery of emergencies, especially for vulnerable populations who spend most of their time at home alone.
3. Analysis and tracking of situation while waiting for the emergency services to come.
4. Quicker mobilization of CFRs for effective early and effective intervention, especially for vulnerable populations.
5. Prompt retrieval process of essential resources like fire extinguishers and AEDs to assist CFRs.

### Solution
ROBOCARES Home Monitoring System can help to:
1. determine if the resident is in an emergency situation.
2. assess the severity of the situation with the use of sensors and a voice chatbot.
3. consistently upload real-time information for analysis by relevant personnels while help is being deployed to the scene.
4. mobilize CFRs in the vicinity early on so that they can provide timely help or resolve any minor emergencies promptly.
5. retrieve essential resources to the scene more quickly, allowing for more timely response from CFRs as they reduce their journey time to the house as they do not have to worry about getting the resources.

### Technology involved
1. Existing technology
- MyResponder App to notify CFRs.
- Home Fire Alarm Device (HFAD) to detect possible fire cases.
2. Internet of Things (IoT)
- Sensors to obtain readings on motion and voice, to make sense of the situation.
3. Artificial Intelligence
- Voice-enabled Chatbot for further analysis of the situation and obtaining of details from casualty.
4. Data Analytics
- Develop model to predict whether there is an event, as well as type and severity of event, based on readings collected.
- Analyse incidents picked up by Robocares (i.e. accuracy of prediction, time taken for help to arrive, etc) for future enhancements.
5. Unmanned Aerial vehicles (UAVs)
- Deploy essential resources like AED and fire extinguisher to the scene of incident.\

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
ROBOCARES leverages on IoT to obtain readings on various environmental factors, which will be compared against a benchmark to detect possible emergencies. It utilises various types of sensors for greater accuracy.

The sensors utilized include:

1. Volume + Frequency (Tone) sensor
- ROBOCARES can pick up abnormal sounds such as:
    * Sudden, loud banging/clashing sounds 
    * Sound of person collapsing (loud thud/ sound of hitting against another surface)
    * Shouts, screams, words like ‘help’, ‘save me’ (in different languages)
- Through the use of AI, ROBOCARES can leverage on Voice Match function to recognise the user's voice, and differentiate between the user's voice and other voices (i.e. from electronic gadgets like television, mobile phones, radio). This prevents false alarms, such as screams from movies.

2. Motion sensor
- ROBOCARES uses AI to track the usual distribution of time spent in various parts of the house, and will be alerted when detecting any abnormalities.
- ROBOCARES also dectects if a fall has occurred.

3. HFAD (heat and smoke detector)
- This is the existing SCDF technology which detect fires
- Some flats may already have HFAD installed via the HFAD Assistance Scheme or mandatory installation for new residential flats.
- Siren will be activated to alert user and neighbours.
- The HFAD will not be placed in the kitchen, and will be given 1 minute for user to deactivate the siren before deploying UAVs, SCDF and CFRs, to prevent false alarms.


#### Voice Chatbot
If there is a suspected emergency, ROBOCARES will ring for 5 seconds, before activating the Voice Chatbot.
The Voice Chatbot will first ask if there is anything wrong and if help is required, in a pre-set language/dialect, and respond accordingly. Depending on the situation, the required help will be deployed.
![Flowchart](flowchart.png)

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
