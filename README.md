# ansible-homework-2

```
[root@ansible project]# ansible-playbook main.yml 

PLAY [web] *********************************************************************

TASK [Gathering Facts] *********************************************************
ok: [143.198.124.18]
ok: [143.198.124.172]

TASK [Tasks for Centos 7 (redhat)] *********************************************
included: /root/project/RedHat.yml for 143.198.124.18
included: /root/project/Debian.yml for 143.198.124.172

TASK [Check if file is connected to main.yml] **********************************
ok: [143.198.124.18] => {
    "msg": "Hello, this is Centos 7!"
}

TASK [Install httpd for Centos 7 (redhat)] *************************************
changed: [143.198.124.18]

TASK [Install unzip for Centos 7 (redhat)] *************************************
changed: [143.198.124.18]

TASK [Check if httpd is running] ***********************************************
changed: [143.198.124.18]

TASK [Download and unarchive into /var/www/html] *******************************
changed: [143.198.124.18]

TASK [Check if file is connected to main.yml] **********************************
ok: [143.198.124.172] => {
    "msg": "Hello, this is Ubuntu!"
}

TASK [Install apache2 httpd for Ubuntu (debian)] *******************************
changed: [143.198.124.172]

TASK [Install unzip for Ubuntu (debian)] ***************************************
changed: [143.198.124.172]

TASK [Check if apache2 is running] *********************************************
ok: [143.198.124.172]

TASK [Download and unarchive into /var/www/html] *******************************
ok: [143.198.124.172]

TASK [Tasks for Ubuntu (debian)] ***********************************************
included: /root/project/RedHat.yml for 143.198.124.18
included: /root/project/Debian.yml for 143.198.124.172

TASK [Check if file is connected to main.yml] **********************************
ok: [143.198.124.18] => {
    "msg": "Hello, this is Centos 7!"
}

TASK [Install httpd for Centos 7 (redhat)] *************************************
ok: [143.198.124.18]

TASK [Install unzip for Centos 7 (redhat)] *************************************
ok: [143.198.124.18]

TASK [Check if httpd is running] ***********************************************
ok: [143.198.124.18]

TASK [Download and unarchive into /var/www/html] *******************************
ok: [143.198.124.18]

TASK [Check if file is connected to main.yml] **********************************
ok: [143.198.124.172] => {
    "msg": "Hello, this is Ubuntu!"
}

TASK [Install apache2 httpd for Ubuntu (debian)] *******************************
ok: [143.198.124.172]

TASK [Install unzip for Ubuntu (debian)] ***************************************
ok: [143.198.124.172]

TASK [Check if apache2 is running] *********************************************
ok: [143.198.124.172]

TASK [Download and unarchive into /var/www/html] *******************************
ok: [143.198.124.172]

PLAY RECAP *********************************************************************
143.198.124.172            : ok=13   changed=2    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   
143.198.124.18             : ok=13   changed=4    unreachable=0    failed=0    skipped=0    rescued=0    ignored=0   

[root@ansible project]# 
```
