Written in Javascript to help you visualize the challenge. 

# Formal Inputs &amp; Outputs

## Input Description

On standard console input, you will be first given a line with two space-delimited integers N and M. N is the number of nodes / vertices in the graph, while M is the number of following lines of edge-node data. A line of edge-node data is a space-delimited set of integers, with the special "-&gt;" symbol indicating an edge. This symbol shows the edge-relationship between the set of left-sided integers and the right-sided integers. This symbol will only have one element to its left, or one element to its right. These lines of data will also never have duplicate information; you do not have to handle re-definitions of the same edges.

An example of data that maps the node 1 to the nodes 2 and 3 is as follows:

    1 -&gt; 2 3

Another example where multiple nodes points to the same node:

    3 8 -&gt; 2

You can expect input to sometimes create cycles and self-references in the graph. The following is valid:

    2 -&gt; 2 3
    3 -&gt; 2

Note that there is no order in the given integers; thus "1 -&gt; 2 3" is the same as "1 -&gt; 3 2".

## Output Description

Print the N x N adjacency matrix as a series of 0's (no-edge) and 1's (edge).

# Sample Inputs &amp; Outputs
## Sample Input

    4
    0 -&gt; 1
    1 -&gt; 2
    2 -&gt; 4
    3 -&gt; 4
    0 -&gt; 3

## Sample Output

    01010
    00100
    00001
    00001
   
