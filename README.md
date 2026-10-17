# Azure Databricks Healthcare Medallion

Pipeline Medallion (Bronze / Silver / Gold) sur Azure Databricks + Unity Catalog :
analyse des réadmissions hospitalières à 30 jours.

- Ingestion : Auto Loader (ADLS Gen2, volume externe)
- Silver : SCD1 / SCD2, quarantaine, masquage PII
- Gold : KPI réadmission par hôpital et diagnostic
- Orchestration : Databricks Jobs (Asset Bundle)
- CI/CD : GitHub Actions + service principal
