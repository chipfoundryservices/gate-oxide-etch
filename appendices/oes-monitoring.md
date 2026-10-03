# Appendix C: OES Monitoring Guide

## C.1 Key Wavelengths and Species

| Species | Wavelength (nm) | Intensity Level | Use |
|---------|---|---|---|
| F (I line) | 685.6 | Medium | Etchant level |
| F (I line) | 690.2 | Medium | Etchant level |
| CF (swan) | 283-295 | Low-Medium | Poly-Si exposure |
| CO (fourth) | 420-500 | Weak | Secondary species |
| O (triplet) | 777.4 | Weak | Oxidizer level |

## C.2 Endpoint Detection Algorithm

**Standard Approach**:
```
Monitor F• intensity (685-690 nm) baseline
When F• drops >20% below baseline AND
CF intensity rises >150% above baseline:
    Trigger STOP (interface transition detected)
```

**Margin Setting**: Adjust stop time ±5 seconds for selectivity control

## C.3 Calibration Procedure

**Frequency**: Every 100-200 operating hours

**Steps**:
1. Run reference oxide etch (known time to endpoint)
2. Record OES baseline (F•, CF, O•)
3. Establish F• drop threshold
4. Update PLC threshold values

---

