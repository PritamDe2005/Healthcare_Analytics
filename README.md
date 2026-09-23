# Hospital Management & Healthcare Operations Analytics

## Project Overview

Hospital Management & Healthcare Operations Analytics is a Python-based business intelligence project that analyzes hospital appointment, treatment, doctor, patient, and billing data.

The project follows a practical analytics workflow:

**Raw Data → Information → Insights → Decision → Action**

The goal is to help management understand appointment performance, operational drivers, treatment billing, payment exposure, and areas that may require operational attention.

> **Dataset note:** The supplied dataset is synthetic and is intended for analytics/project demonstration.

---

## Objectives

- Track key healthcare operations KPIs.
- Analyze appointment status and monthly trends.
- Compare appointment activity across hospital branches.
- Identify patterns by visit reason and medical specialization.
- Analyze doctor workload.
- Understand treatment-level billed value.
- Monitor payment status and financial exposure.
- Convert analytical findings into practical business actions.
- Provide an interactive notebook-based frontend for filtered exploration.

---

## Key KPIs

The analysis currently reports:

- Total Patients
- Total Doctors
- Total Appointments
- Completed Appointments
- Completion Rate
- Cancellation Rate
- No-show Rate
- Scheduled Appointments
- Total Billed Value
- Paid / Pending / Failed Billing Amount

---

## Main Analysis Areas

### 1. Appointment Performance
Examines Completed, Cancelled, No-show, and Scheduled appointments.

### 2. Monthly Trends
Shows how appointment volume changes throughout the year.

### 3. Branch Analysis
Compares appointment volume and appointment-status patterns across hospital branches.

### 4. Visit Reason Analysis
Examines Checkup, Consultation, Therapy, Follow-up, and Emergency appointments.

### 5. Specialization Analysis
Analyzes appointment patterns across Pediatrics, Dermatology, and Oncology.

### 6. Doctor Workload
Provides doctor-level appointment and billed-value visibility.

### 7. Treatment & Billing
Compares treatment volume, total billed value, and average treatment cost.

### 8. Payment Analysis
Examines Paid, Pending, and Failed payment records.

---

## Technology Stack

- **Python** — Core programming and analysis
- **Pandas** — Data preparation, joining and aggregation
- **NumPy** — Numerical operations
- **Matplotlib** — Charts and dashboard visuals
- **ipywidgets** — Interactive filters
- **Jupyter Notebook** — Combined backend analysis and frontend

---

## Project Structure

```text
Healthcare_Analytics/
│
├── healthcare_analysis_ready.csv
├── Healthcare_Analytics.ipynb
├── Healthcare_Analytics_Report.docx
├── README.md
└── requirements.txt
```

---

## Backend

The backend is implemented inside `Healthcare_Analytics.ipynb`.

It performs:

1. Dataset loading
2. Data cleaning and preparation
3. Date processing
4. Data integration
5. KPI calculation
6. Appointment analysis
7. Branch and specialization analysis
8. Doctor workload analysis
9. Treatment and billing analysis
10. Payment analysis
11. Monthly trend analysis
12. Business insight generation

---

## Frontend

The same notebook contains a lightweight interactive frontend.

Users can select:

- Hospital Branch
- Appointment Status
- Medical Specialty

After selecting filters, the **Apply Filters** button updates the dashboard outputs.

The frontend provides:

- KPI summary
- Monthly appointment chart
- Branch appointment chart
- Treatment billing summary
- Filtered analytical view

This keeps the project within the single notebook code submission while providing both analytical backend and user-facing exploration.

---

## Dataset

The project uses a Hospital Management Dataset containing five related data areas:

- Patients
- Doctors
- Appointments
- Treatments
- Billing

An analysis-ready combined CSV is included in the repository.

The dataset is synthetic, so the findings should be treated as project/demo analytics rather than real hospital performance.

---

## How to Run

### 1. Clone the repository

```bash
git clone github.com/PritamDe2005/Healthcare_Analytics
cd Healthcare_Analytics
```

### 2. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 3. Open the notebook

```bash
jupyter notebook Healthcare_Analytics.ipynb
```

Alternatively, open the notebook directly in VS Code with the Jupyter extension.

### 4. Run the notebook

Run the cells from top to bottom.

For the interactive frontend:

1. Select a Branch.
2. Select a Status.
3. Select a Specialty.
4. Click **Apply Filters**.

---

## Key Findings

The supplied dataset contains:

- **50 patients**
- **10 doctors**
- **200 appointments**
- **₹551,249.85 total billed value**

Appointment status distribution:

- **46 Completed**
- **51 Cancelled**
- **52 No-show**
- **51 Scheduled**

The analysis also identifies branch-level differences, visit-reason patterns, treatment billing differences, doctor workload variation, and payment-status exposure.

For detailed findings, charts, tables, limitations, and recommended actions, see:

**`Healthcare_Analytics_Report.docx`**

---

## Business Insights

Examples of actionable observations from the analysis include:

- Appointment completion is relatively low in the supplied dataset, while cancellation and no-show statuses form a substantial share of records.
- Central Hospital has the highest appointment volume and the highest no-show count.
- Consultation appointments show a relatively high cancellation share.
- Therapy appointments show a relatively high no-show share.
- Chemotherapy has the highest total billed value among the treatment categories.
- MRI has the highest average treatment cost among the listed treatment categories.
- Pending and failed payment statuses represent an important area for payment follow-up.

These are observations from the supplied synthetic dataset and do not establish causal relationships.

---

## Recommended Business Actions

- Introduce appointment reminder and confirmation workflows.
- Monitor appointment status by branch on a regular basis.
- Review scheduling patterns for visit types with higher cancellation/no-show shares.
- Use treatment-level billing summaries for resource and revenue monitoring.
- Create follow-up workflows for Pending and Failed payments.
- In a future version, add fields such as waiting time, length of stay, satisfaction, clinical outcomes, and readmission if those business questions need to be analyzed.

---

## Limitations

- The dataset is synthetic and relatively small.
- Waiting time, bed utilization, length of stay, patient satisfaction, clinical outcomes, and readmission are not available.
- Billing amount equals treatment cost in the supplied data, so the project does not measure profit or margin.
- The analysis identifies patterns but does not establish causation.
- No prediction model is included because the available dataset does not define a sufficiently strong predictive objective for this project.

---

## Submission Contents

The repository contains the main project deliverables:

- `Healthcare_Analytics.ipynb` — Main combined code, analytics and interactive frontend
- `healthcare_analysis_ready.csv` — Analysis-ready dataset
- `requirements.txt` — Python dependencies
- `Healthcare_Analytics_Report.docx` — Project report
- `README.md` — Project documentation and setup instructions

---

## License

This project is created for educational and analytics project purposes.
