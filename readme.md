# Applied Data Analytics

Repository for the training program focused on TANF and employment data; developed for the UMD 2018 program.

### Projects
This program is centered around a core data analytics project. The projects in this program focused on return to TANF and combined TANF spells with individuals' employment history from UI wage records.

### Datasets
The primary datasets used in the program are all stored in the PostgreSQL database called `appliedda` on the ADRF; the datasets are:
1. Quarterly Census of Employment and Wages (QCEW) - this is a federally mandated program, and it is also used in conjunction with the Unemployment Insurance program at the Census Bureau to produce the Longitudinal Employer Household Dynamics datasets. There are two data tables associated with the QCEW dataset and for this program we have acess to both for IL and MO:
  + Business data - in the program database the tables are `kcmo_lehd.mo_qcew_employers` and `il_des_kcmo.il_qcew_employers`
  + Job data -  in the program database the tables are `kcmo_lehd.mo_wage` and `il_des_kcmo.il_wage`
2. Illinois Department of Human Services - the class will also have access to case data from IDHS on administering TANF, SNAP, and cash assistance programs; these data are in the `il_dhs` schema
3. Illinois Department of Corrections - this data is from administering State prisons and includes tables for:
  + Admissions to prison - `il_doc_kcmo.ildoc_admit`
  + Exits from prison - `il_doc_kcmo.ildoc_exit`
  + and some auxiliary tables for code definitions and parolees

### Jupyter kernel
The Python3 kernel used in these notebooks was using the `requirements.txt` file.
