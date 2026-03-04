# THOR
Thorium Heat &amp; Open Reactor — open-source conceptual reference architecture for a 10MWt Liquid Fluoride Thorium Reactor. Passive freeze-plug safety, 300yr waste vs 300,000yr, 4kg fuel/yr vs 35,000 tonnes coal. CC0. No patents. Free forever. #ThoriumNow

# T.H.O.R.

## Thorium Heat and Open Reactor

**Disclosure Date: March 3, 2026 — This publication establishes prior art under 35 U.S.C. § 102 and international equivalents.**

**License: CC0 / Public Domain — The door is open. No patents. No toll. Ever.**

> **IMPORTANT:** This is a conceptual reference architecture, not a construction manual. Actual nuclear reactor design, construction, and operation requires credentialed nuclear engineers, institutional infrastructure, and regulatory approval from applicable authorities (NRC, IAEA, and national equivalents). Nothing in this repository constitutes instructions for constructing a nuclear device.

-----

## The Mission

In 1965, scientists at Oak Ridge National Laboratory switched on a Molten Salt Reactor and ran it for four years. It worked. It was safe. It produced no weapons-grade material. And in 1972 it was shut down — not because it failed, but because it didn’t produce plutonium for nuclear weapons. The lead engineer, Alvin Weinberg, was fired for pushing it too hard.

The patents expired. The knowledge became public domain. And for fifty years, the energy industry kept building the same reactors that produce 300,000-year radioactive waste and can melt down when they lose power.

T.H.O.R. exists to make sure that when engineers and institutions are finally ready to take thorium seriously, they find no patent wall waiting for them. This conceptual framework is free. It belongs to everyone. No corporation can change that now.

I am a night shift machinist. I graduated Summa Cum Laude in 2024 while working full-time for six years. These ideas have been building up for a long time. T.H.O.R. is the fourth release in the Open Source Patents project — following FCK-U, REVOLT, and A.I.R.-U. — because if an idea can help humanity, it belongs to humanity.

-----

## Why Thorium?

### The Numbers That End the Argument

|Comparison                |Coal Plant     |Conventional Nuclear|T.H.O.R. (10 MWt)|
|--------------------------|---------------|--------------------|-----------------|
|Annual fuel consumption   |~35,000 tonnes |~30 tonnes uranium  |~4 kg thorium    |
|Waste hazard period       |Permanent (CO2)|300,000 years       |~300 years       |
|Can melt down?            |N/A            |Yes                 |No               |
|Produces weapons material?|No             |Yes — plutonium     |No               |
|Homes powered             |~3,500         |~3,500              |~3,500           |

**4 kilograms of thorium per year.** That is the fuel requirement for a reactor powering 3,500 homes continuously. A nine-million-to-one fuel mass advantage over coal.

### The Waste Problem — Solved

Conventional nuclear waste stays dangerously radioactive for 300,000 years. No human institution has ever survived 300,000 years. There is no credible plan for managing something that long.

Thorium MSR waste reaches background radiation levels in approximately 300 years. Human civilization has maintained libraries, legal systems, and institutional records for 300 years. That is a manageable timescale.

### It Cannot Melt Down

Every nuclear disaster in history — Three Mile Island, Chernobyl, Fukushima — involved solid fuel overheating. In a molten salt reactor, the fuel is already liquid. The word meltdown does not apply.

-----

## The Freeze Plug — Passive Safety

The most important safety feature of the LFTR design requires no pumps, no backup power, and no operator action:

1. A plug of frozen salt seals the drain at the bottom of the reactor
1. A small electric fan keeps the plug frozen during operation
1. **On loss of power from any cause:** fan stops → plug melts in ~10 minutes → fuel drains by gravity into subcritical tanks → fission stops permanently
1. No operator needed. No backup power needed. No pumps needed.

**Fukushima happened because backup generators were flooded.** In a molten salt reactor, flooding the backup generators makes the reactor safer — because loss of power triggers the automatic safe drain.

