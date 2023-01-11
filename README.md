# SoEinH

This program takes an input of a number, n, and uses it to find the prime numbers up to n using the Sieve of Eratosthenes algorithm. The algorithm starts with a list of all integers from 2 to n, and iteratively removes the multiples of each prime number found, until no more multiples are left in the list.

The program starts by defining a function sieve that takes an input n, and returns a list of prime numbers up to n using the Sieve of Eratosthenes algorithm. This function has been implemented using recursion, it starts calling the internal sieve' function, passing as a parameter a list of integers from 2 to n.

The sieve' function receives an input list, if the list is empty it returns an empty list, if not, it selects the first element of the list and remove all elements of the list that are multiple of that element and then it calls itself again with the filtered list until it's empty, all the prime numbers will be returned.

In the main function, it prompts the user to enter a number and then it calls the sieve function passing that number as an argument, and finally prints the result on the screen.

It's important to note that this is a very simple implementation that uses the filter function from Data.List which is not an efficient way of doing this algorithm since it has a time complexity of O(n^2)
