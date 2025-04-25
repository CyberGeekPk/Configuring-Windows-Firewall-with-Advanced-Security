# Scenario 2 - Block Outbound Traffic for Specified Applications (Outbound Rules)

Creating outbound rules to restrict applications from sending data over the internet can help enhance your system’s security and control network traffic. Here are the steps to create such rules using Windows Defender Firewall with Advanced Security.

1. Open the Windows Defender Firewall with Advanced Security options
2. Follow steps in Scenario 1 to open the Advanced Security option window.
3. Select Outbound Rules and create a new Rule
4. In the left pane, click on Outbound Rules.
5. In the right pane, click on New Rule….
6. Choose Rule Type.
7. Select Program and click Next.
8. Specify Program Path
9. Select This program path: and browse to the executable file of the application you want to block.
10. For example, to block Google Chrome, you might navigate to C:\Program Files (x86)\Google\Chrome\Application\chrome.exe and click Open.
11. Click Next.
12. Select Action.
13. Select Block the connection and click Next.
14. Specify Profile.
15. Choose when the rule applies: Domain, Private, and Public.
16. Check all profiles if you want the rule to apply in all scenarios.
17. Click Next.
18. Name the Rule.
19. Give the rule a name (e.g., “Block Chrome Internet Access”) and an optional description.
20. Click Finish.
21. Verify the Rule.
22. Open Chrome browser and try to browse internet. - You will not be able to access internet through the browser. This confirms that Rule is working.
23. If you go back to Outbound Rules setting and disable the Rule “Block Chrome Internet Access”, you will be able to browser internet on Chrome browser again.

