# Bouncing Balls Simulation

## Author
Jibin N, MES College Marampally

## Mulearn ID
jibinn@mulearn

---

**Simulation Logic**

This JavaScript code is for a bouncing balls simulation. Let's break down its main components and functionality:

### Ball Class (ball.js)
- Defines a `Ball` class representing a bouncing ball with properties like position, velocity, and radius.
- Handles collision detection and response between balls using elastic collision formulas.

### HorizontalBall and VerticalBall Classes
- Subclasses of the `Ball` class, representing balls with specific movement behavior.
- `HorizontalBall` simulates balls moving horizontally with reflections on vertical walls.
- `VerticalBall` simulates balls moving vertically with reflections on horizontal and vertical walls, considering gravity.

**Main Script (bouncing-balls.js)**

**Constants:**
- Defines constants like frames per second (fps), interval time, dimensions, and properties of balls and aiming.

**Properties for Communication:**
- Variables used for communication between different parts of the script (helpers, events, update, and public functions).

**Helper Functions:**
- `getCanvasDimensions`: Retrieves canvas dimensions and scale ratio.
- `addNewBall`: Adds a new ball to the simulation.

**Drawing Functions:**
- `drawCanvasBorder`: Draws a border around the canvas.
- `drawBall`: Draws a ball on the canvas.
- `drawAim`: Draws an aiming arrow when a new ball is being aimed.

**Event Listeners:**
- Handles mouse and touch events for aiming and adding new balls.

**Update Function:**
- Clears the canvas and draws the canvas border.
- Handles aiming mode, drawing the new ball and aiming arrow.
- Checks collisions between balls if enabled, updates ball positions and velocities, and draws updated balls.

**Public Functions:**
- `init`: Initializes the simulation with a specified canvas and dimensions.
- `clear`: Clears event listeners and stops the simulation.

**Overall Flow:**
1. **Initialization:**
   - Sets up constants, event listeners, and the main update interval.
   - Initializes parameters such as canvas, context, ball type (horizontal or vertical), and an array to store balls.

2. **User Interaction:**
   - Listens for mouse and touch events to control the aiming and creation of new balls.

3. **Simulation Loop:**
   - Continuously updates the canvas by clearing, drawing the canvas border, handling aiming, checking collisions, and updating ball positions.

4. **Cleanup:**
   - Clears event listeners and stops the simulation when needed.

The simulation allows users to aim and shoot balls on the canvas, observing their interactions and collisions based on the defined physics.
