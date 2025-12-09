# MonoPaw: A Single-Leg Canine Gait Robot 🐾

MonoPaw is a foldable-robotics inspired **single-leg, canine-gait robot**.
A 5-bar leg mechanism is mounted on a lightweight cart, driven by DC/servo
actuators and controlled by an ESP32. The goal is to study how link lengths
and joint phase offsets affect **foot kinematics and energy use**, as a
reduced-order model of a quadruped.

---

## Project Goals

- Build a **low-cost, quickly manufacturable** bio-inspired leg using
  5-layer laminate construction.
- Investigate how **link geometry and phase offset** influence foot
  velocity profiles and gait quality.
- Create an easy-to-reproduce **teaching platform** for legged locomotion
  and gait analysis.

---

## Repository Structure

```text
sim/            – Simulation models and analysis scripts
firmware/       – ESP32 / microcontroller code for gait control
cad/            – DXF and CAD files for leg and cart
hardware/       – Assembly instructions and bill of materials
docs/           – Final report and presentation slides
media/          – Images and video clips of the prototype
old_versions/   – Earlier project scope (2-leg design) for reference
