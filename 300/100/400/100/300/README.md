# 300 - Configuring WiFi on UniFi Express

### Check WiFi Status
1. In UniFi interface:
   - Go to Settings > WiFi
   - Check if any WiFi networks are configured
   - Verify if they're enabled on the UniFi Express

### Create/Enable WiFi Network
1. Create New Network:
   - Go to Settings > WiFi
   - Click "Create New WiFi Network"
   - Set Network Name (SSID)
   - Configure Security:
     - Select WPA2/WPA3
     - Set a strong password
   - Under "AP Groups" or "Access Points":
     - Ensure UniFi Express is selected/enabled
   - Save and apply changes

2. If Network Exists:
   - Click existing network
   - Under "Access Points" or "Broadcasting APs"
   - Verify UniFi Express is enabled
   - Save any changes

### Verify Configuration
1. Wait 2-3 minutes for changes to apply
2. On your iPad:
   - Go to WiFi settings
   - Pull down to refresh available networks
   - Look for your configured network name
3. Check UniFi Express LED:
   - Should show steady light indicating active WiFi

### Troubleshooting
If WiFi still doesn't appear:
1. Verify UniFi Express power (solid light)
2. Check device temperature
3. Try rebooting the UniFi Express from the UniFi interface
4. Ensure radio settings are enabled in device properties