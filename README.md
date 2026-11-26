# STREET WAR — BROKEN CITY 3D

A browser-based 3D urban driving and combat prototype. Built with Three.js and procedural geometry; no build step is required.

## Run
Open `index.html` through a static web host (Vercel, GitHub Pages, or any static server). The Three.js ES module is loaded from jsDelivr, so an internet connection is required.

## Controls
### Desktop
- **W / Arrow Up:** accelerate
- **S / Arrow Down:** reverse / brake
- **A,D / Arrow Keys:** steer
- **Space:** fire at the nearest hostile vehicle
- **Shift:** nitro boost
- **R:** restart after mission failure

### Mobile
- Left virtual joystick: steer and accelerate/reverse
- FIRE: shoot nearest hostile
- NITRO: boost
- BRAKE / DRIVE: brake or accelerate

## Current build
- Real-time WebGL 3D scene with third-person chase camera
- Procedurally generated city blocks, roads, sidewalks, windows, street lights and roadside props
- Player and hostile vehicles assembled from 3D meshes
- Enemy pursuit, hostile projectiles, waves, score, armour and nitro
- Responsive HUD and touch controls for mobile screens
- Adaptive renderer pixel ratio and reduced shadow cost on smaller screens

## Notes
This is a procedural 3D game prototype, not a photorealistic AAA production. Current vehicles and city assets are generated from geometry rather than scanned or professionally authored models. The scene is designed to be extendable with licensed vehicle, building, road and audio assets.
