## About The LTSB Version Of Win10 x64

It is a Long Time Service Branch, Just like ubuntu 16.04 LTS

## Comparing Win10 LTSB 2016 x64 to Win10 x64 professional

- win10 x64 professional needs 2.1G ram when open the system
- win10 LTSB x64 2016 just needs no more than 1.1G ram when open the system, because it remove useless softwares like Cortana,win10 UWP apps and all of useless codes and functions.
- The use of win10 LTSB x64 is same like professonal edition, and all of development work is perfect.

## For better taste of it

- install ConsoleZ, you can find it in sources folder
- install Office 2013, when installing, choose the module you needs. Microsoft Office 2016 would install all module of Office which seems bloated.
- install WangYiYouXiangDaShi to replace windows love mail(windows live mail based on uwp,And WangYiYouXiangDaShi is same with windows live mail and has same UI)

## When Installing Win10_LTSB_x64

After installed,Connect to wifi to auto install your computer drivers, It should wait for some time.You can check it in settings/update

## Activate The LTSB

After installed system and office, You can use autokms activate office and system at same time, If you don't need auto activate after 180days, Just keep autokms and it is in plan task, After 180days would activate one more time.All remove kms and after 180days, you can reinstall it.

## The link of LTSBx64 win10

You can find it at itellyou, the link is below

```
ed2k://|file|cn_windows_10_enterprise_2016_ltsb_x64_dvd_9060409.iso|3821895680|FF17FF2D5919E3A560151BBC11C399D1|/
FileName: cn_windows_10_enterprise_2016_ltsb_x64_dvd_9060409.iso
SHA1: 9E405E950890D2A196565BCA35E152F9CFAD296D
FileSize: 3.56GB
Update Time: 2016-08-11
```

You can check sha1 if file is right.

## The Access of sources of Some software and use of them

1.Win10_LTSB_2016x64(You Can By Thunder Lite, Download in https://pc.qq.com/ , the url is https://sm.myapp.com/original/Download/ThunderSpeed1.0.35.366.exe), and then open thunder , copy the below

ed2k://|file|cn_windows_10_enterprise_2016_ltsb_x64_dvd_9060409.iso|3821895680|FF17FF2D5919E3A560151BBC11C399D1|/

2.Office(You Can By Thunder Lite, Download in https://pc.qq.com/ , the url is https://sm.myapp.com/original/Download/ThunderSpeed1.0.35.366.exe), and then open thunder , copy the below

ed2k://|file|cn_office_professional_plus_2013_x64_dvd_1134006.iso|914106368|E5FBAE9EE9CB35D5E777EA78F7F50410|/

3.Activate Tools

http://7xq5e8.com1.z0.glb.clouddn.com/win10_LTSB_LongTimeServiceBranch2016X64/KMSpico%20v10.2.0%20Install.7z

4.ConsoleZ with a good config

http://7xq5e8.com1.z0.glb.clouddn.com/win10_LTSB_LongTimeServiceBranch2016X64/ConsoleZ.x64.1.18.2.17272.zip

> The config Is Better in use, download this version would be configed ,It saved in xml

- Ctrl + → : Split screen right
- Ctrl + ↓ : Split screen down
- Shift + LeftClick(Mouse) : Select Text
- LeftClick(Mouse): Copy Text (After Selected Test)
- Ctrl + T : New Tab
- Ctrl + W : Close Tab
- Ctrl + Shift + W: close split screen
- Ctrl + V : Paste Text
- Ctrl + Z : Undo Edit
- ↑ : Last Comind
- ↓ : Next Comind

It transfer powershell, You can get better experience.

Some Other config Could Set by yourself.

5.WangYiYouXiangDaShi

http://7xq5e8.com1.z0.glb.clouddn.com/win10_LTSB_LongTimeServiceBranch2016X64/WangYiYouXiangDaShi.exe

Same like windows live mail.

6.AutoKms

http://7xq5e8.com1.z0.glb.clouddn.com/win10_LTSB_LongTimeServiceBranch2016X64/KMSpico%20v10.2.0%20Install.7z

7.NVM

http://7xq5e8.com1.z0.glb.clouddn.com/win10_LTSB_LongTimeServiceBranch2016X64/nvm-setup.exe

A node edition controller

After installed:

example, use :

```
nvm install 8.9.3
```

```
nvm use 8.9.3
```

Then, The node and npm is installed.

And then set Taobao source for better use


```
npm config set registry https://registry.npm.taobao.org
```

8.node-gyp

If you use sass

first:

```
npm install -g node-gyp
```

Then:

```
npm install --global --production windows-build-tools
```

This will install python27, but it will not influce your installed python or your PATH.

## Set multi github account in One PC

### 1.Open the git bash and input the codes:

```
 ssh-keygen -t rsa -b 4096 -C "shinepans@live.com (Your Email)"
```

And it outcomes:

```
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/shinepans/.ssh/id_rsa): id_rsa_cess (id_rsa_cess:We need to create a new name that is different from the previous file name )
```

And it outcomes:

```
Enter passphrase (empty for no passphrase): (Enter)
Enter same passphrase again:(Enter)
Your identification has been saved in id_rsa_cess.
Your public key has been saved in id_rsa_cess.pub.
The key fingerprint is:
SHA256:jgkhEZIjeQNF6CZWU+sIpCUbZBIip+AdgQcZlnXlon0 shinepans@live.com
The key's randomart image is:
+---[RSA 4096]----+
|%/#=oo..         |
|^%+=o o          |
|*=+ooo .         |
|.+..=..          |
|+  o.o ES        |
|     ..+         |
|      o .        |
|                 |
|                 |
+----[SHA256]-----+
```


### 2.Configure the ~/.ssh/config file


```
Host github.com
    HostName github.com
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/id_rsa
Host cess.github.com
    HostName github.com
    PreferredAuthentications publickey
    IdentityFile ~/.ssh/id_rsa_cess
```

### 2.Add the new generated SSH key to the associated Github account

> Add the newly generated key in id_rsa_cess.pub to the associated Github account. 

**And Then Use**

```
$ ssh -T git@cess.github.com
```

**to test whether the association is successful. The xxx.github.com used here is the name of the second host in the previous config.**

And it should be outcomes:

```
$ Hi cessuser! You've successfully authenticated, but GitHub does not provide shell access.
```

### 3.Use multiple SSH Key

If we need use default account whose ssh key is id_ras.pub, we can use 

```
git clone git@github.com:USER/SOMETHING.git
```

If we need use another account whose ssh key is id_ras_cess.pub, we can use 

```
git clone git@cess.github.com:USER/SOMETHING.git

## More Notes..