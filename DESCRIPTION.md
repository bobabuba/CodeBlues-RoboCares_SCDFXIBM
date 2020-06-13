# ROBOCARES Home Monitoring System

## Content
- [Background](#background)
- [Who it helps?](#who-it-helps)
- [Why Robocares?](#why-robocares)
- [What is the ROBOCARES Home Monitoring System?](#what-is-the-robocares-home-monitoring-system)
- [How does it work?](#how-does-it-work)

## Background
With Singapore facing an increasingly silver population, there is a larger vulnerable elderly population. These include elderly living alone, those with no next of kin, and those who are mostly alone at home. As Singapore pushes to be a smart nation, important agencies such as the SCDF can better harness the power of technology to respond more effectively to emergencies (e.g. cardiac arrests, falls, unattended cooking fires etc.). Moreover, SCDF can leverage on enhancing and streamlining the process for mobilising CFRs for early intervention. These improvements will greatly enhance SCDF's capabilities to save lives.  

## Who does it help?
Examples of vulnerable populations include:
- Elderly with no next of kin, living alone
- People with dementia
– Elderly who are alone at home most of the time (eg. their children are working)

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

## What is the ROBOCARES Home Monitoring System?
ROBOCARES Home monitoring system consists of a central cloud system linked to multiple devices (ROBOCARES) which are placed around the house.  The system utilises IoT, AI, Data Analytics and Machine Learning. Each ROBOCARE consist of 3 types of sensors and have the HFAD incorporated. We recommend that these devices be placed in locations where the elderly frequent such as the toilets, bedrooms, living room and kitchen. 

Using the sensors, the ROBOCARES Home Monitoring System tells us 3 important pieces of information: (1) Whether there is truly an emergency (2) Type of emergency [if any] (3) Severity of emergency. This allows for better sense-making at the onset of the incident.

The ROBOCARES Home Monitoring System is linked to the MyResponder app, and will activate CFRs depending on the type of event detected. This will be elaborated on further in the later parts of the explanation.

Additionally, two types of Unmanned Aerial Vehicles (UAVs) will be stationed at the void deck of HDB blocks to complement ROBOCARES. The number of UAVs found in each neighbourhood depends on the population density of vulnerable groups in that location. 

The first type of UAV is the AED UAV, while the second type of UAV is the Fire Extinguisher UAV. As the name suggests, the former will carry around an AED, while the latter carries with it an small portable fire extinguisher. Both UAVs will also be equipped with first aid kits. 

Depending on the type of event suspected, the type of UAV deployed will differ. This allows the CFRs to head directly to the location and have the necessary equipment and/or first aid supplies to help the resident more effectively and quickly. 

## How does it work?
### Component 1: ROBOCARES
####  Sensors
1. Volume Sensor
- Detect sudden increases in volume
- Examples: Shouting, Loud bangs, Clashing, Collapsing, Explosions, Loud thuds (Possibly from someone collapsing)
between person’s voice and others’ voice (Eg. from technological devices - TV, phone, radio)
2. Frequency Sensor
- Detect changes in frequency that may be cause for concern (eg. From Screaming)
- The frequency sensor can be set to be compatible to recognise the resident’s voice. Hence, when the resident is experiencing an emergency, the frequency sensor will be able to differentiate between the resident’s voice and others’ voice (eg. from technological devices - TV, phone, radio) through voice matching.
3. Motion Sensor
- A smart analyzing system can be used to track usual time spent by the resident in various parts of the house. This will allow the system to identify abnormalities in the movement patterns of the resident.
- Sensor will also sound out if if movement is absent for prolonged periods of time
4. Home Fire Alarm Device (HFAD)
- Existing SCDF technology used to detect fires
- Will be placed in kitchen, but resident will be given 1 minute to disarm in case of false alarms before we activate the UAV and MyResponder app.

#### Voice Chatbot
- Robocare will first ring for 5 seconds (like an alarm)
- Chatbot will then ask in Dialect/Malay/the selected language: Is there anything wrong? Do you need help?
- Refer to Flowchart 1 below for the workings of the Voice Chatbot

### Component 2: Unmanned Aerial Vehicles (UAVs)
- As mentioned earlier, two types of Unmanned Aerial Vehicles (UAVs) will be stationed at the void deck of HDB blocks to complement ROBOCARES. The number of UAVs found in each neighbourhood depends on the population density of vulnerable groups in that location. 
- The first type of UAV is the AED UAV, while the second type of UAV is the Fire Extinguisher UAV. As the name suggests, the former will carry around an AED, while the latter carries with it an small portable fire extinguisher. Both UAVs will also be equipped with first aid kits.
- Depending on the type of event suspected, the type of UAV deployed will differ. This allows the CFRs to head directly to the location and have the necessary equipment and/or first aid supplies to help the resident more effectively and quickly. 

-insert image of UAVs-

### Component 3: Mobilization of CFRs for effective early intervention
The mobilization of CFRs will be illustrated through the 4 main types of cases
1. Suspected Minor Fire Case
- Indications: HFAD Activated alarm
- Activates Fire Extinguisher UAV
- Activates CFRs on MyResponder App - “Minor Fire’
- Eg. Unattended Cooking Fire
2. Suspected Major Fire Case
- Indications: HFAD Activated Alarm before being disconnected (eg. damaged due to explosion)
- Activates CFRs on MyResponder App - “Major Incident”
3. Suspected Fall/Cardiac Case
- Voice Chatbot: Activated by abnormalities reported in the Motion, Volume or Frequency Sensors

## Putting it Together
Using the Flowchart for the Voice Chatbot, we illustrate how all the 3 components are put together

Flowchart 1:
-insert image of flowchart-

### Component 4: Using analytics to refine the system
- Use of Artificial Intelligence (AI) to categorize cases and level of emergency more accurately to improve further deployments.
- Information (Including what each of the sensors picked up) from each case will be added into the database and AI will be used to refine the prediction as to what type of event it is, which can help to improve deployments and effectiveness of response to such incidents as it is clearer as to what information are needed for the type of event accordingly.

Information to be included in database:
- Volume Sensor’s indicator (Depending on the instrument)
- Volume Sensor - Abnormality? (Y/N)
- Frequency Sensor’s indicator (Depending on the instrument)
- Frequency Sensor - Abnormality? (Y/N)
- Motion Sensor’s indicator (Depending on instrument)
- Motion Sensor - Abnormality? (Y/N)
- HFAD Triggered? (Y/N)
- To Predict: Type of Event (Cardiac Arrest Case, First Aid Case, Minor Fire Case, Major Fire Case)



