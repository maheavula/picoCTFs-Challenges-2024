## Description
Know of little and big endian?

Source: https://artifacts.picoctf.net/c_titan/116/flag.c

**nc titan.picoctf.net 64710**

## Hint

  - You might want to check the ASCII table to first find the hexadecimal representation of characters before finding the endianness.
  - Read more about how endianness

![endian2](https://github.com/user-attachments/assets/45561f87-1c69-4558-b3ba-aa1dcea9e893)


## Solution

  - As per given, after execting **nc titan.picoctf.net 64710** command, interface showed it like asking little endian and big endian
 for the given word.
  - we need to find the hexadecimal value for the given word so use online calculators, after getting hexa value write in a reverse order for little endian which is from least significant to most significant.
  - Same for Big endian, enter from most significant to least significant.

    ![endian1](https://github.com/user-attachments/assets/1bc7cc1e-79d8-48b2-b0e7-b4565a8dedd9)

  - Finally, after enter correct answer, we will get the flag.

  - The flag is `picoCTF{3ndi4n_sw4p_su33ess_91bc76a4}`.
