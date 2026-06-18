# Civil Construction Estimation App

# Technical Architecture Document (TAD)

Version 1.0

---

# 1. Architecture Overview

## Objective

Build a professional Residential Construction Estimation Platform supporting:

* Android
* iOS
* Web

with a single codebase.

---

# 2. Technology Stack

## Frontend

Framework:
Flutter

Language:
Dart

Benefits:

* Android
* iOS
* Web
* Single codebase

---

## Backend

Firebase

Services:

* Firebase Authentication
* Cloud Firestore
* Firebase Storage
* Firebase Analytics
* Firebase Crashlytics

---

## Local Database

SQLite

Purpose:

* Offline Estimation
* Fast Calculations
* Local Draft Storage

---

## File Generation

Libraries:

PDF:
pdf package

Excel:
excel package

Charts:
fl_chart

---

# 3. System Architecture

Client Layer

Flutter App

↓

Business Logic Layer

Calculation Engine

↓

Data Layer

SQLite

↓

Cloud Layer

Firebase Firestore

↓

Storage Layer

Firebase Storage

---

# 4. Folder Structure

lib/

core/

features/

shared/

services/

models/

database/

exports/

reports/

main.dart

---

# 5. Core Layer

lib/core/

Contains:

constants/

theme/

utils/

validators/

extensions/

unit_conversion/

---

# 6. Features Layer

Each module independent.

features/

authentication/

dashboard/

projects/

quick_estimate/

plan_estimate/

detailed_estimate/

boq/

reports/

settings/

---

# 7. Project Module Structure

Example:

features/projects/

data/

domain/

presentation/

---

# 8. Models

Project Model

class Project

Fields:

id

projectName

clientName

siteAddress

estimateMode

qualityLevel

floors

unitSystem

createdDate

updatedDate

---

Floor Model

class Floor

id

projectId

floorName

area

height

---

Footing Model

class Footing

id

projectId

type

length

width

depth

quantity

grade

---

Column Model

class Column

id

projectId

width

depth

height

quantity

grade

---

Beam Model

class Beam

id

projectId

width

depth

length

quantity

grade

---

Wall Model

class Wall

id

projectId

material

length

height

thickness

quantity

---

# 9. Database Schema

SQLite Database

construction_estimator.db

Tables:

users

projects

floors

footings

columns

beams

slabs

staircases

walls

openings

plaster

paint

flooring

materials

rates

boq

reports

---

# 10. Firebase Structure

Collection:

users

Document:

userId

↓

projects

Document:

projectId

↓

floors

↓

components

↓

reports

---

Firestore Structure

users

userId

```
profile

projects

   projectId

      projectData

      boq

      reports
```

---

# 11. Authentication

Methods

Email Password

Google Login

Phone OTP

Guest Login

---

# 12. State Management

Recommended:

Riverpod

Reason:

* Lightweight
* Scalable
* Testable

Alternative:

Bloc

---

# 13. Calculation Engine

Separate calculation service.

services/

calculation_engine/

---

Modules

excavation_service.dart

pcc_service.dart

rcc_service.dart

steel_service.dart

brickwork_service.dart

aac_service.dart

plaster_service.dart

paint_service.dart

flooring_service.dart

cost_service.dart

boq_service.dart

---

# 14. Unit Conversion Service

unit_conversion_service.dart

Functions:

ftToMeter()

meterToFt()

sqftToSqm()

sqmToSqft()

cftToCum()

cumToCft()

brassToCum()

cumToBrass()

---

# 15. Concrete Library Service

concrete_mix_service.dart

Stores:

PCC

M15

M20

M25

M30

Methods:

getCement()

getSand()

getAggregate()

---

# 16. Steel Library Service

steel_service.dart

Stores:

Bar Weights

Development Length

Lap Length

Methods:

calculateSteelWeight()

calculateLd()

calculateLap()

generateBBS()

---

# 17. Masonry Service

brickwork_service.dart

Functions:

calculateBrickwork()

calculateMortar()

calculateBrickQuantity()

---

aac_service.dart

Functions:

calculateAACBlocks()

calculateAdhesive()

---

# 18. Finishing Service

plaster_service.dart

paint_service.dart

flooring_service.dart

door_service.dart

window_service.dart

---

# 19. Cost Engine

cost_service.dart

Functions:

calculateMaterialCost()

calculateLabourCost()

calculateTotalCost()

calculateProfit()

generateQuotation()

---

# 20. BOQ Engine

boq_service.dart

Generates:

Quantity BOQ

Material BOQ

Cost BOQ

---

Output Models

BOQItem

MaterialSummary

CostSummary

---

# 21. PDF Engine

report_pdf_service.dart

Sections:

Cover Page

Project Details

BOQ

Material Summary

Cost Analysis

Charts

---

# 22. Excel Engine

report_excel_service.dart

Sheets:

Project Summary

Structural BOQ

Masonry BOQ

Finishing BOQ

Material Summary

Cost Analysis

Rate Profile

---

# 23. Rate Library Module

rate_service.dart

Supports:

Default Rates

Custom Rates

Saved Profiles

---

Profiles:

Kolhapur 2026

Raigad Rural

Mumbai Premium

User Defined

---

# 24. Auto Save System

Every 30 seconds

OR

On field change

Save to SQLite

Sync to Firebase

When internet available

---

# 25. Project Backup

Manual Backup

Auto Backup

Restore Backup

Cloud Sync

---

# 26. Security

Firebase Rules

Project Ownership Validation

Encrypted Authentication

Role Based Access

---

# 27. Performance Requirements

Project Opening

< 2 seconds

Estimate Generation

< 3 seconds

BOQ Generation

< 5 seconds

PDF Generation

< 10 seconds

---

# 28. Logging

Crashlytics

Analytics

Performance Monitoring

---

# 29. Future AI Architecture

ai/

drawing_reader/

quantity_extractor/

cost_optimizer/

material_planner/

---

Version 2

Input:

PDF

Image

DWG

Output:

Automatic Quantity Takeoff

---

# 30. Deployment

Android

Google Play Store

---

iOS

Apple App Store

---

Web

Firebase Hosting

Custom Domain

---

# 31. Development Roadmap

Phase 1

Authentication

Dashboard

Projects

SQLite

---

Phase 2

Quick Estimate

Calculation Engine

Rate Profiles

---

Phase 3

Detailed Estimate

Structural Modules

Masonry Modules

---

Phase 4

BOQ

PDF

Excel

---

Phase 5

Cloud Sync

Subscriptions

Analytics

---

Phase 6

AI Drawing Reader

Quantity Extraction

Cost Optimization

---

END OF TECHNICAL ARCHITECTURE DOCUMENT
