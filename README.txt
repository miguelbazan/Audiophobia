Problem Description

The loudness or intensity level of sound is usually measured in decibels and sound having intensity level 130 decibels or higher is considered painful. The intensity level of normal conversation is 60¬65 decibels and that of heavy traffic is 70¬80 decibels.

Consider the following city map where the edges refer to streets and the nodes refer to crossings. The integer on each edge is the average intensity level of sound (in decibels) in the corresponding street.


To get from crossing A to crossing G you may follow the following path: ACFG. In that case you must be capable of tolerating sound intensity as high as 140 decibels. For the paths ABEG, ABDG and ACFDG you must tolerate respectively 90, 120 and 80 decibels of sound intensity. There are other paths, too. However, it is clear that ACFDG is the most comfortable path since it does not demand you to tolerate more than 80 decibels.
  
In this problem, given a city map you are required to determine the minimum sound intensity level you must be able to tolerate in order to get from a given crossing to another.


Input

The first line contains the number of the cases.
For each case comes three integers C (0 < C <=100), S (0 < S <= 1000) and Q (0 < Q < 1000) where C indicates the number of crossings (crossings are numbered using distinct integers ranging from 1 to C), S represents the number of streets and Q is the number of queries.
Each of the next S lines contains three integers: c1, c2 and d indicating that the average sound intensity level on the street connecting the crossings c1 and c2 (c1 ≠ c2) is d decibels. 
Each of the next Q lines contains two integers c1 and c2 (c1 ≠ c2) asking for the minimum sound intensity level you must be able to tolerate in order to get from crossing c1 to crossing c2.
Output

For each test case in the input first output the test case number (starting from 1) as shown in the sample output. Then for each query in the input print a line giving the minimum sound intensity level (in decibels) you must be able to tolerate in order to get from the first to the second crossing in the query. If there exist no path between them just print the line "no path".
Sample Input

2
7 9 3
1 2 50
1 3 60
2 4 120
2 5 90
3 6 50
4 6 80
4 7 70
5 7 40
6 7 140
1 7
2 6
6 2
7 6 3
1 2 50
1 3 60
2 4 120
3 6 50
4 6 80
5 7 40
7 5
1 7
2 4
Sample Output

Case 1:
80
60
60
Case 2:
40
no path
80