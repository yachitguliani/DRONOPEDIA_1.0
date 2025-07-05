# 🔢 Drone Propulsion Calculations

Proper propulsion system selection is key to drone stability, efficiency, and safety. It affects everything from takeoff to hover time to total payload capacity.

---

## ⚖️ Step 1: Estimate AUW (All-Up Weight)

Include:
- Frame + electronics
- Battery
- Payload (camera, GPS, etc.)

> Example:  
> Frame + FC + ESCs + Motors = 600g  
> Battery (3S 2200mAh) = 180g  
> Payload (camera + GPS) = 120g  
> **Total AUW ≈ 900g**

---

## 🧮 Step 2: Thrust-to-Weight Ratio

For a **stable and agile** drone, aim for a **TWR of 2:1** (thrust should be double the weight).

> Required Total Thrust = AUW × 2  
> Per Motor Thrust = Total Thrust ÷ No. of Motors

For 900g quadcopter:  
- Required thrust = 900g × 2 = 1800g  
- Per motor = 1800g / 4 = 450g

---

## ⚙️ Step 3: Motor Selection

Choose a motor that can provide at least **450g thrust** (preferably more at ~60-70% throttle).

- **KV Rating**: Higher KV = high speed, low torque (good for small props)  
- Lower KV = high torque (good for big props + payloads)

> Example: **A2212 1000KV + 1045 prop = ~850g thrust** on 3S

---

## ⚡ Step 4: Battery Selection

| Cell (S) | Voltage | Use Case |
|----------|---------|----------|
| 3S | 11.1V | Most beginner drones |
| 4S | 14.8V | FPV + racing |
| 6S | 22.2V | Long-range, heavy drones |

> Check max current draw of all motors  
> Then pick battery with:
> - Adequate **C rating** (Discharge Rate)
> - Adequate capacity for your flight time (mAh)

---

## 🔌 Step 5: ESC Selection

- ESC rating > 1.2× Motor Max Current
- Example: If motor draws 15A max → Use 20A or 30A ESC
- Match ESC voltage with battery (3S/4S/6S)

---

## 📐 Step 6: Propeller Selection

| Prop Size | Effect |
|-----------|--------|
| Small diameter, high pitch | High speed, less thrust |
| Large diameter, low pitch | More thrust, low speed |

> Match prop with motor's thrust curve (check datasheet or eCalc)

---

## 🛠️ Example Setup

| Component | Spec |
|----------|------|
| Motor | A2212 1000KV |
| Prop | 1045 |
| Battery | 3S 2200mAh |
| ESC | 30A SimonK |
| AUW | ~950g |
| Total Thrust | ~2200g (TWR > 2.3) ✅

---

## 🧮 Tools You Can Use

- [eCalc](https://www.ecalc.ch/xcoptercalc.php) (Online thrust + flight time calculator)
- [Datasheets from motor/ESC manufacturers]
- Digital thrust stand for testing

---

> “Thrust over trust.”  
> Always calculate before you fly.
