# Chapter 3: Fluorine & Hydrocarbon Chemistry in Gate Oxide Etch

## 3.1 CF₄-Based Chemistry (Industry Standard)

### CF₄ Plasma Dissociation

**Primary Dissociation Pathway**:
```
CF₄ + e⁻ → CF₃• + F• + e⁻ (dissociative excitation)
CF₄ + e⁻ → CF₃⁺ + F• + 2e⁻ (ionization)
CF₃ + e⁻ → CF₂• + F• (sequential dissociation)
F• + F• → F₂ (recombination)
```

**Typical Plasma Composition** (CCP, 13.56 MHz, 100W):
- F• (fluorine radicals): 10-30% of molecular input
- CF₃•, CF₂•: 5-15%
- CF⁺, CF₂⁺: 1-5% (ions)
- Unreacted CF₄: 50-70%

### CF₄/O₂ Synergy

**O₂ Addition Effects**:
1. **Enhanced Dissociation**: O⁻ attracts electrons, increases F• generation
2. **Radical Scavenging**: Removes polymer precursors (prevents deposition)
3. **Better Selectivity**: Oxidizes metal surfaces, slowing their etch

**Typical Composition**:
- CF₄: 60-80 sccm
- O₂: 20-40 sccm
- Ar (diluent): 50-200 sccm

**CF₄/O₂ Ratio Effects**:
| CF₄/(CF₄+O₂) | F• Concentration | Oxide Rate | Selectivity | Anisotropy |
|---|---|---|---|---|
| 0.70 | Low | Slow | Good | Poor |
| 0.80 | High | Fast | Moderate | Good |
| 0.90 | Very High | Very Fast | Poor | Excellent |

## 3.2 Hydrocarbon Co-Flows for Selectivity

### C₄F₈ (Octafluorocyclobutane)

**Polymer Formation Reaction**:
```
C₄F₈ + heat/plasma → CFₓ polymer chains + fluorine radicals
CFₓ (n) → CFₓ (n-1) + Cx (depolymerization)
```

**Typical Co-flow**: 5-15% C₄F₈ (relative to total CF₄+C₄F₈)

**Benefits**:
1. **Selectivity to Polysilicon**: 
   - Polymer deposits on cool poly surface
   - Passivates poly while oxide etches through polymer layer
   - Selectivity improvement: 50:1 → 100-150:1

2. **Anisotropy Enhancement**:
   - Sidewall coating (polymer) prevents lateral etch
   - Reduces undercut and notching

3. **Temperature Dependence**:
   - Polymer sticking inversely temperature-dependent
   - Low temperature (40-60°C): More polymer → Better selectivity
   - High temperature (80-100°C): Less polymer → More isotropic

## 3.3 Alternative Chemistries

### CHF₃ (Fluoroform)

**Advantages over CF₄**:
- Faster spontaneous etch (more reactive)
- Better for high-aspect-ratio features
- Lower dissociation requirement

**Disadvantages**:
- More difficult selectivity control
- Faster polysilicon etch
- More sensitive to process variations

### Cl₂-Based Chemistry (Complementary)

**Cl₂ Etch Mechanism**:
```
Cl₂ + e⁻ → Cl• + Cl• (dissociation)
SiO₂ + Cl• → SiCl₂ + O (slower than fluorine)
Si + Cl• → SiCl (faster than SiO₂)
```

**Use Case**: Primarily for polysilicon etch; not preferred for oxide.

## 3.4 Reaction Kinetics

### Temperature Dependence (Arrhenius)

**Etch Rate Temperature Dependence**:
```
R(T) = R₀ × exp(-Ea / kT)

Typical values for oxide etch:
- Ea (activation energy): 40-50 kJ/mol
- Temperature coefficient: ~0.3-0.8 %/°C
```

**Example**:
- At 60°C: Rate = 300 nm/min
- At 80°C: Rate = 300 × exp[-45000/(8.314×353)] ≈ 380 nm/min (+27%)

### Pressure Effects

**Low Pressure** (50-100 mTorr):
- Longer mean free path → More directional radicals/ions
- Better anisotropy, poorer uniformity
- Lower etch rates (fewer collisions)

**High Pressure** (150-300 mTorr):
- Shorter mean free path → More isotropic
- Better uniformity, poorer anisotropy
- Higher etch rates (more collisions)

## 3.5 Damage Mechanisms

### Ion-Induced Damage

**Ion Bombardment Events**:
- Lattice displacement
- Point defect creation (vacancies, interstitials)
- Dislocation formation (extended defects)
- Charged defect states at oxide-Si interface

**Damage Depth**:
- Typical ion penetration: 2-10 nm subsurface
- Interface state creation: Within 1 nm of Si/SiO₂ interface

### Chemical Damage

**F• Attack Effects**:
- Breaking of Si-O bonds
- Creation of Si dangling bonds (precursor to interface states)
- Less invasive than ion damage but still creates defects

**Temperature-Dependent**:
- Higher temperature → Enhanced diffusion → Faster interface damage
- Lower temperature → Reduced damage but slower etch

## Summary of Chemistry Trade-offs

| Objective | Chemistry | Mechanism |
|-----------|-----------|-----------|
| High Etch Rate | High CF₄, Low O₂ | Maximize F• generation |
| High Selectivity | CF₄+O₂ + C₄F₈, Low T | Polymer protection |
| Good Anisotropy | Low P, C₄F₈, Low T | Sidewall passivation |
| Low Damage | Low Power, Low T | Reduce ion energy |

---

## Next Steps

[Continue to Chapter 4: Plasma-Oxide Surface Reactions](04-plasma-oxide-reactions.md)

Or return to [Index](../INDEX.md)
