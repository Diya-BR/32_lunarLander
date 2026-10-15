# Lunar Lander Repair Lab

A Lunar Lander-lite game built with **Python and Pygame**, featuring vector-based movement, gravity, thrust, procedural terrain generation, and multi-condition landing validation.

This project was completed as part of the Software Engineering Lab 4 VibeCoding task, using an AI assistant as a debugging and pair-programming partner.

## Features

- **Ship movement and physics:** Rotate the spacecraft, apply thrust, and experience gravity-based movement.
- **Limited fuel:** Fuel consumption is managed during thrust, and thrust stops when fuel runs out.
- **Horizontal screen wrapping:** The spacecraft wraps around the screen horizontally.
- **Procedural terrain:** The game generates terrain containing exactly two landing pads with different score multipliers.
- **Landing validation:** Successful landings require the spacecraft to be on a landing pad, within the permitted horizontal and vertical speed limits, and within the permitted landing angle.
- **Fuel-based ship colour:** The spacecraft's hull colour shifts toward red as the remaining fuel decreases.
- **Landing effect:** A landing effect is triggered when the spacecraft lands successfully.
- **Bonus lives:** The player can earn an extra life upon reaching the configured score threshold.
- **Scoring and levels:** Successful landings award points, while crashes cost a life. The game ends when no lives remain.
- **HUD and telemetry:** Important gameplay information is displayed during play.

## Requirements

- Python 3.10 or newer
- Pygame

## Getting Started

### 1. Install the dependency

```bash
pip install pygame
```

### 2. Run the game

From the project directory, execute:

```bash
python game.py
```

### Controls

| Key | Action |
|---|---|
| Left Arrow | Rotate the spacecraft left |
| Right Arrow | Rotate the spacecraft right |
| Up Arrow | Apply thrust |
| R | Reset the game |
| Space | Continue after landing or crashing |

## Implemented Lab Tasks

### Task 1: Touchdown validation fix

Updated the touchdown validation so that a landing is only successful when the spacecraft meets the horizontal speed, vertical speed, and landing angle requirements while landing on a pad.

### Task 2: Fuel-based ship colour

Implemented `ship_color(fuel_ratio)` to change the spacecraft's hull colour according to its remaining fuel, shifting toward red at low fuel levels.

### Task 3: Landing effect

Implemented `on_landing(score)` to trigger a landing effect when a successful landing awards points.

### Task 4: Bonus life threshold

Implemented `bonus_life_threshold()` to configure the score threshold at which the player can earn additional lives.

## Project Structure

```text
lunar_lander/
├── game.py
└── README.md
```

## Lab Submission

The Lab 4 submission includes:

- A video showing gameplay before the changes.
- A video showing gameplay after the changes.
- A link to the AI assistant conversation containing the complete chat history.

The before-and-after videos and conversation link are submitted through the designated Software Engineering Lab submission repository.

## Technologies Used

- Python
- Pygame
- AI-assisted debugging and pair programming
