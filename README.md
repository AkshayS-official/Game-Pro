# Readme
The pdf is very good so far. However, I would like an editable GDD so that I am able to make comments directly on your document  
Excellent job. Keeping updating as your game evolves
**Game Design Document: Red Ball Redemption**

**Version:** 1.2

**Author:** Akshay Santhosh

**Course:** Game Programming 1

**Inspired by:** Classic 2D side-scrolling ball games ("Red Ball" series).

**1\. Introduction & Overview**

**Red Ball Redemption** is a 2D side-scrolling platformer where the player controls a red ball. The game focuses on physics-based movement, navigating through three distinct levels, each featuring an entry and exit portal, and filled with obstacles, collectibles, and simple puzzle elements. Levels are constructed by the developer using an image-based data format, where specific colours map to game elements. The project aims to be a simple yet engaging experience, achievable by a beginner game developer.

- **Genre:** 2D Physics Platformer, Side-scroller

**2\. Game Concept**

The player guides a red ball through a series of challenges. Each level, beginning at an entry portal and concluding at an exit portal, presents a unique theme and introduces new mechanics. The core gameplay involves rolling, jumping, interacting with physics objects like crates and push able stones, and navigating various environmental hazards and platforms. The ultimate goal is to reach the exit portal of each level.

**3\. Core Mechanics**

- **Player Control (Red Ball):**
  - **Movement:** Left/Right input applies force for rolling.
  - **Jump:** A dedicated input applies an upward force. The ball has inherent bounciness.
  - **Physics:** Implemented using Unity's Rigidbody2D and CircleCollider2D. A default PhysicsMaterial2D will define bounciness.
- **Level Interaction:**
  - The ball interacts with static platforms, moving platforms, rotating elements, push able objects (stones, crates), and hazards.
  - Hazards (water gaps, lava gaps) result in a level reset or returning the player to the level's entry portal.
  - Collectibles (coins) can be gathered.
  - Simple puzzle elements like pushing stones or using keys to open paths.
- **Gameplay Loop:**
  - Player starts at the level's designated Entry Portal.
  - Player navigates the level using rolling and jumping.
  - Player collects coins, avoids hazards, and interacts with level-specific mechanics.
  - Player reaches the Exit Portal to complete the level and proceed to the next.

**4\. Camera**

- Camera will follow the player as the player moves.

**5\. Level Progression (3 Levels)**

Each level will feature a distinct Entry Portal where the player starts and an Exit Portal to be reached.

**Level 1: Forest Glade**

- **Theme:** Bright, grassy outdoor area with a clear sky. (Similar to the provided inspiration image).
- **Map Base:** Unique map image for this level (or the base for Level 2).
- **Elements Introduced:**
  - Standard Platforms
  - Coins
  - Simple Moving Platform (horizontal)
  - Crates (for minor platforming or aesthetic)
  - One-Way Platforms (for varied jump paths)
- **Gameplay Focus:** Basic platforming, introduction to ball movement, jumping, collecting coins, and interacting with a simple moving platform. Low difficulty.
- **Visuals:** Green grassy tiles, dirt tiles, wooden planks for platforms/crates. Bright blue sky background with 2-3 layers of parallax scrolling (distant hills, closer trees/bushes).

**Level 2: Caves & Waterways**

- **Theme:** Dimly lit caves with underground streams and wooden structures.
- **Map Base:** May use the same base image file as Level 1, but with different colour placements/prefab assignments to introduce new obstacles and alter pathways.
- **Elements Introduced:**
  - Rotating Wooden Plank
  - Push able Stone (used to bridge a gap or weigh down a platform)
  - Water Gaps/Hazards
  - Temporary/Crumbling Platforms
  - Key & Door (simple instance: collect a key to remove a single door block)
  - Bouncy Surface (e.g., a large mushroom or bouncy moss)
- **Gameplay Focus:** Introduction to more complex physics interactions. Timing for rotating planks and temporary platforms. Simple puzzle solving with the push able stone and key/door. Navigating water hazards.
- **Visuals:** Cave rock tiles, wooden plank structures, water elements. Darker background with parallax layers (cave walls, stalactites).

**Level 3: Volcanic Depths**

- **Theme:** Hot, volcanic area with lava flows and strange flora. Developer aims to implement this lava theme.
- **Map Base:** Unique map image for this level.
- **Elements Introduced:**
  - Lava Gaps/Hazards (primary hazard)
  - Enemy Plants (static hazards that reset the player on touch)
- **Gameplay Focus:** Increased hazard density. Precision platforming over lava. Navigating around enemy plants. May reuse elements like moving platforms or push able stones in more challenging configurations.
- **Visuals:** Dark volcanic rock, glowing lava, twisted plant sprites. Fiery red/orange background with parallax layers (distant volcanoes, smoke).

**6\. Art Style / Visuals**

- **Overall Style:** Clean, appealing 2D cartoon style, inspired by the "Red Ball" series image. Sprites should be clear and distinct.
- **Player Ball:** A simple, expressive red ball(animation if possible).
- **Tiles & Objects:** Visually distinct to represent their function. Crates should look like wooden crates. Stones should look like stones.
- **Backgrounds:** Each level will have a unique background that supports its theme. Parallax scrolling with 2-3 layers will be implemented to create depth (e.g., distant scenery, mid-ground elements, foreground elements separate from the main tile map gameplay layer).

**7\. Audio**

- **Priority:** Implementation of sound effects, animation and music will be considered a final polish step, to be undertaken if time permits after core gameplay and level mechanics are functional.
- **Potential Animation:** (Initially simple)
  - Player ball might have a subtle roll animation (texture rotation).
  - Coins might rotate or gleam.
  - Moving platforms will animate their movement.
- **Potential Sound Effects (If implemented):**
  - Ball jump/bounce.
  - Ball landing.
  - Coin collection.
  - Player reset (e.g., splash for water, sizzle for lava).
  - Moving platform sounds.
  - Key collection, Door opening.
- **Potential Music (If implemented):** Simple, thematic background music loop for each level.

**8\. Future Prospects (Post-Course / If Time Allows)**

- **Ball Transformation:** Player ball changes material/physics (e.g., to a stone ball with different weight/bounciness).
- **Boss Encounters & Dialogue:** Simple boss character at the end of Level 3 with dialogue at the start and end of the level.
- **Moving Enemies:** Enemy plants or other simple creatures with basic patrol patterns.
- **Advanced Ball Animation:** Squash and stretch on impact, more expressive idle/rolling animations.
- More complex puzzle mechanics.
- Additional levels and themes.
- UI for score, lives, level selection.
