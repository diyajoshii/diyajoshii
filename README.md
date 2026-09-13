<div align="center">
  <img src="./assets/header.svg" width="100%" alt="Diya Joshi — Data analysis, embedded systems, applied AI, product" />
</div>

<div align="center">
  <a href="https://diyajoshi.vercel.app/"><img src="https://img.shields.io/badge/portfolio-0d1117?style=for-the-badge&logo=vercel&logoColor=d2a8ff" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/diya-joshi19"><img src="https://img.shields.io/badge/linkedin-0d1117?style=for-the-badge&logo=linkedin&logoColor=0a66c2" alt="LinkedIn" /></a>
  <a href="https://crates.io/crates/mpu6050-nostd"><img src="https://img.shields.io/badge/crates.io-0d1117?style=for-the-badge&logo=rust&logoColor=79c0ff" alt="mpu6050-nostd on crates.io" /></a>
  <a href="mailto:diyajoshi1909@gmail.com"><img src="https://img.shields.io/badge/say_hi-0d1117?style=for-the-badge&logo=gmail&logoColor=f85149" alt="Email Diya" /></a>
</div>

<br />

I like working at the point where a signal turns into a decision. Sometimes the signal is an I²C register on a gyroscope, sometimes it is seventeen CSVs of collections data with a headline that doesn't survive a p-value. The job is the same: **measure first, build the thing, then show the numbers that prove it works** (or the ones that prove it doesn't).

> Currently a student at **Netaji Subhas University of Technology (NSUT)**, Delhi.

```text
building_with   → Python · Rust · SQL · embedded-hal · scikit-learn · FastAPI · Next.js
thinking_about  → forensic data analysis · no_std drivers you can test on a laptop · agents that spend a budget
operating_from  → Delhi, India (UTC+5:30)
```

## `> shipped_work`

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>⚡ Prahar</h3>
      <p>An agent that decides whether, when, and how to retry a failed recurring debit in India, spending a hard-capped NPCI attempt budget against a learned model of when the payer will actually have money. Built for the Razorpay AI Buildathon. The headline metric failed, and the README says so, with 95% CIs over five seeds.</p>
      <p><code>Python</code> <code>hazard models</code> <code>simulation</code> <code>ablations</code></p>
      <a href="https://github.com/diyajoshii/Prahar-RazorpayAIbuildathon"><b>source ↗</b></a>
    </td>
    <td width="50%" valign="top">
      <h3>🦀 mpu6050-nostd</h3>
      <p>A register-level <code>no_std</code> Rust driver for the MPU-6050 accelerometer/gyroscope, generic over <code>embedded-hal</code> 1.0, with a fault-injecting mock I²C bus so the whole driver, FIFO and bus failures included, runs under <code>cargo test</code> with no hardware attached. 76 tests, CI-written coverage badge, 10.6 KB of flash on a TM4C123G.</p>
      <p><code>Rust</code> <code>no_std</code> <code>embedded-hal</code> <code>I²C</code></p>
      <a href="https://github.com/diyajoshii/Rust"><b>source ↗</b></a> · <a href="https://crates.io/crates/mpu6050-nostd"><b>crates.io ↗</b></a> · <a href="https://docs.rs/mpu6050-nostd"><b>docs ↗</b></a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🔍 CredResolve analysis</h3>
      <p>A forensic take-down of the claim "recovery improved 11% month-on-month". It hadn't: net recovery was flat, the 11% was a 31-day March next to a 28-day February, and reported figures were overstated by ₹12 Cr through duplicates and reversals. Reproducible pipeline, production-shaped SQL, golden dataset, DiD counterfactual, one-screen CEO dashboard.</p>
      <p><code>Python</code> <code>SQL</code> <code>pandas</code> <code>statistics</code></p>
      <a href="https://github.com/diyajoshii/CredResolve-analysis"><b>source ↗</b></a>
    </td>
    <td width="50%" valign="top">
      <h3>🔮 AURA</h3>
      <p>A research-paper companion for people learning machine learning. Ask a question in plain language, follow up naturally, and inspect the exact passages retrieved before the answer was written. Curated LaTeX-source library, section-aware chunks with provenance, streamed answers.</p>
      <p><code>Next.js</code> <code>Qdrant</code> <code>Gemini</code> <code>RAG</code></p>
      <a href="https://github.com/diyajoshii/AURA-AI-Research-Assistant"><b>source ↗</b></a>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>📈 Prodessy</h3>
      <p>Project risk and completion forecasting for product managers: a ranked queue of at-risk tasks, predicted completion timelines, and SHAP explanations for why a task was flagged. Built for a case competition at IIM Indore.</p>
      <p><code>LightGBM</code> <code>AutoGluon</code> <code>SHAP</code> <code>NLP</code></p>
      <a href="https://github.com/diyajoshii/Prodessy-IIMIndore"><b>source ↗</b></a>
    </td>
    <td width="50%" valign="top">
      <h3>🛡️ Aegis</h3>
      <p>A campus utility platform for NSUT students: scholarship discovery, lost-and-found matching, proctored skill assessments with face detection and tab-switch tracking, and syllabus-based academic help, in one place.</p>
      <p><code>TypeScript</code> <code>Node</code> <code>face-api.js</code></p>
      <a href="https://github.com/diyajoshii/Aegis-NSUT-Campus-Utility-Platform"><b>source ↗</b></a>
    </td>
  </tr>
