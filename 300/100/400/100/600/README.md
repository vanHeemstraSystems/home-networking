# 600 - Remote Access to Mac Mini

## Using UniFi VPN

UniFi VPN (L2TP) is the recommended solution for remote access to our Mac Mini. Here's why:

1. Built directly into UniFi network equipment
2. Works with any device (not just mobile)
3. Provides secure, encrypted connection
4. Allows full network access, including all Mac Mini services

### Setup Requirements

- UniFi Dream Machine Pro (UDM Pro)
- Latest UniFi OS version
- Dynamic DNS configured (if you don't have a static IP)
- Port 1701 (L2TP) and 4500 (IPSec) open on your ISP connection

### UDM Pro Configuration Steps

1. In UniFi OS Dashboard:
   - Log into your UDM Pro interface (https://local-ip:8443)
   - Go to Settings > System > Advanced
   - Enable Remote Access VPN Server
   - Select L2TP Server

2. VPN Server Configuration:
   - Set a strong Pre-shared Key (PSK)
   - Configure VPN subnet (default is usually fine)
   - Set maximum number of clients
   - Enable DNS forwarding if needed

3. User Management:
   - Go to Settings > Users
   - Create new VPN users or enable VPN access for existing users
   - Set strong passwords for each user

### Client Connection Steps

1. On macOS:
   - System Settings > VPN > Add VPN Configuration
   - Select L2TP over IPSec
   - Server Address: Your UDM Pro's public IP or DDNS
   - Account Name: VPN username
   - Enter shared secret (PSK)

2. On iOS:
   - Settings > VPN > Add VPN Configuration
   - Type: L2TP
   - Fill in server, account, and PSK details

Once connected via VPN, you can access your Mac Mini using:
- Screen Sharing (port 5900)
- SSH (port 22)
- File Sharing (port 445)
- Any other enabled services

MORE ...