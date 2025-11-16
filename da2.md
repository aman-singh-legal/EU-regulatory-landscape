# 🔄 Data Lifecycle Map  
### Comprehensive Guidance for GDPR, Privacy, & GRC Workflows

The **data lifecycle** describes how personal data moves through an organization — from collection to deletion.  
Understanding this lifecycle is essential for GDPR compliance, privacy by design, ROPA (Art. 30) accuracy, DPIA quality, and audit readiness.

---

# 1️⃣ Data Lifecycle Stages (High-Level)

Collection →

Ingestion & Entry →

Storage →

Use & Processing →

Sharing & Disclosure →

Transfer (Internal / External / International) →

Retention & Archival →

Deletion / Anonymization

---

# 2️⃣ Detailed Breakdown of Each Stage

## **1. COLLECTION**
How personal data enters the system.

**Sources:**  
- Registration forms  
- Mobile app inputs  
- Website cookies/ trackings  
- CCTV / IoT sensors  
- Support tickets  
- Third-party data providers  

**Compliance Focus:**  
- Lawful basis (Art. 6)  
- Informed consent (Art. 7)  
- Privacy notice (Art. 13)  
- Data minimisation (Art. 5(1)(c))  

---

## **2. INGESTION & ENTRY**
Data enters company infrastructure.

**Examples:**  
- API ingestion  
- CSV uploads  
- CRM/ERP data entry  
- Webhooks  

**Compliance Focus:**  
- Access permissions  
- Secure transfer  
- Logging  

---

## **3. STORAGE**
Data is stored in systems.

**Examples:**  
- Databases (SQL, NoSQL)  
- Cloud storage (AWS S3, Azure Blob)  
- Physical files  

**Compliance Focus:**  
- Encryption (Art. 32)  
- Backups & redundancy  
- Access control policies  
- Retention rules  

---

## **4. USE & PROCESSING**
Data is actively used for business operations.

**Examples:**  
- Sending emails  
- AI/ML training  
- Fraud detection  
- Analytics  

**Compliance Focus:**  
- Purpose limitation (Art. 5(1)(b))  
- Legitimate interest assessments  
- Profiling rules (Art. 22)  
- User rights handling  

---

## **5. SHARING & DISCLOSURE**
Data shared with:
- Cloud vendors  
- Payment processors  
- Support tools  
- Government authorities  

**Compliance Focus:**  
- DPA (Art. 28)  
- Sub-processor list  
- Due diligence  
- Onward transfer rules  

---

## **6. INTERNATIONAL TRANSFERS**
Transfers outside EEA.

**Compliance Focus:**  
- SCCs (Art. 46)  
- Adequacy decisions  
- Transfer Impact Assessments (TIAs)  

---

## **7. RETENTION & ARCHIVAL**
Data is kept only as long as necessary.

**Focus:**  
- Retention schedules  
- Archival policies  
- Audit requirements  
- Storage limitation (Art. 5(1)(e))  

---

## **8. DELETION / ANONYMIZATION**
Final stage.

**Compliance Focus:**  
- Erasure rights (Art. 17)  
- Secure deletion  
- Proof of deletion logs  
- Anonymization best practices  

---

# 3️⃣ Data Lifecycle Map Template (Ready for Use)

| Stage | Source/System | Purpose | Lawful Basis | Storage Location | Retention | Security | Notes |
|-------|---------------|---------|--------------|-------------------|-----------|----------|--------|
| Collection | Signup Form | Account Creation | Contract | Web App | 3 years | HTTPS/TLS |  |
| Processing | Fraud Engine | Fraud Detection | Legitimate Interests | Internal Server | 1 year | Access Control | LIA required |
| Sharing | Payment Provider | Payment Processing | Contract | EU + US | Transaction period | SCCs | TIA needed |
| Deletion | Automated Script | Retention Expiry | Legal Obligation | DB | N/A | Secure Wipe | Evidence logged |

---

# 4️⃣ Visual Diagram (ASCII)
[User]
↓
Data Collection
↓
Ingestion → Storage ← Backups
↓
Processing → Sharing → Transfers
↓
Retention → Archival
↓
Deletion / Anonymization


---

# 5️⃣ Summary  
Use this lifecycle to build:
- DPIAs  
- ROPA entries  
- Incident response paths  
- Vendor assessments  
- Data flow diagrams  

# ⚖️ Lawful Basis Mapping Guide  
### GDPR Article 6 — Operational Mapping for Real-World Systems

Every processing activity requires **one lawful basis** under GDPR.  
Mapping lawful basis ensures accountability and prevents unlawful processing.

---

# 1️⃣ GDPR LAW­FUL BASIS CATEGORIES (Art. 6)

| Basis | Use Case | Notes |
|-------|-----------|-------|
| **Consent** | Marketing emails, cookies | Must be freely given, clear & withdrawable |
| **Contract** | User accounts, payments, service delivery | Most SaaS operations |
| **Legal Obligation** | Tax records, employment data | Cannot be overridden |
| **Vital Interests** | Medical emergencies | Rare in IT companies |
| **Public Task** | Public authorities | Rare in private sector |
| **Legitimate Interests (LI)** | Fraud prevention, analytics | Requires LIA (balancing test) |

---

# 2️⃣ HOW TO MAP LAWFUL BASIS (Step-by-Step)

## **Step 1 — Identify each processing activity**
Examples:
- Collecting user email  
- Running analytics  
- Processing payments  
- AI profiling  
- Customer support logging  

