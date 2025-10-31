# ICSR Workflow Simulation Project

A simulated **Individual Case Safety Report (ICSR)** workflow project demonstrating how Adverse Drug Reaction (ADR) cases are received, processed, reviewed, and reported according to pharmacovigilance (PV) standards.

---

## Introduction
This project simulates the **pharmacovigilance workflow** for ICSR case handling using open-source ADR data.  
It aims to provide practical understanding of:
- How case data is collected and validated
- How seriousness and causality are assessed
- How narratives are written and finalized for regulatory submission

---

## Data Source
Data used in this project was derived from **public pharmacovigilance databases**, including:
- [WHO VigiAccess](https://www.vigiaccess.org/)
- [FDA FAERS](https://open.fda.gov/data/downloads/)
- [EU ADR Reports](https://www.adrreports.eu/en/search_subst.html#)
- [OpenVigil](https://openvigil.sourceforge.net/)

For demonstration, cases involving **Amoxicillin-Clavulanic Acid** and **Ibuprofen** were selected, as they are commonly associated with ADRs.

---

## Simulated Case Data

| Case ID | Drug Name | Age/Gender | Reaction | Outcome | Causality |
|----------|------------|-------------|-----------|-----------|------------|
| DEMO-01 | Simvastatin | 51/M | Muscle spasms | Recovered | Probable |
| DEMO-02 | Ciprofloxacin | 38/F | Tendonitis | Not recovered | Possible |
| DEMO-03 | Montelukast | 22/M | Anaphylactic shock | Hospitalization | Definite |
| DEMO-04 | Paracetamol | 17/F | Diarrhea | Not recovered | Possible |
| DEMO-05 | Atenolol–Amlodipine | 65/F | Hypotension | Hospitalization | Probable |
| DEMO-06 | Salmeterol | 33/M | Tremors | Recovered | Probable |
| DEMO-07 | Aceclofenac | 29/F | Indigestion | Recovered | Possible |
| DEMO-08 | Ceftriaxone | 44/F | Injection site edema | Recovered | Definite |
| DEMO-09 | Amoxicillin–Clavulanic acid | 12/M | Skin rash | Recovered | Probable |
| DEMO-10 | Metformin–Glimiperide | 76/M | Hypoglycemia | Hospitalization | Definite |

---

## Workflow Overview

### **1. Case Receipt & Data Entry**
ADR information is recorded in a standardized format (e.g., MedWatch form).

### **2. Case Validation**
Each report is verified for minimum criteria:
- Identifiable patient  
- Identifiable reporter  
- Suspect drug  
- Adverse event

### **3. Case Triage**
Cases are classified as:
- **Serious** — Death, Life-threatening, Hospitalization, Disability  
- **Non-serious** — Recovered, Not hospitalized

### **4. Medical Review**
Each case is assessed using the **Naranjo Causality Assessment Scale**.

**Key Naranjo Questions:**
1. Did the event occur after the drug was administered?  
2. Did the reaction improve after stopping the drug?  
3. Did the reaction reappear on re-administration?  
4. Were there alternative causes?  
5. Was the reaction confirmed by any objective evidence?  
...and others, scored to determine causality (Definite, Probable, Possible).

### **5. Narrative Writing**
Each case includes a medical narrative summarizing:
- Patient demographics  
- Drug details  
- Reaction timeline and outcome  
- Assessment and conclusion

### **6. Case Closure & Submission**
After validation and review, cases are marked complete and prepared for submission to regulatory authorities.

---

## Example Narrative (Excerpt)
**DEMO-01 – Simvastatin**  
A 51-year-old male experienced muscle spasms following simvastatin therapy for dyslipidemia.  
Reaction onset: within 2 hours of dose initiation; resolved upon switching to fluvastatin.  
The case was validated as *non-serious* and medically confirmed.  
Causality: **Probable** (based on temporal relationship and dechallenge).

---

## Summary & Conclusion
This simulation demonstrates a realistic **ICSR processing workflow**:
- Covers end-to-end steps from intake → validation → triage → medical review → narrative writing  
- Uses real-world-like open data for educational demonstration  
- Provides clear understanding of **how pharmacovigilance teams handle ADRs**

Ideal for:
- B.Pharm/M.Pharm students  
- Pharmacovigilance trainees  
- QA/Regulatory professionals exploring ICSR systems

---

## References
1. [VigiAccess – WHO UMC](https://www.vigiaccess.org/)  
2. [FDA FAERS Database](https://open.fda.gov/data/downloads/)  
3. [EU ADR Reports](https://www.adrreports.eu/en/search_subst.html#)  
4. [OpenVigil – SourceForge](https://openvigil.sourceforge.net/)

---

## Author
Thiruven Adhula.  
GitHub: [thiru-2705](https://github.com/thiru-2705)  
Project Repository: [ICSR Workflow Project](https://github.com/thiru-2705/ICSR-Workflow-Project)

---

## License
This project is released for **educational and non-commercial use**.  
You may reuse or adapt with attribution.

---

