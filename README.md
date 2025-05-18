# kali-termux-udocker
Install and run Kali Nethunter inside udocker in termux | no root

# Requirements 
```
pkg update && pkg upgrade -y && pkg install wget proot tar git python3 -y
```
# Installation
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
udocker run -it kali  
```

# Other options
```
udocker --help
```
