# 03 — Implementation Guide

This guide explains how to set up a practical record-keeping system that complies with CASA requirements. It covers both paper-based and simple digital approaches. You don't need expensive software — you need consistency.

Last review: 18 April 2026

---

## Core Principles

Before choosing tools, understand these principles. They apply regardless of whether you use paper, spreadsheets, or software:

1. **One system, used consistently.** A simple system used every time beats a sophisticated system used occasionally.
2. **Complete records at the time.** Pre-flight records before the flight. Post-flight records immediately after. Don't batch them up a week later.
3. **Every record must be findable.** If CASA asks for the JSA from operation BH-0045, you should be able to locate it in under two minutes.
4. **Back up everything.** Paper gets lost. Hard drives fail. Have at least two copies of your records.
5. **7 years minimum.** Don't delete anything unless you're certain it's past the retention period.

---

## Option 1: Paper-Based System (Rarely Used)

In reality, almost all operators today use a digital system. If you're reading this guide, you're likely already working on a laptop or managing files electronically.

A paper-based system is still technically acceptable, but it is rarely used in practice due to limitations in scalability, searchability, and audit readiness.

If you still prefer a paper approach for very low-volume operations, you can follow the same structure outlined in the digital system — just in printed form.

### What You Need

- A ring binder or expanding file, divided into sections  
- Printed copies of the Operations Record and Personnel/Training Record templates  
- A consistent naming system for individual job folders  

---

## Option 2: Simple Digital System

This is the recommended approach for most small operators. You don't need specialist software, cloud storage and spreadsheets are enough.

### Platform Options

| Platform | Cost | Notes |
|---|---|---|
| Google Drive + Google Sheets | Free | Good collaboration features. Accessible anywhere. |
| Microsoft OneDrive + Excel Online | Free (basic) / included with Microsoft 365 | Better Excel compatibility. Good for operators already using Microsoft. |
| Dropbox + spreadsheets | Free (basic) | Simple file storage. Less suited for collaborative editing. |

Any of these will work. The important thing is to pick one and use it consistently.

### Folder Structure

Set up your cloud storage with this structure:

```
📁 [Company] RPAS Records/
│
├── 📁 01 Operations Manual/
│       Current operations manual (PDF or Word)
│       Previous versions (keep for reference)
│
├── 📁 02 Certificates & Approvals/
│       ReOC certificate
│       CASA instruments / exemptions
│       Insurance certificates
│
├── 📁 03 Operational Records/
│       📄 Operations_Record.xlsx          ← master spreadsheet
│       📁 Job Files/
│           📁 AB-001_RoofInspection_20260110/
│               JSA.pdf
│               RA.pdf
│               FlightPlan.pdf
│               SitePhotos/
│           📁 AB-002_SolarClean_20260115/
│               JSA.pdf
│               ...
│
├── 📁 04 Personnel & Training/
│       📄 Personnel_Training_Record.xlsx   ← master spreadsheet (two sheets)
│       📁 Personnel Files/
│           📁 Smith_John/
│               Induction_Record.pdf
│               RePL_Copy.pdf
│               Assessment_Forms/
│           📁 Tommy_Smith/
│               ...
│
├── 📁 05 Aircraft Records/
│       📁 AB-M400-001/
│           📄 TechnicalLog.xlsx
│           📁 Maintenance/
│               Service_20260301.pdf
│               PropReplacement_20260315.pdf
│       📁 AB-M4T-001/
│           ...
│
├── 📁 06 Pilot Logs/
│       📄 PilotLog_SmithJohn.xlsx
│       📄 PilotLog_TommySmith.xlsx
│
└── 📁 07 Archive/
        Records older than current year but within 7-year retention
```

### File Naming Conventions

Use consistent naming to make files searchable:

**Operations:**
```
[CompanyName]-[OpID]_[DocType]_[YYYYMMDD].[ext]

Examples:
AB-0045_JSA_20260415.pdf
AB-0045_RA_20260415.pdf
AB-0045_FlightPlan_20260415.pdf
```

