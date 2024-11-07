# Devil4NessusReport

> **A PowerShell script to streamline and merge Nessus vulnerability scan reports, providing consolidated results for easier analysis.**

---

## Overview

`Devil4NessusReport.ps1` is a PowerShell script designed to assist security professionals in managing Nessus vulnerability scan data. It merges multiple Nessus files into a single report, enabling easier and more efficient review of vulnerabilities across systems.

## Features

- **Merge Multiple Nessus Files**: Consolidates multiple `.nessus` files into one comprehensive report.
- **Simplified Analysis**: Combines vulnerabilities into a single file, making it easier to review and act on.
- **Customizable Output**: Offers flexibility in how the final report displays key data, tailored to the user's needs.

---

## Requirements

- **PowerShell** (version 5.0 or higher)
- **Nessus Files**: Export `.nessus` files from the Nessus scanning tool before using this script.

---

## Installation & Usage

1. **Download the Repository**  
   Clone this repository or download the ZIP file:
   ```bash
    https://github.com/Anand7758/Devil4NessusReport.git
> ### Setting Up Execution Policy
> To allow the script to run, open PowerShell as an administrator and set the execution policy:
> 
> ```powershell
> Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser
> ```
> 
> This command permits the script to run without restrictions for the current user.

> ### Usage Instructions
> Open PowerShell and navigate to the directory containing the `Devil4NessusReport.ps1` script.
> 
> Run the following command, replacing the example paths with your own:
> 
> ```powershell
> .\Devil4NessusReport.ps1 -InputPath "Path\to\your\nessus\files" -OutputPath "Path\to\save\merged\report"
> ```
> 
> - **`-InputPath`**: The folder containing the `.nessus` files you want to merge.
> - **`-OutputPath`**: The destination path and filename where the merged report will be saved.

> ### Example Command
> To merge all `.nessus` files in `C:\Scans\NessusFiles` and save the output as `MergedReport.nessus` in `C:\Reports`, use:
> 
> ```powershell
> .\Devil4NessusReport.ps1 -InputPath "C:\Scans\NessusFiles" -OutputPath "C:\Reports\MergedReport.nessus"
> ```

## Viewing the Merged Report
Once the script completes, navigate to the specified `OutputPath` to find and review the merged `.nessus` report file.

## Troubleshooting
If you encounter issues running the script, ensure:
- The PowerShell execution policy is set correctly.
- The `InputPath` contains `.nessus` files.
- You have permissions to read from the `InputPath` and write to the `OutputPath`.

---
