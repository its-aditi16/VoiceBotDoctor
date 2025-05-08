
🧠 VoiceBot Doctor Assistant
An intelligent voice-enabled healthcare assistant using multimodal LLMs to interpret patient inputs (voice & image) and provide diagnosis-like outputs via voice.

📌 Project Layout
Phase 1 – Setup the Brain of the Doctor (Multimodal LLM)
Setup GROQ API key

Convert image to required format

Setup Multimodal LLM (LLaMA 3 Vision)

Phase 2 – Setup Voice of the Patient
Setup audio recorder (using ffmpeg & pyaudio)

Setup Speech-to-Text (STT) using OpenAI Whisper for transcription

Phase 3 – Setup Voice of the Doctor
Setup Text-to-Speech (TTS) using gTTS and ElevenLabs

Use TTS model for converting text output into voice

Phase 4 – Setup UI for the VoiceBot
Build an interactive UI using Gradio

🔍 Project Working
The VoiceBot Doctor takes inputs from the patient's voice and a medical image (e.g., skin lesion, wound, visible symptoms). Here's how it works:

Voice Input: The patient speaks about their symptoms; the audio is recorded and transcribed using OpenAI Whisper.

Image Input: The patient uploads a visible image of the affected area (e.g., skin rash).

Multimodal Analysis: LLaMA 3 Vision (via Groq) analyzes the image along with the transcribed text to predict the possible condition or disease.

Doctor's Voice Response: The output is converted to a realistic spoken response using gTTS or ElevenLabs and delivered back to the patient via the VoiceBot UI.

This makes it an inclusive and accessible assistant that can support early detection of visible conditions through natural interaction.

🛠️ Tools and Technologies
GROQ – For AI inference

OpenAI Whisper – Best open-source model for transcription

LLaMA 3 Vision – Open-source multimodal LLM by Meta

gTTS & ElevenLabs – For converting text to speech

Gradio – For building simple and intuitive UI

Python – Core development language

VS Code – Development environment

✅ Requirements
Python 3.8+

ffmpeg

pyaudio

openai-whisper

gtts

gradio

requests

API keys for GROQ and ElevenLabs
