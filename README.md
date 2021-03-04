##                                             Maze Solver project

## Project Description                                             
In this project aim is a maze in the form of matrix will be given in the form of 1's and 0's. Where 1 repersents the open path and 
0 represents the blocked path

    Main goal is to find the path between the source to destination in the maze (if the path exists) otherwise return -1 as output

## Concepts used
   1) Graphs datastructure
   2) Breadth-First-Search Algorithm
   3) Dijkstra's algorithm 
   4) File Handling
   5) Command line parsing

## Following are the import used in the project
   1) Defaultdict -- to store graph datastructure
   2) Argparse -- to read command line arguments

## Idea to solve
   From the given matrix identify the positions, which has 1 and take them as vertices(nodes) of the graph.
   Then identify the position(neighbours) which are immediate left, right, top and bottom to given node, if contains 1
   Whichever neighbour contains 1 for given node, add that particular node as neighbour to given node.
   Repeat process until we obtain the entire undirected-unweighted graph.Now determine if the two nodes(i.e,, source and
   destination node) connected.
   If the two nodes are connected, then determine the path between them(i.e identify the positions).
   Finally print the matrix of the order which contains 1 at the position obtained from the above process and contain 0 at other position. 

## How to run Maze solver
   First import the github repo https://github.com/attainu/project-Vishal-coder-ui-au8 into visual studio code.  
   Project consist of 3 contents:-
   1) maze.py
   2) inputfile.txt
   3) outputfile.txt

   --> Firstly it takes the input from the user in the form of m*n
   --> After input is given open the terminal and give the command to see the output in outputfile.txt

## Run command
              maze.py -i inputfile.txt -o outputfile.txt -s=0,0 -d=4,4     
              
              where s=source point and d=destination point 


