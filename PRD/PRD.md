# Civil Construction Estimation App

## Product Requirements Document (PRD)

### Version 1.0

---

# 1. Product Overview

## Product Name

Civil Construction Estimation App (Working Name)

## Purpose

Develop a professional construction estimation application for residential buildings that enables homeowners, contractors, architects, and civil engineers to generate:

* Quick construction estimates
* Detailed quantity estimates
* BOQ (Bill of Quantities)
* Material consumption reports
* Cost analysis reports
* Excel exports
* PDF reports

The application shall support estimation from foundation to finishing work.

---

# 2. Target Users

## Homeowner

Can:

* Generate quick estimates
* View project cost
* Compare Basic / Standard / Premium construction

---

## Contractor

Can:

* Generate detailed estimates
* Generate BOQ
* Create quotations
* Analyze project profit

---

## Civil Engineer

Can:

* Create detailed structural estimates
* Generate reinforcement estimates
* Generate material schedules
* Export reports

---

## Architect

Can:

* Generate plan-based estimates
* Estimate masonry and finishing quantities

---

# 3. Supported Projects

Version 1 supports:

* Residential Ground Floor Houses
* G+1 Residential Buildings
* G+2 Residential Buildings
* G+3 Residential Buildings

---

# 4. Estimation Modes

## Mode 1 – Quick Estimate

Inputs:

* Built-up Area
* Number of Floors
* Construction Quality

Outputs:

* Approximate Project Cost
* Cement Quantity
* Steel Quantity
* Sand Quantity
* Aggregate Quantity
* Brick / AAC Quantity

---

## Mode 2 – Plan Based Estimate

Inputs:

* Building Dimensions
* Wall Dimensions
* Door Schedule
* Window Schedule

Outputs:

* Brickwork Quantity
* AAC Quantity
* Plaster Quantity
* Paint Quantity
* Flooring Quantity

---

## Mode 3 – Detailed Estimate

Inputs:

* Footings
* Columns
* Beams
* Slabs
* Staircases
* Walls
* Finishes

Outputs:

* RCC Quantity
* Steel Quantity
* BOQ
* Material Consumption
* Cost Analysis

---

# 5. Construction Quality Levels

## Basic

* M20 Concrete
* Ceramic Flooring
* Standard Paint
* Standard Aluminium Windows

---

## Standard

* M20/M25 Concrete
* Vitrified Flooring
* Emulsion Paint
* UPVC Windows

---

## Premium

* M25 Concrete
* Granite / Marble Flooring
* Premium Paint
* Premium Doors & Windows

---

# 6. Structural Modules

## Excavation

Inputs:

* Length
* Width
* Depth
* Quantity

Outputs:

* Excavation Volume
* Backfilling Volume

---

## PCC

Supported Mixes:

* PCC 1:4:8
* PCC 1:3:6
* PCC 1:2:4

Outputs:

* Cement
* Sand
* Aggregate

---

## Footings

Supported Types:

* Square Isolated Footing
* Rectangular Isolated Footing
* Combined Footing

Outputs:

* RCC Volume
* Steel Quantity
* Shuttering Area

---

## Columns

Inputs:

* Width
* Depth
* Height
* Quantity

Outputs:

* RCC
* Steel
* Formwork

---

## Beams

Inputs:

* Width
* Depth
* Length
* Quantity

Outputs:

* RCC
* Steel
* Formwork

---

## Slabs

Inputs:

* Area
* Thickness

Outputs:

* RCC
* Steel
* Formwork

---

## Staircase

Supported Types:

* Dog-legged
* Open Well

Outputs:

* RCC
* Steel
* Formwork

---

# 7. Masonry Modules

## Brickwork

Outputs:

* Brick Quantity
* Mortar Quantity
* Cement
* Sand

---

## AAC Blockwork

Outputs:

* Block Quantity
* Adhesive Quantity

---

# 8. Finishing Modules

## Plaster

Internal:

* 12 mm
* 15 mm

External:

