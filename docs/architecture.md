# Jeffrey – System Architecture & Privacy Model

Author: Laszlo Czako  
Version: 0.1 – Architecture Declaration  
Year: 2025  

This document defines the core **software–hardware architecture** and **privacy model** for the Jeffrey Personal AI Butler system. It focuses on the local-first design, dual-brain model, device-layer integration, and failsafe controls.

---

## 1. System Goals

Jeffrey is designed as a **personal computing layer**, not just a chatbot.

Core goals:

- Run primarily **on the user’s own hardware** (Mac / home server / future appliance).
- Maintain a **persistent, private memory** that never leaves the device.
- Use a **dual-brain architecture** to keep personal identity separated from internet access.
- Act as an **OS-level assistant** that can access files, automations, and system resources under user control.
- Provide a foundation for a **home-wide personal AI network** (future).

---

## 2. Core Components

### 2.1 Inner Jeffrey (Local Brain)

Inner Jeffrey is the **private core** of the system:

- Runs locally on the user’s device (Mac / home node).
- Stores and manages all **personal memory** (preferences, history, tasks, context).
- Holds the user’s **digital identity layer**.
- Executes sensitive tasks: file operations, local search, document organization, personal workflows.
- Never sends personal data to any external service.

Inner Jeffrey is the only component allowed to read or write long-term user memory.

---

### 2.2 Outer Jeffrey (Web Fetcher)

Outer Jeffrey is the **stateless internet interface**:

- Runs as a separate process/module whose only job is to **fetch public information**.
- Receives **no personal data or identity tokens** from Inner Jeffrey.
- Makes outbound requests, returns raw results, and is treated as an untrusted data source.
- Can be disabled entirely in “Total Offline Mode”.

Outer Jeffrey is deliberately blind to who the user is.

---

### 2.3 Memory Store

The **Jeffrey Memory Store** is a local data layer:

- Encrypted storage on disk (database or structured files).
- Holds user profiles, preferences, routines, and historical context.
- Accessible only by Inner Jeffrey.
- Designed to be portable to a future **dedicated hardware appliance**.

---

### 2.4 Orchestration Layer

A small orchestration layer coordinates:

- Message routing between user → Inner Jeffrey → (optional) Outer Jeffrey.
- Execution of local tools: file access, search, automations, scripts.
- Policy enforcement: what is allowed to be sent outbound, and when.

This layer enforces the rule: **personal data never leaves the Inner Jeffrey boundary.**

---

### 2.5 Interface Layer

This includes:

- Terminal / CLI interface (v0–v1).
- Desktop UI or Raycast-style launcher (v2+).
- Future voice interface for always-on butler mode.

All interfaces talk to Inner Jeffrey; none directly talk to Outer Jeffrey.

---

## 3. Privacy & Data Flow

High-level data principles:

1. **Local by default**  
   - All reasoning about the user, their files, and their history occurs on-device.

2. **One-way internet model**  
   - Outer Jeffrey can fetch data from the web.  
   - It never receives personal context.  
   - It returns raw results to Inner Jeffrey for local processing.

3. **No hidden syncing**  
   - No automatic cloud backup of memory.  
   - Any syncing or export must be explicit and user-controlled.

4. **User-owned kill switches**  
   - Ability to shut off all network usage (software switch).  
   - Future hardware switch on a dedicated appliance to cut outbound connections physically.

---

## 4. Hardware Deployment Model

Jeffrey is intended to evolve through multiple hardware stages:

### Stage 1 – Single Device

- Runs on a user’s Mac or PC.
- Uses local LLM (LM Studio / Ollama) where possible, with optional API fallback.
- Stores memory locally on that machine.

### Stage 2 – Home Node

- Runs on a dedicated home server or mini-PC.
- Exposes API/agents to other devices in the home (laptop, phone, TV, smart speakers).
- All devices talk to the same **Inner Jeffrey** instance.

### Stage 3 – Dedicated Appliance (Future)

- A physical Jeffrey box with:
  - Encrypted storage.
  - Network interfaces.
  - Physical failsafe controls.
- Becomes the **central personal AI and identity hub** for the user’s environment.

---

## 5. Failsafes & Controls

Key safety and control concepts:

- **Network Control:** user can switch between:
  - Full hybrid (Inner + Outer),
  - Local-only (Inner only),
  - Completely offline.

- **Data Boundaries:**
  - Inner Jeffrey never exports raw memory to Outer Jeffrey.
  - Any outbound requests are scrubbed of identity and personal history.

- **Auditability:**
  - Option to log when and how Outer Jeffrey is used.
  - Transparent record of external queries for user review.

---

## 6. Version Roadmap (Architecture View)

- **v0:** Terminal prototype; basic Inner Jeffrey with no Outer Jeffrey.
- **v1:** Local memory + persona behavior; simple orchestration layer.
- **v2:** Integration with local LLM hosts (LM Studio, Ollama).
- **v3:** Raycast/desktop integration and basic OS automations.
- **v4:** Multi-device access within a single home network.
- **v5:** Home-node identity layer for multiple devices and users.
- **v6:** Dedicated hardware appliance running Jeffrey as a personal AI hub.

---

This document codifies the **hardware–software–privacy architecture** for Jeffrey and is intended to serve as the reference point for future technical design, IP protection, and implementation.
