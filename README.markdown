# Memory Sequence Game

## Description
A C++ Builder VCL application where players memorize and repeat a growing sequence of 5 colored buttons, each with unique sounds and images. Score increases with each correct sequence. Features a graphical interface, sound effects, and interactive buttons. Created by Adrian Lesniak.

## Features
- Memorize and repeat sequences of 5 colored buttons
- Increasing sequence length with each round
- Visual feedback with button images
- Audio feedback with unique sounds per button
- Score tracking (number of successful sequences)
- Game over on incorrect sequence
- Start game via label click

## Requirements
- C++ Builder with VCL support
- Windows OS (uses `mmsystem.h` for sound)
- Image files (`img/p1.bmp`, `img/p1a.bmp`, etc.) for buttons
- Sound files (`snd/d1.wav`, `snd/d2.wav`, etc.) for feedback
- Form file (`*.dfm`) and header (`Unit1.h`) for GUI setup

## Installation
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Ensure image (`img/`) and sound (`snd/`) folders are in the project directory.
3. Open the project in C++ Builder.
4. Ensure `Unit1.h` and the associated `.dfm` file are included.
5. Build and run the project.

## Usage
1. Launch the application.
2. Click the label to start the game (plays `start.wav`).
3. Watch and listen to the sequence of button highlights and sounds.
4. Click the buttons in the same order to repeat the sequence.
5. If correct, the sequence extends; if incorrect, game ends with score display.
6. Restart by clicking the label again.

## Notes
- Sequence is randomly generated (1-5) for 1000 steps at startup.
- Requires image files (`p1.bmp` to `p5.bmp`, `p1a.bmp` to `p5a.bmp`) for button states.
- Requires sound files (`d1.wav` to `d5.wav`, `start.wav`, `koniec.wav`) for audio feedback.
- Uses VCL components (`TForm`, `TLabel`, `TImage`) for GUI.
- Button interactions include mouse down/up for visual feedback.

## Author
Adrian Lesniak

## License
MIT License