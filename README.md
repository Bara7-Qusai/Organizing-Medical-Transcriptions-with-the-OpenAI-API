# Electronic Medical Records Extraction

This project automates the extraction of key medical information from patient transcription notes and maps recommended treatments to ICD-10 codes using the OpenAI API.

---

## Overview

Medical professionals often summarize patient encounters in free-text transcripts. These transcripts include detailed information on symptoms, diagnosis, and treatments. Manually extracting structured data for billing, research, or insurance purposes is time-consuming and error-prone.

This project leverages OpenAI's GPT models to:

- Extract the patient's age.
- Identify the recommended treatment or procedure.
- Map the treatment to corresponding ICD-10 codes.
- Produce a structured dataset for analysis or integration.

---

## Features

- **Automated Information Extraction:** Extracts patient age and treatment from natural language transcripts.
- **ICD-10 Mapping:** Automatically finds ICD-10 codes for recommended procedures.
- **Error Handling & Retry:** Handles temporary API errors with retry logic.
- **CSV Output:** Saves structured data for further use.
- **Modular and Scalable:** Easy to extend for additional fields like diagnosis or medications.

---

## Data

The dataset used is `transcriptions.csv` with the following columns:

- `medical_specialty`: Medical specialty of the transcription (e.g., Orthopedic, Urology).  
- `transcription`: Full medical transcription in natural language.


---

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Bara7-Qusai/electronic-medical-records.git
cd electronic-medical-records
