# FPGA Pomodoro Timer (Basys 3, VHDL)

A hardware-based Pomodoro Timer implemented on the Basys 3 FPGA board using VHDL.

## Features
- Finite State Machine (IDLE, RUNNING, PAUSED)
- Manual Work/Break toggle
- Automatic mode switching at 00:00
- MM:SS countdown display
- 7-segment display output
- Button-based user control

## Button Controls
| Button | Function |
|--------|----------|
| BTN_C  | Start / Resume |
| BTN_D  | Pause |
| BTN_U  | Reset |
| BTN_L  | Toggle Mode (Work/Break) |

## Switch Mapping
- SW(5:0) → Work time (minutes)
- SW(9:6) → Break time (minutes)

## Hardware
- Board: Basys 3 (Artix-7)
- Language: VHDL
- Clock: 100 MHz

## Architecture
- FSM for control logic
- Countdown datapath for MM:SS
- Clock divider for 1Hz and 1kHz domains

## How It Works
1. Set work/break times using switches
2. Use buttons to control the timer
3. Display shows MM:SS format
4. Timer auto-switches between work and break modes

## Learning Outcomes
- Finite State Machines
- Clock domain handling
- Hardware-based UI
- FPGA design workflow
