# 100 - Moving UniFi Express from Client to Network Device

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