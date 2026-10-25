# Plasma Ring Simulator V0.6

Standalone interactive HTML simulation of a 127 mm glass sphere above a planar multi-turn excitation coil.

## Usage
Open `index.html` in a browser. No dependencies.

## Features
- Adjustable coil turns, radius, pitch, height, peak current and frequency.
- Free-space magnetoquasistatic field estimate using discretized Biot–Savart integration: Aφ, B, and Eφ ≈ ωAφ.
- r–z field map and CSV export.
- Independent visual model of the video's qualitative 0–9 s bright-ring → fading → recovery → fading sequence.
- Sphere rotation, tilt, lateral offset, hand and surface-charge visual controls.

## Scientific limitations
Research gas is **argon (Ar)**, not identified from a sample. Pressure is **unknown / HOLD**. Coil parameters are examples, not measured. The field solver does not account for glass dielectric boundaries, capacitive coupling, plasma response, ionization or discharge kinetics. The glowing ring is **not derived from the calculated electromagnetic field**; the brightness timeline is qualitative. Rotation/hand/charge sliders are visual-only. Do not use for high-voltage device design or safety decisions.

## Next steps
Measure coil dimensions and driving waveform, determine gas composition and pressure, compare electromagnetic field results against FEM, then introduce a coupled plasma model.
