# Appendix F: Standard Operating Procedures

## F.1 Chamber Conditioning (Daily)

**Purpose**: Stabilize fluorocarbon coating and process baseline

**Procedure**:
1. Pump down to <1 mTorr (clean chamber)
2. Run CF₄ pretreatment: 50-100 cycles
   - 50 W, 10 mTorr, 10 seconds each cycle
3. Run reference oxide etch (known recipe)
4. Verify etch rate matches baseline (±5%)

**Time Required**: 30-45 minutes

## F.2 Daily Reference Wafer Run

**Purpose**: Track process drift and maintain recipe control

**Frequency**: Start of shift, after maintenance

**Parameters**:
- Use same film stack (e.g., HfO₂/SiO₂ on 300mm wafer)
- Run standard recipe (documented baseline)
- Record time-to-endpoint (OES detection)
- Measure final etch depth (SEM or optical)
- Track results in control chart

**Action Limits**:
- Etch rate drift >±5%: Investigate/recalibrate
- Endpoint time drift >±10%: Chamber conditioning recommended

## F.3 OES Calibration Procedure

**Frequency**: Every 100-200 operating hours

**Procedure**:
1. Start with clean, conditioned chamber
2. Run reference etch to known endpoint time
3. Record OES baseline spectrum (F•, CF, O•)
4. Update PLC threshold values if needed
5. Verify endpoint detection on next run

---

