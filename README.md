![Long Truong — Design Verification Engineer](https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:0ea5e9&height=210&section=header&text=Logan&fontSize=62&fontColor=ffffff&fontAlignY=38&desc=Design%20Verification%20Engineer&descSize=20&descAlignY=61)

## Hi there! 👋 I'm Long or Logan if u wish, a **Computer Engineering student** pursuing **Design Verification Engineer**.

⚙️ **First-Principles & Clear Contracts:** I build verification environments grounded in simulation semantics and explicit timing boundaries-prioritizing race-free event scheduling, cycle-accurate behavior, and deterministic stimulus over trial-and-error.

🧪 **Constructive Skepticism ("Test the Testbench"):** I don't treat a green simulation log or a 100% coverage hit as proof of correctness. I actively qualify checker fidelity using negative testing, fault injection, and mutation analysis before trusting test results.

📊 **Data-Driven & Reproducible Engineering:** I approach verification as an empirical science—relying on multi-seed regressions, statistical significance, and fully reproducible environments to validate hardware claims rather than anecdotal single runs.

---

### Learning & Verification Focus

![Design Verification](https://img.shields.io/badge/Design_Verification-0EA5E9?style=for-the-badge)
![SystemVerilog Assertions](https://img.shields.io/badge/SVA-8B5CF6?style=for-the-badge)
![Functional Coverage](https://img.shields.io/badge/Functional_Coverage-16A34A?style=for-the-badge)
![Simulation Semantics](https://img.shields.io/badge/Simulation_Semantics-EC4899?style=for-the-badge)

## Tech Stack

![SystemVerilog](https://img.shields.io/badge/SystemVerilog-5C2D91?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![cocotb](https://img.shields.io/badge/cocotb-FFB000?style=for-the-badge)
![Verilator](https://img.shields.io/badge/Verilator-00599C?style=for-the-badge)
![Icarus Verilog](https://img.shields.io/badge/Icarus_Verilog-475569?style=for-the-badge)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## Projects

### [Coverage Saturation Dynamics and Adaptive Test Generation for Data Hazard Verification in a 5-Stage RISC-V Processor](https://github.com/LongTruong111/riscv-pipeline-research)

- **Core Problem:** Mitigating the long-tail closure phenomenon where static random stimulus stalls near coverage saturation during processor pipeline hazard testing.
- **Adaptive CGS Algorithm:** Implemented template-based stimulus generation with reinforcement learning principles; updates template utility ($Q$-values) based on coverage yield per instruction ($\Delta C / N$) to dynamically balance exploration and exploitation across execution batches.
- **Dual Correctness Checkers:** Validates architectural functional correctness via a golden reference scoreboard alongside microarchitectural timing/performance correctness via an Expected-Stall Calculator and Cycle-Gap Checker.
- **Methodology & Rigor:** Python/cocotb and Verilator co-simulation evaluated across independent seeds with Bootstrap 95% CI, Welch's t-test, runtime fault injection, and mutation testing.

### [Design and Verification of UART Controller using SystemVerilog](https://github.com/LongTruong111/uart-sv-verification)

- **RTL Architecture:** Designed a full-duplex UART controller featuring dedicated baud-rate tick generators, 2-FF synchronizer with midpoint sampling, and a 16-entry synchronous FWFT RX FIFO preserving 10-bit packets (payload with embedded parity and frame error flags).
- **Layered OOP Testbench:** Built a self-checking SystemVerilog testbench from scratch (Interface, Transaction, Generator, Driver, Passive Monitor, Scoreboard, FIFO Consumer) without relying on external UVM packages.
- **Timing & Interface Contract:** Applied strict event region contracts (#1step input sampling for monitor and #0 look-ahead for FIFO consumer read scheduling) and clock-accurate TX bit-interval assertion checkers.
- **Verification Closure:** Achieved $33/33$ functional plan goals on Verilator; systematically validated continuous back-to-back frames, full-duplex concurrency, full simultaneous R/W drop policy, in-frame reset recovery, and negative scoreboard self-tests.

---

- 🌱 **Mastering:** Design Verification methodology, SystemVerilog OOP testbench architecture, SVA, and simulation event semantics.
- 🎯 **Targeting:** Rigorous self-checking scoreboards, microarchitectural performance validation, and functional coverage closure.
- 📂 **Repositories:** Explore all verification testbenches and RTL designs in [my repositories](https://github.com/LongTruong111?tab=repositories).
- 💬 **Let's Connect:** [LinkedIn Profile](https://www.linkedin.com/in/longtruongducduy)
