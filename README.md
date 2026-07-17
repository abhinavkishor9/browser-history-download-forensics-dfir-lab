# browser-history-download-forensics-dfir-lab
## Overview

This Digital Forensics and Incident Response (DFIR) lab demonstrates how browser artifacts can be used to reconstruct user activity on a Windows endpoint.

The investigation focuses on browser history, download records, file system metadata, and timeline reconstruction using Microsoft Edge and native Windows artifacts.

No malware or third-party forensic tools are required, making this an excellent beginner-friendly DFIR investigation.

---
## Executive Summary

A Windows user reported suspicious browser activity after downloading files from the Internet. This investigation analyzes Microsoft Edge browser artifacts, download records, and Windows file system metadata to reconstruct user activity and validate whether downloaded files correspond to browser evidence.

The investigation follows a structured DFIR methodology by collecting multiple forensic artifacts, correlating evidence, and reconstructing a chronological timeline of user actions.

## Investigation Scenario

The Security Operations Center (SOC) receives a request to investigate suspected unauthorized downloads performed by a Windows user.

The objective is to determine:

- Which websites were accessed
- Which files were downloaded
- Where the files were stored
- Whether browser artifacts align with Windows file system evidence
- Whether a reliable timeline of user activity can be reconstructed
---

## Objectives

- Investigate Microsoft Edge browser history
- Examine browser download history
- Verify downloaded files
- Correlate browser artifacts with Windows file metadata
- Reconstruct the user's activity timeline

---

## Skills Demonstrated

- Browser Artifact Analysis
- Download Forensics
- Windows File System Analysis
- Timeline Reconstruction
- Evidence Correlation
- User Activity Reconstruction
- Incident Documentation
- Windows DFIR Methodology

---

## Tools Used

- Windows 10
- Microsoft Edge
- File Explorer
- PowerShell

---
## Lab Environment

| Component | Details |
|------------|---------|
| Operating System | Windows 10 |
| Browser | Microsoft Edge |
| Investigation Type | Windows Digital Forensics |
| Evidence Sources | Browser History, Download History, File Metadata |
| Analysis Method | Native Windows Artifacts |

---

## MITRE ATT&CK Mapping

| Tactic | Technique | ID |
|---------|-----------|-----|
| Collection | Data from Local System | T1005 |
| Discovery | File and Directory Discovery | T1083 |
| Execution(simulated) | User Execution: Malicious File | T1204.002 |

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

## Evidence Correlation

| Artifact | Investigation Purpose |
|----------|-----------------------|
| Browser History | Identify websites visited |
| Download History | Confirm downloaded files |
| Downloads Folder | Verify file presence |
| File Metadata | Validate timestamps |
| Timeline | Reconstruct user activity |

Rather than relying on a single artifact, the investigation correlates multiple evidence sources to improve confidence in the findings.

---

## Investigation Findings

- Browser history successfully identified websites visited during the investigation.
- Download history confirmed that the expected files were downloaded.
- Windows file metadata validated the download timestamps.
- Browser artifacts and file system evidence were successfully correlated.
- A complete user activity timeline was reconstructed.
  
---

## Key Takeaway

This investigation demonstrates how browser artifacts and Windows file system metadata can be correlated to reconstruct user activity during a forensic investigation. By validating evidence across multiple sources, investigators can establish a reliable timeline and strengthen confidence in their findings.
