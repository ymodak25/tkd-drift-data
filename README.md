# 🥋 Tkd-Drift-Data

![Project Status](https://img.shields.io/badge/Status-Data%20Collection%20Phase-green?style=for-the-badge)
![Research](https://img.shields.io/badge/Focus-Motion%20Analysis-blue?style=for-the-badge)

## 📌 Project Overview
This repository, **tkd-drift-data**, serves as the central data management hub for the **TKD Drift Analyzer** research project. Our primary objective is to quantify technical "drift" in Taekwondo practitioners by comparing high-fidelity motion metrics before and after specific training interventions.

By analyzing motion data captured from volunteers across various skill levels, this research aims to develop automated models for performance evaluation and technical consistency.

---

## 📂 Repository Structure
To maintain a clear audit trail for the research, data is organized chronologically. Each folder corresponds to a specific data collection session.

ROOT/
├── YYYY-MM-DD/               # Collection Date (e.g., 2026-04-12)
│   ├── [Initials]_[Belt]_[Before].csv
│   ├── [Initials]_[Belt]_[After].csv
│   └── [Initials]_[Belt]_[DriftScore].csv
└── README.md

### Data Point Composition
Every unique data point consists of a triplet of files:
1. **Before CSV**: Pose and motion data extracted from the baseline performance video.
2. **After CSV**: Pose and motion data extracted from the post-intervention performance video.
3. **Drift Score**: A computed results file identifying the variance (drift) between the two performances.

---

## 🏷️ Naming Convention
To ensure data integrity and volunteer anonymity, all files follow a strict naming protocol:

**[Initials]_[BeltDegree]_[Phase].[Extension]**

| Component | Description | Example |
| :--- | :--- | :--- |
| **Initials** | First and Last initials of the volunteer. | JD |
| **Belt Degree** | The current rank/degree of the practitioner. | Black1 |
| **Phase** | The state of the data (Before, After, or DriftScore). | Before |

> **Example File:** JD_Black1_Before.csv

---

## 🔄 Update Frequency & Workflow
This repository is updated **weekly**. As volunteers provide new data, folders are synchronized with the latest validated data points. 

* **Weekly Intake:** New data points are added as they are collected from volunteers.
* **Validation:** Each entry undergoes a quality check to ensure the CSV structure matches the analyzer's requirements before being pushed to the main branch.

---

## � Changelog and Observations

### Changelog
- **2026-04-19**: Initial changelog setup. Repository contains data from sessions up to 04-15-2026.

### Observations
- **2026-04-19**: Today marks the day when we have officially collected 10 data points. A big thank you to all the volunteers, Choi's TKD and Master Jennifer for their unbridled support. After looking at the data we found out that despite the level of the student on an average the drift measured was 70-80 percent. It is also worthwhile to note that students were choosing their own three or four steps for the before and after datapoints. Interestingly in the last three data points, when asked explicitly to chose slightly harder steps, the accuracy fell by six to ten percent. We will continue to keep an eye on these trends as we go forward.

---
*This repository is a part of the TKD Drift Analyzer Research Project. For inquiries regarding methodology or data access, please contact the project maintainers.*
