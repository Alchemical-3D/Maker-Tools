# 🧵 Filament Guide & Use Cases

Choosing the right material is just as important as the hardware itself. Before selecting a filament, you must first identify the **job requirements** for the part you are printing. Will the part be exposed to higher temperatures where it might suffer from heat creep? Will it face significant mechanical stress along its layer lines? Does it need to withstand prolonged UV exposure from sunlight, or harsh chemicals and solvents?

**Example Scenario:** If you are printing a toolhead carriage for an enclosed 3D printer (like the **Alembic**), the part will live inside a heated chamber (often 60°C+) and sit directly above a hotend. Using PLA here is a guaranteed failure; it will soften and warp due to heat creep. Instead, the job requirements dictate a material with a high glass transition temperature and good rigidity, such as **ABS**, **ASA**, or **CF-PC**.

Below is a breakdown of common filament types used in the 3D printing ecosystem and the broader maker community, categorized to help you match the material to your specific job requirements.

<br><hr><br>

## 🟢 Standard Plastics

These are your everyday materials, ideal for rapid prototyping, display models, and low-stress parts.

### PLA (Polylactic Acid)
* **Primary Use Case:** Prototyping, aesthetic prints, structural parts that stay at room temperature.
* **Pros:** Extremely easy to print, highly rigid, no warping, eco-friendly.
* **Cons:** Very low glass transition temperature (~60°C); will deform in hot cars or near printer hotends. Brittle under impact.

---

### PETG (Polyethylene Terephthalate Glycol)
* **Primary Use Case:** Functional parts, mechanical assemblies, water-resistant containers.
* **Pros:** Better temperature resistance than PLA, highly impact resistant, flexes rather than shattering.
* **Cons:** Prone to stringing, can over-adhere to certain build plates (like glass or PEI).

---

### PCTG
* **Primary Use Case:** High-impact functional parts, tough mechanical components.
* **Pros:** Engineered as an advanced successor to PETG. It offers significantly higher impact strength (toughness), improved optical clarity, and slightly better temperature resistance, making it superior for parts that will take a beating.
* **Cons:** Can be more expensive and slightly more difficult to source than PETG.

---

### PP (Polypropylene)
* **Primary Use Case:** Living hinges, chemical-resistant containers, lightweight parts.
* **Pros:** Incredible fatigue resistance (great for hinges), very low density, high chemical resistance.
* **Cons:** Extremely prone to warping, very difficult to adhere to standard build plates (requires specialized tape or adhesives).

<br><hr><br>

## 🟡 Advanced Plastics

These materials sit between standard and true engineering plastics. They offer great thermal resistance and are commonly used for 3D printer structural parts (like the **Alembic Toolhead** or **Pneuma** mounts).

### ABS (Acrylonitrile Butadiene Styrene)
* **Primary Use Case:** Printer parts, automotive components, durable enclosures.
* **Pros:** Excellent temperature resistance (~100°C), easy to sand/smooth (can be acetone smoothed), and highly durable. Very cost-effective.
* **Cons:** **Emits toxic styrene fumes during printing (requires heavy ventilation/filtration).** Prone to severe warping and requires a heated enclosure. Poor UV resistance (will yellow and become brittle in sunlight).

---

### ASA (Acrylonitrile Styrene Acrylate)
* **Primary Use Case:** Outdoor fixtures, printer parts, automotive exterior components.
* **Pros:** Engineered specifically as a modern successor to ABS. It retains all the excellent thermal and mechanical benefits of ABS, but adds exceptional UV resistance (it will not yellow or degrade in sunlight) and is often slightly less prone to warping during printing.
* **Cons:** **Emits toxic styrene fumes during printing (requires heavy ventilation/filtration).** Still prone to warping and requires a heated enclosure. Generally slightly more expensive than ABS.

---

### PC-ABS (Polycarbonate / ABS Blend)
* **Primary Use Case:** Enclosures, durable consumer goods, high-impact structural parts.
* **Pros:** Combines the high impact strength and heat resistance of PC with the better printability of ABS. Less prone to warping than pure PC.
* **Cons:** **Emits toxic styrene fumes during printing (requires heavy ventilation/filtration).** Still requires a heated enclosure. Lower heat resistance than pure PC.

<br><hr><br>

## 🟠 Engineering Grade Plastics

These materials are required for the highest-heat and highest-stress environments due to their extreme thermal and mechanical properties.

### PC (Polycarbonate)
* **Primary Use Case:** High-heat, high-stress mechanical parts.
* **Pros:** Incredible impact strength and very high temperature resistance (~110°C+).
* **Cons:** **Emits harmful VOCs (including BPA) during printing (requires ventilation/filtration).** Extremely difficult to print. Requires very high hotend temperatures and a heated chamber.

---

### PA (Nylon) Series
* **Primary Use Case:** Gears, bearings, high-wear mechanical components.
* **Pros:** Incredible wear resistance, low friction, high impact strength.
* **Cons:** **Emits harmful VOCs and UFPs including caprolactam (requires ventilation).** Extremely hygroscopic (must be printed dry), prone to warping, low stiffness unless fiber-filled.

---

### PAHT (High-Temperature Nylon)
* **Primary Use Case:** High-temperature structural parts.
* **Pros:** Maintains structural integrity at much higher temperatures than standard PA, excellent chemical resistance.
* **Cons:** **Emits harmful VOCs and UFPs (requires ventilation).** Very hygroscopic, requires high extrusion temperatures.

---

