# Part 101 MOS — Quick reference for tethering in a no-fly zone

> Plain-English notes from reading the in-force Part 101 (Unmanned Aircraft and
> Rockets) Manual of Standards compilation (registered as F2026C00984, read in
> November 2026). This is **not** legal advice. The MOS is amended regularly —
> always check the current compilation on the Federal Register of Legislation
> before relying on a clause number or a figure.

Last updated: 22 Nov 2026

---

## 1. The clauses that matter

| Clause | What it says (plain English) |
|---|---|
| 4.02 | Defines the **no-fly zone of a controlled aerodrome**: below 400 ft and either (a) within 3 NM in any direction of the measurement point of any runway, or (b) within the approach and departure paths in 4.05, even beyond 3 NM. The black, grey and cross-hatched areas are defined by reference to 4.05. |
| 4.03(1) | You must not conduct RPA operations or fly an RPA in that zone, subject to the exceptions in 4.03. |
| 4.03(2) | **Exception for tethering:** a certified RPA operator, or its remote pilot, may conduct a tethered operation in the zone if it is done in accordance with 4.04. |
| 4.03(3)–(7) | Other exceptions: exclusively indoor operations; micro RPA and model aircraft of 250 g or less (but not into an approach/departure path or the aerodrome boundary); defined unmanned aircraft operating under an approval or permission. |
| 4.04(3)(a) | Tether **no longer than 150 ft**. |
| 4.04(3)(b) | RPA **not operated higher than 150 ft above the aerodrome elevation** (the aerodrome obstacle limitation data can be used to find the elevation). |
| 4.04(3)(c) | The operation is conducted in accordance with the operator's **documented practices and procedures**. |
| 4.04(3)(d)–(e) | **Notify ATC** before take-off and fly in accordance with any ATC instructions. |
| 4.04(3)(f) | (i) Fly within the **grey** area; or (ii) if flying in the **black** area, not within **3 NM** of the measurement point of any runway. |
| 4.05(2) | Approach and departure path, up to 400 ft: the runway/runway strip from the ground up; **black** from the ground up to **7 km** from the end of the runway strip; **cross-hatched** (7 to 8.5 km) from **300 ft**; **grey** from **150 ft** (heights referenced to aerodrome elevation). |
| 4.05(3) | **Black area** = (a) trapezoids whose short side is the end of a nominal **100 m wide** runway strip, widening at **15°** either side to **8.5 km**, plus (b) a **rectangle 500 m either side of the runway centreline**, overlying the runway strip until it meets the trapezoids. |
| 4.05(4) | **Grey area** = **3 NM in all directions** from the measurement point. |
| 4.05 note | For multi-runway aerodromes the same rules apply per runway: grey areas overlap, and where runways intersect what would be grey becomes black. |
| 9.05(3) | **Non-controlled aerodromes:** same tether (150 ft), height (150 ft above aerodrome elevation), documented-procedures and grey/black rules as 4.04 — but no ATC notification. |
| 9.05(4) | **Helicopter landing sites:** tether no longer than 150 ft; RPA at least **465 m** from the central axis of the HLS no-fly zone; flown within VLOS; documented procedures. |
| 10A.01 | **Significant changes** to documented practices and procedures need CASA's prior approval. |

---

## 2. Geometry at a glance

| Feature | Dimension | Clause |
|---|---|---|
| Runway strip (nominal) | 100 m wide | 4.05(3)(a) |
| Black rectangle at the runway | 500 m **either side** of the centreline (1 km total width) | 4.05(3)(b) |
| Black approach/departure splay | 15° either side from the ends of the strip | 4.05(3)(a) |
| Black — no-fly from the ground up | To 7 km from the end of the runway strip | 4.05(2)(b)(i) |
| Cross-hatched | 7–8.5 km from the end of the strip; path applies from 300 ft | 4.05(2)(b)(ii) |
| Grey | 3 NM (about 5.56 km) from the measurement point; path applies from 150 ft | 4.05(4), 4.05(2)(c) |

**Use the clause text, not the figure.** The MOS figure is labelled as showing
the matters but with a shape that only illustrates them. Read dimensions from
4.05, and check any number you copy from a figure or an older manual against it.

---

## 3. Tether length

```
T = a − (b − c)

a = maximum tether length (150 ft)                       MOS 4.04(3)(a)
b = elevation of the tether ground point (ft AMSL)
c = aerodrome elevation / ARP elevation (ft AMSL)
```

Then **cap T at 150 ft**. The formula comes from the height limit in
4.04(3)(b): ground elevation + tether length − aerodrome elevation must not
exceed 150 ft. When the ground point is *below* the aerodrome, the formula gives
more than 150 ft, but 4.04(3)(a) still limits the tether itself to 150 ft.

Worked examples (illustrative numbers only):

| Case | b (ft AMSL) | c (ft AMSL) | T = 150 − (b − c) | Maximum tether | RPA height above aerodrome at that tether |
|---|---:|---:|---:|---:|---:|
| A. Ground point above the aerodrome | 50 | 20 | 120 | 120 ft | 150 ft |
| B. Ground point well below the aerodrome | 10 | 60 | 200 | **150 ft (capped)** | 100 ft |
| C. Ground point slightly below | 10 | 14 | 154 | **150 ft (capped)** | 146 ft |
| D. Ground point above, higher site | 38 | 15 | 127 | 127 ft | 150 ft |
| E. Much higher ground | 320 | 140 | −30 | **Cannot be conducted** | — |

Practical points:

- Convert metres to feet (1 m = 3.28 ft) and round the ground elevation **up** —
  a shorter tether is the conservative error.
- Take the ground elevation from **two sources** and use the more conservative
  one. Mapping tools can disagree for the same location (CASA noted that Google
  Earth web and desktop can differ), so confirm the height in AMSL on site
  before each tethered operation.
- Take the aerodrome elevation from ERSA or the OLS data, and record which
  edition you used.

---

## 4. Can I fly this site tethered? (decision flow)

1. **Find every runway measurement point** of the nearest controlled
   aerodrome(s). For multi-runway aerodromes, check each runway.
2. **Is the site inside the no-fly zone?** Within 3 NM of a measurement point,
   or inside an approach/departure path (black to 7 km, cross-hatched to 8.5 km).
   If not, the no-fly-zone rules don't apply — check other airspace and standard
   Part 101 rules.
3. **Black area within 3 NM of a measurement point?** Tethered operations are
   **not permitted** (4.04(3)(f)(ii)). Stop.
4. **Grey area, or black area beyond 3 NM?** Continue (4.04(3)(f)).
5. **Calculate the maximum tether length** (section 3). If the answer is zero or
   negative, the operation cannot be conducted at that site.
6. **Check the procedure items** in your approved manual: ATC notified before
   take-off and instructions followed (4.04(3)(d)–(e)), NOTAM raised, risk
   assessment and flight authorisation done, radio monitored, people controls in
   place.
7. **Military controlled aerodrome?** Follow your manual: a valid letter of
   agreement permitting tethered operations and a clearance before take-off.
