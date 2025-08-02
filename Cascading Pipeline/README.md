# 🚀 Cascading Pipeline Agent 

This demo shows how to build a customizable AI voice agent using the CascadingPipeline. With this setup, you can mix and match different providers for Speech-to-Text (STT), Large Language Models (LLM), and Text-to-Speech (TTS)—giving you full flexibility and control over your agent’s design.


## ✨ What is the Cascading Pipeline?

The CascadingPipeline is a key part of the VideoSDK AI Agent framework. It gives you the freedom to build agents using the best tools for each task—whether you're optimizing for cost, speed, or special features. No need to stick to one provider across the board.

### Key Features:

- **Modular Component Selection**: Independently choose providers for STT, LLM, and TTS.
- **Flexible Configuration**: Easily switch between providers like Google, OpenAI, Deepgram, and more.
- **Provider Agnostic**: Integrate a wide range of supported AI services.
- **Advanced Control**: Fine-tune each component to meet your application's needs.

For more in-depth information, please refer to the [official documentation on Cascading Pipeline](https://docs.videosdk.live/ai_agents/core-components/cascading-pipeline).

Change directory to Cascading Pipeline

## 📦 Plugin Installation

### Create and activate a virtual environment with Python 3.12 or higher:
```bash
# On macOS/Linux
python3.12 -m venv venv
source venv/bin/activate
```

### Install all dependencies from requirements.txt

```bash
pip install -r requirements.txt
```
<img width="940" height="472" alt="image" src="https://github.com/user-attachments/assets/5511f60e-3a53-43ba-9aa5-c6f09f055c07" />


## ⚙️ How to Run This Code

### 1. Set Up Your Environment

Before running the script, make sure you have the necessary API keys for the providers you intend to use. Store them in a `.env` file at the root of the project.

```
# .env
VIDEOSDK_AUTH_TOKEN=
DEEPGRAM_API_KEY=
GOOGLE_API_KEY= # here i am using gemini api
ELEVENLABS_API_KEY=
room_id=   
```
refer [prerequisites](https://github.com/KUNAL-MAURYA1470/AI-Voice-Agent/blob/main/README.md#prerequisites)


### 2. Run the Agent

Execute the script from your terminal:

```bash
python "cascading_agent_quickstart.py"
```

The agent will start and print a playground link to your console, which you can use to interact with it directly in your browser. 

<img width="1725" height="383" alt="image" src="https://github.com/user-attachments/assets/44bafa62-c2a9-4d34-814e-b84bbe7b2403" />

### Play with Agent
<img width="940" height="432" alt="image" src="https://github.com/user-attachments/assets/142b4f0a-7fa6-4ec3-a926-240169eecdb6" />

<img width="940" height="154" alt="image" src="https://github.com/user-attachments/assets/c6c03382-0488-4b7d-91df-f6f581b64ade" />


