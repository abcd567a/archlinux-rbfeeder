# archlinux-rbfeeder ver 1.0.10+bullseye 

### Install RadarBox24's Data Feeder on Arch Linux OS on: <br> (1) PC & Laptop: amd64, x86_64, i386  </br> (2) Raspberry PI and other SBC: armhf, armv7 arm64, aarch64, armv8 </br>

### Issue following 3 commands, and rbfeeder will be installed on your Computer / Pi </br>

```
git clone https://github.com/abcd567a/archlinux-rbfeeder
```
```
cd archlinux-rbfeeder
```
```
makepkg -si
```

### When installation is completed:
(A) If you already have a feeder key, then issue following commands to signup  </br>
(Replace `xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx` by your actual key)</br>

```
sudo rbfeeder --setkey xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

sudo reboot
```
</br>
(B) If you dont have a key, then issue following command. </br>
</br>

```
sudo systemctl restart rbfeeder
```

The Radarbox24 System will automatically allot a key and **Station Number**, both of which will be saved in file `/etc/rbfeeder.ini`. Note this number and email to radarbox support to liink it to your account. </br>


#### To check status:
```
sudo systemctl status rbfeeder  

```

</br>
