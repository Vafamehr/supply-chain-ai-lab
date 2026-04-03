# Supply Chain AI Lab

## What this is

An end-to-end supply chain decision system that simulates how real-world planning systems operate.

This project goes beyond modeling and focuses on how data, models, and deterministic logic come together to drive operational decisions.

---

## Problem

In real supply chains, decisions are not just predictions.

We need to:

* forecast demand
* evaluate inventory health
* decide how much to replenish
* simulate scenarios under uncertainty
* understand risks like stockouts and overstock

---

## System Overview

The system follows a structured pipeline:

Demand → Inventory → Replenishment → Decision → Simulation → Explanation

---

## Core Components

### Demand Forecasting

Predicts expected demand using historical signals.

### Inventory Evaluation

Computes current stock position and days of supply.

### Replenishment Logic

Determines how much to order based on demand and constraints.

### Decision Coordinator

Orchestrates modules and produces final decisions.

### Scenario Simulation

Evaluates decisions under different conditions (demand spikes, disruptions).

### Disruption Modeling

Injects shocks into the system (supply delays, demand changes).

### Allocation

Distributes inventory across locations.

### Network Monitoring

Tracks system-level health and risks.

### LLM Explanation Layer

Generates human-readable explanations of system decisions.
LLM is used strictly for interpretation, not decision-making.

---

## Design Principles

* Deterministic-first architecture
* Clear separation between modules
* Data → Model → Decision → Evaluation flow
* LLM used only as an explanation layer
* Traceable and interpretable outputs

---

## Why this matters

Most projects stop at prediction.

This system focuses on:

* how predictions translate into decisions
* how decisions behave under scenarios
* how to reason about tradeoffs in operations

---

## How to Run

```bash
python -m src.run_system
```

---

## Repository Structure

```text
src/
  demand_forecasting/
  inventory/
  replenishment/
  decision_coordinator/
  scenario_analysis/
  simulation_engine/
  disruption_modeling/
  allocation/
  network_monitoring/
  decision_intelligence/
  llm_support/
  tools/

docs/
  knowledge/
  architecture/
```

---

## Summary

A modular, deterministic supply chain system that demonstrates how real-world decision pipelines are designed, evaluated, and explained.
