# SnakeGame-UsingDOTMATRIXDISPLAY

A classic Nokia-style Snake Game built using an ESP32-C6 and a 4-in-1 MAX7219 LED Dot Matrix Display.
The snake moves across the LED matrix, eats food to grow longer, and the game restarts when the snake collides with itself.

---

# Features

* Classic Snake Game gameplay
* Real-time movement
* Snake grows after eating food
* Self-collision detection
* Game Over animation
* 4-button directional control
* Smooth gameplay on MAX7219 LED matrix
* ESP32-C6 based embedded gaming project

---

# Hardware Used

| Component                        | Quantity    |
| -------------------------------- | ----------- |
| ESP32-C6 Dev Board               | 1           |
| MAX7219 4-in-1 LED Matrix Module | 1           |
| Push Buttons                     | 4           |
| Breadboard                       | 1           |
| Jumper Wires                     | As required |
| USB Cable / Power Supply         | 1           |

---

# Display Used

* MAX7219 LED Dot Matrix Display
* 4 chained 8x8 matrices
* Total Resolution: 32x8

---

# Button Connections

| Function | ESP32-C6 GPIO |
| -------- | ------------- |
| UP       | GPIO18        |
| DOWN     | GPIO19        |
| LEFT     | GPIO20        |
| RIGHT    | GPIO21        |

Each button:

* One terminal → GPIO pin
* Other terminal → GND

---

# MAX7219 Connections

| MAX7219 Pin | ESP32-C6 Pin |
| ----------- | ------------ |
| VCC         | 5V           |
| GND         | GND          |
| DIN         | GPIO7        |
| CS          | GPIO6        |
| CLK         | GPIO5        |

---

# Libraries Required

Install the following Arduino libraries:

* MD_MAX72XX
* MD_Parola
* SPI (built-in)

Install from:
Arduino IDE → Library Manager

---

# Game Logic

* Snake starts with 3 dots
* Snake continuously moves across the display
* Food appears randomly
* Eating food increases snake length
* If snake head touches its own body:

  * GAME OVER animation is displayed
  * Game restarts automatically

---

# How to Run

1. Open Arduino IDE
2. Install required libraries
3. Select board:

   ```text
   ESP32C6 Dev Module
   ```
4. Connect ESP32-C6 via USB
5. Upload the code
6. Use buttons to control the snake

---

# Controls

| Button | Action     |
| ------ | ---------- |
| UP     | Move Up    |
| DOWN   | Move Down  |
| LEFT   | Move Left  |
| RIGHT  | Move Right |

---

# Future Improvements

* Score display
* Bluetooth control
* Sound effects using buzzer
* Speed increase with score
* OLED score screen
* Multiplayer mode
* Mobile app control

---

# Applications

* Embedded systems learning
* Electronics mini projects
* Game development using microcontrollers
* LED matrix control projects
* Real-time embedded programming

---

# Author

Developed using:

* ESP32-C6
* MAX7219 LED Matrix
* Arduino IDE

Classic Snake Game inspired by old Nokia phone games.
