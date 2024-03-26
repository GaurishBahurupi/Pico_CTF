# CTF Walkthrough: Where Are the Robots

## Information

- CTF Name: PicoCTF 2024
- Challenge Name: Where Are the Robots
- Category: Web Exploitation
- Points: 100
- Date: 26 March 2024
- Author: Gaurish Bahurupi

## Challenge Description

Can you find the robots? [https://jupiter.challenges.picoctf.org/problem/36474/](https://jupiter.challenges.picoctf.org/problem/56830/) or [http://jupiter.challenges.picoctf.org:36474](http://jupiter.challenges.picoctf.org:56830)

## Writeup

I figured that this had to do with robots.txt.

First, I just tacked robots.txt to the end of the provided URL, which presented a robots.txt file:
<img width="1440" alt="Screenshot 2024-03-26 at 4 24 12 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/b9b3d4c3-a22e-4372-8cfb-ebe27e19c8a0">


Next, I looked at 477ce.html, because this is a strange and non-standard file. The flag was in there:
<img width="1440" alt="Screenshot 2024-03-26 at 4 24 25 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/b6a50707-2b75-4505-b4cb-5e1f913108da">


FLAG: picoCTF{ca1cu1at1ng_Mach1n3s_477ce}

Challenge Solved. Thanks!