The reactor fails into its safest possible state as a direct consequence of any power loss. This is the opposite of every light water reactor ever built.

-----

## Physics Reference

### Thorium Fuel Cycle

```
Th-232 + neutron  →  Th-233
Th-233            →  Pa-233 + β⁻  (half-life: 22 minutes)
Pa-233            →  U-233  + β⁻  (half-life: 27 days)
U-233  + neutron  →  fission products + 2.49 neutrons + ~200 MeV
```

U-233 produces 2.29 neutrons per absorption in a thermal spectrum — above the 2.0 threshold required for breeding. U-233 is the **only** fissile material that achieves this in a thermal reactor. The thorium reactor breeds more fuel than it consumes.

### Reference Salt: FLiBe (2LiF-BeF2)

|Property                |Value                              |
|------------------------|-----------------------------------|
|Melting point           |459°C                              |
|Boiling point           |1430°C                             |
|Operating temperature   |650-750°C                          |
|Thermodynamic efficiency|~42% (vs ~33% conventional nuclear)|
|Viscosity at 700°C      |~6 mPa·s (water-like)              |

### 10 MWt Module Reference

|Parameter            |Value                              |
|---------------------|-----------------------------------|
|Thermal output       |10 MWt                             |
|Electrical output    |~4.2 MWe                           |
|Core volume          |~1,250 liters                      |
|Core diameter        |~134cm                             |
|Homes powered        |~3,500 continuous                  |
|Thorium consumed/year|~4 kg                              |
|Waste hazard period  |~300 years                         |
|Passive safety       |Freeze plug drain — no power needed|

-----

## Decay Heat After Shutdown

```
P_decay(t) = 0.066 × P₀ × t⁻⁰·²   (t in seconds)
```

|Time After Shutdown|Decay Heat (% of rated)|
|-------------------|-----------------------|
|1 second           |6.60%                  |
|1 minute           |2.91%                  |
|1 hour             |1.28%                  |
|1 day              |0.68%                  |
|1 week             |0.46%                  |
|30 days            |0.34%                  |

Decay heat dissipates passively into drain tank geometry. No active cooling required at any point post-drain.

-----

## Repository Contents

```
/docs
    THOR_Plain_English.pdf          — Guide for general readers
    THOR_Patent_Disclosure.pdf      — Full prior art disclosure
    THOR_Technical_Brief.pdf        — Reference data for engineers and institutions

/simulation
    thor_simulation.py              — Physics model — fuel cycle, thermal properties,
                                      passive safety, scaling estimates

DISCLOSURE_DATE.txt                 — Timestamped prior art record
README.md                           — This file
LICENSE                             — CC0 1.0 Universal
```

-----

## License — Public Domain (CC0)

This disclosure is made with the explicit intent of placing all described conceptual elements into the public domain under the Creative Commons Zero (CC0) license. The originator expressly waives all patent rights.

Any person, institution, government, or company worldwide is free to use, build upon, publish, or implement these concepts without restriction, royalty, or attribution.

No entity may obtain valid patent protection for the concepts described herein after the date of this publication.

**DISCLAIMER:** Conceptual reference only. Actual reactor construction requires credentialed nuclear engineers, NRC/IAEA regulatory approval, and institutional infrastructure.

-----

## Part of the Open Source Patents Project

|System   |Domain         |Core Innovation                           |
|---------|---------------|------------------------------------------|
|FCK-U    |Ground vehicle |Cabin separation from crash + battery fire|
|REVOLT   |Emergency power|3D-printable wind turbine — $30 build cost|
|A.I.R.-U.|Aviation safety|Printable ballistic recovery system       |
|T.H.O.R. |Grid energy    |Open thorium MSR reference architecture   |

Four domains. Four open-source contributions. One night shift machinist. All free. Forever.

**X:** [@OpnSorcePatents](https://twitter.com/OpnSorcePatents)

`#OpenSourceEnergy` `#THOR` `#ThoriumNow` `#OpenSourceSafety`

-----

*Built on days off. Released for free. No exceptions.*
