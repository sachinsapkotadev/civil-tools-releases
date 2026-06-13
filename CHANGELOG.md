# 🏗️ Civil Tools Changelog

All notable changes to the **Civil Tools** and **Civil Workspace** suite will be documented in this file. This project is built using **Kotlin**, **Jetpack Compose (Material 3)**, **Jetpack Room (local DB)**, and **Google Gemini API**.

---

## [1.0.0] - Solar Workspace Release - 2026-06-13
This is the maiden stable release (**v1.0.0**) of **Civil Tools**—a premium, industry-grade, offline-first digital portfolio and computation workspace designed for professional civil engineers, site managers, quantity surveyors, and contractors in South Asia (Nepal & India).

### 🎨 Visual & Theme Infrastructure
- **Cosmic Slate Styling Theme**: Configured a dark workspace aesthetic pairing warm slate gray backgrounds with localized safety high-visibility orange and electric cyan hazard accent highlights.
- **Material Design 3 (M3) Integrations**: Embedded dynamic light/dark mode schemes natively supporting Android 12+ adaptive system wallpaper palettes (`Dynamic Colors`).
- **Edge-to-Edge System Presentation**: Unified screen overlays with absolute window insets handling, avoiding status-bar overlap and ensuring fluid gesture navigation.
- **Aesthetic Scale Typography**: Implemented a responsive typographic scale utilizing clean display headers paired with elegant monospaced labels for engineering numbers, maximizing readability on site.

### 📋 Bill of Quantities (BOQ) Spreadsheet Engine
- **Multi-Project Workspace Context**: Support for launching, selecting, naming, and archiving multiple active sandboxed project profiles backed by local Room databases.
- **Dynamic Ledger Spreadsheet**: Real-time quantity recalculation for materials including concrete, bricks, rebar steel, plastering mortar, and painting coats.
- **PDF Exporter Pipeline**: A single-tap native engine that converts BOQ tables into formatted, high-contrast, structured PDF sheets stored in local downloads, ready for sharing and printing.

### 🏠 Building Estimator & Municipal Bylaws
- **Nepal Bylaws Module (Classes A & B)**: Live setbacks, allowable plinth metrics, minimum room parameters, Floor Area Ratio (FAR), and Building Coverage Ratio (BCR) conforme to Nepalese local bylaws.
- **India Building Bylaws Module (NBC Standard)**: Built-in calculation matrices conforming to the Indian National Building Code (NBC) utilizing Lakh/Crore systems and Indian Rupees estimation rates.
- **Land Valuation Calculator**: Dynamic conversion models to calculate land plot area pricing (utilizing Aana/Kattha/Square Feet values).

### 🔩 Bar Bending Schedule (BBS) & Rebar Cutting
- **Deduction Calculators**: Automated stirrup, hook, overlap, and bend deduction algorithms ($135^{\circ}$ and $90^{\circ}$) for structural columns, continuous beams, crank beams, slabs, and trapezoidal column footings.
- **Stirrup Lateral Ties**: Multi-shape loop layout engines (Rectangular, Circular, Diamond, and Helical) calculating active linear cutting lengths based on bar diameters.

### 💪 Structural Engineering & Analysis (SOM)
- **Logically Compiling Beam reactions**: Interactive shear force (SFD) and bending moment (BMD) reaction charts supporting single point load and uniformly distributed load (UDL) configurations.
- **Stress-strain diagnostics**: Built-in equation checkers for section modulus, bending stress, civil shear strain, and deflection benchmarks.

### 🧪 Concrete mix design & Soil Mechanics
- **Sieve Gradation Grading**: Computes cumulative sand percentage retention, texture gradation limits, and outputs the Fineness Modulus index.
- **Aggregate Testing Room**: Calculates Mechanical resistance tests including Aggregate Impact Value (AIV), Aggregate Crushing Value (ACV), and Los Angeles (LA) Abrasion index.
- **Sub-Soil Bearing Capacity (SBC)**: Multi-parameter Terzaghi formulas estimating ultimate and allowable local bearing thresholds across standard foundation parameters.

### 🔄 Region-Specific Unit Converters
- **Local South Asian Land Converters**: Conversions between scientific metric meters and regional systems (Ropani-Aana-Paisa-Daam for hilly regions, and Bigha-Kattha-Dhur for Terai regions of Nepal/India).
- **Specialized Concrete Density Scale**: Density-to-weight algorithms converting aggregate bag volumes ($CFT$) into standard metric volumes.

### 🤖 Generative AI Engineering Companion
- **Server-Side Gemini Integration**: Fully interactive assistant tailored explicitly as an expert engineering advisor, ready to debug concrete mixes, recommend structural sections, or clarify Indian and Nepalese national building codes.

---

## [0.9.0] - Beta Release & CI/CD - 2026-06-12
### Added
- Integrated **GitHub Actions Pipeline** (`/.github/workflows/android.yml`) to support automated cross-architecture Release APK and AAB compilation.
- Embedded local Unit test foundations using JVM Robolectric and Roborazzi visual screenshot frameworks.
- Setup auto-generating Keystore fallbacks to prevent pipeline compilation blockages.
