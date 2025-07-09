# 🧱 Project Architecture – Urban Parking Dynamic Pricing

This file outlines the architecture and processing pipeline for the dynamic pricing system built using Python, NumPy, Pandas, and Pathway.

---

## 🔄 Workflow Overview

```mermaid
flowchart TD
    A[Raw Parking Data (CSV)] --> B[Pathway Data Stream]
    B --> C[Feature Engineering]
    C --> D{Model Selection}
    D --> D1[Model 1: Linear]
    D --> D2[Model 2: Demand-Based]
    D --> D3[Model 3: Competitive]
    D1 --> E[Generate Price]
    D2 --> E
    D3 --> E
    E --> F[Final Pricing CSV]
    E --> G[Bokeh Real-Time Visualization]
