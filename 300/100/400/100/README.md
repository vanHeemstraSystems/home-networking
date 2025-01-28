# 100 - Ubiquiti UniFi Site Management

**Note**: It is recommended to connect the device you are working from (here: **Willems-Mini**) to have it connected to the WiFi Access Point that is closest to the Internet (here: **Ziggo9306631**).

## 100 - Moving UniFi Express from Client to Network Device

### Current Status
- UniFi Express appears under Client Devices
- IP Address: 192.168.1.240
- MAC Address: 94:2a:6f:0e:b0:c3

### Steps to Adopt as Network Device
1. In the cloud interface (https://unifi.ui.com):
   - Find the UniFi Express in Client Devices
   - Note down or copy its MAC address: 94:2a:6f:0e:b0:c3

2. Reset UniFi Express to Factory Settings:
   - Locate the reset button on the UniFi Express
   - Press and hold for about 10 seconds until LED changes
   - Release button
   - Wait for device to restart (LED will indicate status)

3. After Reset:
   - The device should enter adoption mode
   - LED should turn solid white
   - It should disappear from Client Devices
   - It should appear under Devices or in the adoption queue

4. Complete Adoption:
   - Click "Adopt" when it appears
   - Wait for the adoption process to complete
   - Device will download firmware and configure itself
   - Should then appear under Devices as a proper UniFi network device

### Note
- During this process, any existing WiFi networks from the UniFi Express will temporarily go offline
- After adoption, you can reconfigure WiFi networks through the UDM Pro interface

## 200 - UniFi Express Configuration After Successful Adoption

### Current Status ✅
- UniFi Express successfully adopted
- Listed under Devices (not Client Devices)
- Shows green status light
- Properly integrated with UDM Pro

### Next Steps
1. Configure WiFi Networks:
   - Navigate to the UniFi Express in Devices
   - Set up or extend existing WiFi networks
   - Configure SSID (network name)
   - Set security settings and passwords

2. Optimize Placement:
   - Consider optimal location for WiFi coverage
   - Use UniFi's signal strength indicators
   - Ensure good connection back to UDM Pro

3. Monitor Performance:
   - Check client connections
   - Monitor bandwidth usage
   - Review any alerts or notifications

4. Backup Configuration:
   - Consider backing up your UDM Pro settings
   - This saves your network configuration including the UniFi Express setup

Would you like me to help you with any of these next steps, particularly setting up the WiFi networks through your newly adopted UniFi Express?

## 300 - Configuring WiFi on UniFi Express

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

## 400 - Local Access to Ubiquiti Dream Machine (UDM) Pro

Visit on a computer connected to the same (WiFi) network as the Ubiquiti Dream Machine (UDM) Pro in a web browser at the address: https://192.168.1.1

![Image](https://github.com/user-attachments/assets/3bdc4164-9ac2-4983-ab8f-36c8b6c2c919)

https://192.168.1.1

**Note**: If warned in the browser that the site cannot be trusted because there is no certificate signed by a trusted authority, choose "Advanced" and choose nevertheless to visit the page, as we are local to the machine and we know of its validity.

This brings us to the **UniFi Network**:

![Image](https://github.com/user-attachments/assets/6eb8f25d-0149-491b-bfa3-196b9dd77941)

When clicked on **Topology** we see all devices connected to the UniFi Network:

![Image](https://github.com/user-attachments/assets/952d51fe-89a7-4afc-b83c-f9bc702ea50e)


As you can see from the blueish circle around **Willems-Mini**, this is the device we are currently browsing from.

MORE ...

## 500 - Cloud Access to Ubiquiti Dream Machine (UDM) Pro

Visit in a web browser at the address: https://unifi.ui.com

![Image](https://github.com/user-attachments/assets/b7b34eb7-4131-40a7-8c42-b0a6c149ebc8)

https://unifi.ui.com