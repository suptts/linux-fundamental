# linux-fundamental
ใช้สำหรับการเรียนรู้คำสั่งใน unbuntu linux เท่านั้น

Steps:
1. Log in using ssh
```
ssh suparuek@your-azure-ubuntu-server-ip
```
หรือ
```
ssh -i ~/.ssh/id_rsa.pub suparuek@your-azure-ubuntu-server-ip
```

2. Creating a user account using useradd command on Ubuntu
```
sudo useradd -s /bin/bash -d /home/suparuek/ -m -G sudo suparuek
sudo passwd suparuek
```

3. How to delete a user account
```
sudo userdel suparuek
```
4. How to change Linux user password
```
   sudo passwd suparuek
```
To change your own account password, run:
```
passwd
```
