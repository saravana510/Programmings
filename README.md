isBalanced Function->

* isBalanced is a helper function that checks whether a given string is balanced or not.
* It uses a Map (charCount) to count the frequency of each character in the string.
* If there are more or fewer than two different characters, the string is not balanced.
* If there are exactly two different characters, it checks if their frequencies are the same.

getBalancedSubstrings Function->

* getBalancedSubstrings is the main function that finds the longest balanced substrings in the given string.
* It initializes maxLen to 0 and maxSubstrings to an empty array to keep track of the longest balanced substrings.
* It uses nested loops to iterate through all possible substrings in the input string S.
* For each substring, it checks if it is balanced using the isBalanced function and updates maxLen and maxSubstrings 
  accordingly.
* The final result is an array containing the longest balanced substrings.

Example Usage->

* The algorithm is demonstrated using three examples (S1, S2, and S3) to showcase how to use the getBalancedSubstrings function.
