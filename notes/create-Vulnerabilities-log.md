
write vulnerabilities:
![alt text](image-6.png)


mainly anonymous guest access, Weak authentication, Overly permissive file permissions, outdated SMBv1 (NT1) protocol


add smb user share1,
also with a weak password: `password123`
![alt text](image-7.png)


改 /etc/exports：/proj/nas 导出给 *，rw + no_root_squash
![alt text](image-8.png)

重启服务
![alt text](image-9.png)

验证
![alt text](image-10.png)