# eva-voice
**EvaBot Voice — TTS/STT engine & FastAPI voice service (:8000).**

## Contents
- `src/core/` — CloudTTS, EdgeTTS, CloudSTT (TypeScript engine layer)
- `backend/` — FastAPI voice service (`run.py`, `app/`, `requirements.txt`, `evabot-voice.service` systemd unit)
- `data_usage/` — TTS/STT usage accounting (edge-tts, stt, tts JSON)

## Deployment
systemd: `evabot-voice.service`, port 8000, nginx route `/voice` → :8000
