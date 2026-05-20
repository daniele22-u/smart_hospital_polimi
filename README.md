# Smart Hospital – ICU Intelligent Monitoring
**Politecnico di Milano** | Corso Smart Hospital | 2025–2026

Analisi multimodale di dati ICU e predizione della mortalità in terapia intensiva.

## Contenuto

| File | Descrizione |
|------|-------------|
| `notebook_tasks_1_4_2.ipynb` | Notebook principale — Task 1–4 (threshold calibration, IQR features, CNN architecture, subgroup analysis) |
| `smart_hospital_tasks_report.html` | Report bilingue (IT/EN) con risultati e interpretazione clinica di tutte le task |

## Dataset

Coorte sintetica ispirata a MIMIC-III: 500 pazienti ICU, 1717 osservazioni, 10 diagnosi, mortalità 12.6%.

## Modelli

- **XGBoost** con 5-fold Stratified CV + SMOTE → OOF AUROC 0.8646
- **1D-CNN** temporale → OOF AUROC 0.7916
- **Ensemble** (media pesata OOF) → OOF AUROC 0.8377
