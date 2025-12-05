<a name="readme-top"></a>

<p align="center">
  <img src="https://pub-0f9c49dcde884c17995c23a801ee5836.r2.dev/Home/GameVFX3.gif" width="720" alt="CATAS header">
  <br><br>

  <img src="https://img.shields.io/badge/status-active-brightgreen">
  <img src="https://img.shields.io/badge/license-MIT-blue">
  <img src="https://img.shields.io/badge/platform-HoloLens%202%20%7C%20PC-9cf">
  <img src="https://img.shields.io/badge/data-video%20%7C%20audio%20%7C%20eye--tracking-orange">
</p>

<p align="center">
  <a href="#project-overview">📘 Overview</a> |
  <a href="#key-features">✨ Features</a> |
  <a href="#getting-started">🚀 Getting Started</a> |
  <a href="#usage">🧭 Usage</a> |
  <a href="#contribution">🤝 Contributing</a> |
  <a href="#license">📄 License</a>
</p>


<h1 align="center">Context Awareness Text Augmented System (CATAS)</h1>

## Project Overview

The **Context Awareness Text Augmented System** is an open-source project developed under the guidance of **Professor Junxiao Shen** at the *University of Bristol*'s **BIG Lab**. The system uses **HoloLens 2** as a data collection platform and enables **real-time communication** of multimodal data (video, audio, eye-tracking) via a **Peer-to-Peer (P2P) connection** between **XR** and **PC systems** based on HL2SS. This project aims to capture and process user behavior in an immersive environment and generate textual descriptions of these actions using AI models. 

> If your research aligns with AR/VR, XR sensing, or context-aware AI, we welcome discussions and collaboration.

## Key Features

- **Real-Time Multimodal Data Communication**  
  Supports the transmission of video, audio, and eye-tracking data in real time between **HoloLens 2** and a PC system via a stable **P2P connection**. 🌐

- **Data-to-Text AI Models**  
  Utilizes AI-based models to convert raw multimodal data into text representations of user behavior. 🧠➡️📝

- **Multithreading for Parallel Data Handling**  
  Implements multithreading to ensure efficient data processing and timestamp synchronization for accurate communication. 💻⚙️

## Getting Started

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/username/context-awareness-text-augmented-system.git
   ```

2. Install required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up the **HoloLens 2** device for data collection and ensure the **P2P connection** is active between the device and the PC. 🔌

> **Note:** HL2SS must be properly configured on HoloLens 2 and the PC endpoint. Ensure both devices are discoverable within the same network segment.

## Usage

### 1) Establishing Connection

- Ensure both **HoloLens 2** and the PC are connected via the **P2P connection**. 

### 2) Data Collection

- Use **HoloLens 2** to collect video, audio, and eye-tracking data. 

### 3) AI Workflow

- The data will be processed by AI models to generate text versions of user actions. 
- Use the generated text to interact with the **Question-Answering System** for daily behavior tracking. 

### Minimal Run Example

```bash
python MainSys.py
```

## Project Structure

```
├── MainSys.py                    # Main entry point of the system
│
├── Components/                   # Multimodal data modules
│   ├── Audio_Component.py        # Audio data handling
│   ├── Eyetracking_Component.py  # Eye-tracking data capture & processing
│   ├── IMU_Component.py          # IMU sensor integration
│   ├── Video_Component.py        # Video frame streaming
│   └── __init__.py
│
├── clip/                         # CLIP-based text augmentation module
│   ├── __init__.py
│   ├── clip.py
│   ├── model.py
│   ├── simple_tokenizer.py
│   └── bpe_simple_vocab_16e6.txt.gz
│
├── requirements.txt
└── README.md

```

## Contribution

Contributions are welcome! To contribute, fork this repository, make your changes, and submit a pull request. 🔄💡  
Please follow conventional commits and open an issue for major feature proposals.

## License

This project is licensed under the **MIT License**. 📄 See [`LICENSE`](./LICENSE) for details.

---

<p align="right">(<a href="#readme-top">back to top</a>)</p>
