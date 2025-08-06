# 🖼️🔊 Image Caption to Speech

This project demonstrates a simple yet powerful AI pipeline that performs **image captioning** and **text-to-speech (TTS)** conversion.

You provide an image → the model generates a **textual description** (caption) → and then the caption is **converted into speech** (audio). This project combines **vision**, **language**, and **speech** models in one workflow.

---

## 🔍 Project Description

### ✨ Objective:
Extract a meaningful description from an image and convert that description into human-like speech.

### 🧠 How It Works:
1. **Image Captioning (BLIP model)**: An AI model looks at the image and generates a descriptive sentence.
2. **Text-to-Speech (Coqui TTS)**: The generated sentence is spoken aloud using a TTS model.

---

## 🧠 Models Used

### 1. 🔷 BLIP (Bootstrapping Language-Image Pretraining)
- **Model:** `Salesforce/blip-image-captioning-base`
- **Type:** Vision-Language Model (Image → Text)
- **Use:** Generates a caption for an input image.
- **Example Output:** `"A dog sitting on green grass"`

### 2. 🔊 Coqui TTS
- **Model:** `tts_models/en/ljspeech/tacotron2-DDC`
- **Type:** Neural Text-to-Speech Model (Text → Audio)
- **Use:** Converts the generated caption into audio and saves it as a `.wav` file.

---

## 🛠️ Dependencies
transformers – for loading BLIP model

Pillow – for image handling

TTS – for text-to-speech (Coqui TTS)

torch – required for running models

torchaudio – TTS backend audio support

---
Output
Caption Generated: "A girl standing in front of a mountain"

Audio File: caption_audio.wav with spoken version of the caption