## **Step 2 — Determine purpose**
What business need does it serve?

## **Step 3 — Match the lawful basis**
If multiple fit, choose the **one most appropriate**.

## **Step 4 — Document it**
Add to ROPA + internal systems documentation.

## **Step 5 — Ensure supporting evidence**
Example:  
Consent → stored consent logs  
Legitimate Interest → LIA assessment  

---

# 3️⃣ Practical Mapping Table (Use This on GitHub)

| Processing Activity | Purpose | Lawful Basis | System | Evidence Required | Notes |
|---------------------|----------|--------------|---------|-------------------|--------|
| Account Creation | Provide service | Contract | Web App | Terms acceptance |  |
| Email Marketing | Promotions | Consent | CRM | CMP logs | Needs unsubscribe |
| Fraud Detection | Prevent misuse | Legitimate Interests | Fraud Engine | LIA | High risk |
| Payment Processing | Complete purchase | Contract | Payment Gateway | PCI evidence |  |
| Tax Reporting | Legal compliance | Legal Obligation | Finance | Audit log |  |

---

# 4️⃣ LIA (Legitimate Interest Assessment) Mini-Template
Purpose Test – Why do we need this processing?

Necessity Test – Is it essential?

Balancing Test – Do benefits outweigh risks?

Safeguards – Minimization, anonymization, opt-ou
---

# 5️⃣ Mistakes to Avoid
❌ Using "Consent" when contract or LI is appropriate  
❌ No evidence logs  
❌ Forgetting to update mapping when purposes change  
❌ Mixing marketing & operational consent  

---

# 6️⃣ Summary

Lawful basis mapping creates:
- Transparency  
- Accountability  
- Strong GDPR posture  
- Fewer DSAR disputes  
- Cleaner ROPA entries  
# 📥 DSAR Workflow Guide (Data Subject Access Request)

### GDPR Articles 12–23 — Operational Steps & Templates

A DSAR is a request from an individual to access, rectify, erase, or transfer their personal data.  
This workflow ensures your company responds **within 30 days** and meets GDPR operational standards.

---

# 1️⃣ TYPES OF DATA SUBJECT REQUESTS

| Right | Article | Description |
|-------|----------|-------------|
| Access | Art. 15 | Request copy of data + processing details |
| Rectification | Art. 16 | Correct inaccurate data |
| Erasure | Art. 17 | “Right to be forgotten” |
| Restriction | Art. 18 | Pause processing |
| Portability | Art. 20 | Export in machine-readable format |
| Objection | Art. 21 | Stop processing (esp. marketing) |
| Automated Decisions | Art. 22 | Review of profiling decisions |

---

# 2️⃣ DSAR WORKFLOW (STEP-BY-STEP)

## **Step 1 — Receive Request**
- Common channels: email, webform, support system  
- Must be free of charge (with specific exceptions)

## **Step 2 — Verify Identity**  
- Passport/ID  
- Email verification link  
- Account confirmation  

⚠️ No verification → No data release.

---

## **Step 3 — Acknowledge Request (within 48 hours)**

**Sample text:**
> We have received your request. We will respond within 30 days per GDPR requirements.

---

## **Step 4 — Locate Data Across Systems**
Search across:
- CRM  
- Databases  
- Email logs  
- Internal tools (Asana, Jira)  
- Vendors  
- Backup systems  
- Cloud storage  

---

## **Step 5 — Review for Third-Party Data**
Remove:
- Another user’s personal data  
- Proprietary company information  
- Legally exempt information  

---

## **Step 6 — Prepare Response Package**
For access requests:  
- Provide categories of data  
- Processing purposes  
- Recipients  
- Storage periods  
- Data copies  

For erasure requests:  
- Delete data across systems  
- Document proof  
- Handle exceptions (legal retention)

---

## **Step 7 — Respond Within 30 Days**
- Deliver securely (encrypted PDF or portal)  
- Extend by 60 days only for complex cases  

---

## **Step 8 — Log the Entire Process**
Maintain an internal record:
- Date received  
- ID verified?  
- Systems searched  
- Departments involved  
- Response sent date  
- Exemptions applied  

This is required for **accountability (Art. 5(2))**.

---

# 3️⃣ DSAR Workflow Diagram (ASCII)

tRequest Received
↓
Identity Verification
↓
Acknowledge Request
↓
Data Search in Systems
↓
Review + Redaction
↓
Prepare DSAR Response
↓
Send Securely
↓
Log & Close Case


---

# 4️⃣ DSAR Tracker (Template)

| Request ID | Type | Received | ID Verified | Status | Response Deadline | Owner | Notes |
|------------|------|----------|-------------|--------|-------------------|--------|-------|
| 2025-001 | Access | 02-01-2025 | Yes | In Progress | 01-02-2025 | Privacy Team | CRM + Billing |
| 2025-002 | Erasure | 05-01-2025 | Yes | Completed | 04-02-2025 | IT + Legal | Deleted in all systems |

---

# 5️⃣ Common DSAR Pitfalls

❌ Delayed responses  
❌ Missing data in backups  
❌ Wrong lawful basis causing DSAR conflicts  
❌ Unverified identity → data breach risk  
❌ Employees emailing data insecurely  
❌ Over-deletion (erasing needed legal data)

---

# 6️⃣ Summary  
A strong DSAR workflow protects:
- User rights  
- Company compliance posture  
- Operational efficiency  
- Legal risk management  

Use this workflow to build a robust internal DSAR system.


