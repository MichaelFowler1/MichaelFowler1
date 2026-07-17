# Hi, I'm Michael Fowler

I build **trustworthy autonomy** — systems where non-deterministic AI is supervised by rigid, deterministic software.

Across every project on this profile, the same engineering philosophy shows up: the interesting problem isn't making an AI *smart*, it's building the guardrails, interrupts, and validation layers that let you actually trust it with something that matters — a satellite, a network, a live 3D world.

Background: cleared, NAVAIR. Python · PyTorch · CUDA · Node.js.

---

## Featured Work

### Autonomy under guardrails
- **[apex-minecraft-agent-showcase](https://github.com/MichaelFowler1/apex-minecraft-agent-showcase)** — A 12,000+ line autonomous agent that plays Minecraft end-to-end (punching trees → Ender Dragon). GPT-5.1 acts as a strategic consultant, but a deterministic JavaScript supervisor holds veto power: 20 Hz reflex interrupts, prerequisite enforcement, and an action sanitizer that rejects hallucinated commands before they execute.
- **[homegrown-agent](https://github.com/MichaelFowler1/homegrown-agent)** — An autonomous coding agent built from scratch in PowerShell. No agent frameworks — self-directed goals, sandboxed Docker execution, self-evaluation, and retry. Runs local-first on Ollama or free cloud (Groq).
- **[Sentinel-Node](https://github.com/MichaelFowler1/Sentinel-Node)** — Simulated satellite flight software for fault detection, isolation, and recovery. Linear Kalman filters own the deterministic physics; an LLM generates SITREPs during simulated EW jamming. The math flies the satellite — the AI just explains what happened.
- **[Edge-Adaptive-Heuristic-Node](https://github.com/MichaelFowler1/Edge-Adaptive-Heuristic-Node)** — A self-modifying, offline-first execution environment with AST-validated syntax guarding: code evolves continuously on edge hardware, but nothing runs until it parses clean.

### Sensing & geospatial intelligence
- **[Geoint](https://github.com/MichaelFowler1/Geoint)** — Real-time geospatial common operating picture: GPU object detection on georeferenced overhead imagery (DOTA-trained OBB), fused with live ADS-B air tracks and LLM-generated SITREPs. FastAPI · PostGIS · Leaflet.
- **[satnogs-waterfall-classifier](https://github.com/MichaelFowler1/satnogs-waterfall-classifier)** — ResNet18 transfer learning that triages SatNOGS RF waterfalls into signal vs. noise.
- **[gnss-interference-detector](https://github.com/MichaelFowler1/gnss-interference-detector)** — Detecting GNSS jamming and spoofing from aircraft data.

### Security & edge systems
- **[home-security-auditor](https://github.com/MichaelFowler1/home-security-auditor)** — Read-only home network security auditor: nmap + PowerShell host checks + credential exposure detection, with an LLM-generated kill-chain report and prioritized remediation.
- **[lanledger](https://github.com/MichaelFowler1/lanledger)** — Passive home network monitor on a Raspberry Pi edge sensor with local LLM analysis. No cloud, no payload capture.

---

## Currently building

A passive RF anomaly detector — ESP32 edge sensors feeding a Raspberry Pi analysis node. Same philosophy, smaller hardware.

## Reach me

Open an issue on any repo, or connect through the links on my profile.
