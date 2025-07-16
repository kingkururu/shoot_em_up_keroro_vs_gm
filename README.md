# Keroro vs. GM 🎮

A 2D space shoot em up game built with C++ and SFML, featuring Keroro battling against Mobile Suit GM.

## GAME PLAY SCREENSHOTS
<img width="1470" alt="Screenshot 2024-09-01 at 7 35 31 PM" src="https://github.com/user-attachments/assets/52520287-4f17-474d-9d34-e3a3b21970fa">
<img width="1470" alt="Screenshot 2024-09-01 at 7 34 05 PM" src="https://github.com/user-attachments/assets/0c98634b-fbdb-4fbe-b5ad-dc8942557dd3">
<img width="1470" alt="Screenshot 2024-09-01 at 7 34 38 PM" src="https://github.com/user-attachments/assets/f87599fd-e5e7-4b35-903a-be09aa12ce03">

## 🎯 Objective
Eliminate all incoming GM robots before they reach your character. Survive as long as possible and aim for the fastest completion time!

## 🎮 How to Play
- **Movement**: Use `WASD` keys to navigate through space
- **Shooting**: Click anywhere on screen to fire bullets toward your mouse cursor
- **Goal**: Destroy all GM enemies before they touch you
- **Restart**: Press `B` after game over to play again

## 🛠️ Technical Features
- **Engine**: SFML (Simple and Fast Multimedia Library)
- **Language**: C++
- **Architecture**: Object-oriented design with modular structure
- **Physics**: Custom AABB collision detection system
- **Memory Management**: Manual memory allocation and cleanup
- **Audio**: Integrated sound effects and background music

## 🎨 Assets
- **Player Sprite**: Keroro character from [Models Resource](https://www.models-resource.com/pc_computer/keroropangpang/model/22953/?source=genre)
- **Enemy Sprites**: RGM-78 GM from Mobile Suit Gundam
- **Audio**: Mobile Suit Gundam OST and sound effects

## 🚀 Building & Running

### Prerequisites
- SFML 2.x library
- C++ compiler (GCC/Clang)
- Make

### Installation

1. **Install SFML**:
   ```bash
   make install
   ```

2. **If the above fails, install via Homebrew (macOS)**:
   ```bash
   # Install Homebrew if not already installed
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   
   # Install SFML
   brew install sfml@2
   ```

3. **Configure PATH (macOS)**:
   - Go to **System Preferences > Security & Privacy > General**
   - Enable "Allow applications downloaded from App Store and identified developers"
   
   - For Zsh users:
     ```bash
     nano ~/.zshrc
     ```
   - For Bash users:
     ```bash
     nano ~/.bash_profile
     ```
   
   Add these lines:
   ```bash
   export PATH="/opt/homebrew/bin:$PATH"
   export PATH="/opt/homebrew/opt/sfml@2/bin:$PATH"
   ```

### Building the Game
```bash
# Clone the repository
git clone https://github.com/kingkururu/shoot_em_up_keroro_vs_gm
cd shoot_em_up_keroro_vs_gm (location will be different)

# Build using make
make

# Run the game
./run
```

## 📁 Project Structure
```
keroro-vs-gm/
├── assets/        # Game assets (sprites, sounds)
├── game/          # Core logics
├── main           # Entry point
├── .gitignore     # Entry point
├── ReadMe         # Entry point
└── Makefile       # Build configuration
```

## 🎯 Key Learning Outcomes
- Game development fundamentals with SFML
- Object-oriented programming in C++
- 2D graphics rendering and sprite management
- Real-time input handling and game loops
- Collision detection algorithms
- Audio system integration
