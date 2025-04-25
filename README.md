# Configuring Windows Firewall with Advanced Security
This project explores securing a Windows operating system using Windows Defender Firewall and its advanced settings. It involves configuring inbound and outbound rules to control network traffic and applying them to real-world scenarios such as blocking Remote Desktop on public networks and restricting outbound access for specific applications. The project demonstrates practical skills in system security, firewall management, and network protection strategies.

## Objective

In this mini project, I developed a comprehensive understanding of how to secure a Windows operating system using the real-time protection provided by Windows Firewall.
I reviewed following settings to enable firewall:

- 1: Configure Firewall Rules Using Windows Defender Firewall
- 2: Configure Firewall Rules Using Windows Defender Firewall with Advanced Security

## Scenarios

Further in this project, I explored few typical use cases that can be controlled by Windows Firewall service:

- Scenario 1: Block Remote Desktop on the Public Network (Inbound Rules)
- Scenario 2: Block Outbound Traffic for Specified Applications (Outbound Rules)
- Scenario 3: Block Web Server (HTTP) Traffic on a Public Network (Inbound Rules)
- Scenario 4: Allow Key Management Service on the Domain and Private network, and deny the connection on the Public network (Inbound Rules)

## Skills Learned

### Windows OS Security Configuration
Gained practical knowledge of securing Windows systems using built-in firewall features.

### Firewall Rule Management
Learned how to create, modify, and enforce inbound and outbound rules using both basic and advanced Windows Defender Firewall settings.

### Network Traffic Control
Understood how to allow or block traffic based on protocols, ports, application paths, and network profiles (Public, Private, Domain).

### Scenario-Based Problem Solving
Applied firewall configurations to real-world scenarios like:
- Blocking Remote Desktop access on public networks
- Restricting application-level outbound traffic
- Controlling HTTP traffic exposure
- Allowing selective access based on network types

### System Administration Basics
Developed foundational skills in managing Windows security settings and interpreting system behavior in response to rule changes.

### Security Best Practices Awareness
Improved understanding of least privilege, secure defaults, and network segmentation principles.

## Tools Used

- Windows Defender Firewall to configure and manage basic inbound and outbound rules for network protection
- Windows Defender Firewall with Advanced Security (WFAS) for rule creation and advanced network traffic filtering across different profiles (Domain, Private, Public)
- Windows 10/11 Operating System platform on which firewall settings were tested and configured.
- Remote Desktop Protocol (RDP) used in scenarios to simulate and block remote connections based on firewall configurations.

## Typical use cases with Windows Firewall Advanced Security options

In these scenarios, we will look at Windows Defender Firewall with Advanced Security. This advanced view provides in-depth options for configuration. All Windows Firewall rules, and their details, are stored here, allowing you to edit configurations for each rule or exception.

- [Scenario 1: Block Remote Desktop on the Public Network Using Windows Firewall (Inbound Rules)](scenario1.md)

### Additional Exercise : Enable Firewall on different Network Profiles

In this exercise we will review Windows Defender Firewall configuration.

1. Click the Windows Start button. and then select Windows Security.
2. Click Firewall & network protection.
3. Here you will see the firewall status for the following:
- Domain network
- Private network
- Public network
4. Click Domain network.
5. Verify that the Microsoft Defender Firewall is toggled to On.
Observe the option Incoming connections. If you need to block all incoming domain network traffic, including traffic that is typically allowed, then you only need to activate this option.
6. Select the back arrow button to return to the Firewall and network protection window.
7. Click Private network.
8. Verify that the Microsoft Defender Firewall is toggled to On.
Select the back arrow button to return to the Firewall and network protection window.
9. Click Public network.
10. Verify that the Microsoft Defender Firewall is toggled to On.
Select the back arrow button to return to the Firewall and network protection window.
11. Click Allow an app through firewall.
12. Scroll to Google Chrome OR Mozilla Firefox. Observe in the screenshot below that the current configuration allows for Firefox to communicate on the Private network only but denies it from communicating on the Public network.
  
![image](https://github.com/user-attachments/assets/1c01b295-f65a-4624-9590-0b406f177eb7)

13. Click the Public box next to Firefox to allow Firefox to communicate through the Public network as well. A checkmark will appear. Click OK to return to the Firewall & network protection screen. Users will now be able to use Mozilla Firefox on the public network.

![image](https://github.com/user-attachments/assets/bb8dd117-7fd1-4eb0-8203-4f560f01419b)
















