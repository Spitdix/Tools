# Instalation de Visual Studio Code sur CentOS

```
sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
```
Dans le fichier:
```
sudo nano /etc/yum.repos.d/vscode.repo
```
>```
>[code]
>name=Visual Studio Code
>baseurl=https://packages.microsoft.com/yumrepos/vscode
>enabled=1
>gpgcheck=1
>gpgkey=https://packages.microsoft.com/keys/microsoft.asc
>```
Installation
```
sudo yum install code
```

Enjoy !! 😉
