# 🎭 Simli Virtual Avatar Examples

Enhance your AI agents with realistic, lip-synced virtual avatars using the [Simli](https://simli.com/) integration. Create more engaging and interactive experiences with:

- **Real-time Lip Sync**: Avatars that speak in sync with your AI agent's voice
- **Visual Engagement**: Provide a face to your AI agent for better user connection
- **Multiple Avatar Options**: Choose from various avatar faces or use custom ones
- **Seamless Integration**: Works with both RealtimePipeline and CascadingPipeline approaches

## Prerequisites

Before running the script, make sure you have the necessary API keys for the providers you intend to use. Store them in a `.env` file at the root of the project.

```
# .env
VIDEOSDK_AUTH_TOKEN=
DEEPGRAM_API_KEY=
GOOGLE_API_KEY=
ELEVENLABS_API_KEY=

SIMLI_API_KEY=
SIMLI_FACE_ID=

room_id=   
```
refer [prerequisites](https://github.com/KUNAL-MAURYA1470/AI-Voice-Agent/blob/main/README.md#prerequisites)

## Docker Installation

Dockerfile
```bash
FROM python:3.12-slim

# Install system dependencies
RUN apt-get update && apt-get install -y python3-dev

# Set working directory inside the container
WORKDIR /app

# Copy requirements and install dependencies
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy your Python script into the container
COPY simli_realtime_example.py .

# Run your agent
ENTRYPOINT ["python", "-u", "simli_realtime_example.py"]

```

<img width="622" height="202" alt="image" src="https://github.com/user-attachments/assets/0f9ae3cb-7127-41bf-a5f5-a04a31c3760b" />

```bash
docker build -t videosdk-agent .
```
<img width="940" height="283" alt="image" src="https://github.com/user-attachments/assets/319d721f-424d-4c27-a348-511afe5468f9" />

```bash
docker run --env-file .env videosdk-agent
```
<img width="940" height="113" alt="image" src="https://github.com/user-attachments/assets/b26fa26d-4de4-4aff-a6a6-fe20378ae703" />

<img width="940" height="397" alt="image" src="https://github.com/user-attachments/assets/8bee2a3b-c542-4d89-93c6-29c54d5fc054" />

## Manual Installation

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


### Getting Simli Credentials

1. Visit the [Simli Dashboard](https://simli.com/dashboard) to get your API key
2. Optionally, you can specify a custom `faceId` if you have one
3. If no `faceId` is provided, Simli will use a default avatar

### Run 
```bash
python simli_realtime_example.py
```




