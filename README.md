Bilingual AI Voice Assistant (Tamil & English) link: https://colab.research.google.com/drive/1IKPE7cnf6AdZ9zNESXGDCCpHaXdgYFv6?usp=sharing
A powerful, conversational AI voice assistant that understands and responds in both Tamil and English. Built with Python and powered by Google's Gemini LLM, this project runs entirely in a Google Colab notebook, making it accessible to anyone with a browser.

✨ Features
🗣️ Bilingual Conversation: Seamlessly interact with the assistant in either Tamil or English.

🧠 AI-Powered Intelligence: Leverages the Google Gemini 1.5 Flash model to understand context and provide intelligent, human-like answers to complex questions.

🔄 On-the-Fly Language Switching: Instantly switch the assistant's active language with a simple voice command or button click.

🎙️ Voice-Activated: Fully hands-free interaction using real-time speech recognition.

🌐 Zero Local Setup: Runs directly in Google Colab, requiring no local installation of Python or other complex dependencies.

🚀 How It Works
The assistant operates on a multi-step pipeline that processes your voice and generates a spoken response.

Voice Capture: The browser's microphone records your voice command for 7 seconds.

Audio Conversion: The recorded audio is converted from its native web format to a high-quality .wav file using FFmpeg.

Speech-to-Text (STT): The .wav file is sent to Google's Web Speech API, which transcribes the audio into text in the selected language.

AI Processing (The Brain):

The transcribed text is sent to the Google Gemini LLM.

The model analyzes the meaning of the question and generates a thoughtful, relevant response in the same language.

Text-to-Speech (TTS): The AI's text response is converted back into natural-sounding audio using Google's Text-to-Speech service.

Spoken Reply: The final audio is played back to you through your speakers.

🛠️ Getting Started
You can run this assistant yourself in just a few steps.

Prerequisites
A Google Account to use Google Colab.

A Google Gemini API Key. You can get a free key from Google AI Studio.

Installation & Usage
Open the Notebook:

Click the "Open in Colab" badge at the top of this README.

Alternatively, go to colab.research.google.com and upload the .ipynb file from this repository.

Add Your API Key:

In the first code cell, you will see a field for API_KEY. Paste your secret key from Google AI Studio into this field.

Run the Notebook:

Go to the menu and select "Runtime" -> "Restart and run all".

This will install all necessary libraries and start the assistant.

Grant Permissions:

Your browser will ask for permission to use your microphone. You must click "Allow" for the assistant to hear you.

Interact with the Assistant:

Once the setup is complete, two buttons will appear: "Start Listening" and "Switch Language".

Click "Start Listening" and ask a question in the active language (it starts in Tamil).

Click "Switch Language" to change the assistant's language to English and back.

⚙️ Technologies Used
Core Language: Python

Environment: Google Colab

Large Language Model (LLM): Google Gemini 1.5 Flash

Speech-to-Text: SpeechRecognition library (using Google Web Speech API)

Text-to-Speech: gTTS (Google Text-to-Speech)

Audio Conversion: FFmpeg

🔮 Future Improvements
"Wake Word" Detection: Implement a hotword like "Hey Gemini" to start the listening process without needing to click a button.

Longer Conversations: Maintain a history of the conversation to allow for follow-up questions.

API Integration: Connect the assistant to external APIs to fetch real-time data like weather forecasts or news headlines.

Web UI: Build a standalone web interface using a framework like Flask or Streamlit to host the assistant outside of Colab.

