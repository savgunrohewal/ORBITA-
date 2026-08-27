# ORBITA✦

### Move the universe.

**ORBITA✦** is an interactive 3D particle experience controlled entirely through hand gestures. Using your webcam and **MediaPipe Hands**, a field of 3,000 particles responds to your movements in real time—moving, rotating, scaling, changing color, charging, and exploding based on your gestures.

## ✦ Features

* **3,000 interactive particles** forming a dynamic 3D sphere
* **Real-time hand tracking** using MediaPipe Hands
* **Single-hand control**

  * Move your hand to move the sphere
  * Change hand position to rotate the particle field
* **Pinch interaction**

  * Pinch and hold to charge the sphere
  * Release to trigger a particle explosion
  * Particles automatically reform afterward
* **Two-hand scaling**

  * Spread your hands apart to grow the sphere
  * Bring your hands together to shrink it
* **Finger-controlled colors**

  * Different finger counts produce different particle colors
* **Webcam background**

  * Toggle the webcam feed into a fullscreen visual background
* **Minimal dark interface**

  * Serif typography
  * Subtle controls
  * Immersive fullscreen experience
* **Single HTML file**

  * No frameworks
  * No build process
  * Everything contained in one file

## 🛠️ Technologies

* **HTML5**
* **CSS3**
* **JavaScript**
* **Three.js** — 3D rendering and particle system
* **MediaPipe Hands** — real-time hand landmark detection
* **WebRTC / getUserMedia** — webcam access

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/your-username/orbita.git
cd orbita
```

### 2. Open the project

The project is intentionally built as a single HTML file:

```text
orbita/
└── index.html
```

### 3. Run it using the deployed link

https://orbiita.netlify.app/

### 4. Allow camera access

When your browser asks for camera permission, select **Allow**.

Place your hand in front of the camera and interact with the particle field.

## 🖐️ Gesture Controls

| Gesture               | Interaction                |
| --------------------- | -------------------------- |
| 👋 One hand           | Move and rotate the sphere |
| 🤏 Pinch + hold       | Charge the sphere          |
| ✋ Release pinch       | Explode the particles      |
| 👐 Two hands apart    | Increase sphere size       |
| 🤲 Two hands together | Decrease sphere size       |
| ☝️ Finger count       | Change particle color      |
| 📷 Camera button      | Toggle webcam background   |

## 🎨 Color System

The number of detected fingers determines the particle field's hue.

```text
0 fingers → Blue
1 finger  → Pink
2 fingers → Amber
3 fingers → Green
4 fingers → Purple
5 fingers → Red
```

With two hands, the detected finger counts are combined to influence the color.

## ⚡ How It Works

ORBÏTA combines **computer vision** with **WebGL particle rendering**.

```text
Webcam
   ↓
MediaPipe Hands
   ↓
Hand Landmarks
   ↓
Gesture Detection
   ↓
Interaction State
   ↓
Three.js Particle System
   ↓
Real-time Visual Response
```

MediaPipe identifies hand landmarks such as the wrist, fingertips, and finger joints. JavaScript converts those landmarks into interaction values such as:

* Position
* Rotation
* Pinch distance
* Finger count
* Distance between two hands

Those values are then applied to the Three.js particle system.

## 💥 Particle Explosion

When a pinch is released, each particle receives an outward velocity based on its position relative to the sphere.

The particles disperse across the screen and gradually lose velocity while being pulled back toward their original positions.

This creates the effect of:

```text
Sphere
   ↓
Pinch
   ↓
Charge
   ↓
Release
   ↓
EXPLOSION
   ↓
Particles disperse
   ↓
Particles reform
   ↓
Sphere
```

## 📁 Project Structure

The entire experience lives inside one file:

```text
orbita/
└── index.html
```

The HTML file contains:

* UI
* Styling
* Three.js scene
* Particle generation
* Particle physics
* MediaPipe configuration
* Webcam handling
* Gesture recognition
* Animation loop

## 🌐 Browser Compatibility

ORBITA✦ works best in modern browsers that support:

* WebGL
* WebRTC
* ES6 JavaScript
* Webcam access

Recommended:

* Google Chrome
* Microsoft Edge
* Safari
* Firefox

A device with a working webcam is required for gesture interaction.

## 🔐 Privacy

ORBITA✦ uses the browser's webcam API for real-time hand tracking.

The camera feed is processed locally by the browser and is not intentionally uploaded to a server by the application.

Camera permission can be revoked through your browser settings at any time.




---

<div align="center">

### **ORBITA**

**Gesture meets matter.**

*An interactive experiment in motion, vision, and digital matter.*

</div>
