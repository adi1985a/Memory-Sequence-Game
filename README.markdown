# 🎮 Memory Sequence Game – C++ VCL Visual Memory Challenge

A fast-paced visual memory game built with **C++ Builder** and **VCL**, where players must recall and repeat a sequence of colored buttons, each with unique sounds and visual states.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Language: C++](https://img.shields.io/badge/Language-C%2B%2B-blue.svg)](https://isocpp.org/)
[![Platform: Windows](https://img.shields.io/badge/Platform-Windows-lightgrey.svg)](https://www.microsoft.com/windows)

---

## 🧠 Description

**Memory Sequence Game** challenges players to focus, memorize, and replicate growing sequences of five colored buttons. Each button features distinct audio and visual feedback, providing an immersive cognitive workout. The game progressively increases in difficulty and tracks your score based on successfully repeated sequences.

Built as a Windows desktop application using C++ Builder and the VCL framework, it features interactive GUI elements, custom graphics, and engaging sound design.

---

## ✨ Features

- 🔢 **Memory Gameplay**: Repeat sequences of 5 unique colored buttons.
- 📈 **Dynamic Difficulty**: Each round adds a new element to the sequence.
- 🖼️ **Visual Feedback**: Buttons change images on press/release.
- 🔊 **Audio Cues**: Each button plays a unique sound.
- 🎯 **Score System**: Tracks the number of successful sequences.
- 💥 **Game Over Logic**: One wrong move ends the session.
- 🎮 **Intuitive Start**: Game begins with a click on the title label.

---

## 🛠️ Requirements

- Windows OS
- **C++ Builder** with VCL support
- `mmsystem.h` for sound functions
- Image assets in `img/`:
  - `p1.bmp` to `p5.bmp`
  - `p1a.bmp` to `p5a.bmp`
- Sound assets in `snd/`:
  - `d1.wav` to `d5.wav`
  - `start.wav`, `koniec.wav`
- GUI Components:
  - `TForm`, `TLabel`, `TImage`
- Project files:
  - `Unit1.h`, `Unit1.cpp`, `Unit1.dfm`

---

## 📦 Installation
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
