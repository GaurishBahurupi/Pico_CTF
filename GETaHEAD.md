# CTF Walkthrough: GET aHEAD

## Information

- CTF Name: PicoCTF
- CTF Challenge: GET aHEAD
- Challenge Category: Web Exploitation
- Challenge Points: 20
- PicoCTF 2024

## Challenge Description

Find the flag being held on this server to get ahead of the competition [http://mercury.picoctf.net:21939/](http://mercury.picoctf.net:21939/).

Access the given URL in a browser and capture the request/response using the Burp Suite tool.

We can notice only 2 buttons present in the application which changes the color of the page on click. Click on both buttons and analyze all captured traffic till now in the tool. However, nothing looks interesting.

The challenge name, i.e., “Get aHEAD,” seems to be a hint as HEAD is one of the known HTTP methods which we can try in any of the captured requests. Change the method from GET to HEAD and generate a response.

It can be noticed that the Flag value is revealed in the response.

## Writeup

1. Access the provided URL [http://mercury.picoctf.net:21939/](http://mercury.picoctf.net:21939/) in a browser.
<img width="1440" alt="Screenshot 2024-03-26 at 2 32 17 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/8a41eb6b-c013-4f24-b61e-c34512b1f173">

2. Capture the request/response using Burp Suite.
<img width="1440" alt="Screenshot 2024-03-26 at 2 35 37 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/bf0a77a7-0fd8-476d-a9e8-44b6b33bd24f">

3. Click on both buttons on the page and analyze the captured traffic.
4. Change the HTTP method from GET to HEAD in any captured request.
5. Generate the response and observe the result.
6. The Flag value will be revealed in the response.
<img width="1440" alt="Screenshot 2024-03-26 at 2 30 27 PM" src="https://github.com/gaurish303/Pico_CTF/assets/139263378/c61fff8a-e948-4736-acfd-fc471891ad11">


**FLAG:** You need to find your (changes frequently).

Challenge Solved. Thanks..
