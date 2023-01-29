#Lab Report Week 3
---

## Servers
<img width="949" alt="Screen Shot 2023-01-28 at 11 42 03 AM" src="https://user-images.githubusercontent.com/82022298/215288189-fc588586-1382-4391-a558-161c7777fbac.png">

The files called StringServer, this is the files that makes the command works for the URL.`The method is public String handleRequest(URI url)`. 

<img width="1512" alt="Screen Shot 2023-01-28 at 11 44 45 AM" src="https://user-images.githubusercontent.com/82022298/215288201-3bc95afd-a90d-4381-a8b9-b8cfa6371bd5.png">

This is the server files, inside we can copy it from lab 2 files. This files related to the terminal and If we do everything right in the StringServer files then terminal will automatically show us to the website that we need to visit and modified. The method that will show us the website is `public class Server`

### The Hello messages 
<img width="707" alt="Screen Shot 2023-01-28 at 12 31 44 PM" src="https://user-images.githubusercontent.com/82022298/215289611-521d83e3-1a8a-40c5-8512-c44f68bbf6ea.png">
<img width="889" alt="Screen Shot 2023-01-28 at 12 32 06 PM" src="https://user-images.githubusercontent.com/82022298/215289613-02e5a46a-32ac-41ab-97f2-cd137b35c38a.png">

From the screen shots above we can see how we can add a string. What are the relevant arguments to those methods, and the values of any relevant fields of the class? The revelevant arguments methods are, making the first string variable empty. After that we create a class or method that the path and functions will be. The method is called `public class Server`. In this method we add a path and if we add the word `add-messages` the path will need more command. 

### The How are you messages
<img width="887" alt="Screen Shot 2023-01-28 at 12 32 35 PM" src="https://user-images.githubusercontent.com/82022298/215289637-676f0da4-016c-4932-bf90-42c6c17a4184.png">
<img width="910" alt="Screen Shot 2023-01-28 at 12 32 50 PM" src="https://user-images.githubusercontent.com/82022298/215289640-11b7e1dd-72ff-43c5-9621-bcf8afaa69c7.png">

Another relevant argument to reach our desire output, we need to specify query. To get a query we need to add ? after the `add-messages` path after we need to add =. = means we ready to give a string input to our query. Now, first we add Hello as the question said so. After we add the message a sentence of `added messages` will appear. If we go back to our original page then we can see the word Hello. Now, we need the How are you word to be in a new row. We do that by adding a command 20 where we concate old messages with new messages and adding \n (this mean move to another new row). 

How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why. The first that change is the URL itself because we request a specific path and query where we also specified what is the output we wanted to show on our page. If we called the add-messages functions the URL itself already changed from [localho](http://localhost:8500/) to http://localhost:8500/add-messages. Same goes for the URL if we called the query functions where the input also changed everytime we wanted to try different strings. 

 
## Bugs 

### Setup
<img width="1027" alt="Screen Shot 2023-01-28 at 5 40 17 PM" src="https://user-images.githubusercontent.com/82022298/215299753-0549d606-c04b-4a98-9dc8-a904ae7b0914.png">

We see this error because there is no JUnit because the classpath is different from windows to mac. 

### ArrayTest.java
the code :

 public class ArrayTests {
    @Test 
    public void testReverseInPlace() {
      int[] input1 = { 1,5,7 };
      ArrayExamples.reverseInPlace(input1);
      assertArrayEquals(new int[]{ 7,5,1}, input1);`
      
    }
    
@Test
public void testReversed() {
  int[] input3 = { 1, 5, 7};
  assertArrayEquals(new int[]{ 7,5,1}, ArrayExamples.reversed(input3));
}
}

So from the code above we have a variable call Input1 where it contains array of numbers. Here, I input 1,5,7 as my numbers in my array. now we used a functions called reverseInPlace(Input1) meaning that in the assertArrayEquals we filled the new array as our old array but in the reverse order. Here, we don't notice any failure-inducing input. Same goes for the testReversed the idea is the same put numbers in array for variables input3 and we reversed the array numbers. Here I don't notice any failure-inducing input.

## Failure - Inducing input :
### ArrayExamples.java
the code :

  `static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }`
  
   `static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }`

From the code above we can see where the failure-induce input came to play. For the first methods the reverseInPlace we can see the failure because if the array only contains one number then the code works because it swap by nothing but its own number. However, if you put 2 numbers in the array it will cause an error because only one of them did the swapping while one of them stays in the same index. We want to be able to swap places for the numbers we wanted to swap.  For the reversed and averagewithoutlowest it is exactly the same failure as the reversedInPlace.

## An input that doesn’t induce a failure :
### ArrayExamples.java
reverseInPlace code :
  `static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) { 
      int num = arr[i];
      arr[i] = arr[arr.length - i - 1]; 
      arr[arr.length - i - 1] = num;
    }
  } `
  
reversed :
  `static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[i];
    }
    for (int i = 0; i < arr.length; i += 1){
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }`
  
testaverageWithoutLowest : 
  `@Test
  public void testaverageWithoutLowest() {
    double[] input5 = {1, 5, 7, 3, 7 };
    assertEquals((double)3, ArrayExamples.averageWithoutLowest(input5), 0.001);
  }`

## Symptomps
<img width="1204" alt="Screen Shot 2023-01-28 at 9 19 07 PM" src="https://user-images.githubusercontent.com/82022298/215306638-88512558-200d-4646-90e5-525a4acd23d1.png">
<img width="1113" alt="Screen Shot 2023-01-28 at 9 20 38 PM" src="https://user-images.githubusercontent.com/82022298/215306672-afd169e2-5df9-4182-9842-cb0ee2a7ef2f.png">


## Code before:
### ArrayExamples.java
  
  `static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = arr[arr.length - i - 1];
    }
  }`
  
   `static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }`
  
## Code After :
reverseInPlace code :
  `static void reverseInPlace(int[] arr) {
    for(int i = 0; i < arr.length/2; i += 1) { 
      int num = arr[i];
      arr[i] = arr[arr.length - i - 1]; 
      arr[arr.length - i - 1] = num;
    }
  } `
  
reversed :
  `static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[i];
    }
    for (int i = 0; i < arr.length; i += 1){
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }`





---
## Name : Michelle Tian
## PID : A17183450
## Date : 01/28/2023
