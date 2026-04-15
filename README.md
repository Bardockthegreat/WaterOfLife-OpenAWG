# WaterOfLife-OpenAWG
A low-cost, hardware-store-buildable atmospheric water generator (AWG) that condenses clean water from humid air using simple materials, safe 12 V power, and no microcontrollers. Fully open-source, under $100, and designed for off‑grid, emergency, and educational use.
# Simple DIY Atmospheric Water Generator (AWG)
A low‑cost, no‑microcontroller, hardware‑store build for producing clean water from air.

## 1. Overview
This project shows how to build a simple atmospheric water generator (AWG) using 1–2 TEC1‑12706 Peltier modules, common hardware‑store materials, and recycled PC components. It is designed to be affordable ($60–$100), accessible (no microcontroller, no 3D printing), educational, and capable of producing a real trickle of drinkable water in warm, humid climates.

## 2. Features
- 1–2 × TEC1‑12706 Peltiers
- 12 V DC system with inline fuse
- Hot-side CPU/GPU heatsink rated ≥150 W
- Cold-side aluminum plate with increased fin area
- Fully ducted airflow for efficient condensation
- Vertical fins + sloped collector for reliable drainage
- Inline carbon filter for drinking water
- Peltiers run at 9–10 V for higher COP
- All parts from hardware stores or recycled electronics

## 3. Bill of Materials (BOM)
| Component | Qty | Approx Cost | Notes |
|----------|-----|--------------|-------|
| TEC1‑12706 Peltier | 1–2 | $3–$6 ea | Core cooling modules |
| CPU/GPU heatsink + 120 mm fan | 1 | $10–$25 | Hot-side heat rejection |
| Aluminum cold plate (80–100 mm) | 1 | $5–$10 | Cold-side base |
| Aluminum fins / small heatsink | 1 | $5–$15 | Vertical orientation |
| 120 mm intake fan (PWM-capable) | 1 | $5–$10 | Reduced airflow (15–30 CFM) |
| Dust filter | 1 | $3–$10 | Protects fins |
| 12 V PSU (15 A) | 1 | $15–$25 | Powers Peltiers + fans |
| Inline fuse (15–20 A) | 1 | $3–$5 | Safety |
| Rocker switch | 1 | $2–$5 | On/off |
| Buck converter | 1 | $5–$10 | Runs Peltiers at 9–10 V |
| Funnel | 1 | $2–$5 | Water collection |
| Food-grade tubing | 1 | $5–$10 | Water path |
| Inline carbon filter | 1 | $10–$20 | Drinking water |
| Jug/bottle | 1 | $5–$10 | Storage |
| Wood/foam board | — | $10–$20 | Frame + duct |
| Foam insulation | — | $5–$10 | Thermal isolation |
| Silicone sealant / duct tape | — | $5–$10 | Duct sealing |

Total: ~$60–$100 depending on sourcing.

## 4. System Architecture

### 4.1 Thermal Stack (Hot → Cold)
[HOT HEATSINK + FAN]
   ||
Thermal Paste
   ||
[PELTIER @ 9–10 V]
   ||
Thermal Paste
   ||
[COLD PLATE]
   ||
[VERTICAL ALUMINUM FINS]

Edges insulated with foam + sealant. Hot side fully exposed to room air.

## 5. Airflow & Ducting
- Intake fan slowed to 15–30 CFM (PWM or restrictor)
- Sealed cold duct with no bypass
- Outlet vent sized to avoid backpressure
- Dust filter on intake

Flow path:
[INTAKE FAN] → [SEALED COLD DUCT] → [COLD FINS] → [OUTLET VENT]

## 6. Water Collection Path
[COLD FINS]
   ↓
[SLOPED SURFACE ≥5° + DRIP EDGE]
   ↓
[SEALED FUNNEL]
   ↓
[FOOD-GRADE TUBING]
   ↓
[INLINE CARBON FILTER]
   ↓
[COLLECTION JUG]

## 7. Electrical System

### 7.1 Wiring (Parallel)
12 V PSU
   ↓
Inline Fuse (15–20 A)
   ↓
Rocker Switch
   ↓
+------------------------------+
| Peltiers via buck (9–10 V)   |
| Fans at 12 V                 |
+------------------------------+

### 7.2 Wire Gauge
- Peltiers: 14–16 AWG
- Fans: 18–22 AWG

### 7.3 Safety
- Low-voltage DC only
- Fuse required
- Wiring kept high and dry

## 8. Build Instructions

### Step 1 — Build the frame
Back panel for hot-side heatsink, middle section for cold duct, lower section for funnel + filter + jug.

### Step 2 — Mount hot side
Attach CPU heatsink + fan with unobstructed airflow.

### Step 3 — Assemble thermal stack
Apply thermal paste, clamp Peltier between hot and cold sides, add fins, insulate edges.

### Step 4 — Build cold duct
Surround cold plate + fins with foam board/wood, mount intake fan, seal joints, add outlet vent.

### Step 5 — Install water path
Create sloped drip surface, add drip edge, mount funnel, connect tubing → carbon filter → jug.

### Step 6 — Wire everything
Fuse → switch → parallel loads. Buck converter for Peltiers. Fans remain at 12 V.

## 9. Performance Expectations
Environment: 24–30°C, 60–80% RH, 24/7 operation.

1 × TEC1‑12706: 0.3–0.6 L/day  
2 × TEC1‑12706: 0.6–1.2 L/day  
Peak (30°C / 80% RH): up to ~1.4 L/day

## 10. Maintenance
- Clean funnel + jug regularly
- Replace carbon filter as needed
- Check dust filter
- Inspect duct seals
- Watch for frost buildup
- Reapply thermal paste annually

## 11. Safety
- 12 V DC only
- Inline fuse required
- Keep PSU dry
- Keep wiring away from condensate
- Hot side can reach 40–70°C
- Cold side can frost

## 12. License
MIT License or Creative Commons Attribution 4.0

## 13. Purpose
If even one person drinks clean water because of this design, the work was worth it.
