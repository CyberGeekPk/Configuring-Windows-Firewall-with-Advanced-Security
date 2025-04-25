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

The first exercise is based in the consumer-friendly version of Windows Defender Firewall – a simplified interface ideal for a single device in a home setting. In this exercise, we will look at Windows Defender Firewall with Advanced Security. This advanced view provides more in-depth options for configuration. All Windows Firewall rules, and their details, are stored here, allowing you to edit configurations for each rule or exception.

### Scenario 1 - Block Remote Desktop on the Public Network Using Windows Firewall (Inbound Rules)

The Remote Desktop feature in Windows allows you to connect to and control a computer from a remote location. This can be particularly useful for accessing your work computer from home, assisting others with technical issues, or managing servers.

Blocking Remote Desktop on a public network using Windows Firewall can help enhance the security of your system by preventing unauthorized access. Here’s how you can configure Windows Firewall to block Remote Desktop (RDP) on public networks.

### Steps

1. Open the Windows Defender Firewall with Advanced Security options

Here you will see an Overview in the center panel. Make special note of the rule types listed on the left panel:
- Inbound rules: Inbound rules determine what traffic is allowed to the computer.
- Outbound rules: Outbound rules determine what traffic is allowed to leave the computer.
- Connection security rules: Connection security rules define how and when computers should use IPsec (Internet Protocol Security) to secure traffic.
- Monitoring: Monitoring involves tracking and analyzing the traffic that is allowed or blocked by the firewall.
Each of these rules can be configured to filter traffic based on computers, users, applications, ports, protocols, and so on.

![image](https://github.com/user-attachments/assets/b93cc6e5-774d-4425-8fbd-24578ea638a1)

2. Disable Remote Desktop on the Public Network
Create a New Inbound Rule
In the left pane, click on Inbound Rules.
Here you will see a long list of inbound rules. Note that some of the rules have a green checkmark next to them. This indicates that the rule is enabled to allow inbound communication. The rules without a checkmark are available for use but are not enabled.

![image](https://github.com/user-attachments/assets/bf91546f-9474-4742-a78a-5647b72b3af5)

3. In the right pane, click on New Rule….
4. Select Rule Type- Select Port and click Next.

![image](https://github.com/user-attachments/assets/3ec0cb3e-b2ad-4e05-be30-fa9eaf8e1dbd)

5. Specify Port
Select TCP.
In Specific local ports, enter 3389 (the default port for Remote Desktop).
Click Next.

![image](https://github.com/user-attachments/assets/12fce46e-7860-41e9-89d1-59fdbadc0b7d)

6. Specify Action
Select Block the connection.
Click Next.

![image](https://github.com/user-attachments/assets/5a78f4a1-eeae-4af4-a7d7-943b0264e933)

7. Select Profile
Select only Public.
Deselect Domain and Private.
Click Next.

![image](https://github.com/user-attachments/assets/79399e09-2764-425b-b55f-814bd8c347d2)

8. Name the Rule
Enter a name for the rule, such as 'Block Remote Desktop on Public Network'.
Optionally, provide a description.
Click Finish.

![image](https://github.com/user-attachments/assets/e1a7a684-d141-4e0c-b51b-8e8179b80ac8)

9. Verify the rule listed under Inbound Rules
Click Inbound Rules and verify the new rule Enabled. A red circle typically indicates that a rule is blocking traffic.

### Extra Exercise : Enable Firewall on different Network Profiles

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
















