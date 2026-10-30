<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:0ea5e9&height=210&section=header&text=Logan&fontSize=64&fontColor=ffffff&fontAlignY=39&desc=Aspiring%20Design%20Verification%20Engineer&descSize=19&descAlignY=61&animation=fadeIn" width="100%" alt="Logan - Design Verification Engineer" />

### Long Truong

**Computer Engineering Student | Aspiring Design Verification Engineer**

*Building confidence in hardware through rigorous, reproducible verification.*

<br>

[![GitHub](https://img.shields.io/badge/GitHub-0F172A?style=for-the-badge&logo=github&logoColor=white)](https://github.com/LongTruong111)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/longtruongducduy)
[![Repositories](https://img.shields.io/badge/Repositories-0EA5E9?style=for-the-badge&logo=git&logoColor=white)](https://github.com/LongTruong111?tab=repositories)

</div>

<br>

## `01` / About Me

Hi! I'm **Long (Logan)**, a Computer Engineering student pursuing a career in **Design Verification**.

I focus on building verification environments that go beyond passing simulations — emphasizing **simulation correctness, reliable checkers, meaningful coverage, and reproducible evidence**.

My engineering approach is grounded in three principles:

| Principle | Engineering Mindset |
|:---|:---|
| **First Principles** | Understand simulation semantics, event scheduling, and cycle-accurate interface contracts before building verification logic. |
| **Test the Testbench** | Challenge checker fidelity through negative testing, fault injection, and mutation analysis rather than trusting passing logs or coverage numbers alone. |
| **Evidence-Driven Verification** | Use independent seeds, reproducible regressions, and statistical analysis to support verification conclusions. |

<br>

## `02` / Featured Projects

### 01. Implementation of a Five-Stage RISC-V Processor for Investigating Test Generation Algorithms and Coverage Saturation Dynamics in Data Hazard Verification

**Research Project — 5-Stage RV32I Processor**

![RISC-V](https://img.shields.io/badge/RISC--V-RV32I-0F172A?style=flat-square)
![Research](https://img.shields.io/badge/Focus-Coverage_Closure-0EA5E9?style=flat-square)
![Adaptive CGS](https://img.shields.io/badge/Algorithm-Adaptive_CGS-8B5CF6?style=flat-square)
![cocotb](https://img.shields.io/badge/Simulation-cocotb_%2B_Verilator-475569?style=flat-square)

**[View Project Repository →](https://github.com/LongTruong111/riscv-pipeline-research)**

> **Research Objective**
>
> Investigate coverage saturation dynamics and the long-tail coverage-closure problem in data hazard verification of a 5-stage RV32I RISC-V processor.

**Research & Implementation**

- **Adaptive Stimulus Generation:** Develop a template-based Adaptive Coverage-Guided Stimulus (CGS) framework using an **epsilon-greedy multi-armed bandit**. Template utility (Q-values) is updated based on newly covered, attributable **L2 Intent bins per 1,000 accepted instructions** to guide stimulus allocation.

- **Self-Checking Verification:** Integrate a golden-reference architectural scoreboard with microarchitectural timing checkers to verify functional correctness, forwarding behavior, and pipeline stalls.

- **Experimental Evaluation:** Compare five stimulus-generation approaches:
  - Directed Testing
  - Pure Random
  - Static Weighted Random
  - Non-Adaptive CGS
  - Adaptive CGS

- **Evaluation Methodology:** Use Python/cocotb and Verilator to evaluate coverage efficiency, saturation behavior, computational overhead, and fault-detection capability through independent-seed experiments, statistical analysis, fault injection, and mutation testing.

**Key Research Themes**

`Coverage Saturation` · `Adaptive Test Generation` · `Data Hazards` · `Checker Fidelity` · `Statistical Evaluation`

<br>

---


### 02. UART Controller RTL Design & Layered SV Verification

**SystemVerilog RTL & Self-Checking Verification Environment**

![UART](https://img.shields.io/badge/UART-Full_Duplex-0F172A?style=flat-square)
![RTL](https://img.shields.io/badge/RTL-SystemVerilog-0EA5E9?style=flat-square)
![Verification](https://img.shields.io/badge/Focus-Layered_SV_Verification-8B5CF6?style=flat-square)
![Verilator](https://img.shields.io/badge/Simulation-Verilator-475569?style=flat-square)

**[View Project Repository →](https://github.com/LongTruong111/uart-sv-verification)**

> **Project Objective**
>
> Design and verify a full-duplex UART controller using SystemVerilog, combining synthesizable RTL with a layered, self-checking verification environment to validate functional correctness, protocol timing, and FIFO behavior.

**Design & Implementation**

- **RTL Architecture:** Developed a full-duplex UART controller with dedicated baud-rate tick generators, a **2-FF RX synchronizer**, midpoint sampling, and a **16-entry synchronous First-Word Fall-Through (FWFT) RX FIFO** storing 10-bit packets containing payload and parity/frame-error flags.

- **Layered OOP Testbench:** Built a modular SystemVerilog verification environment from scratch without UVM, integrating Interface, Transaction, Generator, Driver, Passive Monitor, Scoreboard, and FIFO Consumer components for automated stimulus generation and end-to-end checking.

- **Timing-Aware Verification:** Applied Clocking Block input sampling (`#1step`), controlled FIFO consumer scheduling, and clock-accurate TX bit-interval checkers to mitigate simulation races and validate serial protocol timing.

- **Verification Closure:** Achieved **33/33 verification-plan goals** on Verilator through systematic functional testing and negative Scoreboard self-tests.

- **Verification Scenarios:** Validated key functional and boundary conditions:
  - Full-Duplex TX/RX Operation
  - Back-to-Back UART Frames
  - FIFO Full/Empty Boundary Conditions
  - Simultaneous FIFO Read/Write at Full Capacity
  - Reset During Active Frames
  - Negative Scoreboard Tests

**Key Engineering Themes**

`RTL Design` · `SystemVerilog OOP` · `Timing-Aware Verification` · `Scoreboarding` · `FIFO Verification` · `Functional Verification`


## `03` / Verification Focus & Technical Stack

### Verification & Methodology

<p>
  <img src="https://img.shields.io/badge/Design_Verification-0EA5E9?style=flat-square" alt="Design Verification" />
  <img src="https://img.shields.io/badge/SystemVerilog_Assertions-8B5CF6?style=flat-square" alt="SVA" />
  <img src="https://img.shields.io/badge/Functional_Coverage-16A34A?style=flat-square" alt="Functional Coverage" />
  <img src="https://img.shields.io/badge/Simulation_Semantics-475569?style=flat-square" alt="Simulation Semantics" />
  <img src="https://img.shields.io/badge/Checker_Validation-EC4899?style=flat-square" alt="Checker Validation" />
</p>

### Languages & Tools

<p>
  <img src="https://img.shields.io/badge/SystemVerilog-5C2D91?style=for-the-badge" alt="SystemVerilog" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/cocotb-FFB000?style=for-the-badge" alt="cocotb" />
  <img src="https://img.shields.io/badge/Verilator-00599C?style=for-the-badge" alt="Verilator" />
  <img src="https://img.shields.io/badge/Icarus_Verilog-475569?style=for-the-badge" alt="Icarus Verilog" />
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git" />
</p>

<br>

## `04` / Current Direction

I'm continuing to deepen my understanding of:

- **SystemVerilog Verification:** OOP testbench architecture, SVA, and simulation event semantics.
- **Checker Reliability:** Golden-reference models, scoreboards, negative testing, and fault injection.
- **Coverage Closure:** Functional coverage modeling, adaptive stimulus generation, and regression analysis.
- **Microarchitectural Verification:** Pipeline hazards, forwarding correctness, and cycle-accurate performance validation.

My goal is to develop verification environments that are not only effective at finding bugs, but also **trustworthy, explainable, and reproducible**.

<br>

---

<div align="center">

### Let's Connect

*Interested in hardware verification, processor microarchitecture, or verification methodology?*

Feel free to explore my projects or connect with me on LinkedIn.

[![LinkedIn](https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/longtruongducduy)

<br>

**"A passing test is only meaningful when the test itself can be trusted."**

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,100:0ea5e9&height=100&section=footer" width="100%" alt="Footer" />

</div>
