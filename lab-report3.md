#Lab Report Week 3
---

## Grep Command
For this lab I have chosen the "grep" command to explain.
**What is grep command?** Grep is *Global Regular Expression Print* We usually use this command when we want to search up text from a file, we also search for a pattern of characters within our files and display them. If you open up the terminal sections you can type `man find` this command will show you manual or guidelines on how to use grep command. 


1. grep -r "string" directory :
<img width="1447" alt="Screen Shot 2023-02-10 at 2 56 54 PM" src="https://user-images.githubusercontent.com/82022298/218287906-cee9ef12-a843-4210-8215-f8bca7eb5a29.png">

What does -r do? Recursively search subdirectories listed (i.e., force grep to behave as rgrep). In the code I'm doing grep -r "believed" written_2/ meaning I want grab all the files containing the words believed withing the directory of written_2/. After that I want to show you the word "believed" together with the text.

* grep -r -l "string" directory :
<img width="1001" alt="Screen Shot 2023-02-10 at 2 57 32 PM" src="https://user-images.githubusercontent.com/82022298/218287989-1bb27af2-596f-4e56-af2d-f4ffbba40209.png">

So, above we learned what is -r means and how do we used it. What is -l? Only the names of files containing selected lines are written to standard output.  grep will only search a file until a match has been found, making searches potentially less expensive. Pathnames are listed once per file searched. If the standard input is searched, the string “(standard input)” is written unless a --label is specified. So, on the code grep -r -l "believed" written_2/ will show instead of the text it will show the directories on which the files contain the word "believed".

2. grep -c  : 
<img width="920" alt="Screen Shot 2023-02-10 at 2 59 27 PM" src="https://user-images.githubusercontent.com/82022298/218287531-4d5ae38e-6c0a-4d72-b4d3-811bc295ef88.png">
What does -c do? It only a count of selected lines is written to standard output. So, in the code I'm doing grep -c "believed" written_2/... meaning, I want to grep the words believe in the written_2/ specific directories. After that the -c will count how many believed words contain in the text files. So, here in the files of Bali-WhereToGo.txt, the text contains 7 words of believed.

* <img width="861" alt="Screen Shot 2023-02-12 at 12 14 33 PM" src="https://user-images.githubusercontent.com/82022298/218334796-d5eb77e4-3b62-40db-aaa2-6c63e7326ff1.png">

Also, when we want to search up the word it

## grep "string" directory :
<img width="1044" alt="Screen Shot 2023-02-10 at 3 04 43 PM" src="https://user-images.githubusercontent.com/82022298/218288000-7955c1bc-c547-45ef-b2e6-54b3e5c00849.png">

grep "string" directory usually used if we want to know if the specific directory contains the word that we wanted or not. As we can see I put the word "insanity" as the word that I wanted to search 

## grep -v "string" directory :
<img width="1464" alt="Screen Shot 2023-02-10 at 3 07 25 PM" src="https://user-images.githubusercontent.com/82022298/218288028-a19a5018-d1e6-4950-9bcc-3e081b1ee385.png">



---
## Name : Michelle Tian
## PID : A17183450
## Date : 01/28/2023
