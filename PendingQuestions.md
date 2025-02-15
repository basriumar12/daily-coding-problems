## Problem-19


> This problem was asked by Facebook.

A builder is looking to build a row of N houses that can be of K different
colors. He has a goal of minimizing cost while ensuring that no two neighboring
houses are of the same color.

Given an N by K matrix where the nth row and kth column represents the cost to
build the nthhouse with kth color, return the minimum cost which achieves this
goal.

## Problem-25


> This problem was asked by Facebook.

Implement regular expression matching with the following special characters:

 * . (period) which matches any single character
 * * (asterisk) which matches zero or more of the preceding element

That is, implement a function that takes in a string and a valid regular
expression and returns whether or not the string matches the regular expression.

For example, given the regular expression "ra." and the string "ray", your
function should return true. The same regular expression on the string "raymond"
should return false.

Given the regular expression ".*at" and the string "chat", your function should
return true. The same regular expression on the string "chats" should return
false.

## Problem-34


> This problem was asked by Quora.

Given a string, find the palindrome that can be made by inserting the fewest
number of characters as possible anywhere in the word. If there is more than one
palindrome of minimum length that can be made, return the lexicographically
earliest one (the first one alphabetically).

For example, given the string "race", you should return "ecarace", since we can
add three letters to it (which is the smallest amount to make a palindrome).
There are seven other palindromes that can be made from "race" by adding three
letters, but "ecarace" comes first alphabetically.

As another example, given the string "google", you should return "elgoogle".

## Problem-54


> This problem was asked by Dropbox.

Sudoku is a puzzle where you're given a partially-filled 9 by 9 grid with
digits. The objective is to fill the grid with the constraint that every row,
column, and box (3 by 3 subgrid) must contain all of the digits from 1 to 9.

Implement an efficient sudoku solver.

## Problem-56


> This problem was asked by Google.

Given an undirected graph represented as an adjacency matrix and an integer k,
write a function to determine whether each vertex in the graph can be colored
such that no two adjacent vertices share the same color using at most k colors.

## Problem-62


> This problem was asked by Facebook.

There is an N by M matrix of zeroes. Given N and M, write a function to count
the number of ways of starting at the top-left corner and getting to the
bottom-right corner. You can only move right or down.

For example, given a 2 by 2 matrix, you should return 2, since there are two
ways to get to the bottom-right:

 * Right, then down
 * Down, then right

Given a 5 by 5 matrix, there are 70 ways to get to the bottom-right.

## Problem-63


> This problem was asked by Microsoft.

Given a 2D matrix of characters and a target word, write a function that returns
whether the word can be found in the matrix by going left-to-right, or
up-to-down.

For example, given the following matrix:

[['F', 'A', 'C', 'I'],
 ['O', 'B', 'Q', 'P'],
 ['A', 'N', 'O', 'B'],
 ['M', 'A', 'S', 'S']]


and the target word 'FOAM', you should return true, since it's the leftmost
column. Similarly, given the target word 'MASS', you should return true, since
it's the last row.

## Problem-64


> This problem was asked by Google.

A knight's tour is a sequence of moves by a knight on a chessboard such that all
squares are visited once.

Given N, write a function to return the number of knight's tours on an N by N
chessboard.

## Problem-68


> This problem was asked by Google.

On our special chessboard, two bishops attack each other if they share the same
diagonal. This includes bishops that have another bishop located between them,
i.e. bishops can attack through pieces.

You are given N bishops, represented as (row, column) tuples on a M by M
chessboard. Write a function to count the number of pairs of bishops that attack
each other. The ordering of the pair doesn't matter: (1, 2) is considered the
same as (2, 1).

For example, given M = 5 and the list of bishops:

 * (0, 0)
 * (1, 2)
 * (2, 2)
 * (4, 0)

The board would look like this:

[b 0 0 0 0]
[0 0 b 0 0]
[0 0 b 0 0]
[0 0 0 0 0]
[b 0 0 0 0]


You should return 2, since bishops 1 and 3 attack each other, as well as bishops
3 and 4.

## Problem-72


> This problem was asked by Google.

In a directed graph, each node is assigned an uppercase letter. We define a
path's value as the number of most frequently-occurring letter along that path.
For example, if a path in the graph goes through "ABACA", the value of the path
is 3, since there are 3 occurrences of 'A' on the path.

