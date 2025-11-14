
# **Adolescent Brain Cognitive Development (ABCD) Study**

The **Adolescent Brain Cognitive Development (ABCD) Study** is the largest long-term investigation of brain development and child health in the United States.  
Across **21 research sites**, the study enrolled **11,880 children (ages 9–10)** and follows them into adulthood, combining MRI, behavioral assessments, environmental surveys, and biospecimen-based measures.

This repository distributes **derived diffusion MRI FIB files** for **ABCD Sites 01–22**, prepared using standardized pipelines for tractography and connectome analyses.  
Raw ABCD data must be obtained through NDA under its Data Use Agreement.

---

## **License**

Derived FIB files are shared under the **CC BY-SA 4.0** license.  
If using these derivatives, please acknowledge:

> “This work used XSEDE/ACCESS computing resources: TG-CIS200026 & MED230052.”

---

# **Download Commands (Linux/macOS and Windows)**

Below are commands for all **ABCD Site 01 → Site 22** releases.

Release tags follow the format:

```

abcd-site01
abcd-site02
...
abcd-site22

````

---

# **Linux / macOS — bash**

Each command downloads one ABCD site using GitHub’s API + jq + curl:

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site01 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
````

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site02 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site03 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site04 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site05 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site06 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site07 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site08 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site09 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site10 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site11 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site12 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site13 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site14 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site15 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site16 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site17 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site18 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site19 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site20 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site21 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

```bash
curl -s https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site22 | jq -r '.assets[].browser_download_url' | xargs -n1 -P4 curl -LO
```

---

# **Windows PowerShell 5.x**

Each one-line PowerShell command downloads a specific ABCD site.

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site01").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site02").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site03").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site04").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site05").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site06").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site07").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site08").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site09").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site10").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site11").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site12").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site13").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site14").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site15").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site16").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site17").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site18").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site19").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site20").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site21").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```

```powershell
(Invoke-RestMethod "https://api.github.com/repos/data-nih/abcd/releases/tags/abcd-site22").assets | ForEach-Object { Invoke-WebRequest $_.browser_download_url -OutFile (Split-Path $_.browser_download_url -Leaf) }
```
