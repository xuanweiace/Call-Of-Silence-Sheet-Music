# Call of Silence - Staff Notation

This repository contains the AI-transcribed sheet music for the piece **Call of Silence**, as seen in the Bilibili video: [https://b23.tv/BrQ4isG](https://b23.tv/BrQ4isG).

## Transcription Process

The transcription was performed using an automated pipeline:
1.  **Media Acquisition**: Extracted audio stream from Bilibili using `yt-dlp` and `curl`.
2.  **Audio Processing**: Converted the raw `.m4s` stream to high-quality `.mp3` using `ffmpeg`.
3.  **AI Transcription**: Used Spotify's `basic-pitch` (deep learning model) to convert the audio into a MIDI file.
4.  **Score Rendering**: Transformed the MIDI file into LilyPond format (`.ly`) and rendered it into a standard 5-line staff notation PDF using `lilypond`.

## File Contents

- `Call-Of-Silence-Staff.pdf`: The rendered sheet music (staff notation).
- `artifacts/`:
    - `Call-Of-Silence.mid`: The AI-generated MIDI transcription.
    - `Call-Of-Silence.ly`: The LilyPond source code used for rendering the PDF.
    - `source_audio.mp3`: The audio source extracted from the video.

## Disclaimer

This transcription is AI-generated and may contain artifacts or errors in rhythm, pitch detection, or rest placement. It is intended as a starting point for further manual arrangement.
