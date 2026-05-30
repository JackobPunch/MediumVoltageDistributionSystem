# Medium-Voltage Distribution System Analysis

University project for the *Electrical Devices and Power Networks* course at AGH University of Science and Technology (Kraków). Full analysis of a 15 kV medium-voltage radial distribution network with 15 transformer stations.

## Scope

- **Network design** — 15 transformer stations (3 on main trunk, 12 on branches), mixed overhead AFL and underground Cu cable lines; total length ~40 km
- **Network model** — equivalent π-circuit per segment; resistance and reactance calculated for AFL-70, AFL-35, and Cu-50 conductor types
- **Load estimation** — node currents calculated for peak and off-peak operating states using transformer rated power and load factors
- **Power flow analysis** — current distribution across all segments; conductor cross-sections verified against long-term current capacity (all within limits)
- **Voltage drop analysis** — node voltages calculated from GPZ outward; max deviation 2.69% at peak, 1.62% at off-peak (both within 5% limit)
- **Power losses** — active (ΔP) and reactive (ΔQ) losses per segment for both operating states
- **Annual energy losses** — 525,457 kWh/year, distributed quarterly

## Network Parameters

| Line type | Conductor | Cross-section | R₀ [Ω/km] | X₀ [Ω/km] |
|-----------|-----------|---------------|-----------|-----------|
| Overhead (trunk) | AFL | 70 mm² | 0.433 | 0.4 |
| Overhead (branch) | AFL | 35 mm² | 0.866 | 0.4 |
| Underground cable | Cu | 50 mm² | 0.370 | 0.1 |

## Results Summary

| State | U_min [V] | U_min/U_max [%] | ΔU [%] |
|-------|-----------|-----------------|--------|
| Peak | 14,596 | 97.31 | 2.69 |
| Off-peak | 14,756 | 98.38 | 1.62 |

## Tools

Excel (calculations), hand-drawn network diagram

## Authors

Jakub Cios, Maciej Duda — Electrical Engineering, AGH University of Science and Technology, Kraków
