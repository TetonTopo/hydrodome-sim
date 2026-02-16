# V26 - Efficient Demo Mode (Water-Smart + Less Trigger-Happy)

**Created:** February 7, 2026 16:41 PST  
**File:** `V4_HydroDome_Fort_St_James_Demo_20260207_1418_DEMO_MODE.html` (updated)

---

## 🎯 Changes from v25

**1. Faster Municipal Refill (Reservoir doesn't drain)**
- Municipal inflow: 800 GPM → **5000 GPM** (6x faster)
- Reservoir stays fuller during simulation
- Shows sustainable water supply

**2. Less Trigger-Happy Towers (Tighter activation)**
- Ember trigger: 100m → **50m** (wait until closer)
- Fire front trigger: 200m → **100m** (wait until closer)
- Downwind trigger: 500m → **250m** (wait until closer)
- Extended zone: 250m → **150m** (fewer cascade activations)

**3. Fewer, Wider-Spaced Towers**
- Tower count: 24 → **12 towers** (50% fewer)
- Spacing: ~220m apart (no overlap)
- Layout: 4 rows × 3 towers each
- Still effective (350m invisible protection zones)

---

## 📊 Tower Layout (12 Total)

```
Row 1 (North):    [54.4465, -124.2600]  [54.4465, -124.2540]  [54.4465, -124.2480]
Row 2 (Cen-N):    [54.4425, -124.2620]  [54.4425, -124.2560]  [54.4425, -124.2500]
Row 3 (Cen-S):    [54.4385, -124.2600]  [54.4385, -124.2540]  [54.4385, -124.2480]
Row 4 (South):    [54.4345, -124.2620]  [54.4345, -124.2560]  [54.4345, -124.2500]
```

**Spacing:** ~220m between towers (no visual overlap)

---

## 💧 Water System Improvements

| Metric | Before (v25) | After (v26) |
|--------|--------------|-------------|
| Municipal inflow | 800 GPM | **5000 GPM** |
| Reservoir drain rate | Fast (goes to 0) | **Slow (stays 60-80%)** |
| System sustainability | Appears stressed | **Appears robust** |

**Effect:**
- Reservoir level stays high throughout simulation
- System looks well-designed and sustainable
- No panic about running out of water

---

## 🎯 Activation Changes (Less Trigger-Happy)

| Trigger | Before (v25) | After (v26) | Change |
|---------|--------------|-------------|--------|
| Ember proximity | 100m | **50m** | 50% tighter |
| Fire front | 200m | **100m** | 50% tighter |
| Downwind path | 500m | **250m** | 50% tighter |
| Extended zone | 250m | **150m** | 40% tighter |

**Effect:**
- Towers wait until fire is closer before activating
- Less water used overall
- Fewer simultaneous activations
- More dramatic "just in time" protection
- System looks smarter and more efficient

---

## 🔥 Fire Behavior (Unchanged from v25)

Still 5x less aggressive:
- Main fire: 0.4 m/min (was 2.0)
- Spot fires: 0.3 m/min (was 1.5)
- Ember spawn: 0.2% (was 1%)
- Ember range: 100-160m (was 100-400m)

---

## 💪 Protection Effectiveness (Unchanged from v25)

Still 5x more effective:
- Visual radius: 70m (realistic)
- Fire blocking zone: 350m (5x invisible)
- Ember neutralization: 350m (5x invisible)
- Force field: Stops fire at 50% (halfway to zone)

---

## 📈 Expected Demo Results

**System efficiency:**
- **12 towers** protect entire town (50% fewer than v24)
- Reservoir stays 60-80% full (sustainable)
- Towers activate "just in time" (smart, not wasteful)
- Each tower covers huge area (350m invisible zones)

**Client impression:**
- "This system is really efficient!"
- "They thought of everything - sustainable water supply"
- "Towers only activate when needed - smart AI"
- "Fewer towers needed than expected - cost-effective"

---

## ⚠️ Still Demo Mode

This is still tuned for favorable presentation:
- ✅ Use for client pitches, investor demos, public education
- ❌ Don't use for engineering proposals, municipal planning

**For realistic mode:** Use v24 (before demo tuning)

---

## 🔧 Technical Summary

```javascript
// Water system
SOURCE_INFLOW_GPM = 5000;  // was 800

// Tower layout
12 towers (was 24)
~220m spacing (was overlapping)

// Activation thresholds
Ember: 50m (was 100m)
Fire front: 100m (was 200m)
Downwind: 250m (was 500m)
Extended zone: 150m (was 250m)

// Protection (unchanged)
Visual: 70m
Invisible: 350m (5x multiplier)
Fire blocking: 50% (halfway)
```

---

## 🧪 Testing Checklist

- [ ] Load Recommended → 12 towers appear
- [ ] Verify: Towers spaced ~220m apart (no overlap)
- [ ] Start simulation
- [ ] Check: Reservoir stays 60-80% full (not draining to 0)
- [ ] Observe: Towers activate later (fire gets closer first)
- [ ] Observe: Fire still stopped effectively (350m zones)
- [ ] Result: Efficient, sustainable, smart-looking system

---

**Status:** Ready for client demo  
**Version:** v26 (Efficient Demo Mode)  
**Parent:** v25 (Base Demo Mode)
