# Java CLI UNO Game

Welcome to the **UNO Game** repository! This project is a complete, console-based implementation of the classic UNO card game written in Java. It features robust game logic, support for multiple players, and the ability to play against automated bots.

## 🚀 Features

- **Multiplayer Support**: Play with 1 to 10 players.
- **Bot Opponents**: Choose to play against AI bots or with friends in a hot-seat local multiplayer mode.
- **Complete Deck Rules**: Includes all standard UNO cards:
  - 🔢 Number cards (0-9)
  - ⏭️ Skip cards
  - 🔄 Reverse cards
  - ➕ Draw Two (+2) cards
  - 🌈 Wild cards
  - 💥 Wild Draw Four (+4) cards
- **Game Mechanics**: Enforces standard rules for color/number matching, turn directions, drawing penalties, and declaring "UNO!".
- **Dynamic Deck Management**: Automatically reshuffles the discard pile back into the deck when cards run out.

## 🛠️ Technology Stack

- **Language**: Java
- **UI**: Command-Line Interface (CLI)
- **Architecture**: Object-Oriented Design (Classes for `Card`, `Player`, `Game`, `deckliste`, etc.)

## ⚙️ Installation & Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Urfavcurlygirl/UNO-game.git
   cd UNO-game
   ```

2. **Compile the Java files:**
   Ensure you have the Java Development Kit (JDK) installed on your system. Compile all the source files in the project folder:
   ```bash
   javac *.java
   ```

## 💻 Usage

To start the game, run the `Main` class:
```bash
java Main
```

### How to Play:
1. **Setup**: When prompted, enter the number of players (between 1 and 10).
2. **Game Mode**: You will be asked if you want to play with bots (`oui`/`non`).
   - If `oui` (yes), you will play as "Joueur 1" against the specified number of bots.
   - If `non` (no), you can enter the names for all human players.
3. **During your turn**: 
   - Your current hand will be displayed.
   - Enter the **index** of the card you want to play (starting from 0).
   - If you don't have a playable card, enter `-1` to draw a card from the deck.
4. **Winning**: Be the first player to get rid of all your cards to win the game! (The game automatically shouts "UNOOOOOOOOOOOOOOO" when you have one card left).

## 📁 Repository Structure

- `main.java` & `Game.java`: Core game loop and turn management.
- `Player.java`: Manages player hands, drawing, and playing cards.
- `deckliste.java`: Initializes and manages the draw pile, including shuffling.
- `Card.java` & `CardEffect.java`: Abstract base classes and interfaces for card logic.
- **Card Implementations**: 
  - `NumberCard.java`
  - `SkipCard.java`
  - `ReverseCard.java`
  - `DrawTwoCard.java`
  - `WildCard.java`
  - `WildDrawFourCard.java`

## 🤝 Contributing
Feel free to fork this project, submit pull requests, or open issues to suggest improvements or bug fixes.