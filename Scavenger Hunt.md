<img width="961" height="441" alt="image" src="https://github.com/user-attachments/assets/edb3aafb-1994-4eee-b903-1572d36e9a51" />



<img width="1911" height="381" alt="image" src="https://github.com/user-attachments/assets/d4ff13a0-bb59-498c-a873-e3517e2c4707" />


Website is written in HTML but when I click in What it gives me information and got the hint.


<img width="309" height="161" alt="image" src="https://github.com/user-attachments/assets/5681986c-7ec1-45ac-9c09-798447eeb2bc" />



Open Inspect Element and here’s my first part of the flag. Wrote it down on my notepad just in case I find another set.



<img width="891" height="344" alt="image" src="https://github.com/user-attachments/assets/6322cfb7-ad67-429b-b437-c47001f526da" />


and then i went by check sourcecode of every file, on CSS another piece of the flag is in the last


<img width="1161" height="120" alt="image" src="https://github.com/user-attachments/assets/56ca245a-f452-4844-959e-77022db650dd" />


went to JS and the comment didn’t provide a piece of flag but it gives me a hint of question:


<img width="658" height="74" alt="image" src="https://github.com/user-attachments/assets/822a5b94-73b3-4e9f-bfce-029eac20c70e" />


So typically in order to prevent Google from indexing your website we usually use robots.txt. It is a file used by website to tell search engines of which can be index or cannot be index. We need to specify the path to robots.txt

On the URL just add /robots.txt then it will redirect you to this page:


<img width="1013" height="207" alt="image" src="https://github.com/user-attachments/assets/54d1af77-a79b-4c71-92d2-2e7211439aea" />


There’s the part 3 of the flag the website tells me that it has an apache server technically apache server has some hidden files like /.htaccess /.htpasswd and other hidden files. I pivot on the /.htaccess and that’s where I got the part 4

<img width="595" height="55" alt="image" src="https://github.com/user-attachments/assets/3acaf98f-ed46-4d1c-b930-d633ad21aa14" />


Then another hint where it says “I love making websites on my Mac, I can store a lot of information there.”

It is referring to MAC OS proprietary file called DS_Store that holds attributes/meta-data about the folder it resides in. So specifying the path as /.DS_Store then the last part of the flag is revealed


<img width="467" height="49" alt="image" src="https://github.com/user-attachments/assets/89d2a8c8-9e2a-40de-aadc-f92cbf1ff72d" />


And we gotttttttttttttttt out flag....

# picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_35844447}

