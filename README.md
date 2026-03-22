# Call of Silence - Staff Notation (Grand Staff v3.0)

This repository contains the AI-transcribed sheet music for the piece **Call of Silence**, as seen in the Bilibili video: [https://b23.tv/BrQ4isG](https://b23.tv/BrQ4isG).

## Latest Version (v3.0) - Grand Staff (Piano Split)

The latest update introduces the **Grand Staff (Piano Split)** version, significantly improving readability for piano players by separating the notes between the right and left hands.

### Major Enhancements:
- **Piano Hand Splitting**: Notes are automatically assigned to the Treble Clef (Right Hand) or Bass Clef (Left Hand) based on a pitch threshold (Middle C).
- **Refined Quantization**: Implemented advanced quantization (1/8 note) to eliminate rhythmic micro-jitters while preserving the musical essence.
- **Enhanced MIDI & XML**: Updated artifacts include a quantized MIDI file and a structured MusicXML file (v3.0) for easy editing in MuseScore, Sibelius, or Finale.

## File Contents

- `Call-Of-Silence-Grand-Staff.pdf`: **(Recommended)** Piano version with Left/Right hand split.
- `Call-Of-Silence-Clean.pdf`: Single-staff version with cleaned quantization (v2.0).
- `Call-Of-Silence-Staff.pdf`: Original raw AI transcription (v1.0).
- `artifacts/`:
    - `Call-Of-Silence-Grand.mid`: Quantized MIDI with hand-split channels.
    - `Call-Of-Silence-Grand.ly`: LilyPond source for the Grand Staff version.
    - `Call-Of-Silence-Grand.xml`: **(Recommended for Editing)** MusicXML for piano notation.
    - `Call-Of-Silence-v2.ly`, `Call-Of-Silence-v2.mid`, `Call-Of-Silence-v2.xml`: Files for the v2.0 single-staff version.
    - `Call-Of-Silence.ly`, `Call-Of-Silence.mid`: Original raw transcription files.
    - `source_audio.mp3`: The original audio source extracted from the video.

## Transcription Process

The transcription follows a refined automated pipeline:
1.  **Media Acquisition**: Extracted audio stream from Bilibili using `yt-dlp`.
2.  **AI Transcription**: Used Spotify's `basic-pitch` for initial pitch and rhythm detection.
3.  **Data Processing (v3.0)**: 
    - **Quantization**: Rhythms were aligned to standard note durations.
    - **Hand Splitting**: Notes were divided between Treble and Bass staves based on pitch (C4 threshold).
    - **Cleaning**: Deduplication and rest optimization were performed to enhance clarity.
4.  **Score Rendering**: High-quality PDF rendering using LilyPond.

## Disclaimer

This transcription is AI-generated and automatically processed. While version 3.0 provides a much more playable piano score, users are encouraged to perform further manual refinements in a score editor if needed.
