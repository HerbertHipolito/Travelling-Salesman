# Travelling-Salesman

which is the shortest route the salesman can choose given that he needs to return to the initial city and does not pass through the same city twice?

The Travelling Salesman problem can be easily solved by brute force. However, The procedure of checking the cost of all possibilities(routes) takes so much time since this problem is an NP-hard problem and the time complexity to solve is O(n!). For that reason, heuristic-based algorithms were developed to provide an approximate solution that, despite not being as good as the shortest, can give us enough short solution. Then, the following algorithm implements the most famous heuristic algorithms.