Create a complete production-quality browser game called "Hill Climb Racer" using only HTML, CSS, and vanilla JavaScript in a SINGLE self-contained file named `index.html`.

The output must be fully playable immediately after opening the file in a browser.

Core Requirements
-----------------
Build a 2D side-scrolling physics-based driving game inspired by Hill Climb Racing.

The game must include:

1. Physics System
- Realistic 2D vehicle physics
- Gravity
- Wheel traction
- Suspension simulation
- Vehicle rotation and angular velocity
- Terrain collision detection
- Smooth movement and stable physics
- Prevent jittering/glitching

2. Vehicle
- Create a car with:
  - Chassis
  - Two wheels
  - Suspension effect
- Wheels should rotate visually
- Vehicle should react naturally to terrain slopes
- Car can flip, jump, land, and crash

3. Terrain
- Infinite procedurally generated terrain
- Smooth hills using noise/spline-based generation
- Terrain should continuously generate as player moves
- Different hill sizes and slopes
- Terrain must render efficiently

4. Camera System
- Smooth side-scrolling camera
- Camera follows vehicle with interpolation/lerp smoothing
- Slight forward offset based on speed
- No camera shaking

5. Controls
Desktop:
- Right Arrow / D → Accelerate
- Left Arrow / A → Brake / Reverse

Mobile:
- On-screen touch buttons for accelerate and brake

6. Fuel System
- Fuel gradually decreases while driving
- Fuel cans spawn across terrain
- Collecting fuel restores fuel
- Fuel bar displayed in HUD

7. Collectibles
- Coins placed naturally on terrain
- Coin collection increases score
- Add pickup animation/effect

8. Score System
- Distance traveled contributes to score
- Coins add bonus score
- High score stored using localStorage

9. Game Over Conditions
Game ends when:
- Fuel reaches zero
- Vehicle crashes badly or flips for too long

After game over:
- Show overlay panel
- Final score
- Distance traveled
- Coins collected
- Restart button

Visual & UX Requirements
------------------------
Create a polished modern arcade-style visual design.

Include:
- Gradient sky background
- Mountains/parallax background layers
- Smooth animations
- Shadows and depth
- Clean HUD/UI
- Speedometer
- Fuel bar
- Score counter
- Distance counter
- Upgrade indicators

Vehicle and terrain should feel visually alive and dynamic.

Audio
-----
Add lightweight generated sound effects using Web Audio API:
- Engine sound
- Coin pickup sound
- Fuel pickup sound
- Crash sound

Do NOT use external audio files.

Upgrade System
--------------
Implement a simple upgrade/shop system:
- Engine power
- Fuel capacity
- Tire grip

Requirements:
- Coins can be spent on upgrades
- Upgrades persist using localStorage
- Upgrade menu accessible from UI

Technical Constraints
---------------------
MANDATORY:
- Single `index.html` file only
- No external libraries/frameworks
- No CDN usage
- No external assets
- Everything must be generated procedurally with code
- Use HTML5 Canvas only
- Responsive design for desktop and mobile
- Maintain good performance

Code Quality
------------
The code must:
- Be clean and modular
- Use classes/modules where appropriate
- Be heavily commented
- Separate logic into sections:
  - Physics
  - Terrain
  - Rendering
  - Audio
  - UI
  - Input
  - Game loop

Performance Requirements
------------------------
- Use requestAnimationFrame
- Optimize rendering
- Avoid memory leaks
- Efficient collision checks
- Cap delta time for stable physics

Game Feel Improvements
----------------------
Add:
- Suspension bounce
- Camera smoothing
- Landing impact effect
- Wheel spin animation
- Speed-based engine pitch
- Particle effects:
  - Dust
  - Coin sparkles
  - Crash debris

Advanced Features
-----------------
Include:
- Pause system
- Day/night cycle
- Procedural scenery objects:
  - Trees
  - Rocks
  - Signs
- Adaptive difficulty:
  - Terrain becomes harder over time

Final Output Requirements
-------------------------
Return ONLY the complete code for `index.html`.

Do not:
- Explain the code
- Add markdown explanations
- Split into multiple files

The generated game should feel polished enough for a YouTube gameplay demo.
