# 🚀 AI-Voice-Agent
This repository contains demo agents built with the VideoSDK framework for integrating AI-powered voice agents into [VideoSDK](https://docs.videosdk.live) meetings using different LLM providers (OpenAI, Google Gemini LiveAPI,etc). Featured: Complete Agent-to-Agent (A2A) multi-agent system implementation and support for virtual avatars—realistic, lip-synced avatars that mirror speech in real time and give your AI agents a visual, human-like presence.

## Prerequisites

Before you begin, ensure you have:

- Python 3.12 or higher
- A VideoSDK authentication token (generate from [app.videosdk.live](https://app.videosdk.live))
- A VideoSDK meeting ID (you can generate one using the [Create Room API](https://docs.videosdk.live/api-reference/realtime-communication/create-room))
- API key for your chosen LLM provider (for Google Gemini API use this [Create Gemini API](https://aistudio.google.com/))
- Client-side implementation with any VideoSDK SDK (you can use [Playground Mode](https://playground.videosdk.live) to test)
- API key for [Deepgram](https://console.deepgram.com/)
- API key for [ELEVENLABS](https://elevenlabs.io/)
- API key for [Simli](https://app.simli.com/avatars)(If you using avatar)

### Generating a VideoSDK Meeting ID

Before your AI agent can join a meeting, you'll need to create a meeting ID. You can generate one using the VideoSDK Create Room API:

### Using cURL

```bash
curl -X POST https://api.videosdk.live/v2/rooms \
  -H "Authorization: VIDEOSDK_AUTH_TOKEN" \
  -H "Content-Type: application/json"
```
<img width="1352" height="323" alt="image" src="https://github.com/user-attachments/assets/5f39dc71-e191-415f-b88f-f8e67cad190c" />



For more details on the Create Room API, refer to the [VideoSDK documentation](https://docs.videosdk.live/api-reference/realtime-communication/create-room).

### Playground Mode

All quickstart examples are configured to run in playground mode by default (`playground=True`). When you run an agent, a direct link to the VideoSDK Playground will be printed in your console. You can open this link in your browser to interact with your agent without needing a separate client application.

```
Agent started in playground mode
Interact with agent here at:
https://playground.videosdk.live?token=...&meetingId=...
```


### 📁 Repository Structure

```
AI-Voice-Agent/
├── README.md
├── Cascading Pipeline/
│   ├── README.md
│   ├── cascading_agent_quickstart.py
│   └── requirements.txt
└── Virtual Avatar/
    ├── README.md
    ├── Dockerfile
    ├── requirements.txt
    └── simli_realtime_example.py
```    

### Clone Repository
```bash
git clone https://github.com/KUNAL-MAURYA1470/AI-Voice-Agent

cd AI-Voice-Agent
```

### Cascading Pipeline

<img width="940" height="432" alt="image" src="https://github.com/user-attachments/assets/be7a5909-efc3-4613-abd0-f8b99566ac43" />

Link:[Cascading Pipeline Documentation](./Cascading%20Pipeline/README.md)

### Virtual avatars AI Voice Agent
<img width="940" height="397" alt="image" src="https://github.com/user-attachments/assets/796d2886-e484-4a5b-b4f6-d7fc0d753cbc" />

Link:[Realtime Pipeline Documentation](./Virtual%20Avatar/README.md)








