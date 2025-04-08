# TOOL-Centers-Capacity

This repository contains tools and data used to define and analyze development capacity in urban centers across the city. The goal is to estimate how much development (jobs and housing) can occur by a given **time horizon** under consistent assumptions, considering market behavior and policy constraints.

## Overview

This tool enables planners and analysts to:

### 1. Define Development Classes & Areas

Group parcels into **development classes** based on shared market patterns and expectations.

- Each class is tied to GIS polygon areas representing neighborhoods, centers, corridors, etc.
- Only **private, non-protected parcels** are considered.

### 2. Set Parameters per Class

Using a consistent **time horizon** (e.g., “by 2045”), define the redevelopment expectations:

- **Eligibility**: Which parcels are likely to develop or redevelop?
  - Based on attributes such as **building age** or **assessed property value**
- **Land Use Mix**: Expected balance between **residential**, **commercial**, etc.
- **Capacity Constraints**: Limits on development intensity such as max FAR, height, or DUA (Dwelling Units per Acre)

### 3. Simulate Growth to Maximum Potential

The model estimates total growth possible within each area:

- Applies eligibility filters and intensity assumptions
- Allocates land use types across developable parcels
- Scales up to represent **maximum realistic capacity** under market and policy constraints

### 4. Generate Reports & Summaries

The tool outputs estimated **jobs** and **housing units** added:

- For each individual area
- Rolled up by **development class**
- Aggregated to **district** and **county** levels

## Why Use a Time Horizon?

Setting a **target year (e.g., 2045)** improves:

- **Realism**: Parameters reflect expected redevelopment over time  
- **Validation**: Results can be checked for plausibility  
- **Consistency**: Different areas and classes operate under the same assumption of how much growth is possible by the time horizon
