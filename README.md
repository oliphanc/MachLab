# MachLab

A 2D compressible flow solver that runs entirely in the browser. Open `index.html`, or host the repository with GitHub Pages.

## What it does

- Solves the compressible Reynolds-averaged Navier–Stokes equations around a 2D body: NACA 4-digit airfoils, a cylinder, an ellipse, or pasted coordinates.
- Far-field boundary set by static pressure, Mach number, static temperature and angle of attack.
- Spalart–Allmaras turbulence model, or laminar flow.
- Steady runs, or time-accurate runs with second-order implicit dual time stepping.
- Two meshes: a static body-fitted O-mesh, or thin wall-normal O-layers inside a quadtree of squares that split and merge as the flow develops.
- Live flow field, force history, surface pressure and skin friction.
- Recording and smooth replay of unsteady runs, with GIF and video export and CSV downloads.

## Hosting on GitHub Pages

In the repository settings, open Pages, choose "Deploy from a branch", and select the `main` branch and the root folder. The page is a single self-contained file; it loads two typefaces from Google Fonts and nothing else.

## Limits

- Mach 0.03 to 4, ideal gas with constant specific heats.
- Fully turbulent or fully laminar; no transition model.
- Runs on one processor thread.
