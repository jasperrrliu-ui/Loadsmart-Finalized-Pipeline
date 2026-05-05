# Loadsmart Warehouse Classification Pipeline

This repository contains a geospatial data sampling and image classification pipeline for identifying likely warehouse locations. The project was designed around a practical business question: can we use geospatial signals and map/satellite imagery to help prioritize potential warehouse or logistics-related sites for downstream prospecting and analysis?

The pipeline combines positive warehouse locations, OpenStreetMap-based negative sampling, density-aware sampling logic, hard negative construction, and image model training. The goal is not only to build a classifier, but also to create a structured workflow that can be evaluated, revised, and potentially adapted for production-style lead generation.

---

## Project Motivation

Warehouse identification is useful for logistics, freight, and supply-chain intelligence. A simple model that can score whether a location looks warehouse-like could support:

- lead generation for potential logistics customers;
- prioritization of candidate sites for business development;
- enrichment of geospatial databases;
- scalable screening of locations before manual review.

Instead of treating this as a generic image classification task, this project focuses on the full pipeline: how positive and negative samples are defined, how sampling bias is controlled, how dense warehouse regions are handled, and how model outputs could eventually connect to business value.

---

## Repository Structure

```text
Loadsmart-Finalized-Pipeline/
│
├── Notebook1_Sampling_pipeline.ipynb
├── Notebook_2_Training_Pipeline.ipynb
├── outline_updated.docx
└── update.txt
