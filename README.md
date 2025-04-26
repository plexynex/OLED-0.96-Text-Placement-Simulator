# OLED 0.96" Text Placement Simulator

A web-based simulator for visualizing text placement on a 128×64 OLED display using the Adafruit GFX library standard.

[![Live Demo](https://img.shields.io/badge/demo-live-green.svg)](https://plexynex.github.io/OLED-0.96-Text-Placement-Simulator/)

## Features

- 🖥️ Accurate 128×64 pixel OLED display simulation (scaled for visibility)
- 🎚️ Interactive sliders for X (0-127) and Y (0-63) positioning
- 🔢 Text size selection (1-4) matching Adafruit GFX standards
- 📐 Real-time display of character dimensions:
  - Size 1: 6×8 pixels
  - Size 2: 12×16 pixels
  - Size 3: 18×24 pixels
  - Size 4: 24×32 pixels
- 📝 Text width and height calculation in real-time
- 🔄 Toggle between `print()` and `println()` methods with visual cursor indicator
- ⬇️ Automatic centering tools (horizontal and vertical)
- 💻 Arduino code generator with syntax highlighting
- 📋 One-click copy to clipboard functionality

## Usage

1. Enter your text in the input field
2. Adjust position using sliders or center buttons
3. Select text size (1-4)
4. Choose between `print()` or `println()` method
5. Click "Generate Arduino Code" when ready
6. Copy the generated code to your Arduino project

## Live Demo

Try the simulator directly in your browser:

[👉 https://plexynex.github.io/OLED-0.96-Text-Placement-Simulator/](https://plexynex.github.io/OLED-0.96-Text-Placement-Simulator/)

## Example Output

```arduino
  display.setTextSize(2);
  display.setCursor(20, 24);
  display.println(F("Hello World"));
  display.display();
