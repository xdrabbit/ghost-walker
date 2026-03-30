# Ghost Walker

**A lightweight, open-source, cable-driven, compliant leg-assist system for gait initiation and hip-flex support.**

Ghost Walker is not a robot exoskeleton. It is a **smart assist layer**: a tendon-like system designed to help lift and advance the leg with minimal force, minimal bulk, and a motion profile that feels natural instead of mechanical.

The project focuses first on one hard, meaningful problem:

> **Can we help initiate and sustain forward swing of the leg using compliant, cable-based assist?**

This repo is open source because mobility should not be trapped behind impossible prices, closed designs, or one-size-fits-none hardware.

---

## Design Intent

Ghost Walker is being designed for people whose movement is limited not by total paralysis, but by some combination of:

- hip flex weakness
- fatigue
- inconsistent leg lift
- toe drag / poor clearance
- day-to-day variability
- asymmetry
- neurological conditions where assist must adapt instead of dominate

The goal is not to replace the body.  
The goal is to **join the motion**.

---

## Core Idea

Ghost Walker treats the leg as a lever and the assist system as a **smart artificial muscle-tendon unit**.

### System concept

- **Anchor A:** waist / pelvis
- **Anchor B:** upper thigh cuff
- **Transmission:** routed cable / Bowden cable
- **Compliance:** elastic tubing, elastomer, or spring element
- **Actuator:** motorized spool / tensioner
- **Sensors:** IMU, optional tension and foot-contact sensing
- **Control:** timed assist, then adaptive assist later

The result is a system that can:

- remove slack
- preload gently
- assist hip flexion
- allow follow-through
- release cleanly
- adapt over time

---

## What Ghost Walker Is Not

Ghost Walker is **not**:

- a rigid full-joint exoskeleton
- a giant wearable robot
- a “walk for you” machine
- a medical-device product claim
- a locked commercial platform

---

## First Functional Target

The first meaningful target is:

> **Hip flex assist for swing initiation**

That means helping the thigh begin moving upward and forward during gait, especially when fatigue or weakness makes that motion hard.

Secondary future targets may include:

- toe-clearance assist
- fatigue-adaptive profiles
- left/right asymmetry tuning
- variable assist for good-day / bad-day conditions

---

## Design Philosophy

- **augment, don’t replace**
- **compliance over rigidity**
- **minimal force, maximum effect**
- **failure should be safe and boring**
- **build the smallest useful thing first**
- **tune to human movement, not idealized motion**

---

## Architecture Overview

### 1. Anchor System
A pelvic belt and upper-thigh interface provide a stable force path without requiring a hard mechanical hip joint.

### 2. Force Transmission
Cable routing is used to create a useful hip-flexion moment while keeping the system lightweight and modular.

### 3. Compliance Layer
Elastic tubing or spring elements provide preload, smoothing, energy storage, and more natural follow-through.

### 4. Actuation
A waist-mounted spool or winch tensioner adjusts cable length and assist timing.

### 5. Sensing
Initial prototypes may use only an IMU. Later versions may add tension sensing, foot contact, and gait-state classification.

### 6. Control
The system begins with a simple state machine and evolves toward adaptive assist tuned to the individual.

---

## Repo Structure

```text
ghost-walker/
├── README.md
├── LICENSE
├── docs/
│   ├── architecture.md
│   ├── biomechanics.md
│   ├── prototype-layout-v1.md
│   ├── force-vector-studies.md
│   └── control-model.md
├── hardware/
│   ├── anchor-system/
│   │   └── README.md
│   ├── cable-routing/
│   │   └── README.md
│   ├── compliance/
│   │   └── README.md
│   └── actuator/
│       └── README.md
├── software/
│   ├── control-loop/
│   │   └── README.md
│   ├── sensor-fusion/
│   │   └── README.md
│   └── profiles/
│       └── README.md
├── experiments/
│   ├── hip-flex-test/
│   │   └── README.md
│   └── cable-force-rig/
│       └── README.md
└── media/
    └── README.md
```

---

## First Prototype Goal

The first prototype does not need to be elegant.

It needs to answer one question:

> **Can a waist-to-thigh compliant cable assist make leg lift and forward swing meaningfully easier without feeling unnatural?**

That is the threshold test.

---

## Prototype Strategy

Rev 1 should prioritize:

- one leg
- one assist path
- one cable
- one compliance element
- one simple control loop
- safe manual override
- easy mechanical adjustment

Do not optimize for polish first.  
Optimize for **truth**.

---

## Safety Notes

This is an experimental open-source mobility-assist project.  
It is not a certified medical device.

Early prototypes should be tested:

- with support nearby
- with controlled environments
- with low force limits
- with quick-release / kill-switch behavior
- with conservative assumptions

---

## Open Source

Ghost Walker is intended to stay open.

The purpose of this project is to explore a new class of lightweight mobility augmentation that is:

- understandable
- modifiable
- repairable
- affordable
- shared

---

## Near-Term Roadmap

- [ ] Define first force-path candidates
- [ ] Build a one-leg bench/standing test rig
- [ ] Measure subjective usefulness of assist
- [ ] Compare elastic-only vs active-tension assist
- [ ] Build simple gait-state controller
- [ ] Add tuning profiles
- [ ] Explore passive-fail / low-power behavior

---

## Project Motto

> **Influence motion. Don’t dictate it.**
