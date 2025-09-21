# PharmaPlayground-Interactive-Pharmacophore-Screening-for-Learning
Browser-based pharmacophore screening demo with 3D visualization, reproducible ligand generation, per-feature scoring, and exportable hit lists — built for EDUCATIONAL AND SIMULATIVE USE ONLY, NOT FOR CLINICAL RESEARCH OR DIAGNOSTICS.
# PharmacophoreScreen: Interactive Feature-Based Drug Design Sandbox

An **educational, browser-based pharmacophore screening demo** that brings concepts from computational drug discovery to life.  
Built with **Three.js** and **Tailwind CSS**, this project visualizes target pharmacophore features, generates candidate ligands, scores their alignment, and allows simple optimization — all interactively in the browser.

> ⚠️ **Disclaimer**  
> This project is an educational simulator. It is **not** a validated docking engine or medical tool, and must not be used for diagnosis, treatment, or drug discovery decisions.  
> Provided *as is* under the MIT License.

---

## 🎯 Why this project
Pharmacophores describe *why* molecules bind: donors, acceptors, hydrophobic patches, and charges aligning in 3D space.  
This tool simulates that idea in an approachable way:
- Students can **visualize** binding pockets and feature matches.  
- Researchers and admissions reviewers can quickly **see my coding and scientific communication skills**.  
- It demonstrates the bridge between **biology concepts** and **interactive computation**.

---

## 🚀 Features
- **3D Visualization**: Interactive target & ligand features with orbit + zoom.  
- **Ligand Generation**: Pseudo-random, reproducible (seeded RNG).  
- **Simple Scoring Model**: Max 25 points per matched feature within a 3.5 Å threshold.  
- **Optimization**: Local nudges to ligand features to simulate lead tweaking.  
- **Hit List**: Keeps top 5 ligands, with export/import in JSON.  
- **Snapshot**: Save the current 3D canvas as a PNG.  
- **Educational UI**: Clear per-feature contributions, match counts, and score interpretation.

---

## 🧩 How it works
1. **Target pharmacophore**: A fixed set of features in 3D (donors, acceptors, hydrophobic, charges).  
2. **Ligand generation**: Random candidate ligands with features placed in 3D.  
3. **Scoring**:  
   - Only features of the same type can match.  
   - Must lie within the pocket bounding box.  
   - Closer than 3.5 Å → contributes up to 25 points.  
   - Maximum score = 100.  
4. **Optimization**: Small random nudges simulate chemical tweaking.  
5. **Results panel**: Displays binding score, match count, matched feature cards, and contribution bars.

---


## 🛠️ Tech Stack
- **Three.js r128** (3D rendering)  
- **OrbitControls** (mouse/touch navigation)  
- **Tailwind CSS** (UI framework)  
- **Vanilla JavaScript** (no build tools required)

---