### PPA (Polyphthalamide / High-Performance Polyamide)
* **Primary Use Case:** Metal replacement parts, automotive under-the-hood components.
* **Pros:** Superior thermal performance and stiffness compared to standard aliphatic nylons (PA), lower moisture absorption.
* **Cons:** **Emits harmful VOCs at high processing temperatures (requires ventilation).** Requires extremely high printing temperatures and a heated chamber, expensive.

---

### PPS (Polyphenylene Sulfide)
* **Primary Use Case:** Aerospace, automotive, and extreme chemical environments.
* **Pros:** Outstanding chemical resistance (insoluble in almost any known solvent under 200°C), inherent flame retardancy, very high continuous use temperature.
* **Cons:** **Emits highly toxic sulfur compounds and VOCs during printing (requires heavy ventilation/filtration).** Very difficult to print, requires highly specialized high-temperature hardware, very expensive.

---

### PET (Polyethylene Terephthalate)
* **Primary Use Case:** High-strength mechanical parts, dimensionally stable structural components (often fiber-filled).
* **Pros:** Extremely high stiffness and tensile strength, excellent chemical resistance, very low moisture absorption compared to nylons. Can be annealed for extreme heat resistance.
* **Cons:** Harder to print than PETG, prone to crystallization/opacity changes depending on cooling rate.

<br><hr><br>

## 🔴 Flexible Materials

### TPU (Thermoplastic Polyurethane)
* **Primary Use Case:** Gaskets, vibration dampeners, flexible hinges, tires.
* **Pros:** Highly flexible, extreme layer adhesion, nearly indestructible.
* **Cons:** Difficult to print on standard Bowden setups; requires a well-constrained direct drive extruder (like the **Pestle** in direct-drive configuration). Must be printed slowly.

---

### PEBA (Polyether Block Amide)
* **Primary Use Case:** High-performance sporting goods, footwear, extremely durable flexible parts.
* **Pros:** Exceptional energy return, maintains flexibility even at very low temperatures, lower density than TPU.
* **Cons:** More difficult to print than TPU, highly hygroscopic, often more expensive.

<br><hr><br>

## 🟣 Additives & Specialty Composites

### Carbon Fiber Filled (CF)
* **Primary Use Case:** Ultra-rigid, lightweight structural brackets (like toolhead components), drone frames, and stealthy matte aesthetic finishes.
* **Pros:** The chopped carbon fibers drastically increase the material's stiffness (Young's modulus), massively reduce warping during printing, and result in highly dimensionally accurate parts.
* **Cons:** Highly abrasive. Requires a hardened nozzle. Makes the base material more brittle, lowering its impact resistance. Often reduces layer-to-layer adhesion strength.

---

### Glass Fiber Filled (GF)
* **Primary Use Case:** High-impact structural components, heavy-duty enclosures, and parts that need increased rigidity without sacrificing all toughness.
* **Pros:** Increases stiffness and reduces warping like CF, but retains significantly better impact resistance and toughness than CF-filled variants. Usually more cost-effective than CF.
* **Cons:** Extremely abrasive (often more abrasive than CF). GF parts are heavier than their CF counterparts. Also reduces layer adhesion compared to unfilled polymers.

---

### Co-Extrusion "Core" Filaments
* **Primary Use Case:** When both maximum stiffness (from fibers) and maximum layer adhesion (from neat plastic) are required simultaneously.
* **Pros:** These advanced materials use a co-extrusion process to wrap a highly stiff, fiber-filled "core" inside a thin jacket of pure, unfilled polymer. This clever manufacturing method allows the outer layers to melt and bond flawlessly with each other (maximizing Z-axis strength), while the internal core provides massive X/Y rigidity.
* **Cons:** Highly abrasive (still requires hardened nozzles), expensive, and currently limited in material availability.

---

### Aero / Lightweight (LW) Filaments (e.g., LW-PLA, LW-ASA)
* **Primary Use Case:** RC aircraft, drones, cosplay props, lightweight structural models.
* **Pros:** Uses active foaming technology to expand during printing. The filament contains a chemical blowing agent that reacts to heat; the hotter you print, the more it foams. By intentionally under-extruding (lowering the flow rate multiplier) to compensate for this expansion, you can achieve parts that are up to 50-65% lighter than standard materials while remaining surprisingly rigid.
* **Cons:** Tuning can be very tricky (requires carefully balancing extrusion multiplier against hotend temperature to dial in the desired density), reduced layer adhesion and overall strength compared to solid materials, very prone to stringing.

<br><hr><br>

> [!TIP]
> **Moisture & Abrasion Control**
> **Moisture:** Almost all filaments (especially PETG, Nylon, and PC) are hygroscopic and absorb moisture from the air, ruining print quality. **Note that composite/filled filaments (like CF or GF variants) tend to be vastly more hygroscopic than their unfilled counterparts**, as the microscopic fibers can act like wicks, pulling moisture deep into the material via capillary action. Check out the **[Retort Dehumidifier](https://github.com/Alchemical-3D/Retort)** project for our solution to active filament moisture management.
>
> **Abrasiveness:** Additives drastically change a filament's wear properties. While CF and GF are famously abrasive, **Glow-in-the-Dark** filaments (which contain strontium aluminate) are actually among the most abrasive materials you can print and will destroy a standard brass nozzle in a single print. Even heavy pigment dyes (like the titanium dioxide used in stark white or matte filaments) can act as mild abrasives over time, requiring periodic nozzle checks!
