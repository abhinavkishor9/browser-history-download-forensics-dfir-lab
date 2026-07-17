# browser-history-download-forensics-dfir-lab
## Overview

This Digital Forensics and Incident Response (DFIR) lab demonstrates how browser artifacts can be used to reconstruct user activity on a Windows endpoint.

The investigation focuses on browser history, download records, file system metadata, and timeline reconstruction using Microsoft Edge and native Windows artifacts.

No malware or third-party forensic tools are required, making this an excellent beginner-friendly DFIR investigation.

---

## Investigation Scenario

The SOC receives a request to investigate a user's browsing activity after reports of unauthorized downloads.

As the DFIR analyst, the objectives are to determine:

- Which websites were visited
- Which files were downloaded
- Where the files were saved
- Whether browser evidence matches file system evidence
- Build an activity timeline

---

## Objectives

- Investigate Microsoft Edge browser history
- Examine browser download history
- Verify downloaded files
- Correlate browser artifacts with Windows file metadata
- Reconstruct the user's activity timeline

---

## Skills Demonstrated

- Browser Forensics
- Windows File System Analysis
- Timeline Reconstruction
- Digital Evidence Correlation
- User Activity Reconstruction
- DFIR Documentation

---

## Tools Used

- Windows 10
- Microsoft Edge
- File Explorer
- PowerShell

---

## MITRE ATT&CK Mapping

| Tactic | Technique | ID |
|---------|-----------|-----|
| Collection | Data from Local System | T1005 |
| Discovery | File and Directory Discovery | T1083 |

---

## Investigation Workflow

1. Create investigation workspace
2. Download safe sample files
3. Generate browser history
4. Investigate browser history
5. Review download history
6. Verify downloaded files
7. Correlate browser evidence with file system metadata
8. Build investigation timeline
9. Cleanup environment

---

## Evidence Collected

- Browser History
- Download History
- Downloaded Files
- File Metadata
- Timeline of User Activity

---

## Key Takeaway

Browser history and download artifacts provide valuable forensic evidence for reconstructing user activity. Correlating browser records with Windows file system metadata enables investigators to validate downloaded files, identify user behavior, and establish an accurate investigation timeline.
