# Applied Data Analytics

Repository for the training program focused on TANF and employment data; developed for the UMD 2018 program.

### Projects
This program is centered around a core data analytics project. The projects in this program focused on return to TANF and combined TANF spells with individuals' employment history from UI wage records.

### Training program agenda
- Oct 31 - Program introduction and overview
  - 09:00 - 09:30 Welcome and Introductions
  - 09:30 - 09:45 Goals for the program
  - 09:45 - 10:45 Project scoping
  - 10:45 - 11:00 Break
  - 11:00 - 12:00 Introduction to ADRF and Security Training
  - 12:00 - 01:00 Lunch
  - 01:00 - 01:15 Review of the morning
  - 01:15 - 03:30 Buffet of Analytics topics
  - 03:30 - 04:00 Logging in to the ADRF
- Nov 1 - Data exploration & Visualization
  - 09:00 - 09:15 Welcome and overview of the day
  - 09:15 - 10:30 Databases
  - 10:30 - 10:45 Break
  - 10:45 - 12:00 Data Visualization
  - 12:00 - 01:00 Lunch
  - 1:25 - 04:00 Hands-on data exploration with SQL & Python
- Nov 2 - Record Linkage
  - 09:00 - 10:15 Data Visualization (notebook)
  - 10:30 - 12:00 Record Linkage (lecture, McDonald “An Introduction to Probabilistic Linkage”)
  - 12:00 - 01:00 Lunch
  - 01:00 - 01:45 Guest Lecture, Rick Hendra: Research Evidence on TANF and Employment
  - 01:45 - 02:45 Data preparation: creating "labels"
  - 02:45 - 03:00 Break
  - 03:00 - 04:00 Data preparation: creating "features"
- Nov 5 - Introduction to Machine Learning
  - 09:00 - 12:00 All (almost) of Machine Learning
  - 12:00 - 01:00 Lunch
  - 01:00 - 02:45 Walk through of example ML prediction model
  - 02:45 - 03:00 Break
  - 03:00 - 04:00 Project discussion: label (outcome) definition and features
- Nov 6 - Text Analysis
  - 09:00 - 10:30 Text Analysis
  - 10:30 - 10:45 Break
  - 10:45 - 12:00 Text Analysis
  - 12:00 - 01:00 Lunch
  - 01:00 - 01:15 Project goals and timeline
  - 01:15 - 04:00 Project work (exploration, discussion, planning)
- Dec 5 - Machine Learning - methods
  - 09:00 - 12:00 Machine Learning lecture - recap and methods
  - 12:00 - 01:00 Lunch
  - 01:00 - 02:00 Project discussion - model set-up
  - 02:00 - 04:00 Project work
- Dec 6 - Machine Learning in Practice
  - 09:00 - 12:00 Machine Learning lecture - model selection, evaluation, and bias
  - 12:00 - 01:00 Lunch
  - 01:00 - 04:00 Project work
- Dec 7 - Privacy and Confidentiality
  - 09:00 - 10:30 Privacy & Confidentiality lecture
  - 10:30 - 10:45 Break
  - 10:45 - 12:00 Disclosure review & export requests
  - 12:00 - 01:00 Lunch
  - 01:00 - 04:00 Project work
- Dec 10 - Inference
  - 09:00 - 10:30 Inference lecture
  - 10:30 - 10:45 Break
  - 10:45 - 12:00 Project work
  - 12:00 - 01:00 Lunch
  - 01:00 - 04:00 Project work
- Dec 11 - Final Presentations
  - 09:00 - 09:10 Program recap
  - 09:10 - 11:00 Finalize project presentations
  - 12:00 - 01:00 Lunch
  - 01:00 - 04:00 Final Presentations

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
