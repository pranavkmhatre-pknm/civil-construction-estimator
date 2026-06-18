# Civil Construction Estimation App

# Screen-by-Screen Functional Specification (SFS)

Version 1.0

---

# SCREEN 1 – SPLASH SCREEN

Purpose:
Application startup screen.

Components:

* App Logo
* App Name
* Version Number

Actions:

* Load user preferences
* Load local database
* Check login status

Navigation:

Splash → Login / Dashboard

---

# SCREEN 2 – LOGIN SCREEN

Components:

* Mobile Number
* Email
* Password

Buttons:

* Login
* Register
* Continue as Guest
* Forgot Password

Validation:

* Mobile Number Required
* Email Format Validation
* Password Minimum 6 Characters

Navigation:

Login → Dashboard

---

# SCREEN 3 – DASHBOARD

Purpose:
Main control center.

Components:

Cards:

* New Project
* Open Project
* Quick Estimate
* Detailed Estimate
* Rate Library
* Reports
* Settings

Recent Projects List

Search Project

Buttons:

* Create New Project
* Open Existing Project

Navigation:

Dashboard → Project Wizard

---

# SCREEN 4 – PROJECT WIZARD

Step 1

Project Details

Fields:

* Project Name
* Client Name
* Mobile Number
* Site Address

Dropdown:

* Structure Type

  * RCC Framed
  * Load Bearing

* Floors

  * GF
  * G+1
  * G+2
  * G+3

* Unit System

  * Metric
  * Imperial

Buttons:

* Save
* Next

Validation:

Project Name Mandatory

---

# SCREEN 5 – ESTIMATION MODE

Options:

○ Quick Estimate

○ Plan Based Estimate

○ Detailed Estimate

Options:

○ Basic

○ Standard

○ Premium

Buttons:

* Previous
* Next

Navigation:

Mode Selection → Respective Module

---

# QUICK ESTIMATE MODULE

SCREEN 6

Fields:

Built-up Area

Floor Count

Quality

Rate Profile

Buttons:

Generate Estimate

Outputs:

* Estimated Cost
* Cost Per Sqft
* Cement Quantity
* Steel Quantity
* Sand Quantity
* Aggregate Quantity
* Brick Quantity

Buttons:

* Export PDF
* Export Excel
* Save Project

---

# PLAN BASED ESTIMATE

SCREEN 7

Building Information

Fields:

Building Length

Building Width

Floor Height

Wall Thickness

Buttons:

Next

---

SCREEN 8

Room Details

Fields:

Room Name

Length

Width

Quantity

Buttons:

Add Room

Remove Room

Next

---

SCREEN 9

Door Schedule

Table:

Door Type

Width

Height

Quantity

Buttons:

Add Door

Next

---

SCREEN 10

Window Schedule

Table:

Window Type

Width

Height

Quantity

Buttons:

Add Window

Next

---

SCREEN 11

Plan Estimate Summary

Outputs:

Wall Area

Brickwork

AAC Quantity

Plaster Area

Paint Area

Flooring Area

Cost Summary

Buttons:

Generate BOQ

Export PDF

Export Excel

---

# DETAILED ESTIMATE MODULE

SCREEN 12

Foundation Module

Table:

Footing Type

Length

Width

Depth

Quantity

Concrete Grade

Buttons:

Add Footing

Delete Footing

Calculate

Outputs:

Excavation

PCC

RCC

Steel

Shuttering

---

SCREEN 13

Column Module

Table:

Column Mark

Width

Depth

Height

Quantity

Concrete Grade

Buttons:

Add Column

Calculate

Outputs:

RCC

Steel

Formwork

---

SCREEN 14

Beam Module

Table:

Beam Mark

Width

Depth

Length

Quantity

Concrete Grade

Buttons:

Add Beam

Calculate

Outputs:

RCC

Steel

Formwork

---

SCREEN 15

Slab Module

Fields:

Area

Thickness

Concrete Grade

Buttons:

Calculate

Outputs:

RCC

Steel

Formwork

---

SCREEN 16

Staircase Module

Fields:

Type

Width

Floor Height

Number of Flights

Buttons:

Calculate

Outputs:

RCC

Steel

Formwork

---

SCREEN 17

Wall Module

Fields:

Material

Length

Height

Thickness

Quantity

Options:

Brick

AAC

Fly Ash Brick

Buttons:

Calculate

Outputs:

Wall Volume

Brick Quantity

AAC Quantity

Mortar

---

SCREEN 18

Opening Module

Door Schedule

Window Schedule

Ventilator Schedule

Buttons:

Calculate Deductions

Outputs:

Deducted Wall Volume

Deducted Plaster Area

Deducted Paint Area

---

SCREEN 19

Plaster Module

Options:

Internal

External

Thickness

Outputs:

Plaster Area

Cement

Sand

---

SCREEN 20

Paint Module

Options:

Putty

Primer

Paint Type

Outputs:

Putty Quantity

Primer Quantity

Paint Quantity

---

SCREEN 21

Flooring Module

Options:

Ceramic

Vitrified

Granite

Marble

Kota

Fields:

Area

Tile Size

Outputs:

Tile Quantity

Mortar

Cement

Sand

---

# COSTING MODULE

SCREEN 22

Rate Profile

Tabs:

Material Rates

Labour Rates

Fields:

Cement Rate

Steel Rate

Sand Rate

Aggregate Rate

Brick Rate

AAC Rate

Buttons:

Save Profile

Create New Profile

Apply Profile

---

SCREEN 23

Cost Analysis

Outputs:

Foundation Cost

Structure Cost

Masonry Cost

Finishing Cost

Labour Cost

Material Cost

Total Cost

Contractor Margin

Final Quote

Charts:

Pie Chart

Bar Chart

---

# MATERIAL PROCUREMENT MODULE

SCREEN 24

Outputs:

Foundation Materials

Structure Materials

Finishing Materials

Stage-wise Quantities

Buttons:

Export Procurement Sheet

---

# BOQ MODULE

SCREEN 25

Quantity BOQ

Table:

Item

Quantity

Unit

Buttons:

Export

---

SCREEN 26

Material BOQ

Table:

Material

Quantity

Unit

Buttons:

Export

---

SCREEN 27

Cost BOQ

Table:

Item

Rate

Amount

Buttons:

Export

---

# REPORTS MODULE

SCREEN 28

PDF Report

Preview

Buttons:

Generate PDF

Download PDF

Share PDF

---

SCREEN 29

Excel Report

Preview

Buttons:

Generate Excel

Download Excel

Share Excel

---

# PROJECT MANAGEMENT

SCREEN 30

Project List

Search

Filters:

Date

Client

Project Type

Buttons:

Open

Duplicate

Delete

Archive

---

# SETTINGS

SCREEN 31

User Profile

Rate Preferences

Units

Theme

Backup Settings

Cloud Sync

---

# ADMIN MODULE (FUTURE)

SCREEN 32

Master Libraries

Concrete Library

Steel Library

Material Library

Door Library

Window Library

Paint Library

Update Default Values

---

# UNIVERSAL FEATURES

Available on all Screens:

* Save Draft
* Auto Save
* Back
* Home
* Help
* Calculator

Validation:

* No Negative Values
* Mandatory Fields Highlighted
* Unit Conversion Automatic

---

# User Journey

Dashboard
→ Project Wizard
→ Estimation Mode
→ Structural Modules
→ Masonry Modules
→ Finishing Modules
→ Costing
→ BOQ
→ Reports
→ Export PDF/Excel

End of Functional Specification
