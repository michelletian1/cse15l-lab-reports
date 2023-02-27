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

We wanted to run the test again by running the javac and the java. So we can do key pressed for javac, such as `<up><up><up><enter>` and for java `<up><up><up><up><enter>` and I will give the results as the picture okay for all running. 

## Commit and push the resulting change to your Github account  :
<img width="839" alt="Screenshot 2023-02-26 at 9 40 12 PM" src="https://user-images.githubusercontent.com/82022298/221499555-3abba41a-f0cd-4772-97c5-0f90345a428b.png">

After that we wanted to do git push and commit. `Git push` is to upload local repository content to a remote repository, and `git commit -m "Updated"` is record changes to the repository. So, we do git push first after that press `<up>` and delete the push change to `commit -m "Updated"` meaning we want the new file to be updated. Final step is to do `git push origin main` to update on my github too. 

## All the step from the lab
### Generating SSH Keys for ieng6
1. In your local terminal, run ssh-keygen
2. Keep entering <Enter> until the program shows some text it calles the “randomart image”.
  <img width="896" alt="Screenshot 2023-02-26 at 9 41 38 PM" src="https://user-images.githubusercontent.com/82022298/221501111-49845fe9-23cd-45da-bb7c-7b404dd22d8b.png">
3. Scroll up a bit to where you were creating the SSH key, find the line where it says: Your public key has been saved in: <path to your public SSH key>, copy the path. Make sure you get the public key file, ending in .pub, here, not the private file.
4. From your local computer, run scp <path to your public SSH key> cs15lwi23__@ieng6.ucsd.edu:~/.ssh/authorized_keys


---
## Name : Michelle Tian
## PID : A17183450
## Date : 01/28/2023
