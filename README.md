# LocalLore

This project is a speech-to-text pipeline that can transcribe audio files and generate a transcript of the speech. The project can also answer default and custom question asked by the user using the GPT-3.5 Turbo model.

## Architechture
![mp3_transcript_workflow](https://user-images.githubusercontent.com/90572559/230643567-360520b8-b467-4367-ac05-d7d4bc65d6ed.png)


## Team Information and Contribution 

Name | NUID | Contribution 
--- | --- | --- |
Karan Agrawal | 001090008 | 25% 
Rishabh Singh | 002743830 | 25% 
Lokeshwaran Venugopal Balamurugan | 002990533 | 25% 
Sivaranjani S | 002742197 | 25% 

## Link to Live Applications 
- Streamlit Application - http://34.138.127.169:8051
- Codelabs - https://codelabs-preview.appspot.com/?file_id=1RQSZ7LmsBowZf_GSkJaX4EfiLUobxXmViHWxYrZ9loU#0
- Demo of application - 

## Project Tree# Assignment-5
```
📦 
├─ .gitignore
├─ Dockerfile
├─ README.md
├─ __init__.py
├─ architechture
│  ├─ architechture.py << Python Code to Create Architechture
│  ├─ openai.png
│  ├─ streamlit.png
│  ├─ text_to_speech.png
│  └─ unsplash.png
├─ core_helpers.py << Core Helper Functions for Resuability
├─ docker-compose.yml
├─ mp3_transcript_workflow.png
├─ navigation
│  ├─ __init__.py
│  ├─ emergency_contacts.py << Code for Emergency Contacts
│  ├─ forex.py << Code for Forec Management
│  ├─ manual.py << Code for PhraseBook
│  ├─ translate.py << Code for Translation
│  └─ youtube.py << Code you YouTube Transcribtion
├─ requirements.txt
├─ temp_audio.mp3
└─ userinterface.py << Streamlit UI Router Code
```
©generated by [Project Tree Generator](https://woochanleee.github.io/project-tree-generator)

## Overview:

Travelling to a new place can be exciting and adventurous, but it can also be challenging and overwhelming. From language barriers to unfamiliar surroundings, travellers often face numerous obstacles during their journey. To make their travel experience stress-free, we have developed a one-stop application for all travellers. Our app provides a wide range of features that can help travellers plan, organise, and manage their trip more efficiently.

## Pages and features:

-*Youtube Page:* This page is designed to help users plan their travel itinerary more efficiently. By inputting a YouTube link to their favorite travel vlog or a vlog of a desired destination, along with the number of days they plan to spend there, users can generate a personalized itinerary for their trip. The system automatically downloads the audio from the YouTube video and sends it to the Wishper API to generate a transcript, which serves as context for the ChatGPT API to generate the itinerary for the specified number of days. Once generated, the itinerary will be displayed to the user for their reference. A logic also scrapes names of Location which are then used to get Images of those specific locations through Unspalsh API

-*Manual Page:* This page generates a phrasebook for a specific city, with translations from the local language to Latin text. It uses the OpenAI API to determine the language spoken in the city and to generate the phrasebook, and the Streamlit library to display the results. The application is useful for anyone interested in learning basic phrases in a foreign language or for travelers looking to communicate with locals in their destination city.  

-*Translate Page:* This page uses Google's Cloud Translation API and Cloud Text-to-Speech API to translate user-provided text into a specified target language and synthesize speech from the translated text. The user inputs the text they want to translate and selects the target language from a dropdown menu. Upon clicking the "Translate" button, the application generates the translated text, its Latin character version, the language code for the target language, and synthesized speech, which are all displayed on the screen.

-*Forex Page:* This page helps users track their expenses in multiple currencies by converting foreign currency to the user's home currency and categorizing expenses based on keywords in the name. It also generates a pie chart visualization that shows the user how much of their total spent belongs to each category, allowing them to identify areas where they are spending the most money. Overall, this script is a useful tool for anyone looking to gain insights into their spending habits and manage their expenses more effectively.

-*Emergency Page:* This page uses the OpenAI API to generate a list of emergency contacts for a specified city. It imports necessary libraries such as openai, streamlit, dotenv, and requests and loads the OpenAI API key from an environment variable using the dotenv library. The generate_emergency_contacts function takes a city as input and uses the OpenAI API to generate a list of emergency contacts for that city by sending a POST request to the OpenAI API endpoint with the prompt and other settings. This script is a useful tool for anyone looking to quickly generate a list of emergency contacts for a city they plan to visit or live in.


## Prerequisites

To run this project, you will need:

- Google Cloud Platform account
- OpenAI API key
- .env file containing the OpenAI,UnSplash,Google Maps keys in the same directory and the web application (Streamlit)


## .env file for streamlit:
- OPENAI_API_KEY=<openai_api_key> <- should be given in double quotes ("")
- UNSPLASH_API_KEY=<unsplash_api_key> <- should be given in double quotes ("")
- places_api_key = <places_api_key> <- should be given in double quotes ("")
- maps_api_key = <maps_api_key> <- should be given in double quotes ("")
- GOOGLE_APPLICATION_CREDENTIALS= <GOOGLE_APPLICATION_CREDENTIALS.json> <- should be given in double quotes ("")


## ATTESTATION:
WE ATTEST THAT WE HAVEN’T USED ANY OTHER STUDENTS’ WORK IN OUR ASSIGNMENT AND ABIDE BY THE POLICIES LISTED IN THE STUDENT HANDBOOK.
