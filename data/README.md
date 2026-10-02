# Data

The dataset is **not included** in this repository.

It is a **synthetic** ICU cohort inspired by MIMIC-III, provided by the *Smart Hospital* course at Politecnico di Milano. No real patient data is involved.

| | |
|---|---|
| Patients | 500 |
| Observations | 1,717 (long format, 2–5 timesteps per patient) |
| Diagnoses | 10 |
| In-hospital mortality | 12.6% (63 / 500) |

To run the notebook, place the file here as:

```
data/dataset.csv
```

Columns used: `patient_id`, static variables (`age`, `bmi`, `sex`, `diagnosis`, `admission_type`, `icu_los`), vital signs (`hr`, `rr`, `sbp`, `temperature`, `spo2`, `gcs`), laboratory values (`lactate`, `creatinine`, `wbc`, `troponin`, `sodium`, `potassium`, `glucose`) and the outcome `mortality_label`. The column `severity_score`, used only to generate the dataset, is dropped when the data is loaded.
