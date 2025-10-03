# 📘 CMOS Project – Day 2 Report

This is my Day 2 log for the CMOS Project.  
It covers MOSFET behavior in linear and velocity saturation regions, short vs. long channel effects, and CMOS inverter basics.  

---

## 🔹 MOSFET Drain Current Equation

When **VGS > VT** and at lower VDS values:

\[
I_d = k_n \left[ (V_{gs} - V_t)V_{ds} - \frac{V_{ds}^2}{2} \right]
\]

- This is the **drain current equation** in the **linear (triode) region** of a MOSFET.  
- Mathematically:  
  - Not strictly linear (because of quadratic term \( V_{ds}^2 \)).  
  - First term \((V_{gs}-V_t)V_{ds}\) is bilinear.  
- Why called *linear region*?  
  - At small VDS, MOSFET behaves like a **voltage-controlled resistor**.  
  - Id ≈ linear with VDS (ignoring quadratic term).  

✅ **Key point:** Mathematically nonlinear, but in device physics called *linear/ohmic region*.:contentReference[oaicite:0]{index=0}

---

## 🔹 Long vs Short Channel Behavior

- **Long Channel (1.2 μm):**  
  - Drain current shows **quadratic dependence** on VGS at a fixed VDS.  

- **Short Channel (0.25 μm):**  
  - Quadratic only at small VGS.  
  - At higher VGS, **linear dependence** due to **velocity saturation**.  

### Velocity Saturation
- At low electric fields: velocity ∝ electric field.  
- At high fields: velocity becomes constant.  
- For short-channel MOSFETs, there is an **extra mode of operation**:  
  - **Velocity Saturation Region** (beyond cutoff, linear, and saturation).  

---

## 🔹 MOSFET Current Models

- At lower technology nodes, drain current depends not only on W/L ratio.  
- Even with same W/L, reducing channel length alters current.  
- Drain current ∝ quadratically with VGS (long channel).  
- Drain current ∝ linearly with VGS (short channel at higher fields).  

---

## 🔹 Lab Activity – Id vs VDS (Short Channel)

- Observed **linear behavior** at small VDS.  
- Peak current reduces as VDSmin increases.  
- ID vs VGS used to extract **VTH**:  
  - Extrapolate Id–Vgs curve back to x-axis.  
  - Example: **VTH ≈ 0.77 V**:contentReference[oaicite:1]{index=1}.  

---

## 🔹 MOSFET as a Switch – CMOS Inverter

- **CMOS = Complementary MOS (PMOS + NMOS):**  
  - PMOS on top (source → VDD).  
  - NMOS at bottom (source → VSS).  
  - Gates tied together (Vin).  
  - Drains tied together (Vout).  

### Voltage Transfer Characteristics (VTC)
- Based on **Vin vs Vout**.  
- Thresholds of NMOS and PMOS differ (electron vs hole mobility).  
- Simplified analysis: only track **Vin and Vout**.  

### Current in CMOS Inverter
- At Vout = 0 → finite current (needed to charge output capacitance).  
- PMOS and NMOS curves differ → combine to get **load curve**.  
- Merging NMOS + PMOS load curves gives complete CMOS VTC.  

---
## ✅ Lab screen shots
![Short channel device Id vs Vds](images/shortchannel_idsvsvds.png)
![Id vs Vds](images/spicecommandshortchannel_ids_vds.png)
![spice commad for idvsvgs](images/spice_vth)
![id vs vgs graph and obtaining vth](images/vth)


## ✅ Summary of Day 2
- Derived MOSFET drain current in **linear region**.  
- Understood **short vs. long channel differences** (velocity saturation effect).  
- Extracted **VTH from Id–Vgs plot (~0.77 V)**.  
- Analyzed **CMOS inverter basics** (PMOS on top, NMOS on bottom, complementary action).  
- Explored **VTC characteristics** and load curves.  

---

✨ *End of Day 2 – Getting deeper into MOSFET physics before diving into delay analysis in Day 3!* 🚀

