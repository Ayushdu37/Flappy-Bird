<h1>Flappy Bird</h1>

<p>
  A simple Flappy Bird game built using Java and Swing. This project demonstrates basic game development concepts,
  including rendering graphics, handling user input, and managing game logic.
</p>

<h2>Features</h2>
<ul>
  <li><strong>Customizable Game Board</strong>: The game window is set to a width of 360px and a height of 640px.</li>
  <li><strong>Swing Framework</strong>: Utilizes Java Swing for creating the game window and rendering graphics.</li>
  <li><strong>Game Logic</strong>: Includes a <code>FlappyBird</code> class (not shown here) to handle the core game mechanics.</li>
</ul>

<hr>

<h2>🎥 Tutorial Video</h2>
<p>Watch the step-by-step guide on how to set up and play the game:</p>

<a href="https://github.com/Ayushdu37/Flappy-Bird/releases/download/v1.0.0/Flappy.Bird.Tutorial.mp4">
  <img src="https://raw.githubusercontent.com/Ayushdu37/Flappy-Bird/main/src/assets/TutorialThumbnail.png" 
       alt="Watch the Tutorial" width="600">
</a>



<hr>

<h2>How to Run</h2>
<ol>
  <li>Clone the repository:</li>
</ol>
<pre><code>git clone https://github.com/Ayushdu37/Flappy-Bird.git
cd Flappy-Bird
</code></pre>

<ol start="2">
  <li>Compile the Java files:</li>
</ol>
<pre><code>javac -d bin src/*.java
</code></pre>

<ol start="3">
  <li>Run the application:</li>
</ol>
<pre><code>java -cp bin App
</code></pre>

<hr>

<h2>Code Overview</h2>
<p>The main entry point of the application is the <code>App</code> class:</p>

<pre><code class="language-java">
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
</code></pre>

<hr>

<h2>Prerequisites</h2>
<ul>
  <li>Java Development Kit (JDK) 8 or higher</li>
  <li>A Java IDE (e.g., IntelliJ IDEA, Eclipse, or Visual Studio Code) or a terminal for compilation and execution</li>
</ul>

<hr>

<h2>Contributing</h2>
<p>Feel free to fork this repository and submit pull requests for improvements or new features.</p>

<hr>

<h2>License</h2>
<p>This project is licensed under the MIT License. See the <code>LICENSE</code> file for details.</p>

<hr>

<h2>Author</h2>
<p>Developed by <strong>Ayushdu37</strong>.</p>
