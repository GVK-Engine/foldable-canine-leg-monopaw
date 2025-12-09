# 🐾 MonoPaw – Single-Leg Canine Gait Robot  
**Course:** Foldable Robotics (RAS 557)  
**Team Members:** Vamshikrishna Gadde, Tirth Kamdar
**Institution:** Arizona State University 
![Robot Type](https://img.shields.io/badge/Robot-Single_Leg_Canine-orange)
![Domain](https://img.shields.io/badge/Domain-Legged_Locomotion-brightgreen)
![Fabrication](https://img.shields.io/badge/Fabrication-Foldable_Robotics-yellow)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📘 Overview

**MonoPaw** is a **single-leg, canine-inspired planar gait robot** built as a testbed for quadruped locomotion.

- Uses a **5-bar leg mechanism** attached to a lightweight cart, inspired by the sagittal-plane motion of a dog leg (*Canis lupus familiaris*).
- Built with **5-layer laminate foldable manufacturing**, making it low-cost, fast to prototype, and easy to modify for future versions.
- Includes a **MuJoCo simulation + Jupyter notebook** that:
  - Models a single 5-bar leg on a cart with an ideal DC motor model and contact-rich ground interaction.
  - Logs foot position, forward velocity, and energy, and generates videos and plots of gait behavior.

**Design variables & study goals**

- Varies two key design parameters:
  - **Phase offset** between the two actuated joints (e.g., π/4, π/2, 3π/4, π).
  - **Leg geometry**, including a **+25% scaled** link-length version.
- Uses a **global parameter sweep** (brute force) instead of fancy optimization to map:
  - `phase offset / link scale → (max foot velocity, kinetic energy)`.
- Aims to understand how **timing and geometry** affect:
  - Foot trajectory  
  - Forward speed  
  - Energy usage  

**Key insights**

- A phase offset around **π/2** produces smoother, faster, and more energy-efficient motion than poorly phased gaits like **π/4**.
- The **scaled-up leg (+25%)** at π/2 increases stride length and improves forward velocity while reducing peak kinetic energy.
- The absolute values won’t match hardware exactly (ideal rigid bodies, ideal motors, stylized friction, 3 kg rig mass), but the **trends** are physically meaningful and guide real-world design.

**Future direction**

- Move from **one leg + cart** to **two legs on the same cart**, fix out-of-plane bending, better match real masses and friction, and compare single-leg vs two-leg locomotion in both sim and hardware.


📄 **Full documentation:**

- **Final Report:** [Final Report (PDF)](https://drive.google.com/file/d/1AOWXZ0Pb7rAI05T3VfAcDUNJhKIu6VGf/view?usp=drive_link)

- **Presentation Slides:** [Google Slides](https://docs.google.com/presentation/d/1pMKry9zL3wVUV_Ld6DZ8tjCflVTVhPLoqp3WUJ9W67Y/edit?usp=sharing)

## 🔗 Quick Links


## 🔗 Quick Links

- 📄 **Final Report:** [Final Report (PDF)](https://drive.google.com/file/d/1AOWXZ0Pb7rAI05T3VfAcDUNJhKIu6VGf/view?usp=drive_link)
- 🖼️ **Final Presentation Slides:** [Google Slides](https://docs.google.com/presentation/d/1pMKry9zL3wVUV_Ld6DZ8tjCflVTVhPLoqp3WUJ9W67Y/edit?usp=sharing)
- 📐 **DXF Geometry (Leg + Cart):** [DXF – Google Drive](https://drive.google.com/file/d/1fpy-IeiIvQU_QDXmIn9awjKsmJiABsrh/view?usp=drive_link)
- 📊 **Results – Plots & Graphs:** [Results Folder](https://drive.google.com/drive/folders/1Jsp6yqqxeOgSJ9IucUhM0W4xEi8tRZYP?usp=drive_link)
- 🤖 **Prototype Photos:** [Prototype Images](https://drive.google.com/drive/folders/1aBIUWjvPDlWAlErf96tD8eg0cyjrpQ81?usp=sharing)
- 🎥 **Demo Video(s):** [Demo Videos Folder](https://drive.google.com/drive/folders/1TzrLLGGUL38yIt5wSvSO4MUmN1KgDojz?usp=sharing)
- 📊 **Final Result (Video Overview):** [Results Summary – YouTube](https://youtu.be/Qhkaji4lUqc)

---

## 🧩 Repository Structure

```text
MonoPaw-Canine-Gait-Robot/
├── README.md
├── LICENSE

├── docs/
│   ├── MonoPaw_Final_Report.pdf        
│   └── MonoPaw_Presentation.pdf        

├── cad/
│   ├── leg_layer_rigid.dxf             
│   ├── leg_layer_flex.dxf
│   ├── leg_layer_adhesive.dxf
│   └── cart_panels.dxf


└── media/
    ├── images/                       
    └── videos/                         
