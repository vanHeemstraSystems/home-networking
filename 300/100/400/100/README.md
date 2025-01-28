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

## 200 - Local Access to Ubiquiti Dream Machine (UDM) Pro

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

## 300 - Cloud Access to Ubiquiti Dream Machine (UDM) Pro

Visit in a web browser at the address: https://unifi.ui.com

![Image](https://github.com/user-attachments/assets/b7b34eb7-4131-40a7-8c42-b0a6c149ebc8)

https://unifi.ui.com