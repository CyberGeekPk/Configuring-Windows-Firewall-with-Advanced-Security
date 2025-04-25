# Scenario 2 - Block Outbound Traffic for Specified Applications (Outbound Rules)

Creating outbound rules to restrict applications from sending data over the internet can help enhance your system’s security and control network traffic. Here are the steps to create such rules using Windows Defender Firewall with Advanced Security.

1. Open the Windows Defender Firewall with Advanced Security options
2. Follow steps in Scenario 1 to open the Advanced Security option window.
3. Select Outbound Rules and create a new Rule
4. In the left pane, click on Outbound Rules.

![image](https://github.com/user-attachments/assets/7f4d895a-7391-407b-9220-7b8d586b54c4)


5. In the right pane, click on New Rule….
6. Choose Rule Type.
7. Select Program and click Next.

![image](https://github.com/user-attachments/assets/c1d467cc-a382-4c81-9e3d-1fbb630a1a8d)


8. Specify Program Path
9. Select This program path: and browse to the executable file of the application you want to block.
10. For example, to block Google Chrome, you might navigate to C:\Program Files (x86)\Google\Chrome\Application\chrome.exe and click Open.

![image](https://github.com/user-attachments/assets/3aa3f1ed-922e-474c-85d8-e9ca40487d23)


11. Click Next.
12. Select Action.
13. Select Block the connection and click Next.

![image](https://github.com/user-attachments/assets/3d4ae8fe-f027-450a-8161-db27836afde1)


14. Specify Profile.
15. Choose when the rule applies: Domain, Private, and Public.
16. Check all profiles if you want the rule to apply in all scenarios.
17. Click Next.

![image](https://github.com/user-attachments/assets/80be02df-beba-40c3-9515-2f793beacb53)


18. Name the Rule.
19. Give the rule a name (e.g., “Block Chrome Internet Access”) and an optional description.
20. Click Finish.

![image](https://github.com/user-attachments/assets/20ad8ba3-e9de-404c-b3ac-c743ba8db7ae)


21. Verify the Rule.

![image](https://github.com/user-attachments/assets/c761d5f0-6f20-4dff-92bb-3c7487aa9cec)


22. Open Chrome browser and try to browse internet. - You will not be able to access internet through the browser. This confirms that Rule is working.
23. If you go back to Outbound Rules setting and disable the Rule “Block Chrome Internet Access”, you will be able to browser internet on Chrome browser again.

