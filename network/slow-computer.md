# 💻 Slow Computer / System Optimization

**Objective:** To identify resource bottlenecks and optimize system performance through hardware and software management.
## 🔍 Symptoms
- Programs take long to open
- System freezes or lags
- High CPU or disk usage

###  Common Causes
| Potential Cause | Description |
| :--- | :--- |
| **Resource Hogging** | Background apps (like Chrome or Antivirus) consuming 90%+ CPU/RAM. |
| **Disk Fragmentation** | Hard drive is struggling to find file fragments (mostly for older HDDs). |
| **System Corruption** | Windows system files have become unstable due to an improper shutdown. |

## Troubleshootiing steps

## 📊 Step 1: Analyze Resource Usage
Identify if the slowdown is caused by CPU, Memory (RAM), or Disk I/O.
- **Windows:** Press `Ctrl + Shift + Esc` to open **Task Manager**. Click the **Performance** tab.
- **Linux:** Run `htop` or `top` in the terminal to view real-line process consumption.
- **Observation:** If Disk usage is constantly at 100%, consider a hardware health check or SSD upgrade.

## 🚀 Step 2: Manage Startup Programs
Too many background applications can significantly increase boot time and drain RAM.
- **Action:** In Task Manager, go to the **Startup** tab.
- **Process:** Right-click and **Disable** any non-essential apps (e.g., messaging apps, cloud sync, or high-impact update checkers).

## 🧹 Step 3: Clean Temporary Files & Disk
Low disk space (specifically on the C: drive) can prevent the OS from creating necessary swap files.
- **Action:** Open **Run** (`Win + R`), type `cleanmgr`, and select the drive.
- **Pro Tip:** Also clear user temp files by running `%temp%` and deleting files older than 24 hours.

## 🛡️ Step 4: Scan for Malware & Bloatware
Malicious background processes often mimic system services to hide resource theft.
- **Action:** Run a full scan using **Windows Security** or a trusted third-party tool.
- **Action:** Use **Add or Remove Programs** to uninstall "bloatware" or software that is no longer in use.

## ⚙️ Step 5: Verify System Integrity
Ensure the OS files themselves aren't corrupted.
- **Action:** Open Command Prompt as Administrator and run:
  `sfc /scannow`
- **Goal:** This repairs corrupted system files that may be causing "hangs" or freezes.

## ✅ Resolution
- Improved system performance
- Reduced resource usage

## 🚨 When to Escalate
- Disk usage stays at 100% continuously
- Suspected hardware failure (HDD/SSD)
- Malware cannot be removed
- System still slow after all steps
