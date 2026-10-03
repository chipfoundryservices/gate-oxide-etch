# Chapter 2: Thermal SiO₂, High-κ Materials & Interfacial Layers

## 2.1 Thermal SiO₂ Properties and Etch Characteristics

### Material Properties

**Silicon Dioxide (SiO₂)**:
- **Density**: 2.27 g/cm³
- **Refractive Index**: 1.46 at 633 nm
- **Band Gap**: 8.9 eV
- **Thermal Conductivity**: 1.3 W/m·K
- **Coefficient of Thermal Expansion**: 0.5 × 10⁻⁶ K⁻¹

### Thermal SiO₂ Etch Rates (CF₄/O₂)

| Condition | Etch Rate | Selectivity to Poly |
|-----------|-----------|-------------------|
| 100W, 50 mTorr, 60°C | 200 nm/min | 50:1 |
| 150W, 100 mTorr, 60°C | 280 nm/min | 80:1 |
| 200W, 100 mTorr, 60°C | 350 nm/min | 70:1 |
| 200W, 150 mTorr, 60°C | 320 nm/min | 60:1 |

### Si/SiO₂ Interface Quality

**Band Diagram**:
- Band offset (EC): 3.1 eV
- Band offset (EV): 4.6 eV
- Provides excellent carrier confinement

**Interface State Density (Dit)**:
- Thermally grown SiO₂: Dit ≈ 10¹⁰ cm⁻² eV⁻¹ (state-of-the-art)
- Decades of process optimization
- Reference baseline for device performance

### Advantages for Gate Dielectric (28nm era)
1. Mature process with proven reliability
2. Excellent interface properties
3. Well-established etch chemistry
4. High breakdown field (>10 MV/cm)
5. Low fixed oxide charge (Qox < 10¹⁰ cm⁻²)

### Fundamental Limitation: Direct Tunneling

Direct tunneling current density:

```
J = q²/16π² ħ |ψ(0)|² (2m*/ħ²)^(1/2) × 
    exp[-4π√(2m*)/3qħ × φ_b^(3/2) / E_ox]
```

At physical thickness t_ox:
- t_ox = 1.5 nm: J ≈ 1 μA/cm² at Vg = 0.8V
- t_ox = 1.0 nm: J ≈ 100 μA/cm² (UNACCEPTABLE for standby power)

**Consequence**: EOT below 1.0-1.2 nm with SiO₂ is impractical for advanced nodes.

## 2.2 High-κ Dielectric Materials

### HfO₂ (Hafnium Dioxide) - Production Standard

**Material Properties**:
- **Dielectric Constant**: κ ≈ 20-25 (measured values vary with crystallinity)
- **Band Gap**: 5.7-6.0 eV
- **Density**: 9.68 g/cm³
- **Refractive Index**: 2.0-2.1
- **Thermal Conductivity**: 2.0 W/m·K
- **CTE**: 3.6 × 10⁻⁶ K⁻¹ (higher than SiO₂)

**Etch Characteristics**:
- HfO₂ etch rate (CF₄/O₂): 100-200 nm/min (typically faster than SiO₂)
- Volatile products: HfF₄ (hygroscopic), sublimes at ~100°C
- Selectivity challenges: Higher affinity to F• than SiO₂

### HfO₂ Etch Reactions

**Primary Etch Mechanism**:
```
HfO₂ + 6HF → H₂HfF₆ + H₂O (wet etch pathway)
HfO₂ + 4F• → HfF₄ + O₂ (plasma pathway)
HfO₂ + Ar⁺ + energy → Sputtering products (ion-assisted)
```

**Product Volatility**:
- HfF₄ is highly volatile and dissociates at moderate temperatures
- Hygroscopic nature means water absorption in chamber
- Byproduct management critical for process control

### ZrO₂ (Zirconium Dioxide) - Alternative High-κ