Given a graph with n nodes and m directed edges, return the largest value path
of the graph. If the largest value is infinite, then return null.

The graph is represented with a string and an edge list. The i-th character
represents the uppercase letter of the i-th node. Each tuple in the edge list 
(i, j) means there is a directed edge from the i-th node to the j-th node.
Self-edges are possible, as well as multi-edges.

For example, the following input graph:

ABACA


[(0, 1),
 (0, 2),
 (2, 3),
 (3, 4)]


Would have maximum value 3 using the path of vertices [0, 2, 3, 4], (A, A, C, A)
.

The following input graph:

A


[(0, 0)]


Should return null, since we have an infinite loop.

## Problem-75


> This problem was asked by Microsoft.

Given an array of numbers, find the length of the longest increasing subsequence
in the array. The subsequence does not necessarily have to be contiguous.

For example, given the array [0, 8, 4, 12, 2, 10, 6, 14, 1, 9, 5, 13, 3, 11, 7,
15], the longest increasing subsequence has length 6: it is 0, 2, 6, 9, 11, 15.

## Problem-76


> This problem was asked by Google.

You are given an N by M 2D matrix of lowercase letters. Determine the minimum
number of columns that can be removed to ensure that each row is ordered from
top to bottom lexicographically. That is, the letter at each column is
lexicographically later as you go down each row. It does not matter whether each
row itself is ordered lexicographically.

For example, given the following table:

cba
daf
ghi


This is not ordered because of the a in the center. We can remove the second
column to make it ordered:

ca
df
gi


So your function should return 1, since we only needed to remove 1 column.

As another example, given the following table:

abcdef


Your function should return 0, since the rows are already ordered (there's only
one row).

As another example, given the following table:

zyx
wvu
tsr


Your function should return 3, since we would need to remove all the columns to
order it.

## Problem-87


> This problem was asked by Uber.

A rule looks like this:

A NE B

This means this means point A is located northeast of point B.

A SW C

means that point A is southwest of C.

Given a list of rules, check if the sum of the rules validate. For example:

A N B
B NE C
C N A


does not validate, since A cannot be both north and south of C.

A NW B
A N B


is considered valid.

## Problem-93


> This problem was asked by Apple.

Given a tree, find the largest tree/subtree that is a BST.

Given a tree, return the size of the largest tree/subtree that is a BST.

## Problem-96


> This problem was asked by Microsoft.

Given a number in the form of a list of digits, return all possible
permutations.

For example, given [1,2,3], return 
[[1,2,3],[1,3,2],[2,1,3],[2,3,1],[3,1,2],[3,2,1]].

## Problem-98


> This problem was asked by Coursera.

Given a 2D board of characters and a word, find if the word exists in the grid.

The word can be constructed from letters of sequentially adjacent cell, where
"adjacent" cells are those horizontally or vertically neighboring. The same
letter cell may not be used more than once.

For example, given the following board:

[
  ['A','B','C','E'],
  ['S','F','C','S'],
  ['A','D','E','E']
]


exists(board, "ABCCED") returns true,exists(board, "SEE") returns true,
exists(board, "ABCB") returns false.

## Problem-106


> This problem was asked by Pinterest.

Given an integer list where each number represents the number of hops you can
make, determine whether you can reach to the last index starting at index 0.

For example, [2, 0, 1, 0] returns true while [1, 1, 0, 1] returns false.

## Problem-122


> This question was asked by Zillow.

You are given a 2-d matrix where each cell represents number of coins in that
cell. Assuming we start at matrix[0][0], and can only move right or down, find
the maximum number of coins you can collect by the bottom right corner.

For example, in this matrix

0 3 1 1
2 0 0 4
1 5 3 1


The most we can collect is 0 + 2 + 1 + 5 + 3 + 1 = 12 coins.

## Problem-130


> This problem was asked by Facebook.

Given an array of numbers representing the stock prices of a company in
chronological order and an integer k, return the maximum profit you can make
from k buys and sells. You must buy the stock before you can sell it, and you
must sell the stock before you can buy it again.

For example, given k = 2 and the array [5, 2, 4, 0, 1], you should return 3.

## Problem-132


> This question was asked by Riot Games.

