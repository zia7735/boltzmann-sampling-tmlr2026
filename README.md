# Boltzmann sampling via normalizing flows

This repository contains the code for our TMLR 2026 paper.
**"Sampling Boltzmann distributions via normalizing flow approximation of transport maps."**

## What's inside
There are two separate experiments:
## 1. Coulomb system (`coulomb_4d_softcore.ipynb`)
A simple 2‑particle system with a Coulomb singularity.  
This notebook compares standard training against training with soft‑core regularization.

# 2. Alanine dipeptide (`alanine_dipeptide_66d.ipynb`)
The main 66‑dimensional experiment from the paper.  
This notebook trains a 12‑layer RealNVP on alanine dipeptide MD data, using a transport consistency penalty.  
It generates all the figures and the layer‑by‑layer animation video.

## How to run
The easiest way is to use Google Colab:
1. Open [Google Colab](https://colab.research.google.com).
2. Click **File → Open Notebook → GitHub**.
3. Paste this link:  
   `https://github.com/zia7735/boltzmann-sampling-tmlr2026`
4. Select either notebook.
5. Set the runtime to **GPU** (`Runtime → Change runtime type → T4 GPU`).
6. Run all cells (`Runtime → Run all`).

**Note:The alanine dipeptide notebook takes roughly 2 hours to run. The Coulomb notebook takes around 2–3 hours.

# Output files
Running the alanine dipeptide notebook will create:

- `phipsi_from_66d_cartesian.pdf` – 3‑panel Phi/Psi validation plot  
- `3d_cartesian_comparison.pdf` – 3D structure comparison  
- `66d_layer_by_layer_animation.mp4` – Gaussian → Boltzmann morphing video

## Citation

If you use this code, please cite our TMLR 2026 paper:
