# 🌌 Project Visual-Art: Real-Time Computer Vision & Volumetric Procedural Particle Engine

An browser-based interactive computer vision suite that maps real-time hand-tracking telemetry into high-density volumetric 3D particle systems. Inspired by advanced TouchDesigner workflows, this engine combines mathematical procedural modeling with client-side WebGL shaders and computer vision algorithms.

---

## 🏗️ Architectural Overview & Technical Stack
```bash
┌─────────────────────────────┐        ┌──────────────────────────────┐        ┌─────────────────────────────┐
│  Google MediaPipe Hands     │───────►│  Real-Time Coordinate Map    │───────►│  Three.js WebGL Renderer    │
│  (Landmark Estimation)      │        │  (Kinematic Calculations)    │        │  (Particle Shader Pipeline) │
└─────────────────────────────┘        └──────────────────────────────┘        └─────────────────────────────┘
* **Core Engine:** JavaScript (ES6+), Three.js (WebGL 3D Rendering & Additive Blending Shaders)
* **Computer Vision Pipeline:** Google MediaPipe Hands (Real-time hand landmark estimation and joint vector tracking)
* **Mathematical Modeling:** Custom procedural generation algorithms mapping parametric equations directly to buffer geometries
```

---

## 🛸 Volumetric Procedural Mesh Library (`touchdesigner_mesh.html`)

This module features a dual-hand interaction schema:
1. **Left Hand Kinematic Control:** Dynamically maps palm coordinates to position a 3D wireframe bounding box while tracking finger span ratios for uniform scaling.
2. **Right Hand Gesture Trigger:** Evaluates Euclidean distance vectors between proximal phalanges to trigger state changes, morphing particles across 9 mathematically defined volumetric geometries:

| Index | Procedural Model | Mathematical & Geometric Foundation |
| :---: | :--- | :--- |
| **1** | **DNA Helix** | Double-helix parameterization using trigonometric backbones ($x = \cos(t)$, $z = \sin(t)$) paired with intersecting orthogonal cross-rungs. |
| **2** | **Butterfly** | Parametric rose and logarithmic scaling equations generating symmetrical wing spans. |
| **3** | **Skull** | Hollow-shell spherical coordinate remapping featuring procedural cartesian carving algorithms for orbital sockets and jaw structures. |
| **4** | **Jellyfish** | Upper hemispherical dome meshes combined with sinusoidal drop equations for flowing tentacle dynamics. |
| **5** | **Tree** | Volumetric spherical canopy distributions paired with tapered trunk structures. |
| **6** | **Whale** | Weighted ellipsoid tapering models featuring arched dorsal profiles, pectoral fins, and tail flukes. |
| **7** | **Human Hand** | Segmented particle cluster arrays mapping palm bases to independent finger phalange extensions. |
| **8** | **Sun** | High-density spherical core implementations with randomized directional vector displacement for solar flare eruptions. |
| **9** | **Nebula** | Multi-armed logarithmic spiral distribution models mapped across flattened galactic coordinate planes. |

---

## 🚀 Getting Started & Local Deployment

### Prerequisites
* A modern web browser with hardware-accelerated WebGL enabled.
* A connected webcam for real-time tracking input.
* [Node.js](https://nodejs.org/) or a local static file server environment (such as the VS Code Live Server extension).

### Installation & Execution
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/KshatraSanctum/Visual-Art.git](https://github.com/KshatraSanctum/Visual-Art.git)
   ```
2. Navigate to the workspace directory:
```bash
cd Visual-Art
```
3. Launch via Local Server:
 ```bash

Open the workspace in VS Code.

Right-click touchdesigner_mesh.html and select "Open with Live Server".

Grant browser permissions for camera input when prompted.
```
🛡️ License
```bash
This project is open-source and available under the terms of the MIT License.
```

