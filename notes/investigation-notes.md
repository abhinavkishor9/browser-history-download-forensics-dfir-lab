# Investigation Notes

## Lab Summary

This investigation demonstrates how browser artifacts can be analyzed to reconstruct user activity using native Windows forensic evidence.

Unlike malware-focused investigations, this lab emphasizes browser history, download records, and file system artifacts.

---

## Investigation Methodology

The investigation followed a structured DFIR workflow:

1. Identify browser activity.
2. Review download history.
3. Verify downloaded files.
4. Compare browser evidence with Windows metadata.
5. Correlate artifacts.
6. Reconstruct the investigation timeline.
7. Document findings.

---

# Browser History

Browser history records websites visited by a user, including visit timestamps and page titles.

It helps investigators determine:

- Websites accessed
- Order of browsing
- Potential phishing activity
- User behavior timeline

In this investigation, Microsoft Edge history showed visits to:

- W3C
- File Examples
- MITRE ATT&CK
- OWASP
- Microsoft Learn
- CISA

These records established the browsing sequence before and after downloads.

---

# Download History

The browser maintains a record of downloaded files.

Observed downloads:

- dummy.pdf
- file-sample_1MB.rtf

The download history provided:

- File name
- Download time
- Download status

This artifact confirmed that both files were successfully downloaded.

---

# File System Verification

Downloaded files were verified inside:

C:\BrowserForensicsLab

The investigation confirmed:

- Files existed
- Creation timestamps matched browser downloads
- Modification timestamps aligned with user activity

This correlation validates the browser evidence.

---

# Evidence Correlation

Multiple artifacts were compared.

Browser History

↓

Download History

↓

Downloaded Files

↓

File Metadata

Each artifact independently confirmed the user's activity.

This is a fundamental DFIR technique because investigators rarely rely on a single source of evidence.

---

# Investigation Timeline

Example

07:02 – Downloaded dummy.pdf

07:04 – Downloaded file-sample_1MB.rtf

07:06 – Visited MITRE ATT&CK

07:06 – Visited OWASP

07:06 – Visited Microsoft Learn

07:06 – Visited CISA

The reconstructed timeline provides a clear sequence of user actions.

---

# Key Findings

• Multiple cybersecurity websites were visited.

• Two files were downloaded successfully.

• Download history matched the downloaded files.

• Windows file metadata confirmed browser evidence.

• Browser artifacts enabled complete reconstruction of user activity.

---

## Analyst Observations

- Browser history alone is insufficient to establish user activity.
- Download history strengthens confidence in browser evidence.
- Windows metadata independently validates downloaded files.
- Evidence correlation reduces the likelihood of false conclusions.

---

# Conclusion

Browser history and download artifacts are valuable sources of digital evidence during forensic investigations.

By correlating browser records with Windows file metadata, investigators can accurately reconstruct user activity and validate downloaded content.
