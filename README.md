# Keroro vs. GM 

A 2D space shoot em up game built with C++ and SFML, featuring Keroro battling against Mobile Suit GM.

## GAME PLAY SCREENSHOTS
<img width="999" height="822" alt="Image" src="https://github.com/user-attachments/assets/6510405a-2d3a-41be-aca7-0bd46a0fb7db" />
<img width="1041" height="841" alt="Image" src="https://github.com/user-attachments/assets/1265438f-e317-4237-ba97-195b1cf7dc67" />
<img width="1052" height="842" alt="Image" src="https://github.com/user-attachments/assets/3be1dd09-1a37-4cc8-91fd-eed8d26d7ea0" />

## Objective
Eliminate all incoming GM robots before they reach your character. Survive as long as possible and aim for the fastest completion time!

## How to Play
- **Movement**: Use `WASD` keys to navigate through space
- **Shooting**: Click anywhere on screen to fire bullets toward your mouse cursor
- **Goal**: Destroy all GM enemies before they touch you

## Technical Features
- **Architecture**: Object-oriented design with modular structure
- **Physics**: Custom AABB collision detection system
- **Memory Management**: Manual memory allocation and cleanup
- **Audio**: Integrated sound effects and background music provided by SFML

## Assets
- **Player Sprite**: Keroro character from [Models Resource](https://www.models-resource.com/pc_computer/keroropangpang/model/22953/?source=genre)
- **Enemy Sprites**: RGM-78 GM from Mobile Suit Gundam
- **Audio**: Mobile Suit Gundam OST and sound effects from freesound.org

## Building & Running

### Prerequisites
- SFML 2.x library
- C++ compiler (GCC/Clang)
- Make

### Installation

1. **Install SFML and install via Homebrew (macOS)**:
   ```bash
   # Install Homebrew if not already installed
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   
   # Install SFML if there is trouble
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

## Project Structure
```
keroro-vs-gm/
├── assets/        # Game assets 
├── game/          # Core logics
├── main           # Entry point
├── .gitignore     
├── ReadMe         
└── Makefile       # Build configuration
```

## Key Learning Outcomes
- Game development fundamentals with SFML
- Object-oriented programming in C++
- 2D graphics rendering and sprite management
- Real-time input handling and game loops
- Collision detection algorithms
- Audio system integration
