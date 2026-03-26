---
description: "How to correctly size a sewage pump — calculating peak flow rate, total dynamic head, solid handling, and HP requirements for residential, commercial, and industrial installations."
---

# How to Properly Size a Sewage Pump for Your Property

# How to Properly Size a Sewage Pump for Your Property

Incorrect pump sizing is the most common cause of premature sewage pump failure and chronic maintenance problems. An undersized pump runs under overload — overheating, wearing rapidly, and eventually failing. An oversized pump cycles on and off excessively, wastes energy, and causes water hammer. Getting the size right is the single most important specification decision.

This guide explains how to calculate what you actually need before selecting a pump.

## Step 1 — Calculate Peak Flow Rate

The pump must handle the maximum flow the system will ever generate — not the average. Sizing to average flow means the pump cannot keep up during peak demand.

**For residential properties**, calculate peak flow based on the number of plumbing fixtures:
- Each toilet: 2.5 litres/flush
- Basin/sink: 6–10 litres/minute when running
- Shower: 8–12 litres/minute
- Bathtub fill: 15–20 litres/minute
- Washing machine: 50–60 litres/cycle

Estimate how many fixtures could realistically be in use simultaneously and add them up. For a family home, peak simultaneous use is typically 2–3 fixtures.

**For commercial buildings**, base the calculation on fixture units per floor and occupancy. Consult IS 1172 or NBC guidelines for fixture unit flow rates, and apply a demand factor based on building type.

**For industrial applications**, use actual measured process flow rates from equipment datasheets and add a safety margin of 20–25% for peak variability.

The result is your required flow rate in litres per minute (LPM) or cubic metres per hour (m³/hr).

## Step 2 — Calculate Total Dynamic Head (TDH)

Head is the total pressure the pump must overcome to move liquid from the pit to the discharge point. Undershooting head means the pump runs but delivers insufficient flow.

TDH = Static Head + Friction Losses + Velocity Head

**Static head** is the vertical distance (in metres) from the water surface in the sump to the highest point of the discharge pipe.

**Friction losses** are caused by resistance as water moves through pipes, bends, and fittings:
- Use the Hazen-Williams equation or a friction loss table for the pipe diameter and material
- Each 90° elbow adds equivalent pipe length — typically 1.5–2 m equivalent length for 50mm pipe
- Each check valve adds approximately 1.5–3 m equivalent length
- Longer runs and smaller diameters increase friction losses significantly

**Velocity head** is usually small (0.05–0.2 m) and can be included as a buffer.

Add 10–15% to your calculated TDH as a safety margin to account for pipe ageing, scaling, and variability.

## Step 3 — Plot on the Performance Curve

Every pump manufacturer publishes a performance curve — a graph showing flow rate on the X-axis and head on the Y-axis. Plot your required flow rate and TDH as a point on the graph. The pump you select must have its best efficiency point (BEP) close to this operating point.

A pump running far from its BEP — either because flow is too high or too low relative to head — consumes excess energy and wears faster. The performance curve tells you exactly where the pump will operate; use it.

## Step 4 — Verify Solid Handling

Confirm the pump's maximum permissible solid size matches your waste stream. For domestic sewage, a 35–50mm solid passage is typical. For commercial buildings where non-standard waste is likely, 50mm minimum. For industrial or municipal applications, 50–70mm.

If fibrous waste (rags, wipes, textiles) is present in any quantity, a cutter pump is required — no impeller clearance specification will handle fibrous material reliably without the cutting mechanism.

## Step 5 — Select Motor Power

Once you have flow rate and TDH, the pump performance curve will indicate which motor power (HP) delivers your required operating point within the efficient range. Do not select the next HP up simply for comfort — oversizing creates the problems described above.

**Approximate HP guide:**

| Application | Typical HP |
|---|---|
| Single residential bathroom, short discharge | 0.5–1 HP |
| 2–3 bathroom residence or small commercial | 1–1.5 HP |
| Multi-floor commercial building | 2–3 HP |
| Municipal lift station (small) | 3–7.5 HP |
| Industrial / large-scale STP transfer | 7.5–15 HP |

## Step 6 — Confirm Phase and Power Supply

Single-phase supply supports pumps up to approximately 2 HP in most residential installations. Three-phase is required for higher HP ratings and is strongly preferred for any pump running in continuous duty — better motor efficiency, lower heat generation, longer service life.

Confirm the available power supply before finalising pump selection.

## Common Sizing Mistakes

**Using total volume instead of flow rate** — a sump holding 500 litres is irrelevant to sizing. What matters is how fast liquid enters and the required discharge rate.

**Ignoring friction losses** — a 10m static head installation with 30m of discharge pipe has significantly more than 10m TDH once friction is calculated.

**Sizing for current occupancy, not design occupancy** — a building at 30% occupancy during commissioning will eventually reach 100%.

**Adding HP "for safety"** — oversizing is as problematic as undersizing. Use the performance curve, not gut feel.

---

## Related reading

- [How to Select a Submersible Pump with the Right Flow Rate and Head Height](how-to-select-a-submersible-pump-with-the-right-flow-rate-and-head-height.md)
- [A Beginner's Guide to Understanding Sewage Pump Flow Rates](a-beginners-guide-to-understanding-sewage-pump-flow-rates.md)
- [Submersible Pump Range](best-submersible-pump.md)
- [Dewatering Pump](dewatering-pump.md)
