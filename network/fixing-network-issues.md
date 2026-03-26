# 🌐 Fixing Network Issues

**Objective:** To diagnose and resolve local connectivity and internet access problems.

### Common Causes

| Potential Cause | Description |
| :--- | :--- |
| **DHCP Failure** | Device isn't receiving an IP address from the router. |
| **DNS Issues** | Local network is fine, but the browser can't "find" website names. |
| **Hardware Link** | Damaged Ethernet cable or a disabled Wi-Fi adapter. |

## 🔍 Step 1: Check IP Configuration
Verify the device has a valid IP address.
- **Windows:** `ipconfig`
- **Linux/macOS:** `ifconfig` or `ip a`
  
## 📡 Step 2: Ping Gateway
Test communication with the local router.
- Command: `ping 192.168.1.1` *(Note: Use the Gateway IP from Step 1)*

## 🌎 Step 3: Test Internet Access
Check if the issue is local or external.
- Command: `ping google.com`

## 🧹 Step 4: Flush DNS
Clear the resolver cache to fix domain name issues.
- **Windows:** `ipconfig /flushdns`

## ✅ Step 5: Restart Network Adapter
A hard reset of the local hardware.
1. Go to **Network Settings**.
2. Select **Disable** on the active adapter.
3. Wait 5 seconds and select **Enable**.

