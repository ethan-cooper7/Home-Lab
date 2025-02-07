# HOME LAB

## Objective

The Home Lab project aimed to establish a basic understanding of installing and configuring virtual machines with different operating systems. The primary focus was to build an environment to test new tools (e.g. Kali Linux) and learn new techniques (e.g. malware, security testing, and system management).

### Skills Learned

- Installing and configuring Operating Systems.
- Knowledge of assigning static IPv4 addresses.
- Ability to use Linux terminal and Command Prompt to confirm connection between machines.


### Tools Used

- VirtualBox for building virtual machines.
- Kali Linux to eventually build malware for penetration testing.
- Windows 10 to simulate a target environment for security testing and system management.


## Steps
##### Prerequisites:
- Install VirtualBox
- Download 7zip
- Download Kali Linux and Windows 10
#
#### Step 1: 
- In VirtualBox, select the blue icon “New” and create a virtual machine using the downloaded “Windows.iso”.
  
![Step 1](https://github.com/user-attachments/assets/fb23814f-71d4-4cb3-89d1-538f0ba20acc)

#### Step 2:
- Use 7zip to extract Kali Linux to the desktop (or preferred location).

#### Step 3:
- Open the new folder and run the “.vbox” version of Kali to automatically import it into VirtualBox.

#### Step 4:
- Run the machines individually to confirm proper installation of each OS.

#### Step 5:
- Click on the Windows machine, open “Settings”, go to “Network”.
- Change the network type from “NAT” to “Internal Network” and give it a unique name.
- Repeat for Kali machine
  
![Step 5](https://github.com/user-attachments/assets/54039b38-c566-4d1f-86ac-7af4461edd4e)

#### Step 6:
- Open Windows Machine.

#### Step 7:
- Right-click globe icon in bottom right of taskbar.
- Click "Open Network & Internet settings".

#### Step 8:
- Scroll down and click “Change adapter options”.
  
![Step 8](https://github.com/user-attachments/assets/bedb2798-9509-4bcb-977a-85df5640ee5b)

#### Step 9:
- Right-click your Ethernet and click “Properties”.

#### Step 10:
- Double-click “Internet Protocol Version 4 (TCP/IPv4)".

#### Step 11:
*Enter the following:*
- **IP address:** 192.168.20.10
- **Subnet Mask:** 255.255.255.0

![Step 11](https://github.com/user-attachments/assets/9934b892-82f9-4c31-bc7d-eea5c5b8249e)

#### Step 12:
- Hit the "Start" button, type "cmd", and open Command Prompt.

#### Step 13:
- To confirm new IP, type "ipconfig" then hit enter.

![Step 13](https://github.com/user-attachments/assets/91ed7d63-b269-4878-9dd1-03197a5303d2)

#### Step 14:
- Open Kali Linux machine.

#### Step 15:
- In the top right corner, click on the Network icon, and select "Edit Connections".

#### Step 16:
- Click on "Wired connection 1", then select the gear icon in the bottom left.

#### Step 17:
- Click on "IPv4 Settings"

![step 17](https://github.com/user-attachments/assets/936980b9-3648-4fdf-947b-5f6e02007ca2)

#### Step 18:
- Change "Automatic (DHCP)" to "Manual".

#### Step 19:
*Enter the following. Hit Add & Save:*
- **Address:** 192.168.20.11
- **Netmask:** 24

![Step 19](https://github.com/user-attachments/assets/f62a08fc-22c7-44a4-b26a-5b3800180205)

#### Step 20:
- Go to Desktop, right-click and select "Open Terminal Here".

#### Step 21:
- To confirm new IP, type "ifconfig" then hit enter.

![Step 21](https://github.com/user-attachments/assets/e6665e78-ae73-4cba-be08-c82f3f392672)

#### Step 22:
- In the Windows machine, once again open Command Prompt.

#### Step 23:
- To confirm connectivity between the two machines, type "ping 192.168.20.11".

![Step 23](https://github.com/user-attachments/assets/a00f7901-63d1-4659-899c-fe468279e200)

#### Step 24:
# CELEBRATE!!!!!!!

