# ⚙️ ESCs and Brushless Motors

In a drone, **ESCs (Electronic Speed Controllers)** and **brushless DC motors (BLDC)** work together to generate and regulate thrust. Choosing the right combo affects stability, speed, and flight time.

---

## 🌀 Brushless DC Motors (BLDC)

BLDC motors have no brushes (unlike brushed motors), making them efficient, durable, and ideal for drones.

### 🔢 Key Parameters:

| Term | Meaning |
|------|---------|
| KV Rating | RPM per Volt. Higher KV = Faster, lower torque |
| Max Current (A) | Max safe current draw |
| Max Thrust (g) | Max lift motor can generate (depends on prop) |
| Shaft Diameter | Needed for prop compatibility |

> Ex: **A2212 1000KV** = Spins 11,100 RPM at 11.1V (3S)

---

## ⚡ ESC – Electronic Speed Controller

ESCs receive throttle signals from the flight controller and regulate power to the motors.

### 🔌 Functions:

- Converts DC battery power to 3-phase AC for BLDC
- Interprets PWM signals from FC
- May include BEC (Battery Elimination Circuit) for powering FC/receiver

---

## 🧠 Choosing ESCs

| Spec | What to Match |
|------|----------------|
| Current Rating | > Max motor draw (by 25–30%) |
| Voltage | Matches battery voltage (3S, 4S, etc.) |
| Firmware | SimonK (fast throttle), BLHeli (configurable), etc. |

> Ex: Motor draws 15A max → use **20A or 30A ESC**

---

## 🛠️ Example Pairing

| Component | Spec |
|----------|------|
| Motor | A2212 1000KV |
| ESC | 30A SimonK |
| Battery | 3S 2200mAh |
| Propeller | 1045 |
| Max Thrust | ~850g per motor

---

## 🔥 Notes on ESC Safety

- Always calibrate ESCs (especially with Pixhawk)
- Check for overheating on heavy throttle
- Use power distribution board (PDB) or 4-in-1 ESC for clean wiring
- Use bullet connectors for easy motor swaps

---

## 🧪 Testing Tools

- Thrust stand + wattmeter
- Multimeter for current checks
- ESC signal tester or FC + QGroundControl

---

> TL;DR:  
> Motors generate power, ESCs control it.  
> Get both wrong, and your drone becomes a flying toaster. 🔥

