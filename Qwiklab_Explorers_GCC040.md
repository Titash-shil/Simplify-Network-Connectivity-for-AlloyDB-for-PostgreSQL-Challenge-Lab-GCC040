# Simplify Network Connectivity for AlloyDB for PostgreSQL: Challenge Lab || [GCC040](https://www.cloudskillsboost.google/catalog?locale=tr) ||

## # Like, comment, share & Don't forget to subscribe [QwikLab Explorers](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN) 👍😄🤝

---
## ⚠️ **Disclaimer:**
#### This script and guide are provided for educational purposes to help you understand the lab process. Please ensure you understand the steps before using any scripts. Before using the script, I encourage you to open and review it to understand each step.The goal is to help you learn how to complete the labs effectively while following Qwiklabs' terms of service and YouTube's community guidelines.
---

### Run the following Commands in CloudShell

```
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/refs/heads/master/Simplify%20Network%20Connectivity%20for%20AlloyDB%20for%20PostgreSQL%20Challenge%20Lab/quicklabgcc040.sh
sudo chmod +x quicklabgcc040.sh
./quicklabgcc040.sh
```
- After  Completing Execution on Cloud Shell, then only proceed next step.
---
- Go to SSH into the ``cloud-vm`` VM instance

```bash
psql -h REPLACE_IP -U postgres -d postgres
```
---
```bash

CREATE TABLE patients (
    patient_id INT PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    date_of_birth DATE,
    medical_record_number VARCHAR(100) UNIQUE,
    last_visit_date DATE,
    primary_physician VARCHAR(100)
);


INSERT INTO patients (patient_id, first_name, last_name, date_of_birth, medical_record_number, last_visit_date, primary_physician)
VALUES 
(1, 'John', 'Doe', '1985-07-12', 'MRN123456', '2024-02-20', 'Dr. Smith'),
(2, 'Jane', 'Smith', '1990-11-05', 'MRN654321', '2024-02-25', 'Dr. Johnson');


CREATE TABLE clinical_trials (
    trial_id INT PRIMARY KEY,
    trial_name VARCHAR(100),
    start_date DATE,
    end_date DATE,
    lead_researcher VARCHAR(100),
    number_of_participants INT,
    trial_status VARCHAR(20)
);


INSERT INTO clinical_trials (trial_id, trial_name, start_date, end_date, lead_researcher, number_of_participants, trial_status)
VALUES 
    (1, 'Trial A', '2025-01-01', '2025-12-31', 'Dr. John Doe', 200, 'Ongoing'),
    (2, 'Trial B', '2025-02-01', '2025-11-30', 'Dr. Jane Smith', 150, 'Completed');
```


---

## Congratulations ..!!🎉  You completed the lab shortly..😃💯

## *Well done..!* 👏

## Thank you for visiting... :) 🗯️

## [QwikLab Explorers](https://youtube.com/@titashshil?si=RgamNu1dc9jVIbJN)

## Join to our community [Digital Dominators](https://chat.whatsapp.com/J0o1beFGCHfJ8ZHGKjcqkd)

## Stay Connected with Our Community! 💬 