Design and implement a HitCounter class that keeps track of requests (or hits).
It should support the following operations:

 * record(timestamp): records a hit that happened at timestamp
 * total(): returns the total number of hits recorded
 * range(lower, upper): returns the number of hits that occurred between
   timestamps lower and upper (inclusive)

Follow-up: What if our system has limited memory?

## Problem-138


> This problem was asked by Google.

Find the minimum number of coins required to make n cents.

You can use standard American denominations, that is, 1¢, 5¢, 10¢, and 25¢.

For example, given n = 16, return 3 since we can make it with a 10¢, a 5¢, and a
1¢.

## Problem-144


> This problem was asked by Google.

Given an array of numbers and an index i, return the index of the nearest larger
number of the number at index i, where distance is measured in array indices.

For example, given [4, 1, 3, 5, 6] and index 0, you should return 3.

If two distances to larger numbers are the equal, then return any one of them.
If the array at i doesn't have a nearest larger integer, then return null.

Follow-up: If you can preprocess the array, can you do this in constant time?

## Problem-149


> This problem was asked by Goldman Sachs.

Given a list of numbers L, implement a method sum(i, j) which returns the sum
from the sublist L[i:j] (including i, excluding j).

For example, given L = [1, 2, 3, 4, 5], sum(1, 3) should return sum([2, 3]),
which is 5.

You can assume that you can do some pre-processing. sum() should be optimized
over the pre-processing step.

## Problem-158


> This problem was asked by Slack.

You are given an N by M matrix of 0s and 1s. Starting from the top left corner,
how many ways are there to reach the bottom right corner?

You can only move right and down. 0 represents an empty space while 1 represents
a wall you cannot walk through.

For example, given the following matrix:

[[0, 0, 1],
 [0, 0, 1],
 [1, 0, 0]]


Return two, as there are only two ways to get to the bottom right:

 * Right, down, down, right
 * Down, right, down, right

The top left corner and bottom right corner will always be 0.

## Problem-160


> This problem was asked by Uber.

Given a tree where each edge has a weight, compute the length of the longest
path in the tree.

For example, given the following tree:

   a
  /|\
 b c d
    / \
   e   f
  / \
 g   h


and the weights: a-b: 3, a-c: 5, a-d: 8, d-e: 2, d-f: 4, e-g: 1, e-h: 1, the
longest path would be c -> a -> d -> f, with a length of 17.

The path does not have to pass through the root, and each node can have any
amount of children.

## Problem-165


> This problem was asked by Google.

Given an array of integers, return a new array where each element in the new
array is the number of smaller elements to the right of that element in the
original input array.

For example, given the array [3, 4, 9, 6, 1], return [1, 1, 2, 1, 0], since:

 * There is 1 smaller element to the right of 3
 * There is 1 smaller element to the right of 4
 * There are 2 smaller elements to the right of 9
 * There is 1 smaller element to the right of 6
 * There are no smaller elements to the right of 1

## Problem-167


> This problem was asked by Airbnb.

Given a list of words, find all pairs of unique indices such that the
concatenation of the two words is a palindrome.

For example, given the list ["code", "edoc", "da", "d"], return [(0, 1), (1, 0),
(2, 3)].

## Problem-170


> This problem was asked by Facebook.

Given a start word, an end word, and a dictionary of valid words, find the
shortest transformation sequence from start to end such that only one letter is
changed at each step of the sequence, and each transformed word exists in the
dictionary. If there is no possible transformation, return null. Each word in
the dictionary have the same length as start and end and is lowercase.

For example, given start = "dog", end = "cat", and dictionary = {"dot", "dop",
"dat", "cat"}, return ["dog", "dot", "dat", "cat"].

Given start = "dog", end = "cat", and dictionary = {"dot", "tod", "dat", "dar"},
return null as there is no possible transformation from dog to cat.

## Problem-181


> This problem was asked by Google.

Given a string, split it into as few strings as possible such that each string
is a palindrome.

For example, given the input string racecarannakayak, return ["racecar", "anna",
"kayak"].

Given the input string abc, return ["a", "b", "c"].

## Problem-186


> This problem was asked by Microsoft.

Given an array of positive integers, divide the array into two subsets such that
the difference between the sum of the subsets is as small as possible.

For example, given [5, 10, 15, 20, 25], return the sets {10, 25} and {5, 15, 20}
, which has a difference of 5, which is the smallest possible difference.

