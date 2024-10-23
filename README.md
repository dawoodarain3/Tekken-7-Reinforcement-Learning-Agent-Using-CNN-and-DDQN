# Tekken-7-Reinforcement-Learning-Agent-Using-CNN-and-DDQN

## Overview
The **RL Agent for Tekken 7** is a reinforcement learning-based bot designed to autonomously play the game Tekken 7. This project addresses challenges in the gaming industry, such as the limited ability of computer-controlled opponents to provide realistic, skill-enhancing gameplay. By leveraging reinforcement learning, the bot learns, adapts, and improves over time, offering players a more competitive experience. 

Additionally, the project incorporates **REM4P** to ensure platform compatibility, enabling smooth communication between the bot and the game console.

---

## Project Brief
The Tekken 7 RL Agent serves as an autonomous bot capable of playing the game without human intervention. It employs **Double Deep Q Networks (DDQN)** and **Prioritized Experience Replay (PER)**, learning and improving from in-game visual data in real-time. With the ability to adopt strategies, practice moves, and defend against attacks, the bot offers an innovative solution to enhance player experiences through AI-driven gameplay.

---

## Relevance to Course Modules
The project reflects core concepts from AI and ML courses by:
- Implementing **reinforcement learning** for gameplay optimization.
- Applying **object-oriented design patterns** for robust software development.
- Using **real-time data extraction techniques** for decision-making.
It bridges the gap between theoretical learning and practical implementation, contributing to advancements in both gaming and AI.

---

## Project Background
Tekken 7, a popular 3D fighting game, presents complex gameplay mechanics that require skillful control. Developing an AI agent for Tekken 7 involves:
- Understanding and analyzing game states.
- Making intelligent decisions based on real-time data.
- Executing precise actions seamlessly.

The bot utilizes advanced libraries and tools:
- **PIL** to extract critical information (e.g., health bars, character positions).
- **MSS** for capturing screen actions and health data.
- **OpenCV** to interpret in-game animations and interactions.
  
These tools collectively power the bot’s ability to make strategic decisions based on visual input.

---

## Literature Review & Analysis
Reinforcement learning has shown remarkable success across games like **Go, Chess, Atari, and StarCraft II**, with RL agents often outperforming human players. Despite these successes, challenges remain in understanding agent behavior. This project extends existing research by developing an RL agent specifically tailored for Tekken 7’s dynamic and complex environment.

The Tekken 7 bot’s learning process aligns with current trends in game AI and RL. It leverages **real-time data extraction** with PIL, MSS, and OpenCV to support effective decision-making, pushing the boundaries of what RL agents can achieve in fighting games.

---

## Methodology & Software Lifecycle
The project follows the **Agile (Scrum)** Software Development Life Cycle (SDLC), ensuring:
- **Incremental development:** Features are built and tested iteratively.
- **Continuous integration & delivery:** Code remains production-ready throughout development.
- **Adaptability:** Agile principles support evolving project needs and rapid improvements.

### Rationale for Agile
The dynamic nature of AI development requires flexibility. Agile methodology enables:
- Frequent testing and feedback loops.
- Smooth adaptation to new challenges or requirements.
- Continuous improvements through retrospectives.

---

## Problem Definition
### Problem Statement
Current Tekken 7 bots lack the sophistication required to provide ongoing challenges for players. The project aims to develop a **visually-driven RL bot** using **DDQN with PER** to offer realistic, challenging gameplay. The bot simulates human-like behavior, learning from visual input alone, enabling players to improve without needing to play online.

---

## Deliverables & Development Requirements
### Key Modules
1. **Data Extraction Module:**  
   Captures game data in real-time using PIL, MSS, and OpenCV.  
   Extracted information includes character positions, health bars, and motion animations.
   
2. **Reinforcement Learning Module:**  
   Trains the bot using RL algorithms to optimize decisions based on game states.  
   Uses **trial-and-error learning** to refine strategies over time.

3. **Action Execution Module:**  
   Uses **REM4P** to bridge communication between the bot and the PS4 console, enabling in-game actions.

4. **Coordination Module:**  
   Ensures smooth interaction between the other modules and manages overall state synchronization.

---

## Use Case Analysis
The following use cases describe the key behaviors and interactions of the Tekken 7 AI bot.

### Use Case 1: Play Tekken 7  
| **Use Case ID** | UC-1 |
|-----------------|------|
| **Actors** | Primary: AI Bot, Secondary: Tekken 7 Game |
| **Trigger** | The game starts. |
| **Preconditions** | The AI bot and the game are running. |
| **Postconditions** | The game ends with a win or loss. |

**Normal Flow:**
1. The bot starts the game.
2. It observes the game state and makes a decision.
3. The bot executes the chosen action.
4. The game state updates, and the bot repeats the process until the game ends.

**Alternative Flows:**
- The bot may win or lose the game.
- Errors may occur, such as game or bot crashes.

---

### Use Case 2: Training  
| **Use Case ID** | UC-2 |
|-----------------|------|
| **Actors** | Primary: AI Bot |
| **Trigger** | The bot is instructed to train. |
| **Preconditions** | The bot is running. |
| **Postconditions** | The bot improves based on training results. |

**Normal Flow:**
1. The bot loads and analyzes previous game states.
2. It identifies patterns and updates its internal model.
3. Training continues iteratively to refine the bot’s strategies.

---

### Use Case 3: Compete Against Players  
| **Use Case ID** | UC-3 |
|-----------------|------|
| **Actors** | Primary: AI Bot, Secondary: Players |
| **Trigger** | The bot is instructed to play against a player. |
| **Preconditions** | Both the player and bot are running the game. |
| **Postconditions** | The bot either wins or loses the match. |

**Normal Flow:**
1. The bot competes against a human player.
2. It updates its model based on the match outcome.
3. Matches continue to help the bot adapt and improve.

---

## Functional Requirements
### FR-1: Start Game  
- **Requirement:** The bot shall start a Tekken 7 game.  
- **Priority:** High

### FR-2: Make Decisions  
- **Requirement:** The bot shall make decisions based on its perception of the game state.  
- **Priority:** High

### FR-3: Execute Decisions and Update Model  
- **Requirement:** The bot shall execute decisions and update its internal model to enhance gameplay.  
- **Priority:** High

---

## Conclusion
The **Tekken 7 RL Agent** combines cutting-edge technologies to deliver an AI-powered gaming experience. It provides:
- A platform for skill enhancement without online play.
- A challenging alternative to traditional game bots.
- A significant contribution to research in AI and reinforcement learning.

This project demonstrates the practical application of AI in gaming, opening new avenues for RL in complex gaming environments.
