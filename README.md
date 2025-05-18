<img src="https://github.com/xiv3r/kali-termux-udocker/blob/main/udocker.png">

## 1. Requirements 
```
pkg update && pkg upgrade -y && pkg install udocker -y
```
## 2. Install kali container
```
udocker pull kalilinux/kali-rolling
```
## 3. Create a kali container
```
udocker create --name=kali kalilinux/kali-rolling  
```
## 4. Run kali
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
## 5. Update & Upgrade kali
```
apt update && apt upgrade -y
```
- install common tools
```
apt install nano git vim sudo wget curl telnet ssh traceroute -y
```
## 6. GUI Setup (Optional - Requires VNC)
```
apt install tightvncserver xfce4 -y
```
```
vncserver :1 -geometry 1280x720 -depth 24  
```  
→ Connect via **VNC Viewer** to `localhost:5901`

## 7. Other options
```
udocker --help
```

## 8. Similar Docker Images
- Blackarch
```
udocker pull blackarchlinux/blackarch
```
- Archlinux
```
udocker pull archlinux
```
- Ubuntu 
```
udocker pull ubuntu:22.04
```
- Debian
```
udocker pull debian:bookworm
```
- Alpine
```
udocker pull alpine:latest
```
- CentOS
```
udocker pull centos:7
```
- Parrot Sec
```
udocker pull parrotsec/security:latest
```
- Fedora
```
udocker pull fedora:latest
```
- Gentoo
```
udocker pull gentoo/stage3
```
- Opensuse
```
udocker pull opensuse/leap:latest
```
- Slackware
```
udocker pull vbatts/slackware:latest
```
- Void
```
udocker pull voidlinux/voidlinux
```
- Alma
```
udocker pull almalinux:9
```
- Artix
```
udocker pull artixlinux/base
```

