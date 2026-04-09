# Alma-public
Public overview of Alma:: system architecture, concept and development direction.
# ALMA

**A passive wearable system for early stress detection and real-time haptic co-regulation.**

---

## What is Alma

Alma is a screenless wearable concept designed to detect early physiological signs of stress and provide subtle, real-time haptic feedback — before conscious awareness.

It acts as a silent co-pilot for the nervous system, helping users return to regulation without cognitive effort.

---

## The Problem

Current approaches to stress and anxiety management have key limitations:

- They rely on conscious awareness, which often comes too late  
- They require active user input (apps, breathing exercises, screens)  
- They do not operate in real time during physiological escalation  
- They are not adapted for children or non-verbal users  

Stress is first a **physiological process**, not a cognitive one.

---

## The Approach

Alma works by detecting deviations in the body's internal rhythms and responding through non-intrusive haptic signals.

Instead of tracking or notifying, Alma **intervenes subtly and rarely**, only when necessary.

Core principles:
- No screens  
- No constant feedback  
- No behavioral pressure  
- Minimal, meaningful intervention  

---

## System Architecture

Alma is built as a multi-sensor, edge-based system:

**Inputs**
- Heart rate / HRV (PPG)
- Electrodermal activity (EDA)
- Motion & respiration proxy (IMU)

**Processing layers**
- Signal preprocessing  
- Multi-sensor validation (false positive reduction)  
- Multi-window baseline comparison  
- State detection (FSM-based logic)  
Each layer is validated independently.
The system responds only when all layers agree —
reducing false positives before they reach the user.

**Output**
- Haptic feedback patterns (closed-loop response)

---

## What Makes Alma Different

- **Closed-loop system**: detects → interprets → responds in real time  
- **No screen dependency**: interaction happens through the body  
- **False-positive aware architecture**: multi-sensor validation instead of single-threshold triggers  
- **Designed for early detection**, not post-event tracking  
- **Works for children and non-verbal users**, not just quantified-self adults  

---

## Current Status

The signal processing core is implemented and running:

- Signal preprocessing pipeline      ✅
- PLV-based cadence detection         ✅
- Pattern memory (Deja-vu module)     ✅
- PSI — Physiological State Index     ✅
- Logic Layer FSM                     ✅
- ESP32 + haptic prototype            ✅

Next step: real sensor integration
and first functional validation prototype.

## Roadmap

 ## Roadmap

| Phase | Milestone | Status |
|---|---|---|
| v0.1 | Signal processing core + Logic FSM | ✅ Complete |
| v0.2 | Real sensor integration + calibration | 🔄 In progress |
| v0.3 | Functional wearable prototype | ⏳ Planned |
| v1.0 | Pilot testing + haptic refinement | ⏳ Planned |

---

## Vision

Alma explores a different interaction paradigm:

**technology that listens to the body — and responds without noise.**

---

## Contact

Raluca-Adelina Luca  
Founder, Alma  
Open to collaboration, research partnerships,
and hardware development conversations.
---

## Technical Repository

The signal processing engine is open and documented:
[alma-systems/alma-cadence-dejavu](link)

Includes PSI model, Logic Layer FSM,
and full implementation notes.

