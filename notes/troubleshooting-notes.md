# Troubleshooting Notes

## Issue 1

### Browser history appears empty

Possible Causes

- InPrivate browsing was used.
- History was recently cleared.

Resolution

Browse several websites using a normal Edge session before beginning the investigation.

---

## Issue 2

### Downloads do not appear in Download History

Possible Causes

- Download cancelled.
- Browser closed before completion.

Resolution

Download the files again and confirm completion before continuing.

---

## Issue 3

### Downloaded files cannot be located

Possible Causes

- Saved to another folder.
- Browser default download location changed.

Resolution

Open Edge Downloads and choose **Open Containing Folder** to verify the actual location.

---

## Issue 4

### File timestamps appear different

Possible Causes

- File opened after download.
- Metadata updated during editing.

Resolution

Compare Created, Modified, and Accessed timestamps together rather than relying on a single timestamp.

---

## Issue 5

### Browser history timestamps differ slightly

Possible Causes

- Time synchronization
- Browser background activity

Resolution

Small differences are expected. Use the overall sequence rather than exact seconds.

---

## Issue 6

### Investigation folder already exists

Resolution

Delete the existing folder before starting.

```powershell
Remove-Item C:\BrowserForensicsLab -Recurse
```

---

## Issue 7

### Cleanup completed but browser history remains

Expected Behavior

Deleting the investigation folder removes only downloaded files.

Browser history is intentionally preserved because it represents forensic evidence.

---

# Lessons Learned

- Browser history alone is not sufficient evidence.
- Download history validates file acquisition.
- Windows file metadata confirms browser activity.
- Correlating multiple artifacts produces stronger forensic conclusions.
- Timeline reconstruction is an essential DFIR skill.
