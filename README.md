# OmniDrone — 360° Propulsion Concept Viewer

An interactive 3D viewer (works great on a phone) that explores the idea of a
drone whose rotors don't all face **up** — but in **every direction**: left,
right, up, down, forward, back, and the diagonals in between.

Drag to orbit, pinch to zoom, and tap between four propulsion concepts.

## The idea

A normal quadcopter has all four rotors pointing straight up. It can only make
thrust *upward*, so to fly sideways it has to **tilt its whole body**.

This concept asks: *what if the blades faced all 360°?* If rotors point in many
directions, the drone can push itself any way it wants **without tilting** — and
even hover upside-down. That unlocks true **6-DOF** (six degrees of freedom)
control: independent movement and rotation on every axis.

## The four modes

| Mode | Rotors | What it shows |
|------|--------|---------------|
| **Classic** | 4 × up | Standard quad — thrust up only, must tilt to move |
| **Hybrid** | 4 up + 2 tilted | Some blades up, some canted — partial omni, the "mixed" version you described |
| **Omni-6** | ±X ±Y ±Z | Rotors on the 6 faces of a cube — thrust on any of 6 axes, no tilting |
| **Omni-Sphere** | 12 around a sphere | Blades facing up, down, sideways **and every diagonal** — full 360° |

🔵 Cyan rotors = up-facing &nbsp;&nbsp; 🟠 Orange rotors = 360° / tilted.
Toggle **Thrust vectors** to see which way each rotor pushes.

## View it on your phone

1. **Easiest — GitHub Pages:** In the repo, go to *Settings → Pages*, set the
   source to the `main` branch (root). After a minute, open the published URL on
   your phone.
2. **Or open the file directly:** download `index.html` and open it in any
   mobile browser. (Needs internet the first time — it pulls the 3D library
   from a CDN.)

## Tech

Single self-contained `index.html` using [three.js](https://threejs.org/).
No build step, no dependencies to install.
