# Fixing VirtualBox Network Issue

## Problem
When using VirtualBox with a **Bridged Adapter** and connecting through a mobile hotspot, the virtual machine fails to obtain an IP address.

## Solution
1. Change network settings in VirtualBox:
   - **Attached to:** `NAT`
   - **Adapter Type:** `Intel PRO/1000 MT Desktop`
2. Restart the VM and check connectivity.
3. Switch back to **Bridged Adapter** and select `Wi-Fi` instead of `Ethernet`.
4. Run the following command inside the VM to check network configuration:
   ```bash
   ip a

