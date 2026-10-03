# Chapter 15: Real-Time Monitoring & Endpoint Detection

## 15.1 OES (Optical Emission Spectroscopy)

**Target Species**:
- F• (685-690 nm): Primary etchant
- CF (280-300 nm): Indicator of poly-Si exposure
- O• (777 nm): Oxidizer status

**Endpoint Detection Algorithm**:
```
if (F• intensity ↓ AND CF intensity ↑):
    trigger STOP (interface transition detected)
```

## 15.2 Electrical Monitoring

**Forward/Reflected Power**:
- Reflects plasma impedance changes
- Can indicate chemistry changes or end-of-etch

**Substrate Current**:
- Ion flux measurement
- Indirect indicator of etch progress

## 15.3 Calibration and Maintenance

**OES Sensor**: Degrades over 500-1000 operating hours
**Chamber Conditioning**: Required for stable optical baseline

---

