# ⚡ CMOS Circuit Design – SPICE Simulation Project  

Welcome to my project repository from the **Cloud-based CMOS Circuit Design SPICE Simulation Workshop (10 Days, SKY130 Node)**.  
This repository captures my **daily reports, lab results, and simulation insights** as I progressed from transistor-level fundamentals to advanced robustness analysis.  

---

## 📘 About the Workshop  

- **Duration:** 10 Days  
- **Platform:** Open-source SKY130 Technology Node  
- **Mode:** Cloud-based, hands-on labs  
- **Organised by:** VSD (VLSI System Design)  

### 🔹 Focus Areas  
- CMOS device physics & SPICE modeling  
- NMOS & CMOS inverter behavior in different operating regions  
- Switching threshold extraction  
- Noise margin analysis & optimisation  
- Robustness under **power-supply** and **process variations**  
- Velocity saturation, dynamic power, delay analysis  
- Full **SPICE deck creation** and parameter sweeps  
- Linking SPICE-level insights to open RTL-to-GDS flows (OpenLane, VSDFlow)  

---

## 🚀 Why This Project Matters  

- **Global semiconductor momentum**: SKY130 PDK is now the go-to platform for startups, national fabs, and academic programs.  
- **Bridging theory and practice**: Every lecture was paired with guided SPICE labs, producing measurable plots.  
- **Reusable IP & workflows**: Simulation decks and scripts here can dovetail into broader RTL-to-GDS flows.  

This project documents **my journey** through this course, combining notes, lab outputs, and analysis into a reproducible and shareable format.  

---

## 📂 Repository Structure  

```plaintext
├── Day1/         # MOSFET basics, SPICE intro, Id-Vds plots
├── Day2/         # Long vs Short channel, Velocity saturation, CMOS basics
├── Day3/         # CMOS Inverter switching threshold & delay analysis
├── Day4/         # Noise margin theory and SPICE lab results
├── Day5/         # Supply scaling, Etching variations, Robustness tests
├── Day6/         # (to be added)
├── ...
└── README.md     # Main project overview (this file)
Each folder contains:

Report.md → My structured notes & theory writeup

images/ → Lab screenshots, VTC curves, transient plots, etc.

SPICE decks (if included)

🧪 Labs & Hands-On Work
Parameter-swept SPICE simulations using SKY130 models

Extraction of switching threshold (Vm)

Noise margin calculation (NMH, NML)

Delay analysis (rise/fall) with transistor sizing

Supply voltage scaling effects on inverter speed & gain

Robustness analysis under process variations & fabrication impacts

🎯 Outcomes
✅ Mastered transistor-level CMOS design with SPICE
✅ Built a repeatable simulation workflow for SKY130 nodes
✅ Learned to link device physics → circuit behavior → design robustness
✅ Produced daily structured reports (available in this repo)
✅ Gained industry-recognized certificate of completion

🏁 Conclusion
This repository is both my personal logbook and a knowledge base for anyone learning CMOS circuit design with SPICE.
Feel free to browse the daily reports, check out the SPICE results, and adapt the workflows for your own research or prototyping.

✨ From device physics to robust digital design – powered by SPICE & SKY130! ✨
