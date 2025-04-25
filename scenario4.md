# Scenario 4 (Inbound Rules) - Allow Key Management Service on Domain and Private Network, and Deny Connection on Public Network

A KMS is used to activate Microsoft products (such as Windows and Office) within an organization without requiring each machine to connect directly to Microsoft for activation.

1. Open the Windows Defender Firewall with Advanced Security options
2. Follow steps in Scenario 1 to open the Advanced Security option window.
3. Scroll to the Key Management Service inbound rule in the Overview panel of Windows Defender Firewall with Advanced Security. Note the following:
- The policy is currently not enabled (the Enabled column says No.)
- If enabled, the rule would allow communication (the Action column says Allow.) Double-click this rule.

![image](https://github.com/user-attachments/assets/5383644b-a6f6-413a-a2b6-476ef4695ee8)

Here you will see the details of this rule. You will note that the General tab includes the name of the rule, a description of the rule, and whether the rule has been allowed or blocked. 

4. In this case, the connection is allowed. Click the Advanced tab.
5. Here you will see which profiles the rule applies to. In this case, Domain, Private and Public are all selected.

![image](https://github.com/user-attachments/assets/28175be9-a05d-4044-a377-b167687abd07)

6. Because we want to allow communication only with the domain and private networks, For Public this box should not have a checkmark. Next, click Apply, then click Ok.
7. Now we will create an inbound rule that blocks communication with the public network. Since the new rule will be similar to the last, we will copy the existing rule. Right-click the Key Management Service (TCP-In) inbound rule and click Copy. Press Ctrl+V to paste.

![image](https://github.com/user-attachments/assets/f2502e40-85c3-45ab-8d2d-5d5b3df625a8)


8. You will now see a second Key Management Service (TCP-In) inbound rule. Double-click the second rule to open the **Key Management Service *TCP-IN) Properties.
9. Since we want to block connection with the public network, select Block the connection on the General tab. Click Apply.

![image](https://github.com/user-attachments/assets/fdcdce3b-4279-42ed-9c42-bc2329121d07)


10. Click the Advanced tab.
11. Click the Domain and Private boxes to remove the checkmarks. Click the Public to add the checkmark. Click Ok.

![image](https://github.com/user-attachments/assets/e852ba31-5aa1-4227-991d-e5682539df8d)


12. The Overview panel will show your changes. Right-click each Key Management Service (TCP-In) rule and click Enable rule.
13. Now you will see that a green checkmark appears next to the first rule indicating that the rule allowing communication is enabled. A circle with a line through it appears next to the second rule indicating that the rule blocking communication is enabled.

![image](https://github.com/user-attachments/assets/a7b751fd-64e8-4932-9a14-d0851f032836)