</table>

## `> tools_i_reach_for`

<div align="center">
  <img src="https://skillicons.dev/icons?i=python,rust,c,sklearn,pytorch,fastapi,nextjs,ts,postgres,docker,linux,git&theme=dark&perline=12" alt="Python, Rust, C, scikit-learn, PyTorch, FastAPI, Next.js, TypeScript, PostgreSQL, Docker, Linux, and Git" />
</div>

<br />

## `> how_the_pieces_fit`

```mermaid
flowchart TB
    subgraph SENSE["01 · SENSE"]
        direction LR
        A1["Sensors<br/>I²C · SPI · FIFO"]
        A2["Transactions<br/>ledgers · mandates"]
        A3["Documents<br/>papers · specs"]
        A4["Product events<br/>tasks · updates"]
    end

    subgraph TRUST["02 · TRUST THE DATA"]
        direction LR
        B1["PROFILE<br/>grain · keys · ranges"] --> B2["FORENSICS<br/>duplicates · reversals · calendar"]
        B2 --> B3["TRANSFORM<br/>SQL · Python"]
        B3 --> B4["GOLDEN SET<br/>one definition per metric"]
    end

    subgraph REASON["03 · REASON"]
        direction LR
        C1["FEATURES<br/>no leakage · as-of joins"] --> C2["MODEL<br/>ML · hazard · retrieval"]
        C2 --> C3["DECIDE<br/>budget · policy · rules"]
        C3 --> C4["EVALUATE<br/>seeds · CIs · ablations · CI"]
    end

    subgraph SHIP["04 · SHIP"]
        direction LR
        D1["SERVE<br/>API · crate · dashboard"] --> D2["ACT<br/>retry · alert · answer"]
        D2 --> D3["OBSERVE<br/>flash size · latency · ₹ harm"]
        D3 --> D4["REVISE<br/>publish what failed too"]
    end

    A1 --> B1
    A2 --> B1
    A3 --> B1
    A4 --> B1
    B4 --> C1
    C4 --> D1
    D4 -. "measure again" .-> B1

    classDef sense fill:#161b22,stroke:#79c0ff,color:#c9d1d9,stroke-width:1px;
    classDef trust fill:#0d1117,stroke:#d2a8ff,color:#c9d1d9,stroke-width:2px;
    classDef reason fill:#0d1117,stroke:#7ee787,color:#c9d1d9,stroke-width:2px;
    classDef ship fill:#0d1117,stroke:#ffa657,color:#c9d1d9,stroke-width:2px;
    class A1,A2,A3,A4 sense;
    class B1,B2,B3,B4 trust;
    class C1,C2,C3,C4 reason;
    class D1,D2,D3,D4 ship;
```

## `> contribution_arcade`

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/diyajoshii/diyajoshii/output/github-contribution-grid-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/diyajoshii/diyajoshii/output/github-contribution-grid-snake.svg" />
    <img alt="Animated snake eating Diya's GitHub contributions" src="https://raw.githubusercontent.com/diyajoshii/diyajoshii/output/github-contribution-grid-snake.svg" />
  </picture>
</div>
