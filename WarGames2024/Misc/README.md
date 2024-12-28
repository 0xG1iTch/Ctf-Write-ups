# CTF Write-Up: Wargames-Ctf2024

## Challenge Title
**Christmas Gift**
 
## Description

<img width="489" alt="Screen Shot 2024-12-28 at 7 37 24 PM" src="https://github.com/user-attachments/assets/75231f82-6e5a-4c63-942c-2137f97b99cb" />

### Challenge Files
- [gif.gif](./gift.gif.zip)

---

## Solution

This challenge involved extracting the Flag from  a GIF file. Here’s how I solved it:
   I opened the [gif.gif](./gift.gif.zip) file using a normal image preview software, that allowed me to view the individual frames of the GIF as static images (ause i opened it as an image).
   The GIF had **1402 frames** in total. I scrolled through all the frames and found the flag in the **last frame**.
   
   <img width="477" alt="Screen Shot 2024-12-28 at 7 32 47 PM" src="https://github.com/user-attachments/assets/2189071a-1610-4b0b-bf96-1902a476011d" />


3. **Alternative Approach (Using Online Tools):**
   You can use online tools like [ezgif](https://ezgif.com/split) to split the GIF into all its frames, if you can't run the gif as image. From there, you can easily locate and copy the flag from the final frame.

---

## Flag:
wgmy{1eaa6da7b7f5df6f7c0381c8f23af4d3}
