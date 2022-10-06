# Lab 2 - Port Scanning

In this lab we will be using nmap to scan the Metaploitable2 system. By now you should have both machines installed and running on the same network. Please upload a word document or PDF file with your answers



**Preparation Steps**

* Launch both your Kali Linux machine and the Metasploitable2 system.
* Logon to Kali by using "kali" for both username and password
* Open a terminal window and type “ifconfig” and make a note of the IP address
* Logon to Metasploitable2 machine by using “msfadmin” for both username and password
* Type “ifconfig” and make a note of the IP address


**TCP Port Scanning**

From your Kali box perform a TCP port scan on the Metasploitable2 to detect running services.

From Kali terminal window run the following command

```$ nmap -sT <METASPLOITABLE IP ADDRESS>```


What ports and services did Nmap find? Please insert a screenshot of the output or copy and paste the table of open ports along with the states and services as listed

From Kali terminal window run the following command

```$ nmap -sS <METASPLOITABLE IP ADDRESS>```



1. What ports and services did Nmap find? Please insert a screenshot of the output or copy and paste the table of open ports along with the states and services as listed?

2. Are there any differences between each scan?

3. What service is running on port 23?

4. What service is running on Port 80

5. Is the service on Port 80 using SSL?

6. What port is VNC running on?



**UDP Port Scanning**

From your Kali box perform a UDP port scan on the Metasploitable2 VM using the following command

```$ sudo nmap -sU -T4 <METASPLOITABLE IP ADDRESS>```



1. What does the switch -T4 do and why is it a good idea to use when scanning for UDP ports?

2. What UDP ports did nmap report as open?

3. What services are running on those ports?

4. What service runs on UDP port 53?



**OS Detection**

Using the following command perform an OS detection on your Metasploitable2 machine.

```$ nmap -O <METASPLOITABLE IP ADDRESS>```

1. According to Nmap what is the operating system running on Metasploitable2?

2. What is listed under “OS details” field?



**Service Version Detection**

From your Kali VM terminal window run the following command

```$ nmap -sV <METASPLOITABLE IP ADDRESS>```

1. What is the version of vsftpd running on the system?

2. What is the version of VNC running on the system?

3. What is the version of ProFTPD running on the system?
