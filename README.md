# NETWORKWALKS---WEEK-3---PASSWORD-CRACKING
PASSWORD CRACKING 
## LIABILITY DISCLAIMER
 This research was conducted exclusively using my personal computers and devices for educational and research purposes, with proper authorization. I do not authorize anyone to use the information provided here for any unlawful or malicious activities. The instructor, authors, and Networkwalks shall not be held responsible for any misuse of this information. Anyone who chooses to use it for unauthorized or illegal purposes will be solely responsible for their actions and any resulting consequences. Unauthorized access to computer systems is illegal in most countries, even when no damage is caused. Such activities may result in permanent criminal records, substantial fines, termination of employment, and criminal prosecution.
## INTRODUCTION

During Week 3 of my ongoing internship program at Networkwalks, I carried out practical exercises on password cracking using Kali Linux tools to recover passwords for encrypted documents provided by Networkwalks. I also explored Claude AI as an alternative approach to assist with the password recovery process.

These exercises helped me understand how attackers may attempt to obtain passwords for password-protected documents and gain unauthorized access to sensitive personal information. They also provided practical insight into the techniques and processes involved in password cracking.

All commands were executed on a Windows computer running Kali Linux. This report documents each step of the exercises, including the exact commands used, the results obtained, relevant screenshots, and brief explanations of the significance of each discovery from an attacker's perspective.
## TOOLS Used
| TOOLS | PURPOSE |
| :--- | :--- |
| Kali Linux and Windows | Operating systems utilized in password cracking operations. |
| John The Ripper | Used for cracking the hashes and reveal the password |
| Hash extractor | To extract the hashes from the password protected document|
| Notepad | To record the hashes. |
| Hash calculator | Alternative way to calculate and reveal the password  |
| Hexstrike  | To install Claude AI. |
| Claude Ai | To Use John the Ripper to crack the password to reveal the password of the password protected document . |
## ACTIVITIES CARRIED OUT

### PASSWORD CRACKING

I used John the Ripper to recover the password of a password-protected document after extracting its password hash using an online hash extractor. I also used the provided hash calculator as an alternative method to carry out the password-cracking exercise and successfully reveal the document's password.

Additionally, I attempted the optional exercises, where I used HexStrike as a bridge to integrate Claude AI into the process. I then installed Claude Desktop on my Kali Linux virtual machine and explored how it could assist in using John the Ripper to recover the password of the encrypted document.

### PASSWORD CRACKING WITH CLAUDE AI

I installed HexStrike to serve as a bridge for integrating Claude AI with Kali Linux. I subsequently installed Claude Desktop on my Kali Linux virtual machine. This allowed me to explore how AI assistance could be used alongside cybersecurity tools to support the password recovery process.

The installation was carried out using the following command:
```curl -fsSL https://claude-desktop-debian.dev | sudo gpg --dearmor -o /usr/share/keyrings/claude-desktop-unofficial.gpg
echo "deb [signed-by=/usr/share/keyrings/claude-desktop-unofficial.gpg arch=amd64,arm64] https://claude-desktop-debian.dev stable main" | sudo tee /etc/apt/sources.list.d/claude-desktop-unofficial.list
sudo apt update && sudo apt install -y claude-desktop-unofficial
```
started the Hexstrike AI MCP server with this code 👇🏼

```cd ~/hexstrike-ai
source hexstrike-env/bin/activate
python3 hexstrike_server.
```

and then connected hexstrike MCP to Claude desktop using this code 👇🏼

```{
  "mcpServers": {
    "hexstrike-ai": {
      "command": "/home/kali/hexstrike-ai/hexstrike-env/bin",
      "args": [
        "/home/kali/hexstrike-ai/hexstrike_mcp.py",
        "--server",
        "http://localhost:8888"
      ]
    }
  }
}
```
## CONCLUSION

I successfully completed the practical exercises on password cracking using different tools to recover the passwords of password-protected documents provided by Networkwalks. These activities were carried out strictly for educational and research purposes, with explicit authorization.

During the exercises, I used John the Ripper to recover passwords from hashes obtained using an online hash extractor. I also explored the use of a hash calculator as an alternative method for password recovery. Furthermore, I attempted the optional exercise, where I integrated Claude AI into the process to assist with using John the Ripper to recover the document passwords.

Overall, these exercises improved my understanding of password-cracking techniques, the tools used in password recovery, and how artificial intelligence can support cybersecurity activities.
## EVIDENCES COLLECTED 

<img width="730" height="277" alt="IMG_7925" src="https://github.com/user-attachments/assets/5e9b405d-2e1b-4b68-b441-d2e70f69ed5e" />


<img width="687" height="235" alt="IMG_7926" src="https://github.com/user-attachments/assets/7e276c92-04a8-4a5e-a543-b2bb70d5c44f" />




<img width="819" height="548" alt="IMG_7929" src="https://github.com/user-attachments/assets/2d487757-dfbd-4731-86cb-08b3c6d507ee" />



<img width="776" height="769" alt="IMG_7941" src="https://github.com/user-attachments/assets/6d08762a-94aa-4444-9c61-1810ae829433" />




<img width="752" height="522" alt="IMG_7924" src="https://github.com/user-attachments/assets/8aa2a103-08bf-4fb1-a7a9-c71dbab45eaf" />




<img width="1200" height="714" alt="IMG_7940" src="https://github.com/user-attachments/assets/67adc6d7-6d19-42f7-a9a1-aa23d619ab2d" />

<img width="953" height="592" alt="IMG_7939" src="https://github.com/user-attachments/assets/e0d5243e-6056-4de6-90a2-5ccb50c4e3ef" />

<img width="1266" height="632" alt="IMG_7946" src="https://github.com/user-attachments/assets/10385239-4b9d-4872-85ae-875295a75c5b" />

<img width="1207" height="727" alt="IMG_7945" src="https://github.com/user-attachments/assets/95f8423c-cad3-4569-905d-025b738bf51e" />


<img width="1297" height="658" alt="IMG_7943" src="https://github.com/user-attachments/assets/be473861-f37b-434e-9294-ccc28c0917cd" />

<img width="1376" height="817" alt="IMG_7947" src="https://github.com/user-attachments/assets/2e433375-5659-4ab5-ada6-635e866a82dd" />



 ## —END—

 
| Category | Details |
| :--- | :--- |
| **👤 Author** | **NWAROH JOYPEACE** — Cybersecurity Professional B084 |
| **📌 Program Name** | Cybersecurity Program at Networkwalks |
| **📅 Week** | Week 03 |
| **💻 Repository** | GitHub |
