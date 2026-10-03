# Chapter 4: Plasma-Oxide Surface Reactions & Ion-Enhanced Etching

## 4.1 F• Radical Attack on SiO₂ and HfO₂

### SiO₂ Etch Mechanism

**Primary Reaction Pathway**:
```
SiO₂ + F• → SiOF• + O• (initial attack)
SiOF• + F• → SiF₂ + O• (sequential fluorination)
SiF₂ + 2F• → SiF₄ (volatile product formation)
```

**SiF₄ Product Properties**:
- Highly volatile, sublimes at ~7°C
- Exits as gas without redeposition
- Results in clean etch with minimal residue

### HfO₂ Etch Mechanism

**Reaction Sequence**:
```
HfO₂ + F• → HfOF• + O•
HfOF• + 2F• → HfF₃ + O•
HfF₃ + F• → HfF₄ (terminal product)
```

**HfF₄ Volatility**:
- More volatile than HfO₂ itself
- Hygroscopic (absorbs water)
- Can redeposit if chamber humidity is high

### Comparative Etch Rates

| Material | Etch Rate (nm/min) | Relative Rate |
|----------|------------------|--------------|
| SiO₂ | 250-350 | 1.0 (baseline) |
| HfO₂ | 150-250 | 0.6-0.9 |
| TiN | 10-30 | 0.04-0.12 |
| Poly-Si | 20-50 | 0.08-0.20 |

**Selectivity Challenge**: Despite HfO₂ etch being slower, selectivity to gate metals requires careful chemistry tuning.

## 4.2 Ion Bombardment Regimes

### Below-Threshold Regime (<5 eV)

**Mechanism**:
- Ions too slow to break bonds
- Physical sputtering minimal
- Chemical etch dominant

**Effect**: Etch rate independent of ion energy; purely chemical

### Ion-Assisted Etch Regime (5-100 eV)

**Optimal Range for Oxide Etch**: 20-80 eV

**Mechanisms**:
1. **Bond Weakening**: Ion impact makes bonds more reactive to radicals
2. **Activation**: Provides local energy for further reactions
3. **Desorption Enhancement**: Helps volatile products leave surface

**Ion Impact Effect**:
- At 50 eV: Etch rate increases 2-3× vs. radical-only etch
- At 80 eV: Further increase, but subsurface damage begins

### High-Energy Sputtering Regime (>100 eV)

**Mechanism**: Physical sputtering dominates; bond specificity lost

**Consequence**: 
- Indiscriminate material removal
- High damage
- Poor selectivity

## 4.3 Interface Damage and Characterization

### Damage Types at Si/SiO₂ Interface

1. **Point Defects**:
   - Vacancy-type (Si or O missing)
   - Interstitial-type (extra Si or O)
   - Creates dangling bonds → Interface trap states (Dit)

2. **Charged States**:
   - Some defects trap charge
   - Positive or negative charge states shift Vth
   - Multi-electron states create hysteresis

3. **Extent**: Typically 2-10 nm subsurface affected

### Dit Measurement (C-V Method)

**Interface State Density Extraction**:
```
Dit = (Cmin - Cmax) / (q × A × kT/q × ln(ωτ))
```

Where:
- Cmin, Cmax: Minimum/maximum capacitance in C-V curve
- ω: Measurement frequency
- τ: Interface state relaxation time

**Dit Specifications**:
- SiO₂/Si (thermally grown): Dit < 10¹⁰ cm⁻² eV⁻¹
- SiO₂/Si (after etch): Dit ≈ 10¹¹-10¹² cm⁻² eV⁻¹ (10-100× increase)
- HfO₂/Si (after etch): Dit > 10¹² cm⁻² eV⁻¹ (significant damage concern)

### Post-Etch Annealing for Recovery

**Rapid Thermal Anneal (RTA)**:
- Temperature: 400-500°C
- Duration: 30-60 seconds
- Atmosphere: N₂ or forming gas (H₂/N₂)

**Dit Recovery**:
- Hydrogen passivation of Si dangling bonds
- Crystal reordering reduces defect density
- Typical improvement: Dit reduction by 2-5×

---

## Key Takeaways

- F• radicals primarily attack oxide; HfO₂ has higher affinity than SiO₂
- Ion bombardment in 20-80 eV range enhances etch rate while maintaining selectivity
- Interface damage (Dit increase) is unavoidable but can be mitigated
- Post-etch annealing provides partial recovery of interface quality

---

## Next Steps

[Continue to Chapter 5: Reactor Architecture & Electrode Materials](05-reactor-design.md)

Or return to [Index](../INDEX.md)
