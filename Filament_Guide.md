# 🧵 Filament Guide & Use Cases

Choosing the right material is just as important as the hardware itself. Before selecting a filament, you must first identify the **job requirements** for the part you are printing. Will the part be exposed to higher temperatures where it might suffer from heat creep? Will it face significant mechanical stress along its layer lines? Does it need to withstand prolonged UV exposure from sunlight, or harsh chemicals and solvents?

**Example Scenario:** If you are printing a toolhead carriage for an enclosed 3D printer (like the **Alembic**), the part will live inside a heated chamber (often 60°C+) and sit directly above a hotend. Using PLA here is a guaranteed failure; it will soften and warp due to heat creep. Instead, the job requirements dictate a material with a high glass transition temperature and good rigidity, such as **ABS**, **ASA**, or **CF-PC**.

Below is a breakdown of common filament types used in the 3D printing ecosystem and the broader maker community, categorized to help you match the material to your specific job requirements.

<br><hr><br>


## 📑 Material Index

| Category | Materials |
| :--- | :--- |
| **🟢 Standard Plastics** | [PLA](#pla-polylactic-acid), [PETG](#petg-polyethylene-terephthalate-glycol), [PCTG](#pctg), [PP](#pp-polypropylene) |
| **🟡 Advanced Plastics** | [ABS](#abs-acrylonitrile-butadiene-styrene), [ASA](#asa-acrylonitrile-styrene-acrylate), [PC-ABS](#pc-abs-polycarbonate--abs-blend) |
| **🟠 Engineering Grade** | [PC](#pc-polycarbonate), [PA Series](#pa-nylon-series), [PAHT](#paht-high-temperature-nylon), [PPA](#ppa-polyphthalamide--high-performance-polyamide), [PPS](#pps-polyphenylene-sulfide), [PET](#pet-polyethylene-terephthalate), [PEI](#pei-polyetherimide--ultem), [PSU](#psu-polysulfone), [PEEK](#peek-polyether-ether-ketone) |
| **🔴 Flexible Materials** | [TPU](#tpu-thermoplastic-polyurethane), [PEBA](#peba-polyether-block-amide) |
| **🟣 Additives & Composites** | [CF Filled](#carbon-fiber-filled-cf), [GF Filled](#glass-fiber-filled-gf), [Co-Extrusion Core](#co-extrusion-core-filaments), [Aero / LW](#aero--lightweight-lw-filaments-eg-lw-pla-lw-asa), [Wood Filled](#wood-filled), [Glitter / Sparkle](#glitter--sparkle), [Color Changing](#color-changing), [Continuous Thread](#continuous-thread) |

<br><hr><br>

## 📊 Understanding Material Data Sheets (TDS)

When evaluating a filament's Technical Data Sheet (TDS), you will often encounter a standardized list of mechanical and thermal properties. Here is an example of what those values look like (using data from [Sirayatech ABS-HT-HF](https://amzn.to/3RedMT4) as an example), along with a layman's explanation of what each test actually means for your 3D printed parts.

| Property | Typical Value | Test Method / Notes | Layman's Description |
| :--- | :--- | :--- | :--- |
| **Tensile Stress at Break** | 39 MPa | ASTM D638 | How much pulling force the material can take before it completely snaps. |
| **Young's Modulus** | 2400 MPa | ASTM D638 | The material's stiffness or rigidity. A higher number means it resists bending and stretching. |
| **Elongation at Break** | 6.5 % | ASTM D638 | How much the material stretches (like a rubber band) before it finally snaps. |
| **Charpy Impact Strength** | 21.5 KJ/m² | ISO 179 | How well the material absorbs a sudden shock or heavy impact (e.g., dropping a part on concrete). |
| **Bending Strength** | 68 MPa | ISO 179 | How much weight or force the material can support while spanning a gap before it cracks. |
| **Bending Modulus** | 2490 MPa | ISO 179 | The material's tendency to flex under a load. Higher values mean the part is stiffer and harder to bend. |
| **Vicat Softening Temperature** | 103 °C | ISO 306 | The temperature at which the material loses its structural integrity and begins to soften on the surface. |
| **Glass Transition Temperature (Tg)** | 101 °C | ASTM D3418 | The critical temperature where the plastic stops acting like a hard solid and becomes soft, rubbery, and prone to severe heat creep/warping. |
| **Shore Hardness D** | 78 | ISO 7619 | A measure of surface hardness and resistance to indentation (often used to rate flexibles, but Shore D applies to rigid/semi-rigid plastics). |
| **Melting Point** | 220 °C | ASTM D3418 | The temperature at which the plastic turns into a printable fluid for extrusion. |
| **HDT (Heat Deflection Temp) Method A** | 99 °C | 1.80 MPa load | The temperature at which a part will start to bend and deform while under a heavy mechanical load. |
| **HDT (Heat Deflection Temp) Method B** | 101 °C | 0.45 MPa load | The temperature at which a part will start to bend and deform while under a lighter mechanical load. |

<br><hr><br>

## 🟢 Standard Plastics

These are your everyday materials, ideal for rapid prototyping, display models, and low-stress parts.

> [!NOTE]
> The property values provided below are estimates and may not reflect specific products. Please reference the Technical Data Sheet (TDS) for your explicit filament choice.

### <u>PLA (Polylactic Acid)</u>
* <u>**Primary Use Case:**</u> Prototyping, aesthetic prints, structural parts that stay at room temperature.
* <u>**Pros:**</u> Extremely easy to print, highly rigid, no warping, eco-friendly.
* <u>**Cons:**</u> Very low glass transition temperature (~60°C); will deform in hot cars or near printer hotends. Brittle under impact.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~45-60 MPa |
| **Young's Modulus** | ~2700-3300 MPa |
| **Elongation at Break** | ~3-5 % |
| **Charpy Impact Strength** | ~15-20 KJ/m² |
| **Bending Strength** | ~75-85 MPa |
| **Bending Modulus** | ~2800-3200 MPa |
| **Vicat Softening Temperature** | ~60-65 °C |
| **Glass Transition Temperature (Tg)** | ~55-60 °C |
| **Shore Hardness D** | ~80-83 |
| **Melting Point** | ~150-180 °C |
| **HDT Method A (1.80 MPa)** | ~52 °C |
| **HDT Method B (0.45 MPa)** | ~55 °C |

</details>

---

### <u>PETG (Polyethylene Terephthalate Glycol)</u>
* <u>**Primary Use Case:**</u> Functional parts, mechanical assemblies, water-resistant containers.
* <u>**Pros:**</u> Better temperature resistance than PLA, highly impact resistant, flexes rather than shattering.
* <u>**Cons:**</u> Prone to stringing, can over-adhere to certain build plates (like glass or PEI).

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~50 MPa |
| **Young's Modulus** | ~2000-2200 MPa |
| **Elongation at Break** | ~20-30 % |
| **Charpy Impact Strength** | ~60-80 KJ/m² |
| **Bending Strength** | ~65-75 MPa |
| **Bending Modulus** | ~2100 MPa |
| **Vicat Softening Temperature** | ~85 °C |
| **Glass Transition Temperature (Tg)** | ~80 °C |
| **Shore Hardness D** | ~76 |
| **Melting Point** | ~230 °C |
| **HDT Method A (1.80 MPa)** | ~68 °C |
| **HDT Method B (0.45 MPa)** | ~75 °C |

</details>

---

### <u>PCTG</u>
* <u>**Primary Use Case:**</u> High-impact functional parts, tough mechanical components.
* <u>**Pros:**</u> Engineered as an advanced successor to PETG. It offers significantly higher impact strength (toughness), improved optical clarity, and slightly better temperature resistance, making it superior for parts that will take a beating.
* <u>**Cons:**</u> Can be more expensive and slightly more difficult to source than PETG.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~45-50 MPa |
| **Young's Modulus** | ~1800-2000 MPa |
| **Elongation at Break** | ~30-40 % |
| **Charpy Impact Strength** | ~80-100+ KJ/m² |
| **Bending Strength** | ~60-70 MPa |
| **Bending Modulus** | ~1900 MPa |
| **Vicat Softening Temperature** | ~88 °C |
| **Glass Transition Temperature (Tg)** | ~85 °C |
| **Shore Hardness D** | ~76 |
| **Melting Point** | ~240 °C |
| **HDT Method A (1.80 MPa)** | ~72 °C |
| **HDT Method B (0.45 MPa)** | ~78 °C |

</details>

---

### <u>PP (Polypropylene)</u>
* <u>**Primary Use Case:**</u> Living hinges, chemical-resistant containers, lightweight parts.
* <u>**Pros:**</u> Incredible fatigue resistance (great for hinges), very low density, high chemical resistance.
* <u>**Cons:**</u> Extremely prone to warping, very difficult to adhere to standard build plates (requires specialized tape or adhesives).

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~25-30 MPa |
| **Young's Modulus** | ~1000-1400 MPa |
| **Elongation at Break** | ~100-200 % |
| **Charpy Impact Strength** | ~40-60 KJ/m² |
| **Bending Strength** | ~35-45 MPa |
| **Bending Modulus** | ~1100 MPa |
| **Vicat Softening Temperature** | ~135 °C |
| **Glass Transition Temperature (Tg)** | ~-10 °C |
| **Shore Hardness D** | ~65 |
| **Melting Point** | ~160 °C |
| **HDT Method A (1.80 MPa)** | ~60 °C |
| **HDT Method B (0.45 MPa)** | ~100 °C |

</details>

<br><hr><br>

## 🟡 Advanced Plastics

These materials sit between standard and true engineering plastics. They offer elevated thermal resistance and are commonly used for 3D printer structural parts (like the **Alembic Toolhead** or **Pneuma** mounts).

> [!NOTE]
> The property values provided below are estimates and may not reflect specific products. Please reference the Technical Data Sheet (TDS) for your explicit filament choice.


### <u>ABS (Acrylonitrile Butadiene Styrene)</u>
* <u>**Primary Use Case:**</u> Printer parts, automotive components, durable enclosures.
* <u>**Pros:**</u> Excellent temperature resistance (~100°C), easy to sand/smooth (can be acetone smoothed), and highly durable. Very cost-effective.
* <u>**Cons:**</u> **Emits toxic styrene fumes during printing (requires heavy ventilation/filtration).** Prone to severe warping and requires a heated enclosure. Poor UV resistance (will yellow and become brittle in sunlight).

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~40-45 MPa |
| **Young's Modulus** | ~2000-2200 MPa |
| **Elongation at Break** | ~15-25 % |
| **Charpy Impact Strength** | ~30-40 KJ/m² |
| **Bending Strength** | ~65-75 MPa |
| **Bending Modulus** | ~2100 MPa |
| **Vicat Softening Temperature** | ~105 °C |
| **Glass Transition Temperature (Tg)** | ~100-105 °C |
| **Shore Hardness D** | ~75 |
| **Melting Point** | ~220-240 °C |
| **HDT Method A (1.80 MPa)** | ~85 °C |
| **HDT Method B (0.45 MPa)** | ~95 °C |

</details>

---

### <u>ASA (Acrylonitrile Styrene Acrylate)</u>
* <u>**Primary Use Case:**</u> Outdoor fixtures, printer parts, automotive exterior components.
* <u>**Pros:**</u> Engineered specifically as a modern successor to ABS. It retains all the excellent thermal and mechanical benefits of ABS, but adds exceptional UV resistance (it will not yellow or degrade in sunlight) and is often slightly less prone to warping during printing.
* <u>**Cons:**</u> **Emits toxic styrene fumes during printing (requires heavy ventilation/filtration).** Still prone to warping and requires a heated enclosure. Generally slightly more expensive than ABS.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~40-45 MPa |
| **Young's Modulus** | ~2000-2300 MPa |
| **Elongation at Break** | ~15-25 % |
| **Charpy Impact Strength** | ~35-45 KJ/m² |
| **Bending Strength** | ~65-75 MPa |
| **Bending Modulus** | ~2200 MPa |
| **Vicat Softening Temperature** | ~105 °C |
| **Glass Transition Temperature (Tg)** | ~100-105 °C |
| **Shore Hardness D** | ~76 |
| **Melting Point** | ~220-240 °C |
| **HDT Method A (1.80 MPa)** | ~86 °C |
| **HDT Method B (0.45 MPa)** | ~96 °C |

</details>

---

### <u>PC-ABS (Polycarbonate / ABS Blend)</u>
* <u>**Primary Use Case:**</u> Enclosures, durable consumer goods, high-impact structural parts.
* <u>**Pros:**</u> Combines the high impact strength and heat resistance of PC with the better printability of ABS. Less prone to warping than pure PC.
* <u>**Cons:**</u> **Emits toxic styrene fumes during printing (requires heavy ventilation/filtration).** Still requires a heated enclosure. Lower heat resistance than pure PC.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~45-55 MPa |
| **Young's Modulus** | ~2200-2500 MPa |
| **Elongation at Break** | ~10-20 % |
| **Charpy Impact Strength** | ~45-60 KJ/m² |
| **Bending Strength** | ~75-85 MPa |
| **Bending Modulus** | ~2400 MPa |
| **Vicat Softening Temperature** | ~115 °C |
| **Glass Transition Temperature (Tg)** | ~110 °C |
| **Shore Hardness D** | ~78 |
| **Melting Point** | ~240-260 °C |
| **HDT Method A (1.80 MPa)** | ~95 °C |
| **HDT Method B (0.45 MPa)** | ~105 °C |

</details>

<br><hr><br>

## 🟠 Engineering Grade Plastics

These materials are required for the highest-heat and highest-stress environments due to their extreme thermal and mechanical properties.

> [!NOTE]
> The property values provided below are estimates and may not reflect specific products. Please reference the Technical Data Sheet (TDS) for your explicit filament choice.


### <u>PC (Polycarbonate)</u>
* <u>**Primary Use Case:**</u> High-heat, high-stress mechanical parts.
* <u>**Pros:**</u> Incredible impact strength and very high temperature resistance (~110°C+).
* <u>**Cons:**</u> **Emits harmful VOCs (including BPA) during printing (requires ventilation/filtration).** Extremely difficult to print. Requires very high hotend temperatures and a heated chamber.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~60-70 MPa |
| **Young's Modulus** | ~2300-2600 MPa |
| **Elongation at Break** | ~5-15 % |
| **Charpy Impact Strength** | ~60-80 KJ/m² |
| **Bending Strength** | ~90-100 MPa |
| **Bending Modulus** | ~2500 MPa |
| **Vicat Softening Temperature** | ~145 °C |
| **Glass Transition Temperature (Tg)** | ~145-150 °C |
| **Shore Hardness D** | ~82 |
| **Melting Point** | ~280-310 °C |
| **HDT Method A (1.80 MPa)** | ~110 °C |
| **HDT Method B (0.45 MPa)** | ~130 °C |

</details>

---

### <u>PA (Nylon) Series</u>
* <u>**Primary Use Case:**</u> Gears, bearings, high-wear mechanical components.
* <u>**Pros:**</u> Incredible wear resistance, low friction, high impact strength.
* <u>**Cons:**</u> **Emits harmful VOCs and UFPs including caprolactam (requires ventilation).** Extremely hygroscopic (must be printed dry), prone to warping, low stiffness unless fiber-filled.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~50-60 MPa (Dry) |
| **Young's Modulus** | ~1500-2500 MPa (Dry) |
| **Elongation at Break** | ~50-100 % |
| **Charpy Impact Strength** | ~50-80 KJ/m² |
| **Bending Strength** | ~60-80 MPa |
| **Bending Modulus** | ~1800 MPa |
| **Vicat Softening Temperature** | ~160 °C |
| **Glass Transition Temperature (Tg)** | ~50-60 °C |
| **Shore Hardness D** | ~75 |
| **Melting Point** | ~220-260 °C |
| **HDT Method A (1.80 MPa)** | ~60 °C |
| **HDT Method B (0.45 MPa)** | ~120 °C |

</details>

---

### <u>PAHT (High-Temperature Nylon)</u>
* <u>**Primary Use Case:**</u> High-temperature structural parts.
* <u>**Pros:**</u> Maintains structural integrity at much higher temperatures than standard PA, excellent chemical resistance.
* <u>**Cons:**</u> **Emits harmful VOCs and UFPs (requires ventilation).** Very hygroscopic, requires high extrusion temperatures.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~60-75 MPa |
| **Young's Modulus** | ~2500-3000 MPa |
| **Elongation at Break** | ~15-30 % |
| **Charpy Impact Strength** | ~40-60 KJ/m² |
| **Bending Strength** | ~85-100 MPa |
| **Bending Modulus** | ~2700 MPa |
| **Vicat Softening Temperature** | ~200 °C |
| **Glass Transition Temperature (Tg)** | ~80-90 °C |
| **Shore Hardness D** | ~80 |
| **Melting Point** | ~260-280 °C |
| **HDT Method A (1.80 MPa)** | ~90 °C |
| **HDT Method B (0.45 MPa)** | ~160 °C |

</details>

---

### <u>PPA (Polyphthalamide / High-Performance Polyamide)</u>
* <u>**Primary Use Case:**</u> Metal replacement parts, automotive under-the-hood components.
* <u>**Pros:**</u> Superior thermal performance and stiffness compared to standard aliphatic nylons (PA), lower moisture absorption.
* <u>**Cons:**</u> **Emits harmful VOCs at high processing temperatures (requires ventilation).** Requires extremely high printing temperatures and a heated chamber, expensive.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~70-85 MPa |
| **Young's Modulus** | ~3000-3500 MPa |
| **Elongation at Break** | ~5-15 % |
| **Charpy Impact Strength** | ~30-50 KJ/m² |
| **Bending Strength** | ~100-120 MPa |
| **Bending Modulus** | ~3200 MPa |
| **Vicat Softening Temperature** | ~250 °C |
| **Glass Transition Temperature (Tg)** | ~120-130 °C |
| **Shore Hardness D** | ~84 |
| **Melting Point** | ~300-310 °C |
| **HDT Method A (1.80 MPa)** | ~110 °C |
| **HDT Method B (0.45 MPa)** | ~180 °C |

</details>

---

### <u>PPS (Polyphenylene Sulfide)</u>
* <u>**Primary Use Case:**</u> Aerospace, automotive, and extreme chemical environments.
* <u>**Pros:**</u> Outstanding chemical resistance (insoluble in almost any known solvent under 200°C), inherent flame retardancy, very high continuous use temperature.
* <u>**Cons:**</u> **Emits highly toxic sulfur compounds and VOCs during printing (requires heavy ventilation/filtration).** Very difficult to print, requires highly specialized high-temperature hardware, very expensive.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~70-80 MPa |
| **Young's Modulus** | ~3500-4000 MPa |
| **Elongation at Break** | ~2-5 % |
| **Charpy Impact Strength** | ~20-30 KJ/m² |
| **Bending Strength** | ~110-130 MPa |
| **Bending Modulus** | ~3800 MPa |
| **Vicat Softening Temperature** | ~270 °C |
| **Glass Transition Temperature (Tg)** | ~90 °C |
| **Shore Hardness D** | ~85 |
| **Melting Point** | ~285 °C |
| **HDT Method A (1.80 MPa)** | ~105 °C |
| **HDT Method B (0.45 MPa)** | ~160 °C |

</details>

---

### <u>PET (Polyethylene Terephthalate)</u>
* <u>**Primary Use Case:**</u> High-strength mechanical parts, dimensionally stable structural components (often fiber-filled).
* <u>**Pros:**</u> Extremely high stiffness and tensile strength, excellent chemical resistance, very low moisture absorption compared to nylons. Can be annealed for extreme heat resistance.
* <u>**Cons:**</u> Harder to print than PETG, prone to crystallization/opacity changes depending on cooling rate.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~55-65 MPa |
| **Young's Modulus** | ~2600-3000 MPa |
| **Elongation at Break** | ~10-20 % |
| **Charpy Impact Strength** | ~30-50 KJ/m² |
| **Bending Strength** | ~80-95 MPa |
| **Bending Modulus** | ~2800 MPa |
| **Vicat Softening Temperature** | ~150 °C |
| **Glass Transition Temperature (Tg)** | ~70-80 °C |
| **Shore Hardness D** | ~80 |
| **Melting Point** | ~250-260 °C |
| **HDT Method A (1.80 MPa)** | ~65 °C |
| **HDT Method B (0.45 MPa)** | ~100 °C |

</details>

---

### <u>PEI (Polyetherimide / Ultem)</u>
* <u>**Primary Use Case:**</u> Aerospace, medical, and extreme environment electrical components.
* <u>**Pros:**</u> Incredible inherent flame retardancy (V-0 rating), exceptional continuous use temperature (up to 170°C+), extremely high dielectric strength, and great chemical resistance.
* <u>**Cons:**</u> **Emits harmful VOCs at high processing temperatures (requires ventilation/filtration).** Extremely demanding to print. Requires hotend temperatures of 360-400°C and a very hot active heated chamber. Very expensive.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~90-105 MPa |
| **Young's Modulus** | ~3200-3500 MPa |
| **Elongation at Break** | ~5-10 % |
| **Charpy Impact Strength** | ~40-60 KJ/m² |
| **Bending Strength** | ~130-150 MPa |
| **Bending Modulus** | ~3300 MPa |
| **Vicat Softening Temperature** | ~215 °C |
| **Glass Transition Temperature (Tg)** | ~215-217 °C |
| **Shore Hardness D** | ~86 |
| **Melting Point** | ~Amorphous |
| **HDT Method A (1.80 MPa)** | ~200 °C |
| **HDT Method B (0.45 MPa)** | ~210 °C |

</details>

---

### <u>PSU (Polysulfone)</u>
* <u>**Primary Use Case:**</u> Medical devices, plumbing components, and applications requiring sterilization.
* <u>**Pros:**</u> High thermal stability, excellent resistance to hydrolysis (can withstand repeated steam sterilization/autoclaving), and good radiation resistance.
* <u>**Cons:**</u> **Emits harmful VOCs at high processing temperatures (requires ventilation/filtration).** Requires high extrusion temperatures and a heated chamber. Prone to internal stresses if not cooled slowly.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~70-80 MPa |
| **Young's Modulus** | ~2600-2800 MPa |
| **Elongation at Break** | ~5-10 % |
| **Charpy Impact Strength** | ~40-50 KJ/m² |
| **Bending Strength** | ~100-110 MPa |
| **Bending Modulus** | ~2700 MPa |
| **Vicat Softening Temperature** | ~190 °C |
| **Glass Transition Temperature (Tg)** | ~190 °C |
| **Shore Hardness D** | ~84 |
| **Melting Point** | ~Amorphous |
| **HDT Method A (1.80 MPa)** | ~175 °C |
| **HDT Method B (0.45 MPa)** | ~185 °C |

</details>

---

### <u>PEEK (Polyether Ether Ketone)</u>
* <u>**Primary Use Case:**</u> Metal replacement in aerospace, automotive, and high-performance engineering applications.
* <u>**Pros:**</u> The gold standard of polymer performance. Incredible mechanical strength, extreme temperature resistance (continuous use above 250°C), and near-universal chemical resistance.
* <u>**Cons:**</u> **Emits harmful VOCs during printing (requires heavy ventilation/filtration).** One of the most difficult materials to print. Requires extreme hotend temperatures (400°C+) and a highly controlled, high-temperature heated chamber. Exorbitantly expensive.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~95-105 MPa |
| **Young's Modulus** | ~3600-4000 MPa |
| **Elongation at Break** | ~15-25 % |
| **Charpy Impact Strength** | ~60-80 KJ/m² |
| **Bending Strength** | ~150-170 MPa |
| **Bending Modulus** | ~3800 MPa |
| **Vicat Softening Temperature** | ~315 °C |
| **Glass Transition Temperature (Tg)** | ~143-150 °C |
| **Shore Hardness D** | ~88 |
| **Melting Point** | ~343 °C |
| **HDT Method A (1.80 MPa)** | ~152 °C |
| **HDT Method B (0.45 MPa)** | ~200 °C |

</details>

<br><hr><br>

## 🔴 Flexible Materials

> [!NOTE]
> The property values provided below are estimates and may not reflect specific products. Please reference the Technical Data Sheet (TDS) for your explicit filament choice.

### <u>TPU (Thermoplastic Polyurethane)</u>
* <u>**Primary Use Case:**</u> Gaskets, vibration dampeners, flexible hinges, tires.
* <u>**Pros:**</u> Highly flexible, extreme layer adhesion, nearly indestructible.
* <u>**Cons:**</u> Difficult to print on standard Bowden setups; requires a well-constrained direct drive extruder (like the **Pestle** in direct-drive configuration). Must be printed slowly.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~30-40 MPa |
| **Young's Modulus** | ~50-150 MPa |
| **Elongation at Break** | ~400-600 % |
| **Charpy Impact Strength** | ~No Break |
| **Bending Strength** | ~N/A |
| **Bending Modulus** | ~N/A |
| **Vicat Softening Temperature** | ~80-100 °C |
| **Glass Transition Temperature (Tg)** | ~-30 to -40 °C |
| **Shore Hardness D** | ~40D-60D (90A-95A) |
| **Melting Point** | ~200-220 °C |
| **HDT Method A (1.80 MPa)** | ~N/A |
| **HDT Method B (0.45 MPa)** | ~N/A |

</details>

---

### <u>PEBA (Polyether Block Amide)</u>
* <u>**Primary Use Case:**</u> High-performance sporting goods, footwear, extremely durable flexible parts.
* <u>**Pros:**</u> Exceptional energy return, maintains flexibility even at very low temperatures, lower density than TPU.
* <u>**Cons:**</u> More difficult to print than TPU, highly hygroscopic, often more expensive.

<details>
<summary><b>View Material Properties (Rough Average)</b></summary>

| Property | Typical Value |
| :--- | :--- |
| **Tensile Stress at Break** | ~25-35 MPa |
| **Young's Modulus** | ~100-200 MPa |
| **Elongation at Break** | ~300-500 % |
| **Charpy Impact Strength** | ~No Break |
| **Bending Strength** | ~N/A |
| **Bending Modulus** | ~N/A |
| **Vicat Softening Temperature** | ~140 °C |
| **Glass Transition Temperature (Tg)** | ~-50 to -60 °C |
| **Shore Hardness D** | ~40D-55D |
| **Melting Point** | ~150-170 °C |
| **HDT Method A (1.80 MPa)** | ~N/A |
| **HDT Method B (0.45 MPa)** | ~N/A |

</details>

<br><hr><br>

## 🟣 Additives & Specialty Composites

### <u>Carbon Fiber Filled (CF)</u>
* <u>**Primary Use Case:**</u> Ultra-rigid, lightweight structural brackets (like toolhead components), drone frames, and stealthy matte aesthetic finishes.
* <u>**Pros:**</u> The chopped carbon fibers drastically increase the material's stiffness (Young's modulus), massively reduce warping during printing, and result in highly dimensionally accurate parts.
* <u>**Cons:**</u> Highly abrasive. Requires a hardened nozzle. Makes the base material more brittle, lowering its impact resistance. Often reduces layer-to-layer adhesion strength.


---

### <u>Glass Fiber Filled (GF)</u>
* <u>**Primary Use Case:**</u> High-impact structural components, heavy-duty enclosures, and parts that need increased rigidity without sacrificing all toughness.
* <u>**Pros:**</u> Increases stiffness and reduces warping like CF, but retains significantly better impact resistance and toughness than CF-filled variants. Usually more cost-effective than CF.
* <u>**Cons:**</u> Extremely abrasive (often more abrasive than CF). GF parts are heavier than their CF counterparts. Also reduces layer adhesion compared to unfilled polymers.


---

### <u>Co-Extrusion "Core" Filaments</u>
* <u>**Primary Use Case:**</u> When both maximum stiffness (from fibers) and maximum layer adhesion (from neat plastic) are required simultaneously.
* <u>**Pros:**</u> These advanced materials use a co-extrusion process to wrap a highly stiff, fiber-filled "core" inside a thin jacket of pure, unfilled polymer. This clever manufacturing method allows the outer layers to melt and bond flawlessly with each other (maximizing Z-axis strength), while the internal core provides massive X/Y rigidity.
* <u>**Cons:**</u> Highly abrasive (still requires hardened nozzles), expensive, and currently limited in material availability.


---

### <u>Aero / Lightweight (LW) Filaments (e.g., LW-PLA, LW-ASA)</u>
* <u>**Primary Use Case:**</u> RC aircraft, drones, cosplay props, lightweight structural models.
* <u>**Pros:**</u> Uses active foaming technology to expand during printing. The filament contains a chemical blowing agent that reacts to heat; the hotter you print, the more it foams. By intentionally under-extruding (lowering the flow rate multiplier) to compensate for this expansion, you can achieve parts that are up to 50-65% lighter than standard materials while remaining surprisingly rigid.
* <u>**Cons:**</u> Tuning can be very tricky (requires carefully balancing extrusion multiplier against hotend temperature to dial in the desired density), reduced layer adhesion and overall strength compared to solid materials, very prone to stringing.


---

### <u>Wood Filled</u>
* <u>**Primary Use Case:**</u> Aesthetic models, architectural models, props requiring a wood-like finish.
* <u>**Pros:**</u> Can be sanded and stained like real wood, excellent for decorative pieces. Often smells like wood while printing.
* <u>**Cons:**</u> Abrasive to nozzles. Prone to stringing and very brittle. Can easily clog smaller nozzles (0.4mm or smaller) due to the wood particles.


---

### <u>Glitter / Sparkle</u>
* <u>**Primary Use Case:**</u> Aesthetic models, hiding layer lines, toys and display pieces.
* <u>**Pros:**</u> The infused glitter flecks scatter light, creating a beautiful finish that does an exceptional job of masking layer lines.
* <u>**Cons:**</u> Extremely abrasive! The metallic or glass flecks used for glitter will rapidly wear down a standard brass nozzle. Increased risk of nozzle clogs.


---

### <u>Color Changing</u>
* <u>**Primary Use Case:**</u> Novelty items, temperature indicators, UV exposure indicators.
* <u>**Pros:**</u> Fun and interactive material that changes color based on temperature (thermochromic) or UV light (photochromic). 
* <u>**Cons:**</u> Color-changing properties can degrade over time (especially UV reactive). Often based on standard PLA or ABS, carrying those inherent material limitations.


---

### <u>Continuous Thread</u>
* <u>**Primary Use Case:**</u> Ultra-high strength, load-bearing parts, replacing machined aluminum parts.
* <u>**Pros:**</u> Inlays a continuous strand of carbon fiber, fiberglass, or Kevlar directly into the printed part, resulting in extreme tensile strength (often rivaling aluminum).
* <u>**Cons:**</u> Requires highly specialized and expensive hardware (dual-nozzle setup with a specialized cutter). Extremely expensive materials, and requires complex path planning in the slicer.


<br><hr><br>

> [!TIP]
> **Moisture & Abrasion Control**
> **Moisture:** Almost all filaments (especially PETG, Nylon, and PC) are hygroscopic and absorb moisture from the air, ruining print quality. **Note that composite/filled filaments (like CF or GF variants) tend to be vastly more hygroscopic than their unfilled counterparts**, as the microscopic fibers can act like wicks, pulling moisture deep into the material via capillary action. Check out the **[Retort Dehumidifier](https://github.com/Alchemical-3D/Retort)** project for our solution to active filament moisture management.
>
> **Abrasiveness:** Additives drastically change a filament's wear properties. While CF and GF are famously abrasive, **Glow-in-the-Dark** filaments (which contain strontium aluminate) are actually among the most abrasive materials you can print and will destroy a standard brass nozzle in a single print. Even heavy pigment dyes (like the titanium dioxide used in stark white or matte filaments) can act as mild abrasives over time, requiring periodic nozzle checks!
