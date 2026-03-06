# igss-db

## Project Idea

**Title:**
Intelligent garbage sorting system

**Purpose:**
Create a database that stores and analyzes real-time waste classification data from a single ESP32-CAM with AI model and a rotating 4-bin mechanism. The system tracks:

* Waste classifications (label + confidence)

* Which bin each item is sent to (via motor rotation)

* Simulated bin fill levels to allow analytics

The goal is to monitor waste distribution, understand bin usage, and demonstrate real-time IoT data handling.

## Functional Requirements
**1. Record AI Classifications where each detection includes**
* Label (paper, plastic, metal, other)
* Confidence
* Timestamp
* Bin slot (1–4)

**2.Track Bins**
* Store information about each bin (waste type, capacity)

**3.Simulated Bin Fill Levels**
* Calculate fill percentage based on number of items detected
* Update per item for analytics

**4.Analytics Queries**
* Most common waste type
* Bin usage statistics
* Average AI confidence per type
* Trends over time
