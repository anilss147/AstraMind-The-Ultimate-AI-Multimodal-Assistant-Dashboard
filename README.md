# 🚀 AstraMind: The Ultimate AI Multimodal Assistant Dashboard

[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/Framework-FastAPI-00a676.svg)](https://fastapi.tiangolo.com/)
[![Gradio](https://img.shields.io/badge/UI-Gradio-orange.svg)](https://www.gradio.app/)
[![Docker](https://img.shields.io/badge/Docker-Supported-blue.svg)](https://www.docker.com/)
[![Deploy on Hugging Face](https://img.shields.io/badge/HF%20Spaces-Deployed-blueviolet?logo=huggingface)](https://huggingface.co/spaces)

> AstraMind is a powerful, all-in-one AI dashboard that enables users to interact with text, image, voice, and video models through a unified, real-time interface. Built with FastAPI and Gradio/React, it supports leading open-source models like Mistral, LLaMA, Whisper, Stable Diffusion, Coqui-TTS, and more.

---

## 🧠 Features

- ✅ Text, Voice, Image, and Video AI interaction
- 🎤 Real-time STT with Whisper + Voice replies (Coqui TTS)
- 🖼️ Image generation, segmentation & enhancement with SD & SAM
- 🌐 Language translation & emotion detection
- 💬 Streaming chat responses with WebSocket
- 🧩 Modular architecture with model auto-switching
- 🔐 Authenticated API access with JWT / API Keys
- 💾 Memory & history with SQLite/PostgreSQL + VectorDB
- 📊 Dashboard logging, progress bars, and analytics
- 🐳 Docker + Hugging Face Spaces + GitHub Actions ready

---

## 🏗 Architecture

```plaintext
🌐 FRONTEND UI (Gradio/React)
└── Input: Text | Voice | Image | Video
    └── WebSocket / FastAPI REST
        └── FASTAPI SERVER (Routing + Auth + Stream)
            ├── AI Orchestration Engine
            │   ├── Text (Mistral, LLaMA, LangChain)
            │   ├── Image (Stable Diffusion, SAM)
            │   ├── Voice (Whisper, Coqui-TTS)
            │   └── Video (YOLO, WebRTC)
            ├── Sentiment + Translation Modules
            ├── Memory Manager (SQLite/PG + ChromaDB)
            └── Logs, User Sessions, Model Cache
                └── Docker / Spaces / CI/CD Deployment
