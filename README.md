Ashik Gesture Engine v4.0: Ultra Bright
An interactive, web-based 3D model viewer designed for high-fidelity car visualization (optimized for the GT-R). This engine uses MediaPipe Hand Landmarker for gesture-based interaction and Three.js for a cinematic rendering experience.

Features
Hand-Gesture Rotation: Control the rotation of your 3D model in real-time by moving your hand across the webcam's field of view.

Dynamic Pinch-to-Zoom: A custom "Pinch" gesture detection (distance between thumb and index finger) triggers a cinematic camera zoom.

Ultra Bright Lighting: Enhanced with ACESFilmicToneMapping and high-intensity Directional/Hemisphere lights for a "Studio Look."

Auto-Normalization: Automatically scales and centers any uploaded .glb or .gltf model to fit the viewport perfectly.

Cyberpunk UI: A sleek, neon-themed interface with real-time status updates.

Tech Stack
Three.js: Core 3D engine for rendering and lighting.

MediaPipe Vision: AI-powered hand tracking and landmark detection.

JavaScript (ESM): Modern module-based architecture.

HTML5/CSS3: Custom stylized HUD and responsive canvas.

How to Use
Open the Application: Launch the index.html in any modern web browser (Chrome or Edge recommended for best WebGL performance).

Allow Camera Access: The engine requires webcam access to track your gestures.

Upload Your Model: Click the "SELECT YOUR GT-R (.GLB)" button to load your 3D car model.

Interact:

Rotate: Move your hand left or right to spin the car.

Zoom: Close the gap between your thumb (Landmark 4) and index finger (Landmark 8) to zoom in for a close-up.

Customization
If you want to adjust the "Ultra Bright" settings, look for the cinematic lighting section in the <script>:

JavaScript

// Increase/Decrease the exposure for different lighting environments
renderer.toneMappingExposure = 1.5; 

// Change the light intensity
const sunLight = new THREE.DirectionalLight(0xffffff, 5);
License
Designed and developed by Ashik. For personal and experimental use.
