# ⚡ HK Junior Science (S1–S3) Electric Circuits Quiz Web App
### 香港初中科學 電路學互動測驗 Web App

![HTML5](https://img.shields.io/badge/HTML5-Single--File-orange?style=for-the-badge&logo=html5)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla%20JS-yellow?style=for-the-badge&logo=javascript)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![Curriculum](https://img.shields.io/badge/Curriculum-HK%20EDB%20S1--S3%20Science-green?style=for-the-badge)

🌐 **Live Application:** [https://charlotte-lau-hk.github.io/Junior-Science-Circuit-Quiz/](https://charlotte-lau-hk.github.io/Junior-Science-Circuit-Quiz/)

An interactive, single-file HTML5 web application tailored for Hong Kong Junior Secondary (S1–S3) Science students learning electric circuits. Designed to strengthen students' conceptual understanding of circuit symbols, closed loops, switch logic, short circuits, meter placements, and cell polarities.

---

## ✨ Features & Highlights

### 🎯 1. Curriculum-Aligned Difficulty Progression
* **100-Question Procedural Pool**: Programmatically generated across **10 progressive difficulty tiers** (10 questions per tier).
* **Dynamic Quiz Selection**: Each 10-question quiz run dynamically selects 1 random question per tier to ensure high replay value.
* **Tier Roadmap**:
  * **Tier 1**: Basic single-loop closed/open circuits (1 cell, 1 switch, 1 bulb).
  * **Tier 2–4**: Series vs. parallel branches with multiple switches and bulbs.
  * **Tier 5**: Short-circuit bypass paths across Bulb X.
  * **Tier 6–7**: Ammeter (series) and Voltmeter (parallel) connection rules.
  * **Tier 8**: Rheostats and variable resistance loops.
  * **Tier 9**: Cell polarity alignment (+ to + facing opposing EMFs).
  * **Tier 10**: Master complex multi-branch circuits with short-circuit options.

### 🧮 2. Built-in Modified Nodal Analysis (MNA) Physics Engine
* Uses a custom **linear system solver (Gaussian Elimination with partial pivoting)** written in pure JavaScript to calculate branch node voltages and currents in real time.
* **Accurately handles complex electrical scenarios**:
  * Open switches / gaps $\rightarrow$ Infinite resistance ($10^8\,\Omega$) $\rightarrow$ Zero current flow.
  * Short-circuit wires $\rightarrow$ Path of zero resistance ($0.001\,\Omega$) bypassing components.
  * Voltmeters in series $\rightarrow$ High internal resistance ($\approx 10\,\text{M}\Omega$) blocks current completely.
  * Ammeters in parallel $\rightarrow$ Near-zero resistance creates an unintended short circuit.
  * Opposing cell polarities $\rightarrow$ Equal opposing voltages cancel out to $0\,\text{V}$ net potential.

### 🎨 3. Interactive Inline SVG Engine
* Dynamically renders crisp, vector-based circuit diagrams using native SVG.
* **IEC Standard Symbols**: Light bulbs strictly follow IEC standard lamp symbols (circle containing a cross filament), switches feature realistic lever arms, cells feature long (+) / short (-) plates, and rheostats display diagonal arrows.
* **Animated Current Flow**: Dashed lines animate along conducting branches carrying current.
* **Bulb Glow Effect**: Visual lighting animation when Bulb X receives sufficient operating current.

### 🧪 4. Real-time Interactive Sandbox Mode
* After submitting an answer, students unlock an **Interactive Sandbox Control Panel** directly inside the feedback card.
* Live toggling of switches updates the circuit state, current flow animations, and bulb glows in real time to promote inquiry-based learning.

### 🌐 5. Full Bilingual Support (Traditional Chinese / English)
* Instant language toggle button in the header.
* Chinese mode utilizes standard Hong Kong EDB Junior Science terminology (閉合迴路, 斷路, 短路, 變阻器, 電壓表, 電流表).

### 📊 6. End-of-Quiz Diagnostic Skill Report
* Evaluates overall score (e.g., `8/10`) and generates a competency breakdown across 6 primary skill pillars:
  1. *Basic Closed Loops (基本閉合迴路)*
  2. *Series & Parallel Circuits (串聯與並聯電路)*
  3. *Short Circuits (短路現象)*
  4. *Ammeter & Voltmeter Placement (電錶正確連接)*
  5. *Rheostats & Variable Components (變阻器與元件)*
  6. *Cell Polarity & Voltage Alignment (電池極性方向)*
* Categorizes performance into **Mastered (概念已掌握)** or **Needs Practice (需要加強練習)**.

---

## 🛠️ Tech Stack & Constraints

| Component | Specification |
|---|---|
| **Architecture** | **Single File (`index.html`)** containing all HTML structure, CSS styling, and JS logic. |
| **Dependencies** | **Zero external dependencies**, libraries, frameworks, fonts, or CDN calls. |
| **Styling** | Modern CSS3 theme with card-based UI, soft shadows, and fully responsive layout. |
| **Graphics** | Native SVG (Scalable Vector Graphics) generated dynamically via JavaScript DOM manipulation. |
| **Compatibility** | Fully responsive across modern desktop browsers, tablets, and interactive whiteboards. |

---

## 🚀 Deployment & Local Usage

### Accessing the Published Web App
The app is live on GitHub Pages:  
👉 **[https://charlotte-lau-hk.github.io/Junior-Science-Circuit-Quiz/](https://charlotte-lau-hk.github.io/Junior-Science-Circuit-Quiz/)**

### Running Locally
1. Clone or download this repository:
   ```bash
   git clone [https://github.com/charlotte-lau-hk/Junior-Science-Circuit-Quiz.git](https://github.com/charlotte-lau-hk/Junior-Science-Circuit-Quiz.git)
