# Flappy Bird

A simple Flappy Bird game built using Java and Swing. This project demonstrates basic game development concepts, including rendering graphics, handling user input, and managing game logic.

## Features
- **Customizable Game Board**: The game window is set to a width of 360px and a height of 640px.
- **Swing Framework**: Utilizes Java Swing for creating the game window and rendering graphics.
- **Game Logic**: Includes a `FlappyBird` class (not shown here) to handle the core game mechanics.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/Ayushdu37/Flappy-Bird.git
   cd Flappy-Bird
   ```
2. Compile the Java files:
   ```bash
   javac -d bin src/*.java
   ```
3. Run the application:
   ```bash
   java -cp bin App
   ```

## Code Overview
The main entry point of the application is the `App` class:
```java
public class App {
    public static void main(String[] args) {
        int boardWidth = 360;
        int boardHeight = 640;

        JFrame frame = new JFrame("Flappy Bird");
        frame.setVisible(true);
        frame.setSize(boardWidth, boardHeight);
        frame.setLocationRelativeTo(null);
        frame.setResizable(false);
        frame.setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);

        FlappyBird flappyBird = new FlappyBird();
        frame.add(flappyBird);
        frame.pack();
        flappyBird.requestFocus();
        frame.setVisible(true);
    }
}
```

## Prerequisites
- Java Development Kit (JDK) 8 or higher
- A Java IDE (e.g., IntelliJ IDEA, Eclipse, or Visual Studio Code) or a terminal for compilation and execution

## Contributing
Feel free to fork this repository and submit pull requests for improvements or new features.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

## Author
Developed by **Ayushdu37**.