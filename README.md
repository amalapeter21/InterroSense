## 🔍 InterroSense: Scenario-Based AI-Driven Criminal Interrogation System with Real-Time Micro-Expression Analysis

**InterroSense** is a next-generation, AI-driven criminal interrogation support system that integrates **adaptive dialogue generation**, **facial behavior analysis**, and **real-time deception detection**. Designed to address the limitations of traditional and existing automated methods, InterroSense offers a **scalable**, **explainable**, and **scenario-conditioned interrogation framework** to assist law enforcement officers during suspect evaluation.

---

### 🎯 Problem Statement

Conventional interrogation processes often rely on human intuition, making them prone to bias, fatigue, and inconsistency. Existing automated systems are limited by single-modality inputs (e.g., only text or only video) and lack real-time adaptability or feedback. InterroSense bridges this gap with a **multi-modal, real-time AI assistant** that provides dynamic support during live or remote interrogations.

---

### 🚀 Key Features

#### 🗣️ Adaptive Dialogue Interrogation

* Fine-tuned **Qwen1.5–1.8B-Chat** LLM generates **scenario-based interrogation questions**.
* Accepts **text and audio** input from suspects.
* Uses **Google Speech-to-Text API** for audio transcription.
* Dynamically adapts based on suspect responses using baseline, contradiction, and cognitive-load strategies.

#### 🎥 Real-Time Facial Behavior Analysis

* Detects **micro-expressions** using a **MobileNetV3-based AU classifier**, trained on the **Bag-of-Lies** dataset.
* Tracks **gaze direction** and **head pose** to analyze stress, evasion, or deception.
* Uses **OpenCV** and **MediaPipe** for live computer vision processing.

#### 🔀 Multimodal Fusion for Deception Detection

* Fuses **linguistic deception cues** (e.g., hesitation, contradictions, emotional tone) with **facial behavior**.
* Uses **weighted late fusion**, adapting modality weights in real time based on reliability.
* Generates an interpretable **deception probability score** visible to officers during questioning.

#### 📊 Officer Dashboard & Feedback

* Built using **Django**, with a clean and interactive UI.
* Displays live deception scores, cue breakdowns, and recommended follow-up questions.
* Offers full session logs for training, audit, or review.

---

### ⚙️ Tech Stack

| Component           | Technology                                   |
| ------------------- | -------------------------------------------- |
| **Frontend**        | HTML, CSS, JavaScript                        |
| **Backend**         | Django (Python)                              |
| **LLM**             | Qwen1.5–1.8B-Chat (fine-tuned)               |
| **Speech-to-Text**  | Google Speech-to-Text API                    |
| **Computer Vision** | MobileNetV3, OpenCV, MediaPipe               |
| **Facial Analysis** | Action Unit classifier (Bag-of-Lies dataset) |
| **Database**        | Firebase                                     |
| **Model Framework** | PyTorch                                      |

---

### 📥 Inputs

* Live webcam feed (video)
* Suspect's spoken or typed responses
* Case scenario context (e.g., robbery, cybercrime)
* Pre-trained model weights
* Real-time audio/video stream

---

### ✅ Expected Outcomes

* Scenario-adaptive dialogue flow
* Real-time deception probability with visual cue overlays
* Reduction of officer bias and fatigue
* Enhanced transparency and accountability
* Full logs for post-analysis and officer training

---

### 📚 Datasets Used

* **Bag-of-Lies**: Multimodal deception dataset with audio, video, gaze, and EEG cues.
* **Custom Scenario-Based Dataset**: Synthesized from legal transcripts, role-play simulations, and interrogation records to train Qwen1.5–1.8B-Chat on rich, contextual dialogue.

---

### 🌐 Applications

* Criminal and cybercrime investigations
* Virtual suspect interviews
* Law enforcement officer training modules
* Psychological and behavioral research

---
