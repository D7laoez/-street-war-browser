# STREET WAR — BROKEN CITY 3D

A browser-based 3D urban driving-combat game built with Three.js and procedural geometry. It runs as a static site and supports desktop keyboards and mobile touch controls.

## Play

Open the production site on Vercel or serve this repository with any static HTTP server. The Three.js ES module is loaded from jsDelivr, so an internet connection is required.

## Controls

### Desktop
- **W / Arrow Up:** accelerate
- **S / Arrow Down:** reverse
- **A / D / Arrow Keys:** steer
- **Space:** fire at the nearest hostile vehicle
- **Shift:** nitro boost
- **B / Ctrl:** handbrake
- **Escape:** pause / resume
- **R:** restart after mission failure

### Mobile
- **Left joystick:** steer and accelerate / reverse
- **DRIVE:** hold to accelerate
- **BRAKE:** hold to brake
- **FIRE:** hold to fire
- **NITRO:** hold to boost

## Gameplay systems

- Third-person chase camera and responsive WebGL renderer
- Procedurally generated city blocks, roads, sidewalks, windows, street lights and roadside props
- Player and hostile vehicles assembled from 3D meshes
- Hostile pursuit, enemy projectiles, target acquisition and escalating waves
- Player armour, nitro, score, collision damage and mission-failure/retry flow
- Building collision checks, vehicle-to-vehicle contact and world-boundary handling
- Pause/resume flow and touch controls with pointer-cancel handling
- Adaptive pixel ratio and reduced shadow cost on smaller screens

## Current limitations

This is an evolving browser-game prototype, not a photorealistic AAA production. The city and vehicles are generated from geometry rather than scanned or professionally authored assets. Browser performance and WebGL support vary by device. The game requires internet access to load Three.js from the CDN. The next major visual milestone is replacing procedural placeholder geometry with optimized, properly licensed 3D environment and vehicle assets.

## Development

No build step is required. Open `index.html` through a local static server or a static host such as Vercel.