**Properties**:
- **Dielectric Constant**: κ ≈ 25-30
- **Band Gap**: 5.8 eV
- **Density**: 5.68 g/cm³
- **Lower thermal conductivity than HfO₂** (0.6 W/m·K)

**Status**: 
- Alternative to HfO₂ in research
- Limited production use (thermal management challenges)
- Higher κ appeals to advanced nodes

### Al₂O₃ (Aluminum Oxide) - Interfacial Material

**Properties**:
- **Dielectric Constant**: κ ≈ 8-10
- **Band Gap**: 8.8 eV
- **Density**: 3.97 g/cm³

**Use Cases**:
- As component in mixed-oxide stacks
- As passivation layer on HfO₂
- Al₂O₃/HfO₂ combination improves interface quality and charge trapping

## 2.3 Interfacial Layers (IL)

### Definition and Role

Thin dielectric layer (0.5-2.0 nm) between high-κ material and silicon substrate:

```
Silicon Substrate
        ↑
    [IL - typically SiO₂ or SiOₓNᵧ, 0.5-1.5 nm]
        ↑
    [High-κ - HfO₂ or ZrO₂, 4-8 nm]
        ↑
[Gate Electrode - TiN, Ru, or metal]
```

### SiO₂ Interfacial Layer

**Advantages**:
- Excellent Si/SiO₂ interface (Dit ≈ 10¹⁰)
- Prevents intermixing of high-κ and silicon
- Familiar process and properties

**Disadvantages**:
- Adds to total EOT (reduces κ benefit)
- Adds capacitive resistance in series with high-κ
- Requires careful thickness control (±0.1 nm)

### SiOₓNᵧ Interfacial Layer

**Nitrogen Addition Benefits**:
- Reduces boron penetration from P-channel substrate doping
- Improves carrier mobility in inversion layer
- Better passivation of dangling bonds at Si surface

**Drawback**:
- Etch selectivity becomes more complex (oxide vs. nitride component)
- Incomplete nitrogen removal complicates subsequent steps

## 2.4 Gate Electrode Materials

### Polycrystalline Silicon (Poly-Si)

**Properties**:
- **Conductivity** (n-doped): σ ≈ 10² (Ω·cm)⁻¹
- **Work Function**: 
  - n-doped (n-channel gate): 4.1-4.2 eV
  - p-doped (p-channel gate): 5.2-5.3 eV
- **Etch Rate** (Cl₂-based): 50-300 nm/min

**Advantages**:
- Mature process (decades of optimization)
- Easy doping engineering (n+ or p+)
- Good CMOS compatibility

**Disadvantages**:
- **Poly Depletion Effect**: In inversion, mobile charge in poly reduces effective Tox
  - Typical: 10-20 mV Vth shift, 1-2% capacitance loss
- Non-ideal work function for NMOS/PMOS (symmetric, not optimized)

**Usage**: Legacy 28nm and early 14nm production; now phased out in advanced nodes

### Metal Gate Systems (14nm and beyond)

**TiN (Titanium Nitride)**:
- **Composition**: Typically TiN₁.₀ to TiN₀.₉
- **Work Function**: ~4.3 eV (intermediate)
- **Resistivity**: ~200 μΩ·cm
- **Etch Rate** (fluorine): Moderate (difficult selectivity vs. oxide)

**Ta/Tan (Tantalum/Tantalum Nitride)**:
- **Work Function**: ~4.3 eV
- **Resistivity**: ~150 μΩ·cm
- **Etch Rate**: Similar to TiN

**Ru (Ruthenium)**:
- **Work Function**: ~4.6 eV
- **Resistivity**: ~7 μΩ·cm (lowest among metal gates)
- **Etch Rate**: Very slow in standard fluorine chemistry (good selectivity)

**Mo (Molybdenum)**:
- **Work Function**: ~4.6 eV
- **Etch Rate**: Moderate

### Work Function Tuning Strategy

Modern gate stacks use multiple metals for NMOS/PMOS work function engineering:

```
NMOS Gate Stack:
Poly-Si/TiN/Ru (work function ≈ 4.2-4.3 eV) - approaching n-type ideal

PMOS Gate Stack:
Poly-Si/Ta/Ru or similar (work function ≈ 5.0-5.2 eV) - approaching p-type ideal
```

**Benefit**: 
- Reduced gate-induced drain leakage (GIDL) at high Vgs
- Better electrostatic control at advanced nodes
- Enables scaling to smaller gate lengths

## 2.5 Material Interaction and Etch Selectivity

### SiO₂/Metal Selectivity Challenge

Metals used as gate electrodes have varying fluorine affinity:

| Material | Etch Affinity | Etch Rate Ratio (Metal/SiO₂) | Challenge |
|----------|----------------|------------------------|-----------|
| Ru | Very Low | 0.01-0.05 | High selectivity (excellent) |
| TiN | Medium | 0.2-0.5 | Selectivity possible with optimization |
| TiW | Medium | 0.3-0.6 | Similar to TiN |
| Ta | Medium | 0.2-0.4 | With TaN layer, better selectivity |

### SiO₂/Poly-Si Selectivity - Classical Challenge

Polysilicon etch rates in fluorine chemistry:
- CF₄/O₂ alone: Poly etch rate ≈ 20-50 nm/min (poor selectivity ~50:1-70:1)
- CF₄/O₂ + C₄F₈: Poly etch rate ≈ 2-5 nm/min (good selectivity >100:1)

**Mechanism**:
- C₄F₈ deposits polymer (CFₓ) on poly surface
- Polymer deposits preferentially on cooler poly (lower substrate temperature helps selectivity)
- Polymer protects poly from F• attack while oxide still etches through polymer

## 2.6 Thermodynamic Data for Common Reactions

### SiO₂ Etch in Fluorine Plasma

| Reaction | ΔG (kJ/mol) | ΔH (kJ/mol) | Spontaneous? |
|----------|-------------|------------|-------------|
| SiO₂ + 4HF → SiF₄ + 2H₂O | -1250 | -1280 | Yes |
| SiO₂ + 4F• → SiF₄ + 2O | -780 | -750 | Yes |
| 2O + 2CF₂ → CO₂ + CF₄ (regeneration) | -450 | -480 | Yes |

### HfO₂ Etch in Fluorine Plasma

| Reaction | ΔG (kJ/mol) | ΔH (kJ/mol) | Spontaneous? |
|----------|-------------|------------|-------------|
| HfO₂ + 6HF → H₂HfF₆ + H₂O | -1650 | -1700 | Yes |
| HfO₂ + 4F• → HfF₄ + O₂ | -1050 | -1100 | Yes |

**Observation**: HfO₂ has higher thermodynamic driving force than SiO₂ for fluorine reactions, explaining higher etch rates.

## 2.7 Summary Table: Material Properties for Gate Oxide Etch

| Property | SiO₂ | HfO₂ | TiN | Poly-Si |
|----------|------|------|-----|---------|
| **Density (g/cm³)** | 2.27 | 9.68 | 5.43 | 2.33 |
| **Refractive Index** | 1.46 | 2.1 | ~2.5 | ~3.5 |
| **Thermal Cond. (W/m·K)** | 1.3 | 2.0 | 30 | 140 |
| **CTE (10⁻⁶ K⁻¹)** | 0.5 | 3.6 | 9.35 | 2.3 |
| **Etch Rate (CF₄/O₂, nm/min)** | 250-350 | 150-250 | 5-20 | 20-50 |
| **Interface Quality (Dit)** | 10¹⁰ | 10¹²-10¹³ | N/A | Good |
| **Selectivity Metric** | Reference | Comparison | To SiO₂ | To SiO₂ |

---

## Next Steps

[Continue to Chapter 3: Fluorine & Hydrocarbon Chemistry](03-etch-chemistry-fundamentals.md)

Or return to [Index](../INDEX.md)
