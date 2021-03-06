# Task_4 2019
Task 4 : Circular Double Linked List

# DEADLINE = MARCH 4TH, 2019 - 23:59

## Reading Material
* [git cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf)
* [markdown cheat sheet](https://enterprise.github.com/downloads/en/markdown-cheatsheet.pdf)

## Workflow
1. FORK this repositori ASD_Task_4 to your GitHub account
2. CLONE ASD_Task_4 repository from YOUR OWN ACCOUNT
3. open and modify codes in *.cpp and *.h files inside project ASD_Task_4
4. write your code inside the provided space in each functions/procedures 
5. COMMIT and PUSH your project to your account
6. create a Pull Request

Introduction to Double Circular Linked List  <br>
Create a music player application to implement the double circular linked list data structure

## [IMPORTANT] library integration
1. on Code::Blocks, go into menu project->Build Option
2. go to Linker Settings tab
3. click `Add` to add new lib function
4. type `winmm`
5. click OK

## list.h
modify the elemenList and List structure to implement Double Circular linked list
* use only **one head**
	
## list.cpp
modify each function to fit the data structure
* `createList`
* `allocate`, `deallocate`
* `insertFirst`, `insertLast`, `insertAfter`
* `deleteFirst`, `deleteLast`, `deleteAfter`
* `findElmByID`, `findElmByName`<br>
to implement Double Circular Linked List mechanism
	
## player.cpp
<i>these function are already defined:
* `int randomInt(int  max_int);` <br>function to produce random integer<br> 
* `void printInfo(List L);` <br>function to print music list inserted to List L<br>
* `void playMusic(address P);` <br>function to play current music pointed by P<br> 
</i>
TODO : 
create function according to the header defined in player.h
  
* function to play the music list from the first music and repeat the list n times  <br>`void playRepeat(List &, int n);` <br>
  
* function to delete any music defined by its ID<br>
  ```void deleteMusicByID(List &L, infotype x);```

* function to shuffle the order of the music list<br> `void shuffleList(List &);`<br>simple logic example: <br> 

```
   repeat n times
      P <- first
      x = randomInt
      for i to x, 
          move P to next element
      delete after P
      insert first P
   end repeat
  ```
  <br>  you can define another mechanism to shuffle the order
  
		
## main.cpp
* modify the main menu progam
* run the application
	
