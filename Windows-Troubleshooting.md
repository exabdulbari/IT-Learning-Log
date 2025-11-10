## ** Windows-Troubleshooting.md**
# Windows Troubleshooting

Common errors and steps to fix them.

## 1. Blue Screen of Death (BSOD)
#Often RAM or PSU issue
- Causes: Driver issues, hardware failure, corrupted files.
- Fix:
  1. Note the error code (e.g., `IRQL_NOT_LESS_OR_EQUAL`).
  2. Update drivers via Device Manager.
  3. Run system file check:
     ```powershell
     sfc /scannow
     ```
  4. Check hardware (RAM, HDD/SSD).

## 2. Network Issues
- Steps to fix:
  1. Restart router and PC.
  2. Check cables.
  3. Renew IP:
     ```powershell
     ipconfig /release
     ipconfig /renew
     ```
  4. Flush DNS:
     ```powershell
     ipconfig /flushdns
     ```

## 3. Software Installation Problems
- Ensure correct version (32-bit vs 64-bit).
- Run installer as Administrator.
- Temporarily disable antivirus/firewall if blocking installation.
