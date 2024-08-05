## Description

Want to play a game? As you use more of the shell, you might be interested in how they work! Binary search is a classic algorithm used to quickly find an item in a sorted list. Can you find the flag? You'll have 1000 possibilities and only 10 guesses.
Cyber security often has a huge amount of data to look through - from logs, vulnerability reports, and forensics. Practicing the fundamentals manually might help you in the future when you have to write your own tools!

You can download the challenge files here: https://artifacts.picoctf.net/c_atlas/20/challenge.zip

## Hints
  - Have you ever played hot or cold? Binary search is a bit like that.
  - You have a very limited number of guesses. Try larger jumps between numbers!
  - The program will randomly choose a new number each time you connect. You can always try again, but you should start your binary search over from the beginning - try around 500. Can you think of why?

![Binary search2](https://github.com/user-attachments/assets/e3b6fc27-adfe-4358-a6cd-cb7b1b54be6c)

## Solution

As a beginner, initally I tried in a different ways with changing in code to get the flag but later trying many times, I saw the hints and tried guessing the target number untill I get the Flag. 

![Binary search1](https://github.com/user-attachments/assets/d726587d-8aab-42cd-81ef-39ebc581ade5)

Finally after so many attempts I got the correct guessing number and flag which is `picoCTF{g00d_gu355_bee04a2a}`
