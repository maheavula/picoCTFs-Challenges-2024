## Description

Using a Secure Shell (SSH) is going to be pretty important.

Can you **ssh** as **ctf-player** to **titan.picoctf.net** at port **51318** to get the flag?

You'll also need the password **1db87a14**. If asked, accept the fingerprint with yes.

## Hint
  - https://linux.die.net/man/1/ssh
  - You can try logging in 'as' someone with <user>@titan.picoctf.net
  - How could you specify the port?
  - Remember, passwords are hidden when typed into the shell

![SSH2](https://github.com/user-attachments/assets/5bf28ab5-2f54-4be3-956e-d0d824dbd9f6)


## Solution

  - With the given credential I connected to SSH service of picoCTF and it gave the flag just after establishing secure connection.

   ![SSH1](https://github.com/user-attachments/assets/58d58c33-30fa-4160-81de-17d10255af54)

  - The flag is `picoCTF{s3cur3_c0nn3ct10n_45a48857}`.
    

