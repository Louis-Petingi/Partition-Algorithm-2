# Partition-Algorithm-2
The algorithm is written in C++. The program takes the adjacency matrix of the dual-graph representation of an RNA Secondary Structure and splits the graphs into blocks. Then the algorithm classifies each block either as a Pseudoknot (PK) or Pseudoknot-free region.
The output of the program is the partition of the dual-graph into blocks and the algorithm classifies each of the blocks as either a pseudoknot or pseudoknot-free region. In the main C++ routine the input is the file:
infile.open("C:/Users/lpetn_000/desktop/RnaDv/PKB236.txt").
For example RNA PKB 236 dual-graph has 7 vertices (corresponding to 7 stems) labeled 0 thru 6.
       
    0    2   0   0   0   0     1
    2    0   2   0   0   0     0      
    0    2   0   2   0   0     0       
    0    0   2   0   2   0     0       
    0    0   0   2   0   2     0  
    0    0   0   0   2   0     2     
    1    0   0   0   0   2     0    
   
    When the program is run, the user enters first the number of vertices (in this case 7) 
    and the Motif id (in this case PKB 236)
    The output of the program is written into the file outfile.open("C:/Users/lpetn_000/desktop/RnaDv/PKB236_out.txt");
    PKB 236 has only one block that is a PK. The program output is:
    
    ===================== New Block ================== 

(6,0) - (5,6) - (5,6) - (4,5) - (4,5) - (3,4) - (3,4) - (2,3) - (2,3) - (1,2) - (1,2) - (0,1) - (0,1) - 

---- this block represents a pseudoknot ----

----------- Summary information for Motif :PKB 236 --------------------------------

----------- Total number of blocks: 1

----------- number of PK blocks: 1

----------- Total number of regular blocks : 0

-----------------------------------------------------
