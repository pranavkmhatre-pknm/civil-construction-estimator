# Concrete_Library.md

# Civil Construction Estimation App

# Concrete Mix Design Library

Version 1.0

---

# Purpose

This library defines standard concrete mixes, material consumption rates, and calculation formulas used throughout the application.

All calculations are based on 1 m³ of finished concrete.

---

# PCC MIXES

## PCC 1:4:8

Application:

* Foundation Bed
* Lean Concrete

Material Consumption per 1 m³

| Material  | Quantity  |
| --------- | --------- |
| Cement    | 3.4 Bags  |
| Sand      | 0.474 m³  |
| Aggregate | 0.948 m³  |
| W/C Ratio | 0.55–0.60 |

---

## PCC 1:3:6

Application:

* Foundation PCC
* Retaining Wall Base

| Material  | Quantity |
| --------- | -------- |
| Cement    | 4.4 Bags |
| Sand      | 0.462 m³ |
| Aggregate | 0.924 m³ |
| W/C Ratio | 0.55     |

---

## PCC 1:2:4

Application:

* Flooring Base
* Foundation Core

| Material  | Quantity |
| --------- | -------- |
| Cement    | 6.3 Bags |
| Sand      | 0.440 m³ |
| Aggregate | 0.880 m³ |
| W/C Ratio | 0.50     |

---

# RCC MIXES

## M15

Ratio:
1 : 2 : 4

| Material  | Quantity |
| --------- | -------- |
| Cement    | 6.3 Bags |
| Sand      | 0.440 m³ |
| Aggregate | 0.880 m³ |

---

## M20

Default RCC Grade

Applications:

* Footings
* Columns
* Beams
* Slabs
* Staircases

| Material  | Quantity |
| --------- | -------- |
| Cement    | 8.1 Bags |
| Sand      | 0.425 m³ |
| Aggregate | 0.850 m³ |

---

## M25

Applications:

* Heavy Footings
* High Load Columns
* Premium Residential Structures

| Material  | Quantity  |
| --------- | --------- |
| Cement    | 11.1 Bags |
| Sand      | 0.385 m³  |
| Aggregate | 0.770 m³  |

---

## M30

Design Mix

Estimation Purpose Only

| Material  | Quantity     |
| --------- | ------------ |
| Cement    | 380–420 kg   |
| Sand      | 680–720 kg   |
| Aggregate | 1100–1200 kg |

---

# CONCRETE CALCULATION FORMULAS

Volume = Length × Width × Depth

RCC Quantity = Sum of all RCC Volumes

Material Consumption = Concrete Volume × Library Consumption

---

# RMC OPTION

If user selects Ready Mix Concrete:

Skip Cement/Sand/Aggregate calculations.

Cost = RCC Volume × RMC Rate

---

# DENSITY TABLE

| Material | Density    |
| -------- | ---------- |
| PCC      | 2400 kg/m³ |
| RCC      | 2500 kg/m³ |
| Cement   | 1440 kg/m³ |

---

# DRY VOLUME FACTORS

Concrete

Dry Volume = Wet Volume × 1.54

Mortar

Dry Volume = Wet Volume × 1.33

End of File

