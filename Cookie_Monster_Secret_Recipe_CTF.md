🍪 Cookie Monster Secret Recipe – picoCTF 2025


🔹 Challenge Information
Name: Cookie Monster Secret Recipe
Category: Web Exploitation
Difficulty: Easy
Event: picoCTF 2025
Tags: browser_webshell_solvable
Authors: Brhane Giday and Prince Niyonshuti N.
Solved by: Harsh Patle

<img width="966" height="541" alt="image" src="https://github.com/user-attachments/assets/097b7df3-68e5-4595-a1d7-3d0b44255a3d" />


🔹 Approach / Walkthrough
1. Launch the Instance
After starting the challenge, a web application is provided.

2. Initial Recon
Open the browser’s developer tools (F12) and inspect:
HTML source code
Network traffic
Cookies / Storage tab

3. Finding the Secret
I noticed a suspicious cookie storing a key/flag.
By reading the cookie value and decoding it, I found the hidden recipe.

To decode the cookie, I used Burp Suite. I went to the Decoder tab, pasted my cookie, selected Base64 decoding, and obtained the flag in plaintext.

<img width="1633" height="595" alt="image" src="https://github.com/user-attachments/assets/0b6ece24-f308-4755-abf0-f0ec78a88446" />


🔹 Learnings
How to inspect cookies in a browser.
Web applications may store sensitive data in client-side storage.
Always check developer tools during web exploitation challenges.
