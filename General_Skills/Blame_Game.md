## Description

Someone's commits seems to be preventing the program from working. Who is it?

You can download the challenge files here: https://artifacts.picoctf.net/c_titan/73/challenge.zip

## Hint

  - In collaborative projects, many users can make many changes. How can you see the changes within one file?
  - Read the chapter on Git from the picoPrimer
  - You can use python3 <file>.py to try running the code, though you won't need to for this challenge.

![blame1](https://github.com/user-attachments/assets/9f77bdc6-c118-4aa2-95cb-1913b7c5ec77)

## Solution 

  - Initally with given **message.py** file, I got an syntax error and I made it correct, even though I did not get flag.
  - Then I taught if I would see the flag with difference between two files.

![blame2](https://github.com/user-attachments/assets/7a29ff65-39b9-42db-9ef8-e1e5428fe611)

  -   But I could not finf it, so then i would like try with **$git log -p** command because i can show the commit hashes and their authors so then I can find who is preventing from working.

 ![blame3](https://github.com/user-attachments/assets/e80f9733-26ef-4be0-9f33-69b9243c6615)

  - Finally I found who preventing the program from working as flag.
  - The flag is `picoCTF{@sk_th3_1nt3rn_e9957ce1}`.
