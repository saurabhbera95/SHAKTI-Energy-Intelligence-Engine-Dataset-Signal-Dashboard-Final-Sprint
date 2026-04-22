# SHAKTI-Energy-Intelligence-Engine-Dataset-Signal-Dashboard-Final-Sprint

Overview

This project implements a deterministic energy intelligence system that processes multi-device energy data and generates structured, traceable signals and actions.
The system is designed to operate under realistic conditions with validation, domain logic, and dashboard outputs — without using any machine learning.

Pipeline Flow

Dataset → Validation → Metrics → Signal Engine → Routing → Output → Dashboard

Key Features

🔹 Multi-device dataset (supply, demand, renewable, region)
🔹 Validation layer (ALLOW / FLAG / REJECT)
🔹 Energy domain logic (efficiency, renewable ratio)
🔹 Deterministic signal generation
🔹 Role-based + region-based routing
🔹 Deep traceability (input → computation → signals)
🔹 Dashboard visualization (charts)

Core Signals

SUPPLY_DEMAND_GAP,
LOW_EFFICIENCY,
LOW_RENEWABLE_USAGE

Sample Output
{
  "device_id": "S2",
  "signals": ["SUPPLY_DEMAND_GAP", "LOW_EFFICIENCY", "LOW_RENEWABLE_USAGE"],
  "actions": ["GRID_OPERATOR_South", "MAINTENANCE_TEAM", "SUSTAINABILITY_TEAM"],
  "trace": {
    "input": {"supply": 80, "demand": 110},
    "computed": {"efficiency": -0.375, "renewable_ratio": 0.25},
    "signals": ["SUPPLY_DEMAND_GAP", "LOW_EFFICIENCY", "LOW_RENEWABLE_USAGE"],
    "validation": "FLAG"
  }
}

Dashboard

The system includes basic visualizations:

Efficiency per device,
Renewable usage per device

System Properties

Deterministic (no ML / no black-box),
Traceable (full decision transparency),
Modular pipeline,
Handles multi-device data,
Executable end-to-end

Summary

This project demonstrates a working energy intelligence pipeline that moves beyond static demos to a multi-device, rule-based system with validation, domain logic, and visualization, aligned with real-world execution requirements.





