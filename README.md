# Nessus Vulnerability Scanner Prerequisites
- Install Windows VM
- Go to Windows update settings > advanced options > pause for the longest date available 
  
  ![image](https://github.com/ali0999109/Nessus/assets/145396907/6ff4896e-33bf-48a9-a895-6332ec017925)
  ---
  ![image](https://github.com/ali0999109/Nessus/assets/145396907/33d1aa5f-aaf2-4b02-94bb-4ee248681743)
  ---------------
- Go to windows updates, view update history, uninstall updates
  
  ![image](https://github.com/ali0999109/Nessus/assets/145396907/f9950294-7537-4732-a205-4324026b37ee)
  ---
- Go to windows defender firewall, advanced settings, windows defender firewall properties, change the firewall state to off for all the profiles
  
  ![image](https://github.com/ali0999109/Nessus/assets/145396907/fc967a6b-876a-4f1e-86e6-4b201f0150b7)
  ---
  ![image](https://github.com/ali0999109/Nessus/assets/145396907/f7d0e517-06da-438c-87d2-d5ccf309150e)
  ---
- click on devices, network, network settings, host only adapter
- type ipconfig and ping your ip address you should get a response back 
  ![image](https://github.com/ali0999109/Nessus/assets/145396907/7158655d-acc6-42ca-8ec5-97dc4c0e759f)
  ---


# Installing Nessus
- Installation link https://www.tenable.com/products/nessus/nessus-essentials?action=register
- once on this screen select continue, register for nessus essentials, Skip, and put in your registration code
- ![image](https://github.com/ali0999109/Nessus/assets/145396907/8bc07147-0709-4c2c-863c-8267ac22c939)
  ----------------------------


  
# Configuring Nessus for Scanning 
- Click basic network scan, put in VM's IP address, click save, and run
- You will get a list of vulnerabilities, click on each vulnerability for more details and a solution 

  ![image](https://github.com/ali0999109/Nessus/assets/145396907/96c25c9e-d362-4780-85b6-b6e42853ef73)
  ---
  ![image](https://github.com/ali0999109/Nessus/assets/145396907/f3e651c1-b050-4870-91aa-5d1751af10ea)

# Nessus credential scan
- click on the scan you just made and click configure on the top right. Move to the credential section > Windows > password > put in VMS username and password > VMS domain > You can find the info by typing whoami in CMD
- Go to windows VM > search for services > remote registery > startup type automatic
- User account control settings > put the bar all the way down
- Registery editor > HKEY_LOCAL_MACHINE > software > microsoft > windows > current version > policies > system > right click in the blank space > New DWORD 32 bit value > type in 
 EXACTLY LocalAccountTokenFilterPolicy > Click on it to edit properties and change value data to 1 > restart
- Now start the scan! You will see a lot more critical issues
- if you want to learn more about a CVE copy and paste it into your browswer 

![image](https://github.com/ali0999109/Nessus/assets/145396907/8044da12-ecea-4ba6-b9cc-05a969bda3b7)
----------------------------------------------------------------------------------------------------
![image](https://github.com/ali0999109/Nessus/assets/145396907/90b364a0-5633-4e0d-9992-3d8d3d7a3b99)
---
# Installtion of vulnerable software
-

=




  

 











