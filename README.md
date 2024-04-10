# Asssignment3.2
Jessica D.
4/10/2024

# Firewall
# UFW Package Installation 
To start, we must install, enable and start the UFW package with the following commands:
```
sudo pacman -S ufw
sudo systemctl enable ufw.service
sudo systemctl start ufw.service
```

# UFW Configuration
Now that we have UFW installed to ensure that no unwanted connections occur, we will input the following to set some rules:
```
sudo ufw default deny
sudo ufw allow from 192.168.0.0/24
sudo ufw allow Deluge
sudo ufw limit ssh
```
As a quick breakdown, "sudo ufw default deny" denies all connections and the following lines add the exceptions.
