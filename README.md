# Stack Project

Digital logic implementation of a Tetris-like stacking game built with LogicCircuit. The project simulates a complete game system using fundamental logic components such as flip-flops, registers, adders, counters, multiplexers, demultiplexers, collision validators, row management circuits, and display modules.

## Overview

Stack Project is an educational digital logic project that recreates the core mechanics of a falling-block puzzle game without using a traditional programming language. Instead, the full game behavior is modeled through interconnected logic circuits.

The simulation includes player input, piece movement, board state storage, collision detection, row clearing, combo counting, scoring, victory/defeat control, timing management, and visual output through a matrix display and 7-segment displays.

The project was designed in LogicCircuit and is stored as a single `.CircuitProject` file containing a hierarchical architecture of reusable digital components.

## Key Features

* Tetris-like game implemented with digital logic circuits
* Hierarchical circuit design using LogicCircuit
* Top-level `GAME` circuit as the main simulation entry point
* Central `SISTEMA` circuit for game logic coordination
* Player input handling through digital control signals
* Piece movement and position tracking
* Boundary and collision detection
* Row and mask management
* Row clearing and line-cut logic
* Combo counter and scoring system
* Victory and defeat state control
* Clock and frequency management
* LED matrix-based game visualization
* 7-segment display pipeline for numeric output
* Modular use of flip-flops, registers, adders, counters, multiplexers, and demultiplexers

## Tech Stack

* LogicCircuit
* Digital Logic
* Flip-Flops
* Registers
* Adders
* Counters
* Multiplexers
* Demultiplexers
* LED Matrix
* 7-Segment Displays
* XML Circuit Project

## Architecture

The project follows a hierarchical digital circuit architecture. The game is organized from low-level logic primitives to high-level game control circuits.

### Top-Level Circuit

The `GAME` circuit acts as the main entry point of the simulation. It contains the visible game interface, input controls, LED matrix, and 7-segment displays.

### Core System

The `SISTEMA` circuit works as the central controller of the game. It coordinates the main logic modules, including movement validation, board state updates, row clearing, scoring, and game state control.

### Sequential Logic

Flip-flops and registers are used to store important game state information, such as current piece position, active masks, used rows, counters, and state flags.

### Arithmetic and Routing

Adders, counters, multiplexers, and demultiplexers are used to calculate positions, route signals, select rows or columns, and manage data movement across the circuit.

### Game Logic Subsystems

The game logic is divided into multiple subsystems:

* **Row and Mask Management:** Tracks the occupied grid spaces and active piece shapes.
* **Boundary and Collision Detection:** Prevents invalid movement outside the board or into existing blocks.
* **Row Clearing Logic:** Detects completed rows and updates the board state.
* **Combo and Scoring:** Tracks successful placements and updates the score.
* **Game State Control:** Handles timing, victory conditions, defeat conditions, and game progression.

### Display System

The display system translates internal game state into visual output.

It includes:

* A matrix display for the main game board
* A decorative handheld-console style frame
* 7-segment displays for numeric information such as score or level
* Signal mapping circuits that connect game state with visual output

## Getting Started

### Requirements

* LogicCircuit software
* The `StackProject.CircuitProject` file

### Running the Simulation

1. Open LogicCircuit.
2. Go to `File > Open`.
3. Select the `StackProject.CircuitProject` file.
4. Open the `GAME` circuit.
5. Run the simulation using the LogicCircuit clock.

The project is designed to run with a default simulation frequency of 50 Hz.

## Project Purpose

This project was created to practice digital logic design by building a complete interactive game without using conventional software code.

It demonstrates understanding of computer architecture, sequential logic, combinational logic, timing control, data routing, state management, arithmetic circuits, display pipelines, and modular circuit design.

Stack Project highlights how complex behavior can be created from basic hardware-level logic components.
