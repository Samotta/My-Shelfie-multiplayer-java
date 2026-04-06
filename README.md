# My Shelfie – Multiplayer Java Version

## Project Overview
"My Shelfie" is a digital multiplayer adaptation of the board game [*My Shelfie*](https://www.craniocreations.it/en/product/my-shelfie) for 2–4 players, implemented in Java with both GUI and CLI interfaces.
This public repository is a showcase of the project and my contributions as part of a team.

> **Note:** The login system automatically creates an account on first access. 
> Credentials are stored in plaintext, as authentication security was out of scope for this project.

## My Contributions
- Designed and implemented the full GUI interface (JavaFX)
- Implemented Socket-based multiplayer networking with resilience to disconnections
- Developed chat functionality
- Added support for multiple concurrent games
- Assisted in implementing complete game rules and logic

## Features
### Advanced Features
- Multiple concurrent games (Lobbies)
- Chat functionality with private and public mode
- Robustness to player disconnections
- Full implementation of the original game rules
- GUI interface
- CLI interface (with ANSI support)

## Screenshots

### Login
<img width="2558" height="1391" alt="Screenshot 2026-04-06 161804" src="https://github.com/user-attachments/assets/43873a52-3f0c-4b77-8d54-c5f1f39c3f34" />

*CLI (left) and GUI (right) login screens*

### Lobby
<img width="2558" height="1391" alt="Screenshot 2026-04-06 161804" src="https://github.com/user-attachments/assets/935d54f9-d9fc-4596-85f9-a85bf576d18e" />

*Create or join a lobby from both interfaces*

### Waiting Room
<img width="2556" height="1391" alt="Screenshot 2026-04-06 161829" src="https://github.com/user-attachments/assets/38edc90c-2675-47d9-a07b-2654916b4767" />

*Lobby waiting room with live chat*

### Gameplay
<img width="1918" height="1100" alt="Screenshot 2026-04-06 162035" src="https://github.com/user-attachments/assets/1b09b174-35e3-4501-b6df-926bba0dd0c1" />

*GUI: early game view*

<img width="1920" height="1104" alt="Screenshot 2026-04-06 162720" src="https://github.com/user-attachments/assets/a213b2bb-cd35-4a95-8558-87b15056b5b3" />


*GUI: mid game with shelves filling up*

<img width="2558" height="1390" alt="Screenshot 2026-04-06 162054" src="https://github.com/user-attachments/assets/82af8175-c133-40e9-821b-be43a4ed6ba4" />

*CLI: main board view*

<img width="2557" height="1392" alt="Screenshot 2026-04-06 162211" src="https://github.com/user-attachments/assets/36d1d7c4-0c6e-43a6-98bb-11f6e5b01c32" />

*CLI: goal cards view*

## Technologies
- JavaFX for GUI
- Java Socket programming for multiplayer
- Java RMI for multiplayer
- Socket and RMI are interchangeable: a single game session can host players using different protocols simultaneously

## How to Run
> **Note:** If you cannot download the JAR files directly from GitHub, clone the repository instead.

1. Navigate to the directory containing the JAR file.
```bash
cd deliverables/final/jar
```
2. Execute `chcp 65001` in terminal (Windows only) to handle UTF-8 encoding.
> **Note:** Windows 10 CMD does not support ANSI color codes, so the CLI may not display correctly. Use Windows 11 Terminal or a Linux terminal for the best experience.

3. Run the game:
```bash
java -jar server.jar
java -jar client.jar
```
