## Description
I accidentally wrote the flag down. Good thing I deleted it!

You download the challenge files here: https://artifacts.picoctf.net/c_titan/77/challenge.zip

## Hint

  - Version control can help you recover files if you change or lose them!
  - Read the chapter on Git from the picoPrimer
  - You can 'checkout' commits to see the files inside them

![git commit5](https://github.com/user-attachments/assets/56868fa5-b9d5-4557-abcf-ae3ac91a66ff)

## Solution

  - With the given **message.txt** file, I opened but the content is like
    
![Git commit1](https://github.com/user-attachments/assets/59b744e4-03d6-4211-bb49-6637406dcea5)

  -  To see what commits have made, the command is to use **$git log** to find commit hashes.
![git commit2](https://github.com/user-attachments/assets/caa7d254-9d28-4dc5-b19b-75bdf4096558)
  -  With hashes it is possible to checkout what was content inside the file. 
![git commit3](https://github.com/user-attachments/assets/bafb0b68-02e0-45d9-8def-cefcfffd1577)

  - After executing the **$git checkout <hash>** Head positions will be changed and at last if you try to open the file to get flag, you will see it.

![git commit4](https://github.com/user-attachments/assets/e305e360-edd1-4d87-aa42-825746c0a580)

  - The flag is `picoCTF{s@n1t1z3_30e86d36}`.
