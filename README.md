# Knuth-Morris-Pratt-algorithm-in-Java-Finding-a-string-in-a-matrix-v1-
The basic version of the Knuth-Morris-Pratt algorithm allows finding all occurrences of one string in another. Along with this version, there exist some modifications that can be used to solve more sophisticated problems. One of them allows finding a string in another string represented as a matrix. In this task, you need to implement this modification of the Knuth-Morris-Pratt algorithm.

Input: the first line contains a pattern pp. The second line contains two integer numbers nn and mm. The rest of the lines represent a matrix tt: nn rows each containing mm characters.

Output: the first line should contain one integer kk: the number of times the patter pp occurs in the matrix tt. Each of the next kk lines should contain a pair of indexes where pp occurs in tt. The first element of each pair should correspond to a row, the second one should be a column. The pairs should be sorted in ascending order (see the example below for details).

Assume, for example, that we want to find a pattern pp = "baac" in the below matrix:



As you can see, the pattern appears in the matrix twice: the first time at the index (0, 1), the second one at (2, 3). Note that although the second occurrence is split into two rows, it is still considered as an occurrence. Hence, the output should be:

2
0 1
2 3
Keep in mind that all occurrences should be sorted by their row index first, and then by column index in case the firsts match.

 Report a typo
Sample Input 1:

baac
4 5
abaac
fbcde
abbba
accba
Sample Output 1:

2
0 1
2 3
Sample Input 2:

abcdef
2 2
ab
ab
Sample Output 2:

0