**Training:**
```
TR-[Ref]_[TraineeName]_[TrainingType]_[YYYYMMDD].[ext]

Examples:
TR-001_SmithJ_Induction_20260415.pdf
TR-002_SmithJ_M400TypeRating_20260418.pdf
```

**Aircraft:**
```
[AircraftID]_[DocType]_[YYYYMMDD].[ext]

Examples:
AB-M400-001_Service_20260301.pdf
AB-M400-001_FirmwareUpdate_20260310.pdf
```

### Version Control

For your master spreadsheets (Operations Record and Personnel/Training Record), version control is important:

1. **Use the live file** as your current working document. Don't create copies for each update.
2. **At the end of each month or quarter**, save a dated snapshot (e.g. `Operations_Record_Snapshot_202604.xlsx`) in the Archive folder.
3. **Never delete rows** from the master spreadsheet. If you need to correct an entry, add a note in the Notes column — don't overwrite the original.
4. If using Google Sheets, the built-in **version history** acts as automatic version control.

### Backup Strategy

Follow the **3-2-1 rule**:

- **3** copies of your data
- **2** different storage types (e.g. cloud + local hard drive)
- **1** copy offsite (the cloud copy counts)

Practical approach:

1. **Primary:** Cloud storage (Google Drive / OneDrive) — this is your working copy.
2. **Secondary:** Monthly download of the entire folder to a local external drive.
3. **Tertiary:** The cloud provider's own redundancy (built in to Google/Microsoft).

---

## Setting Up the Templates

### Step 1: Copy the Template Files

Download the template spreadsheets from this repository:

- `Template_Operations_record.xlsx` — your combined operational record
- `Template_Personnel_Training_record.xlsx` — your personnel register and training log

Place them in your `Operational Records` and `Personnel & Training` folders respectively.

### Step 2: Customise for Your Operation

Before first use:

1. Upadate with your own **company name** throughout.
2. Add your **Organisation / Individual ARN**.
3. **Update the operation ID prefix**.
4. **Review the aircraft type columns** in the Personnel Register and update to match your fleet.
5. **Read the Guide sheet** in the Operations Record, it maps every column to its MOS 101 reference.

### Step 3: Start Using Them

Begin with the very next operation. Don't try to backfill old operations: start clean and move forward.

---

## Daily Workflow

Here's what the record-keeping process looks like for a typical operation:

### Before the Flight

1. Open the Operations Record spreadsheet.
2. Create a new row with the next operation ID.
3. Complete all pre-flight columns (B through P): date, purpose, aircraft, location, crew, VLOS type, serviceability, release approval.
4. Complete and file the JSA (and RA/flight plan if applicable) in the job folder.
5. Mark the document tracking columns (U, V, W) once documents are filed.

### During the Flight

6. Fly the operation as planned.
7. Note any deviations, unserviceability, or incidents.

### After the Flight

8. Complete the post-flight columns (Q through T): actual times, flight segments, unserviceability, PIC sign-off.
9. If the operation was "as per release," simply note that, you don't need to repeat everything.
10. Update the pilot's personal Remote Pilot Log.
11. Update the RPAS Technical Log with flight hours/cycles for the aircraft used.

### After Training Events

12. Add a new row to the Training Log with all required fields.
13. Update the relevant person's entry in the Personnel Register to reflect any new qualifications or approvals.
14. File assessment forms in the person's individual folder.

---

## Tips for Sole Operators

If you're a sole operator (ReOC holder, CRP, and only RP all in one), the system is the same, but simpler in practice:

- You don't need the "release approved by" field (s10.04(5)).
- Your personnel register has one entry: you.
- Your training log may be minimal, but you should still record any self-directed training or currency activities.
- Your pilot log and operational log will closely mirror each other — but keep them both.
- Don't skip records just because you're the only one who sees them. CASA will also see them.

---
 
**Next:** [04 — Review and Compliance](04-review-and-compliance.md) — how to maintain and audit your records.
