# Stick Hero - Advanced Programming Project

## Group Members
- **Tejus Madan** (Roll No: 2022540)  
- **Vaibhav Chopra** (Roll No: 2022552)

## Description

This project is a Stick Hero–style platformer game developed using Java. The game incorporates animation, sound effects, and dynamic gameplay mechanics such as character flipping and platform bridging.

### Design Patterns Used

- **Singleton Pattern**  
  Applied to the main character. Only one instance exists throughout the game. Changing the character is handled by switching skins.

- **Factory Pattern**  
  Used for creating sound players through a single `MusicFactory`. The factory creates instances implementing the `GameMusic` interface.

### Features

- **Character Switch Button**  
  Located to the left of the play button. Opens a character switch menu in a pop-up.  
  - Use mouse clicks to toggle characters.  
  - Selected character is highlighted on the right.  
  - Close the pop-up using the red dot at the top-right corner.  
  - Currently, two character skins are available.

- **Animated Sprites**  
  Character animations include:
  - **Idle Animation**: 15 frames  
  - **Running Animation**: 15 frames  
  - Realistic effects like bandanna fluttering and hair movement, created using keyframes.  
  - Animations are subtle due to small character size.

- **Design Detail**  
  A miniature stick hero stands on top of the game title on the home screen.

- **Diamond Collectibles**  
  Diamonds have replaced cherries from the original Stick Hero game.  
  - Used for reviving the player if they fall.  
  - Requires **3 diamonds** to revive.

## How to Play

- **Hold `Spacebar`** to extend the stick as far as needed.
- **Double-press `Down Arrow`** to flip the character.
- **Double-press `Up Arrow`** to flip it back.

## Objective

- Extend the stick to reach the next platform.
- New platforms keep spawning.
- Collect diamonds using the flip mechanic.
- Use **3 diamonds** to revive the character upon falling.

## Sound & Music

- Background music and sound effects are included.
- **Mute Button**:  
  - Toggles background music only.  
  - Visual cue: A cross appears when unmuted and disappears when muted.
- **SFX** continue to play even when background music is muted.

## Additional Details

- **Pause/Home Button**: Acts as both pause and return to home functionality.
- **Diamond Persistence**:  
  - Collected diamonds are saved in a file named `numdiamonds`.
  - Score is session-based, but revives restore the current score if you have enough diamonds.
- **JDK Version Used**: Java Development Kit 21
- **Testing**: 4 JUnit tests have been defined.

## How to Run

### Prerequisites

- Java Development Kit (JDK) version **21**
- A Java IDE (e.g., IntelliJ IDEA, Eclipse) or terminal access
- Project resources (images, sounds) must be in the correct directories as referenced in the code

### Steps

#### Option 1: Run via IDE
1. Clone the repository:
   ```bash
   git clone https://github.com/Vaibhav-Chopra-GT/AP_Project.git

   Open the project folder in your IDE.

Set the JDK version to 21.

Locate the class with the main method (e.g., Main.java).

Right-click and choose Run, or press the run button.

#### Option 2: Run via Command Line
Open terminal and navigate to the project directory.

Compile the Java files:

bash
Copy
Edit
javac -d bin src/*.java
Run the main class (replace Main with actual class name):

bash
Copy
Edit
java -cp bin Main
