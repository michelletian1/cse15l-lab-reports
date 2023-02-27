#Lab Report 4
---

## Connecting to remote server
<img width="828" alt="Screen Shot 2023-02-25 at 9 07 05 PM" src="https://user-images.githubusercontent.com/82022298/221484420-1559cfa8-2bea-4ab1-8a39-a1bbb8fe2948.png">
Here I access my ssh `cs15lwi23abb@ieng6.ucsd.edu` remote server. I don't have to enter key anymore because I have generate ssh keys for ieng6 by using ssh-keygen and then running scp \<our public key\> from ssh-keygen. After you finish setting that up exit and run it again. Here I user \<up\> to get ssh command line. 


## grep -r "string" file :
<img width="1447" alt="Screen Shot 2023-02-10 at 2 56 54 PM" src="https://user-images.githubusercontent.com/82022298/218287906-cee9ef12-a843-4210-8215-f8bca7eb5a29.png">

What does `-r` do? Recursively search subdirectories listed (i.e., force grep to behave as rgrep). In the code I'm doing `grep -r "believed" written_2/` meaning I want grab all the files containing the words believed withing the directory of written_2/. After that I want to show you the word "believed" together with the text.

### Example 2 grep -r -l "string" d :
<img width="1001" alt="Screen Shot 2023-02-10 at 2 57 32 PM" src="https://user-images.githubusercontent.com/82022298/218287989-1bb27af2-596f-4e56-af2d-f4ffbba40209.png">

So, above we learned what is `-r `means and how do we used it. What is `-l`? Only the names of files containing selected lines are written to standard output.  grep will only search a file until a match has been found, making searches potentially less expensive. Pathnames are listed once per file searched. If the standard input is searched, the string “(standard input)” is written unless a --label is specified. So, on the code `grep -r -l "believed" written_2/` will show instead of the text it will show the directories on which the files contain the word "believed".

## grep -c  "believed" file: 
<img width="920" alt="Screen Shot 2023-02-10 at 2 59 27 PM" src="https://user-images.githubusercontent.com/82022298/218287531-4d5ae38e-6c0a-4d72-b4d3-811bc295ef88.png">
What does `-c` do? It only a count of selected lines is written to standard output. So, in the code I'm doing `grep -c "believed" written_2/...` meaning, I want to grep the words believe in the written_2/ specific directories. After that the -c will count how many believed words contain in the text files. So, here in the files of Bali-WhereToGo.txt, the text contains 7 words of believed.

### Example 2 grep -c "tequila" file:
<img width="861" alt="Screen Shot 2023-02-12 at 12 14 33 PM" src="https://user-images.githubusercontent.com/82022298/218334796-d5eb77e4-3b62-40db-aaa2-6c63e7326ff1.png">

Also, when we search the word try to use grep string first and then you count the words. Please note that this is case sensitive, if you accidentally wrote it in caps lock, it will try count that words with caps lock. 

## grep "string" file :
<img width="1044" alt="Screen Shot 2023-02-10 at 3 04 43 PM" src="https://user-images.githubusercontent.com/82022298/218288000-7955c1bc-c547-45ef-b2e6-54b3e5c00849.png">

`grep "string" file` usually used if we want to know if the specific directory contains the word that we wanted or not. As we can see I put the word "insanity" as the word that I wanted to search in the file directory. Then I specify the diretory showing that the txt files do contain the word we are looking for.

### Example 2 
<img width="629" alt="Screen Shot 2023-02-12 at 8 42 54 PM" src="https://user-images.githubusercontent.com/82022298/218372385-0b69783b-5c54-41ed-bf85-4471c097ab71.png">

In this example I searched the word "Columbus" please note this is case sensitve. As we can see we can't grab or display that there's a word Columbus contain in this file. Hence, it return nothing.

## grep -i "string" file :
<img width="696" alt="Screen Shot 2023-02-12 at 9 52 05 PM" src="https://user-images.githubusercontent.com/82022298/218381134-76b56a9d-9e0b-4ac3-8ef2-2cc3f506c8f9.png">

What does `-i` do? Ignores, case for matching. So, above I tried to search word "this" in the text file. But, in the code instead of "this" I wrote "This", the command -i makes it ignore the case sensitive and just search for the desire word and display the text with the desire word displayed in red. 

### Example 2
<img width="664" alt="Screen Shot 2023-02-12 at 9 57 32 PM" src="https://user-images.githubusercontent.com/82022298/218381923-84bd77ca-523f-4dc4-b75b-7bb4f46579a2.png">

<img width="654" alt="Screen Shot 2023-02-12 at 9 57 38 PM" src="https://user-images.githubusercontent.com/82022298/218381960-3ce9b434-9b91-41e3-a211-3ed8a424964f.png">

So, the in the command I used `grep -r -i "Language" written_2/` meaning that I want to grep every single file text in the directory. And then I want to ignore the capital letter or case sensitive for the language. Hence, it will search the word "Language" in every single file in the written_2/ as you can see I provided two screenshots where one you can match the word "Language" even though it is lower case and second "Language" with upper case. 

---
## Name : Michelle Tian
## PID : A17183450
## Date : 01/28/2023
