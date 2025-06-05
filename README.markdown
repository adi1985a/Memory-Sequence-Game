# 🧠💡 Memory Spark: The Sequence Challenge 🎮
_A classic memory game built with C++ Builder VCL, testing your recall with colors, sounds, and images!_

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![C++ Builder](https://img.shields.io/badge/Framework-C%2B%2B%20Builder%20VCL-orange.svg)](https://www.embarcadero.com/products/cbuilder)
[![Platform: Windows](https://img.shields.io/badge/Platform-Windows-lightgrey.svg)](https://www.microsoft.com/windows)

## 📝 Project Description

**Memory Spark: The Sequence Challenge** is an engaging VCL application developed in C++ Builder, designed to put your memory to the test! Players are tasked with memorizing and correctly repeating an ever-lengthening sequence of five colored buttons. Each button features a unique image and an associated sound, engaging both visual and auditory senses. For every correctly repeated sequence, the player earns points. The game boasts an intuitive graphical interface, dynamic sound effects, and interactive buttons, ensuring a satisfying gameplay experience.

![Demo GIF](screenshots/1.gif)


## ✨ Key Features

*   🧠 **Memory Training**: Memorize and replicate sequences of five unique, colored buttons.
*   📈 **Increasing Difficulty**: The length of the sequence to remember grows after each successfully completed round.
*   🎨 **Visual Feedback**: Each button has dedicated images for its active and inactive states.
*   🔊 **Audio Feedback**: Unique sound effects for each button aid in memorizing the sequence.
*   🏆 **Score Tracking**: The number of correctly replicated sequences is tallied as the player's score.
*   🛑 **Game Over Condition**: Incorrectly reproducing the sequence ends the game, displaying the achieved score.
*   ▶️ **Easy Start**: Begin a new game by clicking the start label.
*   🎲 **Random Sequences**: The game generates a long, random sequence at startup, ensuring variety in every playthrough.

## 🖼️ Screenshots

_Showcasing the interface and gameplay._

<p align="center">
  <img src="screenshots\1.jpg" width="300"/>
  <img src="screenshots\3.jpg" width="300"/>
  <img src="screenshots\4.jpg" width="300"/>
  <img src="screenshots\5.jpg" width="300"/>
</p>

## ⚙️ System Requirements & Assets

### Software:
*   **Development Environment**: Embarcadero C++ Builder (with VCL support).
*   **Operating System**: Windows (the game utilizes `mmsystem.h` for sound playback).

### Assets:
*   **Button Images**: Required `.bmp` files located in the `img/` folder in the project's root directory:
    *   Inactive state: `p1.bmp`, `p2.bmp`, `p3.bmp`, `p4.bmp`, `p5.bmp`
    *   Active (highlighted) state: `p1a.bmp`, `p2a.bmp`, `p3a.bmp`, `p4a.bmp`, `p5a.bmp`
*   **Sound Files**: Required `.wav` files located in the `snd/` folder in the project's root directory:
    *   Button sounds: `d1.wav`, `d2.wav`, `d3.wav`, `d4.wav`, `d5.wav`
    *   Game start sound: `start.wav`
    *   Game over sound: `koniec.wav`
*   **C++ Builder Project Files**:
    *   Form definition file (`*.dfm`, e.g., `Unit1.dfm`)
    *   Form header file (`Unit1.h`)
    *   Main project file (`*.cbproj`)

## 🛠️ Installation and Running

1.  **Clone the Repository**:
    ```bash
    git clone <repository-url>
    ```
    (Replace `<repository-url>` with your repository's URL)
2.  **Folder Structure**: Ensure the `img/` (with `.bmp` images) and `snd/` (with `.wav` files) folders are present in the root directory of the cloned project, at the same level as the C++ Builder project files.
3.  **Open the Project**: Open the project file (`*.cbproj`) in the Embarcadero C++ Builder IDE.
4.  **Verify Components**: Make sure that `Unit1.h` and its associated `.dfm` form file are correctly included and recognized by the project. VCL components (TForm, TLabel, TImage, etc.) should be defined in these files.
5.  **Build and Run**: Build the project and then run it from within C++ Builder.

## ▶️ How to Play

1.  Launch the application after a successful compilation.
2.  To start the game, click on the start label. The `start.wav` sound will play.
3.  Carefully watch and listen to the sequence of button highlights and their accompanying sounds.
4.  After the game finishes presenting the sequence, your task is to click the buttons in the exact same order.
5.  **Correct Sequence**: Congratulations! Your score increases, and the game will present a new, longer sequence.
6.  **Incorrect Sequence**: Game Over! The `koniec.wav` sound will play, and your final score will be displayed on the screen.
7.  To play again, click the start label.

## 💡 Game Mechanics & Technical Details

*   **Sequence Generation**: On the first game launch (or after a restart), a long (e.g., 1000 steps) random sequence of button numbers (1 to 5) is generated. The game then plays successive segments of this pre-generated sequence.
*   **Button Interaction**: The game uses `OnMouseDown` and `OnMouseUp` events for `TImage` components (representing the buttons) to change their appearance (loading `*a.bmp` and `*.bmp` images) and play sounds.
*   **VCL Components**: The user interface is built using standard VCL components such as `TForm`, `TLabel` (for start/score display), and `TImage` (for interactive buttons).

## 🤝 Contributing

Contributions to **Memory Spark** are welcome! If you have ideas for improvements, new features, or bug fixes:

1.  Fork the repository.
2.  Create a new branch for your changes: `git checkout -b feature/your-amazing-feature`
3.  Make your modifications and commit them: `git commit -m "Add: Your amazing feature"`
4.  Push your changes to your branch: `git push origin feature/your-amazing-feature`
5.  Open a Pull Request.

Please ensure your code adheres to the existing style and includes comments where necessary.

## ✍️ Author

**Adrian Lesniak**
_C++ Builder Developer & Game Enthusiast_


## 📃 License

This project is licensed under the **MIT License**.
The full text of the license is available at: [https://opensource.org/licenses/MIT](https://opensource.org/licenses/MIT)

---
🚀 _Test the limits of your memory and have fun!_
