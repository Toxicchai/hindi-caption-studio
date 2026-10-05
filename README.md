# Caption Lab — Hindi / Hinglish / English

A plain-local Expo Android app prototype for personal, unlimited caption editing.

## Included in this version

- Import a local video from the Android gallery.
- Preview the selected video inside the app.
- Hindi, Hinglish, and English language chips.
- Editable caption lines with start/end time fields.
- Add unlimited caption lines.
- Four starting styles: Cinematic, Neon Pop, Clean, and Karaoke.
- Live word-highlight toggle.
- Color swatches, size preview, font/weight/corner/background details.
- No login, account, watermark, subscription, or cloud API in the editor.

## Run on a realme Android phone

1. Install **Expo Go** from the Play Store.
2. Connect the phone and computer to the same Wi‑Fi network.
3. From this folder run:

   ```bash
   npm install
   npx expo start
   ```

4. Scan the QR code in Expo Go.

For a standalone Android build, use a local Android Studio/SDK setup and run `npm run android`, or generate an APK with the Expo/EAS Android build workflow later.

## Important scope note

The editor is fully local and unlimited. High-quality automatic Hindi/Hinglish speech-to-text and MP4 rendering require a native on-device transcription/rendering layer (for example, a bundled Whisper model plus FFmpeg). Those are deliberately kept separate from this first UI so the app stays lightweight and does not send private videos to a server. The current app ships with editable demo captions and the video import/preview foundation for that next native module.
