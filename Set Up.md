**1. Install Pygame**

- Open your command prompt or terminal.
- Type the following command and press Enter:
    
    Bash
    
    ```
    pip install pygame
    ```
    

**2. Create a New Python File**

- Open your favorite text editor or IDE (like VS Code, IDLE, etc.).
- Create a new Python Project and name it something like "Canibal_Game".

**3. Basic Pygame Setup**

- Paste the following code into your new Python file:
    
    Python
    
    ```
    import pygame
    
    # Initialize Pygame
    pygame.init()
    
    # Game Constants
    SCREEN_WIDTH = 800
    SCREEN_HEIGHT = 600
    BLACK = (0, 0, 0)
    WHITE = (255, 255, 255)
    
    # Set up the display window
    screen = pygame.display.set_mode((SCREEN_WIDTH, SCREEN_HEIGHT))
    pygame.display.set_caption("Cannibals and Missionaries")
    ```
    

**Explanation**

- `import pygame`: Imports the necessary Pygame module.
- `pygame.init()`: Initializes all the Pygame modules you'll be using.
- `SCREEN_WIDTH`, `SCREEN_HEIGHT`: Define the dimensions of your game window.
- `BLACK`, `WHITE`: Define colors for convenience.
- `screen = pygame.display.set_mode(...)`: Creates the main display window.
- `pygame.display.set_caption(...)`: Sets the title of your game window.

**4. Run the code**

- Save the Python file.
- From your terminal or command prompt, navigate to the directory where you saved the file.
- Run the file using: `python cannibals_missionaries.py`

You should now see a blank black window titled "Cannibals and Missionaries"!

You'll notice that the window closes up immediately and that inroduces up to the loop game concept !

**Game loop**
your program at this stage finishes executing and doesn't have anything to keep the window open.
Let's fix that by adding a game loop to keep the window active until the player closes it.
**Here's how to add a basic game loop:**

```Python
# ... (Your existing setup code)

# Main game loop
running = True
while running:
    # Handle events
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            running = False

    # Clear the screen (fill with white)
    screen.fill(WHITE)

    # Update the display
    pygame.display.flip()

# Quit Pygame
pygame.quit()    ```

### Let's add some elements now ! 