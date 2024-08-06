## Description

What was I last working on? I remember writing a note to help me remember...

You can download the challenge files here: https://artifacts.picoctf.net/c_titan/66/challenge.zip

## Hint
  - The cat command will let you read a file, but that won't help you here!
  - Read the chapter on Git from the picoPrimer.
  - When committing a file with git, a message can (and should) be included.
    
![time machine2](https://github.com/user-attachments/assets/b2eb7c85-e54d-4534-8005-6148a0acc80f)

## Solution

I moved to last directory and from the given file, opened file using cat command and I haven't seen any usefull thing,
so I opened the source file using `vim` editor. After looking into content of file, the tempting thing is COMMIT CONFIG sentence, so
clicked on it.


![Time machine1](https://github.com/user-attachments/assets/cd8e1aa8-be1a-4b1c-8fd0-042d6bcb0576)

Then finally I got the flag `picoCTF{t1m3m@ch1n3_d3161c0f}`.

