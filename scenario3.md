# Scenario 3 (Inbound Rules) - Block Web Server (HTTP) Traffic on a Public Network

Blocking HTTP traffic to your computer when connected to a public network ensures that no web server services are exposed to potential threats.

This rule will block all incoming HTTP traffic (port 80) when your computer is connected to a public network. This helps to secure your system by preventing potential web server attacks or unauthorized access through HTTP.

## Steps

1. Open the Windows Defender Firewall with Advanced Security options
2. Follow steps in Scenario 1 to open the Advanced Security option window.
3. Disable File and Printer Sharing Rules

![image](https://github.com/user-attachments/assets/614ffdc3-041c-406f-9620-b442f3bb5596)


4. In the left pane, click on Inbound Rules.
5. In the right pane, click on New Rule
6. Choose Port and click Next.
7. Specify Ports:
8. Select TCP.
9. In Specific local ports, enter 80 (the default port for HTTP).

![image](https://github.com/user-attachments/assets/1cdf8cd8-7015-4982-9a3e-bfeddfc9781b)

10. Click Next.
11. Specify Action:
12. Select Block the connection.
13. Click Next.
14. Specify Network Profile:
15. Check only the Public option.
16. Uncheck Domain and Private.

![image](https://github.com/user-attachments/assets/3e11bd99-c57d-48ad-bded-ec96f9135973)

17. Click Next.
18. Name the Rule:
19. Enter a name for the rule, such as “Block HTTP on Public Network“.

![image](https://github.com/user-attachments/assets/3b85e5b1-7c94-4263-b0cb-842ad58e01ce)


20. Add a description if desired.
21. Click Finish.
