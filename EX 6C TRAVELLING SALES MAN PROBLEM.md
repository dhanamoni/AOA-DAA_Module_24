# EX 6C TRAVELLING SALES MAN PROBLEM
## DATE: 06/05/24
## AIM:
To Solve Travelling Sales man Problem for the following graph.

## Algorithm :

1.Take the cost matrix that shows the cost between every pair of cities.

2.Generate all possible orders (permutations) in which the cities can be visited.

3.For each order, calculate the total travel cost, including returning to the starting city.

4.Keep track of the minimum total cost found so far.

5.After checking all possible orders, return the minimum cost as the final answer.

## Program :
```
Developed by: MONIKA D
Register Number:  2122223240096
```
```
def tsp_cost(tsp):
    return min(sum(tsp[i][j] for i, j in zip(path, path[1:] + path[:1])) for path in permutations(range(len(tsp))))

from itertools import permutations
tsp = [[-1, 30, 25, 10], [15, -1, 20, 40], [10, 20, -1, 25], [30, 10, 20, -1]]
print("Minimum Cost is :",tsp_cost(tsp))
```

## Output :

![image](https://github.com/user-attachments/assets/ecf9c7a0-3e7b-445b-96cd-5a069c62bebc)


## Result :

Thus the program was executed successfully for finding the minimum cost to vist all cities.

