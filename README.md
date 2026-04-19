# ACARE Voice Orchestration Module 🎙️🤖

> **Autonomous Clinical Assistance Robot** — Voice Interaction Layer  
> *ROS 2 Jazzy | Ubuntu 24.04 | Python 3.10*

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![ROS2](https://img.shields.io/badge/ROS2-Jazzy-blue)](https://docs.ros.org/en/jazzy/)
[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)

## 📋 Overview

The `acare_voice` module handles all voice-based interaction for the ACARE clinical assistance robot. It provides:
- **Streaming STT** via Deepgram Nova-2 WebSocket (en-IN optimized)
- **Voice Activity Detection** using Silero VAD (32ms chunks, local)
- **Intent Parsing** via Groq API (llama3-8b, JSON mode)
- **Speaker Verification** using SpeechBrain d-vector embeddings
- **TTS Responses** via Google Cloud WaveNet + pyttsx3 fallback for safety-critical messages
- **Emergency Keyword Monitoring** (always-on, <200ms latency)

## 🗂️ Repository Structure

## 🚀 Quick Start

### Prerequisites
```bash
# Ubuntu 24.04 + ROS 2 Jazzy installed
# Python 3.10+, pip, virtualenv recommended
# API keys: Deepgram, Groq, Google Cloud TTS (store in config/system.yaml)
