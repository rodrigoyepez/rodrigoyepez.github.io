---
title: "NASA Satellite Cloud Classification Pipeline"
excerpt: "Scalable data pipeline improving cloud classification accuracy by 20% using NASA satellite imagery<br/><img src='/images/portfolio-nasa.png' width='500'>"
collection: portfolio
---

## Overview

Developed scalable data pipelines for processing NASA satellite imagery, improving cloud classification by 20% and enhancing weather forecasting models. This project leveraged distributed computing to handle massive amounts of satellite data.

## Technical Approach

### Data Pipeline
```
NASA ABI Data → Data Ingestion → Preprocessing → Feature Extraction
      ↓                                                  ↓
CloudSat/CALIPSO ─────────────────────────────→ ML Classification
                                                         ↓
                                               Weather Forecasting
```

### Machine Learning
- Addressed class imbalance in multi-layer cloud classification
- Developed novel sampling and weighting strategies
- Improved classification accuracy by 20%

### Infrastructure
- Linux-based processing environment
- SQL databases for structured data storage
- Spark clusters for distributed computation

## Impact

- Enhanced accuracy of cloud layer identification
- Improved inputs to weather forecasting models
- Created reusable pipelines for satellite imagery analysis

## Technologies

`Python` `Apache Spark` `SQL` `Linux` `Satellite Imagery` `Machine Learning`

---

*Research conducted at American University's Big Data Lab in collaboration with NASA.*
