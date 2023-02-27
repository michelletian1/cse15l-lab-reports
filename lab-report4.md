#Lab Report 4
---

## Connecting to remote server
<img width="828" alt="Screen Shot 2023-02-25 at 9 07 05 PM" src="https://user-images.githubusercontent.com/82022298/221484420-1559cfa8-2bea-4ab1-8a39-a1bbb8fe2948.png">

Here I access my ssh `cs15lwi23abb@ieng6.ucsd.edu` remote server. I don't have to enter key anymore because I have generate ssh keys for ieng6 by using ssh-keygen and then running scp `<our public key>` from ssh-keygen. After you finish setting that up exit and run it again. Here, keys pressed :`<up><up>` to get ssh command line and then `<enter>`


## Clone your fork of the repository from your Github account
<img width="693" alt="Screen Shot 2023-02-25 at 9 07 38 PM" src="https://user-images.githubusercontent.com/82022298/221492925-fb58f037-7b7e-4366-98b5-a6ae4d3906dd.png">

So here I didn't do any key pressing as I needed to write the `git clone`. I clone the github using the github ssh by setting up ssh keys for Github. First, same thing with the first step, ssh-keygen and then we use cat to show full ssh keys. Then we copy it from the terminal to our github ssh and keys sections on the github. After we set that up we do `git clone git@github.com:michelletian1/lab7.git` it will clone the folder to our remoter server. Key pressed `<enter>`

## Run the tests, demonstrating that they fail:
<img width="870" alt="Screen Shot 2023-02-26 at 12 03 47 AM" src="https://user-images.githubusercontent.com/82022298/221495056-69334911-8800-46dc-9cb6-c00dc29ec018.png">
<img width="1210" alt="Screen Shot 2023-02-26 at 12 07 28 AM" src="https://user-images.githubusercontent.com/82022298/221495070-e580aef7-7c34-4983-aa63-c507971883c6.png">

In this step, I first cd to lab7 first then I pressed `<up>` key because I already wrote it so there exist a history to get the first javac running and then I pressed another `<up>` key because I wanted to change the back of the code while have the front the same except the javac to java and then I pressed `<enter>`.

## Edit the code file to fix the failing test: 
<img width="589" alt="Screenshot 2023-02-26 at 9 37 48 PM" src="https://user-images.githubusercontent.com/82022298/221496590-006bc13b-199b-4898-b6f2-4bd8c8f47706.png">
<img width="1248" alt="Screenshot 2023-02-26 at 9 37 57 PM" src="https://user-images.githubusercontent.com/82022298/221496606-c0a9a15f-ce87-4fef-8d57-a74a7fcfcfcf.png">

We can fix the mistake with 2 options doing nano and doing git push and commit. In this case, doing nano is much more simpler than doing so many git push and commit within the file. We first have to find the mistake and in which file. I already know the mistake, it is in the file of ListExamples.java. To fix it I simply do `nano ListExamples.java` after that I scroll down to find the mistake that I wanted to fix. With second image provided I fixed the last while loop, changing from `index1 += 1 to index2 += 1` after that pressed `control + o` to save the changes and then `control + x` to exit.

## Run the tests, demonstrating that they now succeed:
<img width="1145" alt="Screenshot 2023-02-26 at 9 39 01 PM" src="https://user-images.githubusercontent.com/82022298/221498275-72fced99-436a-4e9a-86b9-1bb137bc2336.png">

We wanted to run the test again

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
