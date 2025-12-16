# Alzheimer's Disease Tests Database

A SQL Server database schema for storing and managing results from various Alzheimer's disease and cognitive assessment tests.

## Overview

This repository contains SQL table definitions for a comprehensive cognitive assessment database (`NoroNest_TestsDb`). The database is designed to store results from multiple standardized tests used in the diagnosis and monitoring of Alzheimer's disease and other cognitive impairments.

## Database Tables

### 1. MMSE Results (`dbo.mmse_results`)
Mini-Mental State Examination - A widely used test for cognitive impairment screening. 

**Key Fields:**
- Orientation (time and place)
- Registration, attention, and recall scores
- Language and visuospatial skills
- Total score (0-30 scale)
- Diagnosis category classification

### 2. MoCA Results (`dbo.moca_results`)
Montreal Cognitive Assessment - A screening tool for mild cognitive impairment.

### 3. ADAS-Cog Results (`dbo.adas_cog_results`)
Alzheimer's Disease Assessment Scale - Cognitive - A comprehensive neuropsychological test for evaluating cognitive function.

### 4.  AVLT Results (`dbo.avlt_results`)
Auditory Verbal Learning Test - Assesses verbal memory and learning capabilities.

### 5. GDS Results (`dbo.gds_results`)
Geriatric Depression Scale - Screens for depression in older adults, as depression can affect cognitive testing.

### 6. Katz ADL Results (`dbo.katz_adl_results`)
Katz Activities of Daily Living - Evaluates functional independence in daily activities.

## Features

- Structured storage for multiple cognitive assessment types
- Detailed scoring breakdowns for each test component
- Support for qualitative responses (written sentences, verbal responses)
- Test metadata (date, duration, conditions)
- Diagnosis categorization support
- Primary key constraints for data integrity

## Database Structure

All tables are created in the `NoroNest_TestsDb` database and use the `dbo` schema. Each table includes:
- Primary key on `id` field
- Test date tracking
- Detailed subsection scoring
- Total/composite scores
- Optional fields for test-specific metrics

## Usage

1. Create the database: 
```sql
CREATE DATABASE NoroNest_TestsDb;
```

2. Execute each `.sql` file to create the respective tables: 
```sql
USE NoroNest_TestsDb;
-- Run each table creation script
```

## Requirements

- Microsoft SQL Server 2016 or later
- Appropriate database permissions for table creation

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Clinical Context

These assessment tools are commonly used in:
- Alzheimer's disease diagnosis and staging
- Cognitive impairment screening
- Treatment efficacy monitoring
- Clinical research studies
- Longitudinal cognitive decline tracking

---

**Note:** This database schema is designed for research and clinical data management purposes.  Ensure compliance with relevant healthcare data regulations (HIPAA, GDPR, etc.) when implementing in production environments.