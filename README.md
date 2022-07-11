# Travelling-Salesman

which is the shortest route the salesman can choose given that he needs to return to the initial city and does not pass through the same city twice?

The Travelling Salesman problem can be easily solved by brute force. However, The procedure of checking the cost of all possibilities(routes) takes so much time since this problem is an NP-hard problem and the time complexity to solve is O(n!). For that reason, heuristic-based algorithms were developed to provide an approximate solution that, despite not being as good as the shortest, can give us enough short solution. Then, the following algorithm implements the most famous heuristic algorithms.

## The algorithms implemented:

* Greedy(select the shortest available route at each iteration).
* Hill Climbing(the submethod used is '2 swap').
* VND.
* Random Multi Start.
* GRASP(the nodes of the initial route in each iteration are randomly selected from the k shortest available route using the costs as weights).
* Brute Force(This one is not recommended if the 'k' is larger than 10 since it might take a long time).

## demonstrating an example.

The following pictures show the solutions(20=n) obtained by some above algorithms:

Greedy:

![greedy](https://user-images.githubusercontent.com/94997683/177010028-35be97f0-dcd9-4017-afbc-96592e4ac2aa.png)

Iterated Local Search:

![ILS](https://user-images.githubusercontent.com/94997683/177010029-e590b7f2-9532-43db-b42a-d54cfd0ca758.png)

Grasp:

![grasp](https://user-images.githubusercontent.com/94997683/177010031-d01fb697-e948-461a-a4ed-39a3128c0880.png)

The below table shows us the costs found by the methods.

| {Methods}                    | Cost | Time used(s) |
|-----------------------|---------------|-------------------|
| Random             | 1795.5178     | NaN               |
| Greedy                | 427.1587      | 0.000104          |
| Hill Climbing         | 1084.1500     | 0.000721          |
| VND                   | 394.3840      | 0.001521          |
| Random Multi Start    | 846.6160      | 0.003752          |
| Grasp                 | 392.0400      | 0.140790          |


As you can see, The GRASP reaches the best result.

