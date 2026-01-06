# Feely Drone 🛸

**Feely Drone** is a meta-repository that aggregates all software components used for the development of a tactile gripper drone, developed by the **BioMorphic Intelligence Lab** at **TU Delft**.

The project focuses on enabling aerial robots to safely and intelligently interact with their environment using **tactile sensing**, **physical interaction**, **system identification**, and **closed-loop control**.

---

## 📌 Overview

This repository serves as a **central hub** combining all major software modules required for the Feely Drone project. Each component is maintained as an independent repository and included here via **Git submodules**.

The meta-repository allows easy cloning, version tracking, and coordinated development across simulation, firmware, ROS2 interfaces, and data analysis.

---

## 📦 Included Submodules

| Submodule | Description |
|---------|-------------|
| `feely_drone_common` | Shared message definitions, utilities, and interfaces |
| `feely_drone_genesis` | Genesis simulation environment and robot setup |
| `feely_drone_plots` | Python plotting and visualization tools |
| `feely_drone_ros2` | ROS2 packages for PX4, sensors, and control |
| `feely_drone_sysID` | System identification tools and workflows |
| `feely_drone_teensy` | Embedded firmware for Teensy-based tactile hardware |

---

## 🚀 Getting Started

### Prerequisites

- Git (≥ 2.20)
- ROS2 (for `feely_drone_ros2`)
- PX4 development tools (if flying on real hardware)
- Python (for plotting and analysis tools)
- Teensy toolchain (for embedded firmware)

Exact dependencies are documented in the individual submodule repositories.

---

### Clone the Repository with Submodules

```bash
git clone https://github.com/BioMorphic-Intelligence-Lab/feely_drone.git
cd feely_drone
git submodule update --init --recursive
```

### 📁 Data & Design

All recorded experimental data used for analysis, benchmarking, and system identification is hosted externally:

#### 📂 Feely Drone Dataset (Google Drive)

[Drive](https://drive.google.com/drive/folders/1qB7zECcjWVdrE33aIGa4r1efsfwKtLYG?usp=drive_link)

Please refer to the folder for descriptions of individual datasets and usage guidelines.

#### 📐 Design Files 

The CAD files can be found [here](https://cad.onshape.com/documents/e76b263494e0d1d2d95702f8/w/33ff3b94d6654c453e767fd3/e/4ac8c4743e1d3bf3a7664d8a)

### 📜 Citation

If you use this repository or the associated data in academic work, please cite the relevant paper.

```
@article{bredenbeck2026,
  title  = {Aerial Tactile Perching via an Anthropomorphic Hand with Embodied Soft Tactile Receptors},
  author = {Anton Bredenbeck, Anish Jadoenathmisier, Salua Hamaza},
  year   = {2026},
}
```
