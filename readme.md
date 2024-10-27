This repo containg two python files for different search algorithims, a submission for the shield hackathon held on 22/10/2024

File 1: searchInRotatedSortedArray, tackles a challenge where we are required to design an algorithm that efficiently locates a specific target value within an array that ahas been sorted in ascending order and rotated at an unknown pivot point. For this we need to use a binary search algorithm. We start by defining a python function called 'search' with two parameters 'nums' and 'target', nums is the var name of the rotatated ascending ordered list which we will be iterating through to find the target value, 'target' also in the same way is also the user input value that we'll be searching for in the list, these tow parameters are the heart of our algorithm, in the defined function we'll need a loop that goes through all the elements of the list, we'll define two pointer variables, one for for the lest side of the array, one for the right, these pointers give the while loop a range with with to iterate through and find the target, for a binary search algorithm we need to split the list in question into two, we do that by creating midpoint 'mid' by dividing the total length of the list by 2. We start searching for the target at the midpoint index, if the value of the midpoint is the same as the target, then there's no need to continue going through the other elements, if not we continue with the algorithm,(i) we use an if statement to check if the left pointer is less than or equal to the midpoint, if yes we check if the the target is on that side of the list(left side), if the target is there we move the right pointer to midpoint and search through it, if not we move the left pointer to the midpoint and search the other side of the list for the target. If the left pointer is greater than or equal to the midpoint, if yes we check if the target is on the other side of the list(right side), if it is we move the left pointer to the midpoint, if not we move the right pointer to the midpoint to search that side.
These instructions cover all scenarios to ensure we locate the target even if the list itself is rotated at an unknown pivot point. 
The function returns -1 if the target is not found.
We finish of by testing our algorithm by presenting a list to test its functionality. We create a user input function to get the user's input on which target element they would like to find, and finally print the result for the user to see.


