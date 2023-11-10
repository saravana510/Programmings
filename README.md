1. Write a simple application using a recursive function that accepts a value (integer) and returns the fibonacci value at that position in the series.
The application should be performant at scale to handle larger numbers without slowing down exponentially.

Base Case (Step 1):
The function begins by checking if x is less than or equal to 1. If true, it means we have reached the base case, and the function returns x. This is because Fibonacci numbers at positions 0 and 1 are 0 and 1, respectively.

Initialization (Step 2):
Two variables, prev and curr are initialized to 0 and 1, respectively. These variables will be used to keep track of the previous and current Fibonacci numbers during the iteration.

Iterative Calculation (Step 3):
The function enters a loop that iterates from i = 2 to i = n. This loop calculates Fibonacci numbers iteratively, avoiding the need for recursion.

Calculate Next Fibonacci Number (Step 4):
Inside the loop, the next Fibonacci number (curr) is calculated by adding the previous two Fibonacci numbers (prev and curr). A temporary variable (temp) is used to store curr before the update, ensuring correct calculation.

Return Result (Step 5):
After the loop, the function returns the final Fibonacci number at position x, which is stored in the variable curr


2. A string is balanced if it consists of exactly two different characters and both of those characters appear exactly the same number of times. For example: "aabbab" is balanced (both 'a' and 'b' occur three times) but "aabba" is not balanced ('a' occurs three times, 'b' occurs two times). String "aabbcc" is also not balanced (it contains three different letters).A substring of string S is a string that consists of consecutive letters in S. For example: "ompu" is a substring of "computer" but "cmptr" is not.Write a function solution called getBalancedSubstrings(List<String> S) that, given a string S, returns an array of the longest balanced substring of S.Examples:
1. Given S = "cabbacc", the function should return ["abba"] because it is the longest balanced substring.
2. Given S = "abababa", the function should return ["ababab", "bababa"] which are the longest balanced substrings.
3. Given S = "aaaaaaa", the function should return [] since S does not contain a balanced substring.Write an efficient algorithm for the following assumptions:
 - N is an integer within the range [1..100,000];
 - string S is made only of lowercase letters (a−z).

isBalanced Function (Step 1):

* isBalanced is a helper function that checks whether a given string is balanced or not.
* It uses a Map (charCount) to count the frequency of each character in the string.
* If there are more or fewer than two different characters, the string is not balanced.
* If there are exactly two different characters, it checks if their frequencies are the same.

getBalancedSubstrings Function (Step 2):

* getBalancedSubstrings is the main function that finds the longest balanced substrings in the given string.
* It initializes maxLen to 0 and maxSubstrings to an empty array to keep track of the longest balanced substrings.
* It uses nested loops to iterate through all possible substrings in the input string S.
* For each substring, it checks if it is balanced using the isBalanced function and updates maxLen and maxSubstrings 
  accordingly.
* The final result is an array containing the longest balanced substrings.

Example Usage (Step 3):

* The algorithm is demonstrated using three examples (S1, S2, and S3) to showcase how to use the getBalancedSubstrings function.



Note: To run a code individually open any code editor ,For your reference **https://playcode.io/javascript** and copy paste the program which will present in separate folder of fibonacci and stringBalance programs.
