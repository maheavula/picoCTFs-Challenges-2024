## Description

My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?

You can download the challenge files here: https://artifacts.picoctf.net/c_titan/70/challenge.zip

## Hint

  - git branch -a will let you see available branches
  - How can file 'diffs' be brought to the main branch? Don't forget to git config!
  - Merge conflicts can be tricky! Try a text editor like nano, emacs, or vim.

![collab1](https://github.com/user-attachments/assets/bf294994-b96f-4c4c-b8ef-71d3df0c0c11)

## Solution

  - They have given **flag.py** and after opened it, just showed string.

    ![collab2](https://github.com/user-attachments/assets/e00388d7-33c3-46b2-9dca-355b4e01f6df)
    
  - I tried moving to different directories in **.git**, but i could not find the flag.
  - Later I saw hints, executed first command **$git branch**, it listed some parts of the features.

![collab3](https://github.com/user-attachments/assets/d9033af4-d425-468a-90d3-676e43fd135a)

  - Later with **diff** command from **git**, I opened all 3 parts and merged the flags and found final flag.

![collab4](https://github.com/user-attachments/assets/3219f45c-e739-4c05-83e0-b3755c891b52)
![collab5](https://github.com/user-attachments/assets/9dada2c7-b3b1-479c-a886-7bb69a08159a)


  - The flag is `picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_7ffa0077}`.
