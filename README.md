# Audio Command Detection System - TriCode

This project is our team's solution for the AAICO February 2024 Voice Processing Challenge. It implements an audio command detection system using Python, focusing on processing streaming audio data to detect specific commands.

## Team Information

- **Team Name:** TriCode
- **Team Members:**
  - <a href= https://www.linkedin.com/in/muflihadawood/> Mufliha Dawood </a>
  - <a href= https://www.linkedin.com/in/swapna-m15/> Swapna Manikandan </a>
  - <a href= https://www.linkedin.com/in/shyamsundarvelmurugan/> Shyam Sundar Velmurugan </a>

## Challenge Overview

The challenge involves processing the 'audio_aaico_challenge.wav' file, simulating real-time streaming. The main tasks are:
- Process audio frames of 512 samples each (16000 Hz sample rate)
- Detect and label commands in the audio stream
- Label samples as 0 (command detected) or 1 (no command)
- Save results for evaluation

## Features

- Simulates real-time audio streaming
- Implements wake word detection and command identification
- Uses multithreading for parallel processing
- Saves detection results in 'results.pkl' for evaluation

## Prerequisites

- Python 3.9
- Required libraries: librosa, numpy

## Installation

1. Clone this repository
2. Install required libraries:
   ```
   pip install librosa numpy
   ```

## Usage

1. Ensure 'test_aaico_challenge.wav' is in the same directory as the script
2. Run the script:
   ```
   python aaico_voice_processing_challenge.py
   ```
3. The script processes the audio file and outputs frame processing times
4. Results are saved in 'results.pkl'

## Solution Approach

Our solution focuses on:
1. Efficient audio frame processing
2. Wake word detection using correlation techniques
3. Command identification for specific keywords (BATTERY, OXYGEN, TEMPERATURE)
4. Optimized multithreaded processing for real-time performance

## Evaluation

Results can be evaluated using the provided Colab notebook:
[AAICO Challenge Evaluation Colab](https://colab.research.google.com/drive/1ekMF1UFfr3djseliJleUNpvzfyIJP57G?usp=sharing)

## Note

This solution was developed specifically for the AAICO February 2024 Voice Processing Challenge and may require adjustments for other applications.

## Acknowledgements

We thank the AAICO team for organizing this challenge and providing the opportunity to work on this exciting project.
