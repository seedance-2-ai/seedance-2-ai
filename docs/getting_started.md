# Getting Started with Seedance 2.0 SDK

This guide provides instructions on how to integrate the **Seedance 2.0 (Oriental Skylark)** API into your creative workflow.

## Prerequisites
- Python 3.8 or higher
- An API Key from **BytePlus** or **Jimeng AI** developer portal.

## Installation
Currently, the SDK is in early access. You can clone this repository to use the local wrapper:

```bash
git clone https://github.com/seedance-2-ai/seedance-2-ai.git
cd seedance-2-ai
pip install requests
```

## Quick Start: Text-to-Video
To generate your first AI video using the Seedance 2.0 model:

```python
from src.seedance_api_wrapper import SeedanceClient

client = SeedanceClient(api_key="YOUR_API_KEY")

# Generate video
response = client.generate_video(
    prompt="Cinematic shot of a dragon flying over snowy mountains",
    mode="cinematic"
)

print(f"Task ID: {response['task_id']}")
```

## How to use Lip-Sync
One of the most powerful features of **Seedance 2.0** is the audio-to-video lip-sync.
1. Provide a base video.
2. Provide an audio file (MP3/WAV).
3. The model will regenerate the mouth movements to match the audio perfectly.

[Read more about Pricing and Rate Limits...](#)
```

---
