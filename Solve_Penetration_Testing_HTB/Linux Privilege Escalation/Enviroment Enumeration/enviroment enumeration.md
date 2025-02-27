1.  Enumerate the Linux environment and look for interesting files that might contain sensitive data. Submit the flag as the answer.
kết nối từ xa tới máy chủ đích sử dụng ssh với user:htb-student password:HTB_@cademy_stdnt!
```bash
┌─[eu-academy-5]─[10.10.14.42]─[htb-ac-1522420@htb-o37yfkajwf]─[~]
└──╼ [★]$ ssh htb-student@10.129.140.10
The authenticity of host '10.129.140.10 (10.129.140.10)' can't be established.
ED25519 key fingerprint is SHA256:HfXWue9Dnk+UvRXP6ytrRnXKIRSijm058/zFrj/1LvY.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? ýe 
Please type 'yes', 'no' or the fingerprint: yes
Warning: Permanently added '10.129.140.10' (ED25519) to the list of known hosts.
htb-student@10.129.140.10's password: 
Welcome to Ubuntu 20.04.3 LTS (GNU/Linux 5.4.0-148-generic x86_64)

 * Documentation:  https://help.ubuntu.com
 * Management:     https://landscape.canonical.com
 * Support:        https://ubuntu.com/advantage

  System information as of Sat 11 Jan 2025 09:37:21 AM UTC

  System load:             0.11
  Usage of /:              50.7% of 7.33GB
  Memory usage:            6%
  Swap usage:              0%
  Processes:               260
  Users logged in:         0
  IPv4 address for ens160: 10.129.140.10
  IPv6 address for ens160: dead:beef::250:56ff:fe94:ec64

 * Strictly confined Kubernetes makes edge and IoT secure. Learn how MicroK8s
   just raised the bar for easy, resilient and secure K8s cluster deployment.

   https://ubuntu.com/engage/secure-kubernetes-at-the-edge

190 updates can be applied immediately.
116 of these updates are standard security updates.
To see these additional updates run: apt list --upgradable


The list of available updates is more than a week old.
To check for new updates run: sudo apt update

$ 
```
Sử dụng câu lệnh cat /etc/os-release để xem phiên bản của máy chủ đích 
```bash
$ cat /etc/os-release
NAME="Ubuntu"
VERSION="20.04.3 LTS (Focal Fossa)"
ID=ubuntu
ID_LIKE=debian
PRETTY_NAME="Ubuntu 20.04.3 LTS"
VERSION_ID="20.04"
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
VERSION_CODENAME=focal
UBUNTU_CODENAME=focal
$ 
```

```bash
$ ls /home
htb-student  lab_adm
$ cd htb-student
-sh: 8: cd: can't cd to htb-student
$ ls
$ cd lab_adm
-sh: 10: cd: can't cd to lab_adm
$ 
```