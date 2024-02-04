# Thêm người dùng trên linux

- ssh root@182.168.1.1 + password
- adduser independence -> pasword: kh17112003
- su - independence
- exit


- ls -l /etc/sudoers 
- chmod u+w /etc/sudoers 

```bash
root ALL=(ALL:ALL) ALL
sondang ALL=(ALL:ALL) ALL
```

- chmod u-w /etc/sudoers 