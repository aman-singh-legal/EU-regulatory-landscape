# GDPR Article 89 – AI & Research Compliance (Practical Note)

## Purpose
This note explains how **GDPR Article 89** enables the use of personal data
for **research and AI model training**, while protecting individual rights.
It is written for legal, compliance, and tech teams.

---

## What Article 89 Allows
GDPR Article 89 permits the processing of personal data for:
- Scientific or academic research
- Statistical analysis
- Artificial Intelligence / Machine Learning development

**Condition:** Appropriate safeguards must be in place to protect individuals.

---

## Core Principle (In Simple Terms)
> Research and AI are allowed — but privacy must come first.

---

## Key Safeguards Required

### 1. Data Minimisation
- Use only the data strictly necessary for AI training
- Avoid collecting or retaining excess personal information

### 2. Anonymisation (Preferred)
- Remove all identifiers (names, emails, IDs, locations, metadata)
- Ensure re-identification is not reasonably possible
- Once anonymised, the data is no longer “personal data” under GDPR

> Anonymous data falls outside the scope of GDPR (Recital 26)

### 3. Pseudonymisation (Secondary)
- Replace identifiers with codes (e.g., User123)
- Still considered personal data
- GDPR obligations continue to apply

### 4. Purpose Limitation
- Data used for AI training must not be reused for unrelated purposes
  (e.g. marketing or profiling)

### 5. Access & Security Controls
- Limit access to authorised personnel only
- Apply technical and organisational security measures

---

## Interaction with the Right to Erasure (Article 17)

If a user requests deletion:
- All personal identifiers must be deleted
- If training data is **irreversibly anonymised**, it may be retained
- If anonymisation is not possible, the data must be deleted

Models do not usually need retraining if they do not store personal data.

---

## Practical Compliance Architecture (Best Practice)

- Separate identity data from training data
- Anonymise before AI training
- Maintain documentation (RoPA, DPIA if required)
- Apply privacy-by-design principles

---

## Key Takeaway
GDPR does not block AI innovation.
It requires **responsible AI**, built on anonymisation, minimisation,
and strong governance.

---

## References
- GDPR Article 89
- GDPR Article 17
- GDPR Recital 26
