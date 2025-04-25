# Scenario 3 (Inbound Rules) - Block Web Server (HTTP) Traffic on a Public Network

Blocking HTTP traffic to your computer when connected to a public network ensures that no web server services are exposed to potential threats.

This rule will block all incoming HTTP traffic (port 80) when your computer is connected to a public network. This helps to secure your system by preventing potential web server attacks or unauthorized access through HTTP.

## Steps

1. Open the Windows Defender Firewall with Advanced Security options
2. Follow steps in Scenario 1 to open the Advanced Security option window.
3. Disable File and Printer Sharing Rules
4. In the left pane, click on Inbound Rules.
5. In the right pane, click on New Rule
6. Choose Port and click Next.
7. Specify Ports:
8. Select TCP.
9. In Specific local ports, enter 80 (the default port for HTTP).
10. Click Next.
11. Specify Action:
12. Select Block the connection.
13. Click Next.
14. Specify Network Profile:
15. Check only the Public option.
16. Uncheck Domain and Private.
17. Click Next.
18. Name the Rule:
19. Enter a name for the rule, such as “Block HTTP on Public Network“.
20. Add a description if desired.
21. Click Finish.
