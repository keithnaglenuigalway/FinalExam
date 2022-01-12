## Week 6

You have been asked to sort a series of timestamps into chronological order from earliest to latest. The timestamps are supplied in a text file as strings in the following format: “dd/mm/yyyy-hh:mm:ss” e.g.  29/11/2021-15:33:56

### Question 1
Write a program which takes the name of the text file as input and produces an output file with the sorted timestamps.
Your program should:
       
   1. Prompt the user for the names of the input and output files and store for later use. If the input file does not exist, display an error message and re-prompt.
       
   2. Read in the series of strings from the text file and store these in an array of strings.
       
   3. Sort the array alphabetically using the bubble sort algorithm.
       
   4. Write the sorted array to the output file and comment on the results.


### Question 2
Develop a special function to convert the timestamps into something that can be sorted from earliest to latest based on a numerical value rather than alphabetical. Re-write your program in a new file with the same functionality as above, along with the following enhancements:

1. The array of strings should be allocated dynamically to minimise the amount of memory used.
2. Create a function called timeStampToSeconds() that converts a timestamp string to a long int, which represents the number of seconds elapsed since 01/01/2000 00:00:00.

   Your code will need to check that each character is a valid number between 0 and 9, ignoring formatting characters ('/', ' ', ':', '-') and convert the characters to their equivalent integers before being used to calculate the number of seconds elapsed since the above starting point.

3. Sort the string array using the timeStampToSeconds() function and any suitable sort algorithm. Write the sorted array to the output file and compare with the output file from question 1. Comment on the results.
4. Loop through the array and find timestamps from the year 2016.
5. Display on screen a list of only those timestamps that come from the year 2016.

Note: For the purposes of this assignment the number of days per year can be taken as 365.25 with 31,557,600 seconds per year.
