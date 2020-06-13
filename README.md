# CodeBlues-RoboCares_SCDFXIBM

## Content
- [The Team](#the-team)
- [Short Description](#short-description)
- [Demo Video](#demo-video)
- [The Architecture](#the-architecture)
- [Detailed Solution Description](#detailed-solution-description)
- [Getting Started](#getting-started)
- [Built With](#built-with)

## The Team
Our team is called CodeBlues.
Our team members consist of:
- Crystal Teo
- Gini Wong 
- Claire Tang
- Koh Hui Juan

## Short Description
### Problem Statement: Emergency Medical Services
With Singapore facing an increasingly silver population, there is a growing segment of vulnerable elderly population. These include elderly living alone, those with no next of kin, and those who are mostly alone at home. The occurence of emergencies in these homes may be oblivious to the public eye, until it is too late. 

### How can technology help?
As Singapore pushes to be a smart nation, SCDF can better harness the power of technology to respond more effectively to emergencies (e.g. cardiac arrests, falls, unattended cooking fires etc.). Moreover, SCDF can leverage on enhancing and streamlining the process for mobilising CFRs for early intervention. These improvements will greatly enhance SCDF's capabilities to save lives.

### Idea: Robocares
There is a crucial need for the ability to detect incidents in homes, especially for vulnerable populations. Robocares is a home monitoring system, developed with IBM Cloud and Watson Services, which allow for better understanding and prompt alert at the onset of incidents which require emergency response, which in turn enhances the process of mobilising CFRs for effective early intervention.

## Demo Video
[![Watch the video](Link to image of video)](youtube link to video)

## The Architecture
1. System detects potential emergency
2. System rings, then activates voice chatbot.
3. Watson Speech to Text processes audio and extracts the text
4. Watson Language Translator translate text to desired language
5. Watson Text to Speech for chatbot to respond to user
6. Watson Tone Analyser to derive emotions of casualty
7. Information sent to SCDF and myResponder App, to deploy help
8. Data collection of incidents for data analysis and future enhancement

## Detailed Solution Description
d) A hyperlink to your detailed solution* (Long description of your solution)
make a DESCRIPTION.md, copy and paste the google docs we wrote

## Getting Started
f) Getting started* (Step-by-step instructions to install the required software and how
to run a demo of your solution)

## Built With
1. Voice Chatbot: Watson Assistant, Speech to Text, Text to Speech, Tone Analyser, Language Translator, Node Red
2. Data Analysis

2. Node Red
i) What your team used to build your solution* (e.g. IBM Cloudant, IBM Cloud Functions, etc…)
