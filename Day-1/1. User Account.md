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


- `-s /bin/bash` – Set /bin/bash as login shell of the new account
- `-d /home/suparuek/ – Set /home/suparuek/ as home directory of the new Ubuntu account
- `-m` – Create the user’s home directory
- `-G sudo `– Make sure suparuek account can sudo i.e. give admin access to the new account

3. How to veryfi that user account added to the system
```
   cat /etc/passwd
   grep '^suparuek' /etc/passwd
```

4. How to delete a user account
```
   sudo userdel suparuek
```
5. How to change Linux user password
```
   sudo passwd suparuek
```
6. To change your own account password, run:
```
   passwd
```
