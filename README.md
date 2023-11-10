1. Write a simple application using a recursive function that accepts a value (integer) and returns the fibonacci value at that position in the series.
The application should be performant at scale to handle larger numbers without slowing down exponentially.




2. A string is balanced if it consists of exactly two different characters and both of those characters appear exactly the same number of times. For example: "aabbab" is balanced (both 'a' and 'b' occur three times) but "aabba" is not balanced ('a' occurs three times, 'b' occurs two times). String "aabbcc" is also not balanced (it contains three different letters).A substring of string S is a string that consists of consecutive letters in S. For example: "ompu" is a substring of "computer" but "cmptr" is not.Write a function solution called getBalancedSubstrings(List<String> S) that, given a string S, returns an array of the longest balanced substring of S.Examples:
1. Given S = "cabbacc", the function should return ["abba"] because it is the longest balanced substring.
2. Given S = "abababa", the function should return ["ababab", "bababa"] which are the longest balanced substrings.
3. Given S = "aaaaaaa", the function should return [] since S does not contain a balanced substring.Write an efficient algorithm for the following assumptions:
 - N is an integer within the range [1..100,000];
 - string S is made only of lowercase letters (a−z).

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
