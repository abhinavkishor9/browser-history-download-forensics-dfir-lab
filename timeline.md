# Investigation Timeline

## Overview

This timeline reconstructs the sequence of user activity by correlating Microsoft Edge browser artifacts with Windows file system evidence. The objective is to establish a chronological view of browsing activity, file downloads, and artifact verification performed during the investigation.

> **Note:** This investigation was conducted in a controlled lab environment for educational purposes. The timestamps below are representative of the investigative workflow rather than actual incident timestamps.

---

## Investigation Timeline

| Step | Activity | Evidence Source | Investigation Purpose |
|------|----------|-----------------|-----------------------|
| 1 | Opened Microsoft Edge browser | User Activity | Begin investigation of browser artifacts |
| 2 | Reviewed browsing history | Edge History | Identify websites visited by the user |
| 3 | Examined download history | Edge Downloads | Identify downloaded files and associated URLs |
| 4 | Located downloaded files in the Downloads folder | Windows File Explorer | Verify downloaded files exist on disk |
| 5 | Reviewed file properties | NTFS File Metadata | Validate file name, size, and timestamps |
| 6 | Compared browser download records with Windows metadata | Browser + File System | Correlate multiple evidence sources |
| 7 | Captured screenshots of forensic artifacts | Investigation Documentation | Preserve evidence for reporting |
| 8 | Documented findings | Investigation Notes | Summarize observations and conclusions |

---

## Evidence Correlation

The investigation correlated multiple forensic artifacts rather than relying on a single evidence source.

| Artifact | Evidence Obtained |
|----------|-------------------|
| Browser History | Websites visited during the investigation |
| Download History | Downloaded file names and download events |
| Downloads Folder | Physical presence of downloaded files |
| File Metadata | File timestamps and attributes |
| Investigation Notes | Analyst observations and documented findings |

---

## Investigation Flow

```text
User Browsing
        │
        ▼
Browser History Review
        │
        ▼
Download History Analysis
        │
        ▼
Downloads Folder Verification
        │
        ▼
File Metadata Validation
        │
        ▼
Evidence Correlation
        │
        ▼
Timeline Reconstruction
        │
        ▼
Investigation Findings
```

---

## Key Findings

- Browser history successfully identified websites visited by the user.
- Download history confirmed files downloaded during the browsing session.
- Windows File Explorer verified that downloaded files were present on disk.
- File metadata aligned with browser download records, increasing confidence in the investigation.
- Correlating browser artifacts with Windows file system evidence enabled reconstruction of user activity.

---

## DFIR Analyst Notes

This investigation demonstrates the importance of correlating multiple forensic artifacts when reconstructing user activity. Browser history provides evidence of websites visited, while download history and Windows file metadata independently validate that downloaded files exist and were stored on the endpoint.

Using multiple evidence sources reduces reliance on any single artifact and improves the reliability of forensic conclusions.

---

## Investigation Outcome

**Status:** Completed

**Result:** Browser artifacts and Windows file system evidence were successfully correlated to reconstruct user download activity and validate the integrity of the collected forensic evidence.

---

## Skills Demonstrated

- Browser Artifact Analysis
- Download Forensics
- Windows File System Analysis
- Evidence Correlation
- Timeline Reconstruction
- Digital Forensics and Incident Response (DFIR)
- Incident Documentation