* 20 mm

Outputs:

* Cement
* Sand

---

## Flooring

Supported Types:

* IPS
* Ceramic Tile
* Vitrified Tile
* Granite
* Marble
* Kota Stone

Outputs:

* Tile Quantity
* Bedding Mortar
* Cement
* Sand

---

## Paint

Supported Types:

* Distemper
* Emulsion
* Luxury Emulsion
* Weatherproof Exterior Paint

Outputs:

* Putty
* Primer
* Paint

---

## Doors

Types:

* Main Door
* Bedroom Door
* Toilet Door

Outputs:

* Door Area
* Frame Length

---

## Windows

Types:

* Aluminium
* UPVC
* Casement

Outputs:

* Window Area
* Frame Length
* Glass Area

---

# 9. Calculation Libraries

The application shall include:

## Unit Conversion Library

* ft ↔ m
* sqft ↔ sqm
* cft ↔ cum
* Brass ↔ cft
* Brass ↔ cum

---

## Concrete Mix Library

* PCC 1:4:8
* PCC 1:3:6
* PCC 1:2:4
* M15
* M20
* M25
* M30

---

## Reinforcement Library

Standard diameters:

* 6 mm
* 8 mm
* 10 mm
* 12 mm
* 16 mm
* 20 mm
* 25 mm
* 32 mm

Supports:

* Development Length
* Lap Length
* BBS Calculations

---

## Masonry Library

* Brickwork
* AAC Blockwork
* Mortar Mixes

---

## Paint Library

Coverage Rates

* Putty
* Primer
* Interior Paint
* Exterior Paint

---

# 10. Costing Engine

Supports:

* Material Costing
* Labour Costing
* Contractor Profit Margin

User may:

* Use default rates
* Create custom rate profiles

Examples:

* Kolhapur Profile
* Raigad Profile
* Mumbai Profile

---

# 11. BOQ System

Generate:

## Quantity BOQ

* Excavation
* PCC
* RCC
* Brickwork
* Plaster
* Flooring

---

## Material BOQ

* Cement
* Steel
* Sand
* Aggregate
* Bricks
* AAC Blocks

---

## Cost BOQ

* Foundation Cost
* RCC Cost
* Masonry Cost
* Finishing Cost

---

# 12. Material Procurement Planner

Generate stage-wise procurement:

## Foundation Stage

* Cement
* Steel
* Sand
* Aggregate

## Structure Stage

* Cement
* Steel
* Shuttering

## Finishing Stage

* Tiles
* Paint
* Putty

---

# 13. Reports

## PDF Report

Include:

* Cover Page
* Project Summary
* BOQ
* Material Summary
* Cost Analysis
* Charts

---

## Excel Export

Sheet 1 – Project Summary

Sheet 2 – Structural BOQ

Sheet 3 – Masonry BOQ

Sheet 4 – Finishing BOQ

Sheet 5 – Material Summary

Sheet 6 – Cost Analysis

Sheet 7 – Rate Library

---

# 14. Database

Core Tables:

* Users
* Projects
* Floors
* Footings
* Columns
* Beams
* Slabs
* Staircases
* Walls
* Openings
* Plaster
* Paint
* Flooring
* Materials
* Rate Profiles
* BOQ
* Reports

---

# 15. Technology Stack

Frontend:
Flutter

Backend:
Firebase

Local Storage:
SQLite

Authentication:
Firebase Authentication

Cloud Sync:
Firebase Firestore

Exports:
Excel (xlsx)
PDF

Platforms:

* Android
* iOS
* Web

---

# 16. Future Version 2 Features

* Floor Plan Reader
* PDF Drawing Reader
* Image Drawing Reader
* AI Quantity Extraction
* AI Cost Optimization
* AI Material Planner

---

# 17. Success Criteria

The application shall enable a user to:

* Create a complete residential estimate
* Generate BOQ
* Generate material summary
* Generate cost analysis
* Export PDF
* Export Excel

within 30 minutes without requiring external software.
