# 🏵️ Ofrenda Viva (Living Altar)

> A private, open-source digital sanctuary honoring the Mexican tradition of **Día de los Muertos** through AI-powered remembrance, oral history preservation, and voice narration.

Built for the **[Hacktoberfest Open-Source AI Challenge Week 4: Ghost in the Machine](https://dev.to/challenges/hacktoberfest-week4-2026-10-26)**.

---

## 📖 Overview

When we lose someone, what lingers most are the tactile, everyday memories: the scent of roasted coffee at dawn, the songs hummed in the kitchen, or the pocket treats shared across a porch. 

**Ofrenda Viva** is a client-first web application designed to preserve personal oral heritage before it fades. A user speaks or types an unstructured, freeform story about an ancestor or loved one. The application leverages Google's open-weight **Gemma 2** model to channel the remembrance:
- Extracting the ancestor's name
- Identifying tangible favorite offerings (foods, drinks, habits, symbols)
- Calculating sacred *cempasúchil* (marigold) petal counts
- Composing a poetic bilingual remembrance tribute

The tribute is then transformed into a spoken vigil using **ElevenLabs** expressive speech synthesis, accompanied by flickering candlelight and drifting marigold petals.

---

## ✨ Features

- **🕯️ Open-Weight Intelligence (Gemma 2):** Powered by Google's `google/gemma-2-2b-it` model via Hugging Face Serverless Inference (or locally via Ollama).
- **🎙️ Expressive Voice Narration (ElevenLabs):** Translates written tributes into a warm, lifelike spoken vigil using the multilingual TTS model (with native browser speech fallback).
- **🔒 Local-First & Sovereign:** Sensitive memories and API keys stay on the user's device (`localStorage`). No private family stories are sent to closed enterprise training datasets.
- **🏵️ Atmospheric Altar UI:** Zero-dependency vanilla HTML5/CSS/JS with a simulated HTML5 `<canvas>` marigold petal particle effect and CSS candlelight glow.
- **📋 Share & Export:** One-click copy tool to preserve and share the completed memorial card.

---

## 🛠️ Tech Stack & Partner Tools

| Technology | Role |
| :--- | :--- |
| **Google Gemma 2 (`2b-it`)** | Open-weight foundation model parsing memories and writing eulogies |
| **ElevenLabs API** | High-fidelity voice synthesis (`eleven_multilingual_v2`) |
| **Hugging Face Inference** | Serverless open-weight inference gateway |
| **Vanilla HTML5 / CSS3 / JS** | Zero-bloat, responsive, standalone single-page interface |

---

## 🚀 Quick Start (Running Locally)

### Prerequisites
- Any modern web browser (Chrome, Edge, Firefox, Safari).
- A free **[Hugging Face Access Token](https://huggingface.co/settings/tokens)** (Read permissions).
- *(Optional)* An **[ElevenLabs API Key](https://elevenlabs.io)** for neural voice narration.

### Instructions

1. **Clone the repository:**
   ```bash
   git clone [https://github.com/sanjana806/Ofrenda-Viva.git](https://github.com/sanjana806/Ofrenda-Viva.git)
   cd Ofrenda-Viva
