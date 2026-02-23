# Case Study: Enterprise Employee Self-Service (ESS) Portal & SAP Integration
**Role:** Co-Project Lead / Systems Architect  
**Org:** Geothermal Development Company  
**Impact:** 40+ Man-Hours Saved Monthly | 100% Paperless HR Operations

---

## 🚀 Executive Summary
Successfully co-led the design and implementation of a SharePoint Online-based Employee Self-Service (ESS) portal. This project bridged the gap between modern cloud interfaces and legacy on-premises SAP systems, digitizing critical HR workflows for 1,000+ employees and eliminating a significant administrative bottleneck.

---

## 🛠️ The Challenge
* **Manual Bottleneck:** HR and Payroll teams were spending 40+ hours per month manually processing paper-based requests for vacations, allowances, and travel.
* **Data Silos:** On-premises SAP data was inaccessible to the remote workforce, leading to delays and "desk-bound" productivity.
* **Employee Friction:** Lack of mobility in submitting requests negatively impacted the employee experience and workforce agility.

---

## 📈 The Strategy: Hybrid Integration & UX
I approached this project with an "Operations-First" mindset, focusing on a seamless user experience backed by robust data integrity.

### 1. Hybrid Architecture
We utilized **SharePoint Online** as the front-end "Action Center" and integrated it with our on-premises **SAP** core. This allowed for real-time data validation (e.g., checking leave balances) without exposing the SAP core directly to the internet.

### 2. Workflow Digitization
Using **Power Automate**, we replaced physical signatures with a multi-level digital approval hierarchy.
- **Vacation Requests:** Auto-calculated balances from SAP.
- **Travel Allowances:** Standardized per-diem calculations with automated manager notifications.

### 3. Change Management
Co-led training sessions to transition a 1,000-user workforce from a "Paper Culture" to a "Digital-First" mindset.

---

## 📊 Logic Flow: From Request to Payroll
*This diagram illustrates the automated bridge between SharePoint and SAP.*

```mermaid
graph TD
    A[Employee: Submits Request in SharePoint] --> B{Manager Approval}
    B -- Approved --> C[Automated Workflow: Logic App/Power Automate]
    B -- Rejected --> D[Notify Employee]
    C --> E[On-Premises Data Gateway]
    E --> F[Update SAP Payroll/HR Module]
    F --> G[Employee Receives Final Confirmation]
