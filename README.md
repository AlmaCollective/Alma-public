# Alma — Physiological Co-Regulation System

Alma is a screenless wearable system designed to detect early physiological signs of stress and deliver real-time haptic feedback — before conscious awareness.

It acts as a silent co-regulation layer for the nervous system.

---

## What Alma Does

Most systems measure stress after it happens.

Alma detects **direction of change in real time**  
and responds through subtle haptic signals.

No alerts.  
No screens.  
No cognitive load.

---

## The Problem

Current stress-management tools:

- Depend on conscious awareness (often too late)
- Require active interaction (apps, breathing exercises)
- Do not operate during early physiological escalation
- Are not suited for children or non-verbal users

Stress begins as a **physiological process**, not a cognitive one.

---

## The Approach

Alma detects deviations in internal physiological patterns  
and responds with minimal, non-intrusive feedback.

Core principles:

- No screens
- No constant feedback
- No behavioral pressure
- Minimal, meaningful intervention

---

## System Architecture

**Inputs**
- Heart rate / HRV (PPG)
- Electrodermal activity (EDA)
- Motion & respiration proxy (IMU)

**Processing**
- Signal preprocessing
- Multi-sensor validation (false-positive reduction)
- Multi-window baseline comparison
- FSM-based state detection

**Output**
- Real-time haptic feedback patterns

The system responds only when signals align across layers.

---

## What Makes Alma Different

- Closed-loop system: detect → interpret → respond
- No screen dependency — interaction happens through the body
- False-positive aware architecture (multi-sensor validation)
- Designed for early intervention, not post-event tracking
- Built for children and non-verbal users

---

## Current Status

- Signal processing pipeline — ✅ implemented  
- Cadence detection (PLV-based) — ✅ implemented  
- Pattern memory (Deja-vu) — ✅ implemented  
- PSI (Physiological State Index) — ✅ implemented  
- Logic Layer (FSM) — ✅ implemented  
- ESP32 + haptic prototype — ✅ running  

**Next step:** real sensor integration and calibration

---

## Roadmap

| Phase | Milestone | Status |
|------|----------|--------|
| v0.1 | Signal processing core + FSM | ✅ Complete |
| v0.2 | Sensor integration + calibration | 🔄 In progress |
| v0.3 | Functional wearable prototype | ⏳ Planned |
| v1.0 | Pilot testing + refinement | ⏳ Planned |

---

## Vision

Alma explores a different interaction paradigm:

**technology that listens to the body — and responds without noise**

---

## Founder

Raluca-Adelina Luca  
Founder & System Architect

---

## Technical Repository

Core signal processing engine:  
https://github.com/alma-systems/alma-cadence-dejavu

---

## Contact

Open to collaboration, research partnerships, and hardware development discussions.

---

© Alma Systems — 2026
