# SCENTED_DW

A dimensional data warehouse project designed to model and analyze fragrance-related data using a star schema architecture. This project reflects governance-first engineering, symbolic clarity, and maintainable design principles.

## 🧱 Schema Overview

- **Fact Table**: `FactFragranceRating` — captures user ratings and load dates
- **Dimensions**:
  - `DimFragrance`: fragrance metadata (name, brand, gender)
  - `DimBrand`, `DimGender`, `dim_year`: supporting attributes
  - `DimNote`, `DimAccord`: scent taxonomy
- **Bridge Tables**:
  - `BridgeFragranceNote`: many-to-many relationship with ordered notes
  - `BridgeFragranceAccord`: many-to-many relationship with ordered accords

## 🗺️ Schema Diagram

![SCENTED DW Schema](SCENTED_DW_Data_diagram.png)

## 🧠 Features

- Designed in SQL Server 2022
- Includes stored procedures for dimension and fact table population
- Surrogate keys and referential integrity enforced
- Supports analytical slicing by brand, gender, scent profile, and release year

## 🎯 Purpose

This project demonstrates:
- Dimensional modeling for catalog-style data
- ETL logic using stored procedures
- Governance-first design for maintainability and auditability
- Symbolic and branded alignment in technical architecture

## 🚀 Next Steps

- Extend with reporting layer (Power BI or SSRS)
- Add sample data and query examples
- Integrate with resume_app for cross-project analytics
