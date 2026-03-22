# Call of Silence - Staff Notation (Cleaned/Quantized v2.0)

This repository contains the AI-transcribed sheet music for the piece **Call of Silence**, as seen in the Bilibili video: [https://b23.tv/BrQ4isG](https://b23.tv/BrQ4isG).

## Update: Version 2.0 (Cleaned/Quantized)

A major update has been performed to improve the readability and musicality of the transcription:
- **Quantization**: Rhythms have been cleaned and aligned to standard note durations, removing micro-jitters common in raw AI MIDI output.
- **Improved Transcription**: Pitch detection and rest placement have been refined.
- **Metadata Integration**: Cleaned up the LilyPond source for better score presentation.

## Transcription Process

The transcription was performed using an automated and refined pipeline:
1.  **Media Acquisition**: Extracted audio stream from Bilibili using `yt-dlp` and `curl`.
2.  **Audio Processing**: Converted the raw `.m4s` stream to high-quality `.mp3` using `ffmpeg`.
3.  **AI Transcription**: Used Spotify's `basic-pitch` (deep learning model) to convert the audio into a MIDI file.
4.  **Cleaning & Quantization (v2.0)**: MIDI data was processed to align rhythms and optimize notation.
5.  **Score Rendering**: Transformed the MIDI file into LilyPond format (`.ly`) and rendered it into a standard 5-line staff notation PDF using `lilypond`.

## File Contents

- `Call-Of-Silence-Clean.pdf`: The cleaned and quantized sheet music (v2.0).
- `Call-Of-Silence-Staff.pdf`: The original raw AI-generated transcription (v1.0).
- `artifacts/`:
    - `Call-Of-Silence-v2.mid`: The cleaned MIDI file.
    - `Call-Of-Silence-v2.ly`: The LilyPond source code for the cleaned version.
    - `Call-Of-Silence-v2.xml`: MusicXML export of the cleaned version.
    - `Call-Of-Silence.mid`: The original raw AI MIDI transcription.
    - `Call-Of-Silence.ly`: The original LilyPond source code.
    - `source_audio.mp3`: The audio source extracted from the video.

## Disclaimer

This transcription is AI-generated and may contain artifacts or errors in rhythm, pitch detection, or rest placement. It is intended as a starting point for further manual arrangement.
