# Auto Caption Lab — Hindi / Hinglish / English

A plain-local Expo web/mobile prototype that generates timed captions using Whisper AI in the browser.

## Automatic caption flow

1. Open the live site.
2. Choose an MP4, MOV, WEBM, or audio file.
3. Select Hindi, Hinglish, or English.
4. Tap **Generate automatic captions**.
5. The browser decodes the audio and runs `Xenova/whisper-tiny` locally through Transformers.js.
6. Timed caption lines appear and can be edited.

The first generation downloads the speech model from the public model CDN. The browser caches it for later use. Video/audio stays in the browser and is not sent to a project server.

## Live site

https://toxicchai.github.io/hindi-caption-studio/

## Current capabilities

- Automatic speech-to-text caption generation.
- Hindi, Hinglish, and English language selection.
- Timestamped caption chunks.
- Editable generated caption text and timing.
- Live word highlighting preview.
- Karaoke, Neon Pop, Clean, and Cinematic styles.
- Color, size, weight, and rounded-background controls.
- No account, watermark, subscription, or server-side usage limit.

## Practical device note

The browser model is intentionally free and local, but the first model download is large and transcription speed depends on the phone. Newer Android phones will work better. A production Android APK can later bundle a native Whisper model and FFmpeg export for faster offline processing and burned-in MP4 export.
