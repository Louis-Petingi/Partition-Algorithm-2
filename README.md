# Partition-Algorithm-2
The algorithm is written in C++. The program takes the adjacency matrix of the dual-graph representation of an RNA Secondary Structure and splits the graphs into blocks. Then the algorithm classifies each block either as a Pseudoknot (PK) or Pseudoknot-free region.
The output of the program is the partition of the dual-graph into blocks and the algorithm classifies each of the blocks as either a pseudoknot or pseudoknot-free region.In the main C++ routine the input is the file:
infile.open("C:/Users/lpetn_000/desktop/RnaDv/PKB236.txt");
For example for motif PKB236, it has 7 vertices (correspondng to 7 stems)
       
    0    2   0   0   0   0     1
    2    0   2   0   0   0     0      
    0    2   0   2   0   0     0       
    0    0   2   0   2   0     0       
    0    0   0   2   0   2     0      
   
    When the program is run, the user enters first the number of vertices (in this case 7) 
    and the Motif id (in this case PKB236)
    
