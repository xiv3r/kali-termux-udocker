# Requirements 
```
pkg update && pkg upgrade -y && pkg install wget proot tar git python3 -y
```
# Install udocker
```
git clone https://github.com/xiv3r/kali-termux-udocker.git
cd kali-termux-udocker
```
```
bash install.sh
```
# Install kali nethunter
```
udocker pull kalilinux/kali-rolling
```
# Create a kali container
```
udocker create --name=kali kalilinux/kali-rolling  
```
# Run kali
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

# Other options
```
udocker --help
```
