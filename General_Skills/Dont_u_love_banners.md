## Description

Can you abuse the banner?

The server has been leaking some crucial information on **tethys.picoctf.net 54965**. Use the leaked information to get to the server.

To connect to the running application use **nc tethys.picoctf.net 59985**. From the above information abuse the machine and find the flag in the /root directory.

## Hint

  - Do you know about symlinks?
  - Maybe some small password cracking or guessing

![Banner1](https://github.com/user-attachments/assets/db2f5424-b5ea-4c3f-9a88-e473585d4e42)

## Solution
  - We have an address for leaked information and Netcat address for to get to the server. With given address, we are greeted crucial inforamation which is a password.
  - But for what it is ?

![banner2](https://github.com/user-attachments/assets/0286f194-e061-4377-8965-48f5a07bcc4a)

  - Let explore with Netcat command, we got banner of welcome with Netcat cmd and with the a question asking like.

![Banner4](https://github.com/user-attachments/assets/f6dcf0cf-67fd-4104-ac19-50916256b89b)

  - We will try with leaked password here, certainly it is correct password. So then next is asked like top cyber security conference in the world ?

![Banner5](https://github.com/user-attachments/assets/0291c5d2-fec1-4b2e-9845-99e5f02e0305)

  - Basically I taught there would many top conferences but later I got to know that the top most is **DEF CON**.

![Banner6](https://github.com/user-attachments/assets/8a19d48e-909f-4992-abd0-e4823d34e7b9)

  - After giving it, another question is posed like first hacker ever was known for phreaking, for this I got answer from internet, who was names as **John Draper**.

![Banner7](https://github.com/user-attachments/assets/1059f9af-2e02-4c10-9db3-a1cbe19b1ddf)

  - Then we got the server shell, just need to explore for the flag.
  - As we are in the player user directory, we can see two file, those are banner and text file.
  - Once executing the banner file, it showed the welcome bannet, that's it.

![Banner8](https://github.com/user-attachments/assets/0e622b5f-cbda-423c-830a-7d8b660fdda7)

  - In the description, it was like to abuse in the root directory for the flag.
  - In the root directory, we had two files, flag.txt and script.py.
    
![Banner9](https://github.com/user-attachments/assets/8fb2d980-7072-4106-9347-6e038634f2e8)

  - So the flag.txt file looked like it contains the flag but after trying with cat to open, litterally file showed permission denied.
  - Even try to execute python file but it is asking same questions quite previously mentioned.

![Banner10](https://github.com/user-attachments/assets/6b06a9d5-c333-4ed8-9e3a-027b9c66a683)

  - I just want to edit the python file with editors but same response from shell like you dont have permission.
  - Finally, after doing so much non sense in the terminal, I saw the hint..........Cheatingg right but hints are for given for solving right ?

  - **Do you know about symlinks?**
  - A symlink, or a symbolic link, is a file that points to another file or directory on your system. Think of it almost like a shortcut.

  - Here it is how to create a symlinks, `ln -s /directory/file ./link file`.
  - ln is the link command. The -s flag specifies that the link should be soft. -s can also be entered as -symbolic.
  - By default, ln command creates hard links. The next argument is path to the file (or folder) that you want to link. (That is, the file or folder you want to create a shortcut for.)

![Banner11](https://github.com/user-attachments/assets/9931cfd7-7089-4d5a-91b7-acc9fd4cdb01)

  - Before creating link, remove the banner in user home directory and from there create the link which is `ln -s /root/flag.txt ./banner`.
  - This is beacuse of as we dont have permission to open the banner file, we are linking to flag.txt file with banner to have sudo permissions.
  - After doing symlink, try to open the banner file but still same banner results. So just tried with Netcat command from the beginning process.

![Banner12](https://github.com/user-attachments/assets/4e31fc69-2332-4242-afd7-b1de3361f366)

  - Finally we found the flag with Netcad command.
  - The flag is `picoCTF{b4nn3r_gr4bb1n9_su((3sfu11y_a0e119d4}`.


     



