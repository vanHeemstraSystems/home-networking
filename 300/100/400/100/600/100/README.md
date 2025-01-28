# 100 -  Using Remote.it

Remote.it provides a secure, web-based remote access solution that requires no port forwarding or VPN configuration. Here's why it's recommended:

1. No client software needed - works through web browser
2. Zero-trust security model
3. No port forwarding required
4. Built-in monitoring and management
5. Free tier available for personal use

### Setup Requirements

- Mac Mini with internet connection
- Remote.it account (free tier available)
- Web browser for access

### Installation Steps

1. Create Remote.it Account:
   - Visit https://remote.it
   - Sign up for a free account
   - Verify your email

2. Configure Mac Mini:
   - System Preferences > Sharing
   - Enable "Screen Sharing"
   - Set a strong password for your Mac user account

3. Install Remote.it:
   - Download Remote.it for macOS
   - Install and run the application
   - Sign in with your Remote.it account
   - In the Remote.it dashboard, click the "+" button
   - Select your Mac's name from the list (e.g., "Willems-Mac-Mini")
   - When prompted for services:
     - ✅ Select "vnc (VNC-5900)" for screen sharing
     - ❌ Skip "kerberos-sec (TCP-88)" - not needed for remote access
   - Follow the setup wizard to complete configuration

4. Access Your Mac Mini:
   - Log into remote.it web dashboard
   - Select your Mac Mini from devices
     > If your device is not listed:
     > 1. Check if Remote.it app is running on Mac Mini
     > 2. Open Remote.it app and click the "+" button
     > 3. Select your Mac's name from the device list
     > 4. Select "Screen Sharing" service to enable
     > 5. Wait a few moments for device to appear in dashboard
   - Click "Connect" to start remote session
   - Access through web browser

### Security Recommendations

1. Enable 2FA on your Remote.it account
2. Use strong passwords
3. Regularly update Remote.it software
4. Monitor access logs in Remote.it dashboard
5. Use device sharing features for temporary access

### Advantages Over Traditional VPN

1. No port forwarding needed
2. Works through firewalls
3. Zero-trust security model
4. Centralized access management
5. Real-time monitoring

### Service Configuration Details

After successful registration, your Remote.it service will be configured with these parameters:

- **Service Type**: VNC
- **Protocol**: TCP
- **Local Host**: 127.0.0.1
- **Port**: 5900
- **Creation Date**: 28/01/2025, 14:24:28

> Note: The Service ID and Device ID are unique identifiers assigned by Remote.it. 
> Keep these IDs for troubleshooting purposes if needed.
