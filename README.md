
---

# War Scene AR Application - SE4010 Assignment 3 - Mixed Reality

## Introduction
This report outlines the development of an Augmented Reality (AR) application for war scenes, created as part of SE4010 Assignment 3 - Mixed Reality. Using Unity and Vuforia, I designed an immersive AR experience featuring three distinct war scenarios triggered by unique image markers. The scenes depict a battle between three barbarians, a barbarian versus a goblin, and barbarians facing a dragon, set against a rugged mountain terrain with rocks and trees. Creative elements such as combat animations, particle effects, and realistic soundscapes enhance engagement, aligning with the assignment’s objectives.

## Development Process
The development began with setting up Unity 2022.3 LTS and integrating the Vuforia Engine SDK. I obtained a Vuforia License Key from the Developer Portal and configured an AR Camera in the scene. Three image markers were designed using high-contrast war-themed patterns and uploaded to Vuforia’s Target Manager to create the “WarSceneTargets” database. This database was imported into Unity, and corresponding Image Targets were added to the scene.

I sourced 3D models from the Unity Asset Store, including barbarian warriors, a goblin, a dragon, mountain terrain, rocks, and trees. These assets, primarily in .fbx format with high-quality textures, were imported into Unity and positioned as children of their respective Image Targets. The mountain terrain served as a base, with rocks and trees scattered to enhance the battlefield’s realism. Scaling and positioning were adjusted to ensure proper alignment with the markers.

Creative elements were implemented using Unity’s tools. Animations were crafted with the Animation window: barbarians swung axes, the goblin dodged, and the dragon flapped its wings. Particle effects—neutral combat sparks for the barbarian fight, ground mist for the goblin scene, and smoke trails for the dragon—were added using Unity’s Particle System. Sound effects, sourced from Freesound.org (e.g., “battle clash,” “goblin grunt,” “dragon roar”), were integrated with Audio Source components. Interactivity was added via a C# script (`InteractableObject.cs`), allowing users to tap models to speed up animations and increase sound volume.

The scene was enhanced with a rocky ground plane and optimized lighting (Directional Light at 0 5 0, Intensity: 1.2, Ambient Light: 0.3) to highlight the war-torn environment. Testing on a mobile device ensured marker recognition, model display, and creative elements functioned seamlessly.

## Key Features
- **AR Environment Integration**: Utilizes Vuforia’s ARCamera to seamlessly overlay 3D models into the real-world environment, creating a convincing war scene.
- **Interactive Scenarios**: Users can explore dynamic battles—three barbarians clashing, a barbarian versus a goblin, and barbarians facing a dragon—triggered by specific markers.
- **User Interaction**: Tapping models accelerates animations and enhances sound effects, adding an interactive layer to the experience.
- **User-Friendly Interface**: Designed for ease of use with smooth navigation, requiring only marker detection to activate the AR content.
- **Enhanced Realism**: High-quality 3D models from the Unity Asset Store and lifelike animations ensure a realistic portrayal of war movements and appearances.

## Creative Elements
- **Barbarian Fight (Marker 1)**: Three barbarians engage in a fierce melee, with swinging axe animations and combat spark particles illuminating their strikes. A looping “battle clash” sound immerses the user in the chaos. Tapping a barbarian accelerates the combat speed and amplifies the sound.
- **Barbarian vs. Goblin (Marker 2)**: A barbarian swings a sword while a goblin dodges, accompanied by ground mist particles adding an eerie battlefield effect. A “goblin grunt” sound plays continuously. Tapping enhances the dodge animation and sound intensity.
- **Barbarians vs. Dragon (Marker 3)**: Two barbarians thrust spears at a flapping dragon, with smoke trails enhancing the dragon’s presence. A “dragon roar” sound echoes through the scene. Tapping speeds up the spear thrusts and dragon flaps, increasing the roar’s volume.

## Challenges and Solutions
- **Challenge**: Marker tracking was inconsistent with initial low-contrast images.
  - **Solution**: Redesigned markers with sharper, war-themed patterns, improving Vuforia’s recognition to a 4-5 star rating.
- **Challenge**: Animating 3D models was complex due to limited pre-animated assets.
  - **Solution**: Used Unity’s Animation window to manually create combat and flap animations, requiring trial and error to achieve natural movements.
- **Challenge**: Finding relevant sound effects was time-consuming.
  - **Solution**: Explored Freesound.org extensively, testing multiple clips to match the war theme (e.g., selecting “battle clash” over generic clangs).
- **Challenge**: Integrating 3D models with realistic appearances was difficult.
  - **Solution**: Adjusted scales and lighting, and used high-quality textures from the Unity Asset Store to enhance realism.

## Conclusion
This AR app successfully integrates marker-based technology with a war-themed narrative, enhanced by high-quality 3D models and creative effects sourced from the Unity Asset Store. The use of Unity and Vuforia provided a robust platform to meet the assignment’s requirements, offering an engaging and realistic experience within the war scene context.

## Contribution
| Member            | Contribution                                      |
|-------------------|--------------------------------------------------|
| Fernando W.T.R.P. (IT21278280) | Marker 1: Three barbarians fight scene (animations, combat sparks, sound effects, interactivity) |
| Member 2          | Marker 2: Barbarian vs. goblin fight scene (animations, ground mist, sound effects, interactivity) |
| Member 3          | Marker 3: Barbarians vs. dragon fight scene (animations, smoke trails, sound effects, interactivity) |

---
