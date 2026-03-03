# HydroDome Wildfire Defense Simulations

Interactive wildfire defense simulations by [Carmanah Wildfire](https://carmanahwildfire.com). Each demo models HydroDome tower deployment, hydraulic analysis, and fire behavior for a specific BC community.

## 🔴 Live Demos

| Community | Description | Link |
|-----------|-------------|------|
| **Fort St. James, BC** | V4 — 54 towers, 409 roads, full fire spread modeling | [Launch Demo](https://tetontopo.github.io/hydrodome-sim/) |
| **Harrison Hot Springs, BC** | V10 — 76 towers, 253 water mains, 4-level hydraulic cascade | [Launch Demo](https://tetontopo.github.io/hydrodome-sim/harrison-hot-springs.html) |
| **Jackson, WY** | Priority area analysis | [Launch Demo](https://tetontopo.github.io/hydrodome-sim/jackson-areas.html) |

## About HydroDome

HydroDome is a permanent wildfire defense infrastructure system that uses Nelson Big Gun 100 Series sprinklers on 30ft towers to create humidity domes protecting structures from wildfire. Key features across all simulations:

- **Tower Placement** — Interactive drag-and-drop positioning with coverage analysis
- **Hydraulic Modeling** — Real water network data with pipe capacity constraints
- **Fire Simulation** — Elliptical spread with wind, ember showers, and spot fires
- **Zone Duty Cycling** — Capstone C65 microturbine-powered rotation
- **SCADA Dashboard** — Real-time system monitoring
- **Cost/ROI Analysis** — System cost vs. estimated loss prevention

## Harrison Hot Springs (V10)

The latest simulation features a 4-level hydraulic cascade refill model:
1. **Cistern connection** — 750 GPM max per tower (150mm service line)
2. **Distribution main** — Street pipe capacity shared among towers
3. **Trunk line** — Larger pipes feeding multiple street pipes
4. **Reservoir feed (F1)** — Ultimate system bottleneck

Additional V10 features:
- 253 water mains from FVRD ArcGIS data
- 525 mapped structures
- Evacuation mode with adjustable hydraulic slope
- Auto-activate towers based on fire proximity
- Per-tower refill priority (emptiest first, fire-threatened get priority)
- Save/load tower layouts
- PDF report export

## Development

Each simulation is a standalone HTML/JavaScript application — no build step required. Edit and push to see changes live via GitHub Pages.

## Data Sources

- Water network: FVRD ArcGIS (Harrison), OpenStreetMap (Fort St. James)
- Buildings: OpenStreetMap
- Hydrants: FVRD ArcGIS Layer 81

---

Built by **Carmanah Wildfire** | HydroDome Innovation Team
