# PICOCTF WRITEUP – INSP3CT0R
by Gaurish Bahurupi

## Information

- CTF Name: PicoCTF
- CTF Challenge: Insp3ct0r
- Challenge Category: Web Exploitation
- Challenge Points: 50
- PicoCTF 2019.

## Challenge Description

Kishor Balan tipped us off that the following code may need inspection: 

[https://jupiter.challenges.picoctf.org/problem/41511/](https://jupiter.challenges.picoctf.org/problem/41511/) 

or 

[http://jupiter.challenges.picoctf.org:9670](http://jupiter.challenges.picoctf.org:41511)

## Writeup

After opening either one of the previous links we get to this page:

<img width="1440" alt="Screenshot 2024-03-26 at 2 13 23 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/e717faf9-fae0-4ec4-b953-022186e5a766">


In the challenge description, it is stated “the following code may need inspection”, after reading this, I decided to inspect the page. To do that there are three main ways, either press F12, press Ctrl + Shift + I, or right-click on the page and choose the option “Inspect”.

I decided to use F12. After doing so, I was presented with this:

<img width="1440" alt="Screenshot 2024-03-26 at 2 13 58 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/e4e8772b-5f07-4636-9447-12d014bb2fb0">


As we can see on the right we have the developer tools. At the top of the developer tool environment, we can see a tab that says “Sources”. By clicking on it we get to this:

<img width="1440" alt="Screenshot 2024-03-26 at 2 14 08 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/6f42b846-7348-44a7-b1bc-e266ef2ab968">


In the developer tool environment, on the left, we have a folder named “problem/9670 and inside this folder, there are 3 files.

- 41511/
- myjs.js
- mycss.css

By clicking on each one to see the contents we can see:

**41511**

<img width="1440" alt="Screenshot 2024-03-26 at 2 06 58 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/58482f4e-d3fe-4059-ac30-8b0985b53d58">

**myjs.js**

<img width="1440" alt="Screenshot 2024-03-26 at 2 07 08 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/12c3d4a4-4414-47d8-b0b3-bd0cb05bc2ba">

**mycss.css**

<img width="1440" alt="Screenshot 2024-03-26 at 2 07 15 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/d36053fd-7984-4e5a-8477-9845c1b67f9a">

As we can see highlighted in these images we have the flag split into 3 parts, to get the full flag one simply has to concatenate the partial flags in the proper order. 

**Here is the complete flag:**

**picoCTF{tru3_d3t3ct1ve_0r_ju5t_lucky?832b0699}**

Thank you very much for reading!

Cheers,

Gaurish Bahurupi

