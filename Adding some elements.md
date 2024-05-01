Let's add some basic shapes to represent the cannibals and missionaries for now. Here's how to approach this:

**1. Define Colors**

- In your existing code, add some color definitions for the cannibals and missionaries:
    
    Python
    
    ```
    # ... (Your existing code)
    
    # Colors
    BLACK = (0, 0, 0)
    WHITE = (255, 255, 255)
    RED = (255, 0, 0)  # Color for cannibals
    BLUE = (0, 0, 255)  # Color for missionaries
    ```
    

**2. Draw Cannibals and Missionaries**

- Inside your main game loop (`while running:` block), add code to draw circles for the cannibals and missionaries. You can use `pygame.draw.circle()` for this:
    
    Python
    
    ```
    # ... (Your existing loop code)
    
    # Draw cannibals and missionaries (example positions)
    for i in range(3):  # Draw 3 circles for cannibals (left side)
        pygame.draw.circle(screen, RED, (100 + 40 * i, 100), 20)
    for i in range(3):  # Draw 3 circles for missionaries (left side)
        pygame.draw.circle(screen, BLUE, (100 + 40 * i, 150), 20)
    ```
    
- This code assumes you want the cannibals and missionaries on the left side initially. You can adjust the positions (`(100 + 40 * i, 100)`, etc.) as needed.
    

**3. Update the Display**

- Make sure you call `pygame.display.flip()` after drawing the circles to update the screen:
    
    Python
    
    ```
    # ... (Your drawing code)
    
    pygame.display.flip()
    ```
    

**Run the Code and See the Results!**

Now, when you run your code, you should see a game window with three red circles (cannibals) and three blue circles (missionaries) on the left side.

**Next Steps:**

- We can enhance this further by adding a rectangle to represent the river in the middle of the screen.
- We'll also need to create a way to represent the boat on either side of the river.
- Later, you can explore using image files (sprites) for more visually appealing characters.

Let me know when you're ready to move on to the next step!