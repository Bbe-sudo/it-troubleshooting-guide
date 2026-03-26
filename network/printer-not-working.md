# 🖨️ Printer Not Working

**Objective:** To resolve document stuck in queue, hardware connectivity issues, and driver-related failures.

## 🔄 Step 1: Restart Print Spooler
Often, the software service managing the print queue hangs and needs a reset.
- **Action:** Open **Run** (`Win + R`), type `services.msc`, and press Enter.
- **Process:** Locate **Print Spooler**, right-click it, and select **Restart**.

## 🔌 Step 2: Check Physical Connectivity
Ensure the hardware is communicating with the workstation.
- **USB:** Unplug and re-seat the cable into a different port.
- **Network:** Print a "Configuration Page" from the printer menu to verify it has a valid IP address.
- **Ping Test:** Run `ping [Printer_IP]` to confirm network visibility.

## 🛠️ Step 3: Clear Print Queue
If a corrupt job is blocking the printer, it must be removed manually.
- **Path:** Navigate to `C:\Windows\System32\spool\PRINTERS`.
- **Action:** Delete all files in this folder (Note: You may need to stop the Spooler service first).

## 📥 Step 4: Reinstall Drivers
If the printer is seen but won't print, the driver may be corrupt.
- **Action:** Remove the device from **Settings > Printers & Scanners**.
- **Source:** Download the latest "Full Software Suite" from the manufacturer's official support site (e.g., HP, Canon, Epson).

##  Step 5: Perform a Test Print
- **Action:** Use the **Print Test Page** feature in the driver properties to verify the fix.
