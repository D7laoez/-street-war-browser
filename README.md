# STREET WAR — BROKEN CITY 3D

A browser-based 3D urban driving-combat game built with Three.js. It runs as a static site and supports desktop keyboards and mobile touch controls.

## Play

Open the production site on Vercel or serve this repository with any static HTTP server. Three.js and GLTFLoader are loaded as ES modules from jsDelivr; the CC0 GLB models are streamed from the upstream asset repository, so an internet connection is required.

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
- City blocks populated with external GLB building models instead of the former box-only building placeholders
- Player and hostile vehicles use a shared GLB car model, with procedural fallback geometry if the asset cannot load
- Hostile pursuit, enemy projectiles, target acquisition and escalating waves
- Player armour, nitro, score, collision damage and mission-failure/retry flow
- Building collision bounds, vehicle-to-vehicle contact and world-boundary handling
- Pause/resume flow and mobile pointer controls
- Adaptive pixel ratio and reduced shadow cost on smaller screens

## 3D asset credits and license

The city buildings and car are loaded from **[Low Poly City Kit](https://github.com/kayquer/kit-cidade-lowpoly)** by Kayquer. The repository declares the pack as **CC0 1.0** (public domain), allowing modification and commercial use without attribution requirements. Credits are included here as a courtesy.

The imported pack is stylized low-poly geometry, not photogrammetry or photorealistic AAA assets. It replaces the former primitive-only city/building and car visuals, but it does not make the game photorealistic. Assets are currently loaded from the upstream raw GitHub host at runtime rather than copied into this repository.

## Current limitations

This remains an evolving browser-game prototype. Character models, weapons, detailed destructible environments, advanced vehicle physics, mission progression, and full runtime QA remain future work. Browser performance and WebGL support vary by device. The game requires internet access for Three.js, GLTFLoader, and the external GLB models.

## Development

No build step is required. Open `index.html` through a local static server or a static host such as Vercel.
