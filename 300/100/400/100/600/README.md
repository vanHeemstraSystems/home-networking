# 600 - Remote Access to Mac Mini

## Using UniFi VPN

UniFi VPN (L2TP) is the recommended solution for remote access to our Mac Mini. Here's why:

1. Built directly into UniFi network equipment
2. Works with any device (not just mobile)
3. Provides secure, encrypted connection
4. Allows full network access, including all Mac Mini services

### Setup Requirements

- UniFi Security Gateway, Dream Machine, or UDM Pro
- UniFi Network application
- Port 1701 (L2TP) and 4500 (IPSec) forwarded to your UniFi gateway
- Valid RADIUS user credentials configured in UniFi

### Configuration Steps

1. In UniFi Network application:
   - Navigate to Settings > Teleport & VPN
   - Enable L2TP Server
   - Configure a strong pre-shared key
   - Add VPN users under User Management

2. On client devices:
   - Use built-in L2TP VPN client (available on macOS, iOS, Windows, Android)
   - Enter your UniFi gateway's public IP or DDNS hostname
   - Use your RADIUS credentials and pre-shared key

Once connected via VPN, you can access your Mac Mini using:
- Screen Sharing (port 5900)
- SSH (port 22)
- File Sharing (port 445)
- Any other enabled services

MORE ...