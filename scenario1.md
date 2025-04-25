# Scenario 1 - Block Remote Desktop on the Public Network Using Windows Firewall (Inbound Rules)

The Remote Desktop feature in Windows allows you to connect to and control a computer from a remote location. This can be particularly useful for accessing your work computer from home, assisting others with technical issues, or managing servers.

Blocking Remote Desktop on a public network using Windows Firewall can help enhance the security of your system by preventing unauthorized access. Here’s how you can configure Windows Firewall to block Remote Desktop (RDP) on public networks.

## Steps

1. Open the Windows Defender Firewall with Advanced Security options

Here you will see an Overview in the center panel. Make special note of the rule types listed on the left panel:
- Inbound rules: Inbound rules determine what traffic is allowed to the computer.
- Outbound rules: Outbound rules determine what traffic is allowed to leave the computer.
- Connection security rules: Connection security rules define how and when computers should use IPsec (Internet Protocol Security) to secure traffic.
- Monitoring: Monitoring involves tracking and analyzing the traffic that is allowed or blocked by the firewall.
Each of these rules can be configured to filter traffic based on computers, users, applications, ports, protocols, and so on.

![image](https://github.com/user-attachments/assets/b93cc6e5-774d-4425-8fbd-24578ea638a1)

2. Disable Remote Desktop on the Public Network
3. Create a New Inbound Rule
4. In the left pane, click on Inbound Rules.
5. Here you will see a long list of inbound rules. Note that some of the rules have a green checkmark next to them. This indicates that the rule is enabled to allow inbound communication. The rules without a checkmark are available for use but are not enabled.

![image](https://github.com/user-attachments/assets/bf91546f-9474-4742-a78a-5647b72b3af5)

6. In the right pane, click on New Rule….
7. Select Rule Type- Select Port and click Next.

![image](https://github.com/user-attachments/assets/3ec0cb3e-b2ad-4e05-be30-fa9eaf8e1dbd)

8. Specify Port
9. Select TCP.
10. In Specific local ports, enter 3389 (the default port for Remote Desktop).
11. Click Next.

![image](https://github.com/user-attachments/assets/12fce46e-7860-41e9-89d1-59fdbadc0b7d)

12. Specify Action
13. Select Block the connection.
14. Click Next.

![image](https://github.com/user-attachments/assets/5a78f4a1-eeae-4af4-a7d7-943b0264e933)

15. Select Profile
16. Select only Public.
17. Deselect Domain and Private.
18. Click Next.

![image](https://github.com/user-attachments/assets/79399e09-2764-425b-b55f-814bd8c347d2)

19. Name the Rule
20. Enter a name for the rule, such as 'Block Remote Desktop on Public Network'.
21. Optionally, provide a description.
22. Click Finish.

![image](https://github.com/user-attachments/assets/e1a7a684-d141-4e0c-b51b-8e8179b80ac8)

23. Verify the rule listed under Inbound Rules
24. Click Inbound Rules and verify the new rule Enabled. A red circle typically indicates that a rule is blocking traffic.
