## 1. Requirements 
```
pkg update && pkg upgrade -y && pkg install wget proot tar git python3 -y
```
## 2. Install udocker
```
git clone https://github.com/xiv3r/kali-termux-udocker.git
cd kali-termux-udocker
```
```
bash install.sh
```
## 3. Install kali nethunter
```
udocker pull kalilinux/kali-rolling
```
## 4. Create a kali container
```
udocker create --name=kali kalilinux/kali-rolling  
```
## 5. Run kali
```
udocker run kali  
```
---
| Command | Description |  
|---------|-------------|  
| `udocker ps` | List containers |  
| `udocker start kali` | Start Kali |  
| `udocker attach kali` | Re-enter Kali |  
| `udocker rm kali` | Delete Kali |

---
## 6. Update & Upgrade kali
```
apt update && apt upgrade -y
```
- install common tools
```
apt install nano git vim sudo wget curl telnet ssh traceroute -y
```
## 7. GUI Setup (Optional - Requires VNC)** 
```
apt install tightvncserver xfce4 -y
```
```
vncserver :1 -geometry 1280x720 -depth 24  
```  
→ Connect via **VNC Viewer** to `localhost:5901`


## 8. Other options
```
udocker --help
```
