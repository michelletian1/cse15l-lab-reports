#Lab Report 5
---

## The grading script

We first fork the Github repository called (https://github.com/ucsd-cse15l-w23/list-examples-grader)

This is the originial file without any additional grading command :
<img width="1149" alt="Screenshot 2023-03-12 at 1 09 17 PM" src="https://user-images.githubusercontent.com/82022298/224570629-871769cb-e39d-4582-bea7-2c81146fe1e1.png"> 

We want to display if we can find the ListExamples.java file using echo because every grading script will be contain insde the ListExamples.java. Then If we are able to find the file, we will continue with the grading process. We have learned in lab6 to construct the grading script that includes if condition where the parameters is -e (enables the interpretation of the following backslash escapes). I also incorporate tail functions that will be useful printing the last N number of data of the given input. Below I will provided the second edition of the grading script before finalizing

### Second edtion :
<img width="1133" alt="Screenshot 2023-03-12 at 1 26 08 PM" src="https://user-images.githubusercontent.com/82022298/224572209-63765202-2406-432b-a3fc-d619bbcb9cab.png">

The pictures presents all of the command I have mentioned above, all though the code is running it is not quite right as I haven't wrote the part where we can count the mistakes and overall grades for the Files we're about to grade. In lab 8, I have discovered how to write the grading script by discussing with my teammates. In the picture below is the finalized versions of grading script.

### Third edition :
<img width="934" alt="Screenshot 2023-03-12 at 1 15 20 PM" src="https://user-images.githubusercontent.com/82022298/224572415-cea5bef7-8ee3-41f8-922f-b53e34374a9f.png">
<img width="1117" alt="Screenshot 2023-03-12 at 1 44 03 PM" src="https://user-images.githubusercontent.com/82022298/224572539-d2a85159-6cef-4584-a97b-cfe322e7287b.png">

As it can be observed above, first I searched the file of ListExamples.java from the github repo that the professor gave. If we are able to find the file, we proceed with grading. Second, I want to clone my code to the students' directory because I want to be able to search up which part they got wrong and right. After we can detect the errors we can produced an output, which is the student's score. 

## Running some Grading:

If we want to run the grading script we can first open the github repo that contain the ListExamples.java then we copy the URL of the github repo. In our terminal we can start by writing `bash grade.sh (GITHUB REPO URL)` 

### lab-methods-lab3
<img width="1053" alt="Screenshot 2023-03-12 at 1 56 08 PM" src="https://user-images.githubusercontent.com/82022298/224573166-69f26daf-a3a1-4397-a8ec-d72324f8a0ef.png">
<img width="650" alt="Screenshot 2023-03-12 at 1 56 13 PM" src="https://user-images.githubusercontent.com/82022298/224573175-59570fbd-4c31-48a2-b4d8-ab93aabcb988.png">

On the grading above, I first implement the `bash grade.sh(https://github.com/ucsd-cse15l-f22/list-methods-lab3)`. Then it will automatically run itself to count the grades. 

### list-methods-compile-error
<img width="1105" alt="Screenshot 2023-03-12 at 2 00 28 PM" src="https://user-images.githubusercontent.com/82022298/224573406-55dea1f1-fa6c-41ac-ab83-398c69e7607b.png">

The final score is 0/2

### list-methods-corrected
<img width="1086" alt="Screenshot 2023-03-12 at 2 04 22 PM" src="https://user-images.githubusercontent.com/82022298/224573635-c8c347ff-7a7a-4b43-a5e5-9938b6903ab9.png">

Here we can see the final score is 2/2 

---
## Name : Michelle Tian
## PID : A17183450
## Date : 03/11/2023
