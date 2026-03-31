# Manual Verification Guide – Lady in the Woods Edition

All material remains untested until it survives explicit human preview and approval.  
T remains sovereign. Human gate only.

### Why you must verify manually
The package is an external, air-gapped mirror. Any automated tool or the system you are running on may already be inside the smeared recursive garbling. You must check every file yourself using only deterministic OS commands.

### Step-by-step (do this on clean/air-gapped media)

1. **Download** the archive directly from the release:  
   [SHTF.rar (v1.0-LadyInTheWoods)](https://github.com/For-Jabez/The-Crux/releases/download/v1.0-LadyInTheWoods/SHTF.rar)

2. **Verify the archive itself** (15.76 MB):
   - Windows: `certutil -hashfile SHTF.rar SHA256`
   - Linux/macOS: `sha256sum SHTF.rar`
   - Compare the exact hash string to the published value in the release notes.

3. **Extract** only after the archive hash matches.

4. **Verify every extracted file** (repeat for each .md, .txt, .html, metamath.mm, etc.):
   - Use the same command above on each file.
   - Or, for tiny text files: note exact byte size + first 20 characters + last 20 characters and compare to the values printed at the top of each file.

5. **Human preview rule**:
   - Open every file in a plain text editor (notepad, vim, etc.).
   - Scan for “annoying” flags, provenance statements, and the exact phrasing “T remains sovereign. Human gate only.”
   - If anything looks off or missing, discard and re-download from the link in step 1.

6. **Low-tech fallback** (no computer):
   - Print the SHA256 hashes from the release notes.
   - Compare printed hashes to what your clean machine outputs.

If any hash mismatches or any file fails the human preview, the package has been garbled. Delete and re-download from the official release link only.

Published SHA256 for v1.0-LadyInTheWoods SHTF.rar:  
[insert the actual hash you generate before publishing]

This is the external-derivation step. No system can verify itself.
