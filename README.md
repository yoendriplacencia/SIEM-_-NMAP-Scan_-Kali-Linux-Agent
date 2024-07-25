# SIEM_NMAP-Scan_Kali-Linux-Agent
" SIEM using the Elastic Web portal and a Kali Linux VM "

One of the most commonly used commands by hackers is [Nmap], with the goal of mapping the network and finding vulnerabilities. For this reason, I developed a SIEM that can receive and monitor alerts from an agent installed on a Kali Linux VM whenever someone tries to use this tool.

## 1- Set up an Elastic Account
   
   Sign up for a free trial to use Elastic Cloud at 
   
   https://cloud.elastic.co/registration

## 2- Setting up the Agent to Collect Logs


![Screenshot 2024-07-25 100426](https://github.com/user-attachments/assets/4ec452a6-5829-40ef-b28b-b1de3f0bbb91)


![Screenshot 2024-07-25 100219](https://github.com/user-attachments/assets/0a9c8388-527c-4bf1-8b1e-b8e454b5f3e1)


  ## 3- We need to install the agent into the Kali terminal
  
![Agent code 2024-07-25 095123](https://github.com/user-attachments/assets/1ff14605-9e38-4fc4-bf22-e4cf7cb7b7bf)

 ## 4- Verifying that the agent has been insatalled correctly

![verify 2024-07-25 101059](https://github.com/user-attachments/assets/1ae7192f-819c-4e3e-9ab1-de06acf7dfb7)

 ## 5-  Generating Security Events on the Kali VM

   Run a scan on Kali machine by running the command: sudo nmap <vm-ip>. You can also run a scan of your host machine if you place your Kali VM on a “bridged” network

![nmap 2024-07-25 102928](https://github.com/user-attachments/assets/7916caa5-4bb8-459c-869e-2d9ac6f18c1a)

![nmap2 2024-07-25 103113](https://github.com/user-attachments/assets/bb984b26-52b8-4727-9912-d840c250b454)

 ## 6- Querying for Security Events in the Elastic SIEM

![query](https://github.com/user-attachments/assets/4927cc2b-3c25-41a0-ae52-e8e9a44bdc0f)

## 7- Create a Dashboard to Visualize the Events

![board](https://github.com/user-attachments/assets/74046f98-ee45-41d0-88c5-25648895634e)

## 8- Create an Alert

![rule](https://github.com/user-attachments/assets/7579b638-abc4-46bb-969d-4e6f8f0519d9)

## 9- Testing 
Below we can see how the three [Nmap] attempts are reflected on our SIEM board.

![Screenshot 2024-07-23 005215](https://github.com/user-attachments/assets/2eaeff18-076c-44b7-a52d-ca5137aa1bca)



These screenshots were taken in subsequent tests.


![Screenshot 2024-07-23 005351](https://github.com/user-attachments/assets/863ae88b-fc21-4430-9d45-28ee34c7dcb0)

![Screenshot 2024-07-23 105028](https://github.com/user-attachments/assets/5d7a848b-13a4-4d18-bcc3-a0df03527458)

![Screenshot 2024-07-23 105200](https://github.com/user-attachments/assets/97fbc100-0cf3-4064-be49-233ea6188f17)



