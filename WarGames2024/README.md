# WarGames ctf 2024

# Cryptography

## Challenge: Credentials

### Description

<img width="419" alt="Screen Shot 2024-12-28 at 7 23 19 PM" src="https://github.com/user-attachments/assets/83a85aad-6db9-4d00-945f-50147c0d9abb" />

#### Challenge Files: [Leak_stuff.rar](../Files/Leak_stuff.rar)

### Solution

This challenge was straightforward, and here's how I solved it step-by-step:

1. **Decompressing the Archive:**
   First, I extracted the contents of the [Leak_stuff.rar](../Files/Leak_stuff.rar) file. Inside the archive, I found two files: `user.txt` and `password.txt`.

2. **Identifying the User:**
   The challenge prompt asked to search for the user "osman" in the `user.txt` file. I quickly found the user at line 337.

3. **Finding the Encrypted Password:**
   I looked for the corresponding line in the `password.txt` file. The entry related to "osman" turned out to be: `ZJPB{e6g180g9f302g8d8gddg1i2174d0e212}`

4. **Decrypting the Password:**
   The string looked like a Caesar cipher with a shift. I tried various Caesar cipher shifts using the online tool [Cryptii](https://cryptii.com/). The shift of **23** decrypted the string correctly.
<img width="1455" alt="Screen Shot 2024-12-28 at 7 09 08 PM" src="https://github.com/user-attachments/assets/0505e2f3-0a7d-44a6-a012-89f181c4c59d" />

### Flag:
   WGMY{b6d180d9c302d8a8daad1f2174a0b212}

---

# Misc

## Challenge-1: Christmas Gift
 
### Description

<img width="489" alt="Screen Shot 2024-12-28 at 7 37 24 PM" src="https://github.com/user-attachments/assets/75231f82-6e5a-4c63-942c-2137f97b99cb" />

#### Challenge Files: [gift.gif.zip](.//Files/gift.gif.zip)

### Solution

This challenge involved extracting the Flag from  a GIF file. Here’s how I solved it:
   I opened the [gif.gif](../Files/ gift.gif.zip) file using a normal image preview software, that allowed me to view the individual frames of the GIF as static images (ause i opened it as an image).
   The GIF had **1402 frames** in total. I scrolled through all the frames and found the flag in the **last frame**.
   
   <img width="477" alt="Screen Shot 2024-12-28 at 7 32 47 PM" src="https://github.com/user-attachments/assets/2189071a-1610-4b0b-bf96-1902a476011d" />

3. **Alternative Approach (Using Online Tools):**
   You can use online tools like [ezgif](https://ezgif.com/split) to split the GIF into all its frames, if you can't run the gif as image. From there, you can easily locate and copy the flag from the final frame.

### Flag:
wgmy{1eaa6da7b7f5df6f7c0381c8f23af4d3}

## Challenge-2: Invisible Ink

### Description

<img width="487" alt="Screen Shot 2024-12-29 at 2 08 42 PM" src="https://github.com/user-attachments/assets/8b09cf12-79c6-496f-8c39-fc5eb0e4f9b7" />

#### Challlenge Files: 
![challenge](https://github.com/user-attachments/assets/6adb9af4-da05-42f6-bb8d-5f38325d7064)

### Solution

 **Initial Analysis:**
   -Given a GIF file that presumably contains hidden information
   -"Invisible ink" Title suggests that some parts of the image might be hidden or partially visible
 **Steganography analysis tool:**
    -Analyzing the GIF file using *StegSolve* to extract individual frames, found 2 distinct frames:
    ![trial1](https://github.com/user-attachments/assets/35699cd0-5e9b-4adc-8275-1e11bf18cdb0)   ![trial2](https://github.com/user-attachments/assets/46ecb3ff-4dbb-4d39-85bf-a63bbabe28b5)

 **Flag Recovery:**

 -The flag was split across two frames. Using Stegsolve's frame combiner we merge the two frames, revealing the complete flag.
 ![invinkflag](https://github.com/user-attachments/assets/eacde539-2719-4479-a2cc-4d0148593415)
 
### Flag:
   wgmy{d41d8cd98f00b204e9800998ecf8427e}
