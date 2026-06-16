



# 🔋 sim-to-real-battery-copilot

> **An autonomous AI agent combining local SLMs with neural physics surrogates for closed-loop EV battery thermal design.**

---

## 🌌 Overview

`sim-to-real-battery-copilot` is an open-source, multi-modal AI engineering agent designed to bridge the gap between abstract language instructions and complex physical realities. Traditional Large Language Models (LLMs) possess deep text-based reasoning but completely lack spatial, physical, and mathematical intuition. They cannot calculate fluid dynamics or thermal propagation natively. 

This project implements a **Closed-Loop Artificial General Engineer Framework**. It pairs a localized Small Language Model (SLM) acting as the rational controller with a high-fidelity electrochemical and thermal neural surrogate engine. The agent ingests raw, high-frequency EV battery telemetry, diagnoses localized thermal runaway risks, executes real-time physical simulations, and programmatically iterates geometric cooling channel architectures to maximize cell yield and pack safety.

---

## 🗺️ System Architecture

## 🗺️ System Architecture

```text
[ Real-World Battery Telemetry ] ──► (Voltage, Current, Temp)
               │
               ▼
┌────────────────────────────────────────┐
│ 1. The Controller Layer (SLM)          │ ◄── Localized Llama-3/Mistral via Function Calling
└────────────────────────────────────────┘
               │ 
               ▼ (Triggers Automated Simulation Toolpaths)
┌────────────────────────────────────────┐
│ 2. Neural Physics Surrogate            │ ◄── PyTorch Model + PyBaMM Mathematical Truth
└────────────────────────────────────────┘
               │
               ▼ (Identifies Localized Thermal Constraints)
┌────────────────────────────────────────┐
│ 3. Autonomous Optimization Loop        │ ◄── Programmatically rewrites micro-channel 3D paths
└────────────────────────────────────────┘
               │
               ▼
[ Output: Analytical Diagnosis Report & Verified Geometric CAD Coordinates ]
```

