# Graphs
an exploration of non-linear data structures.

# Terminology:

- vertex: also called a node, data object with N sibling Nodes
- Edge: just as with trees, connection between nodes, represented visually by a line
- neighbor: node or nodes adjacent to the current node, use this term instead of *sibling* or *next*
- degree: number of edges connected to a given node


## Directed v Undirected: "FIGHT!"

mortal combat references aside, an Undirected graph contains no rules for which edges connect to which node. or more accurately no rule for which node is to be referenced "next". a directed graph also called a digraph, (not to be confused with a di-a-graph?) contains directional rules for each node indicating which node should be accessed next.

## Battle Royale: complete, connected, disconnected

Complete Graphs: there are no empty spaces that fill the graph with holes. sorry BackstreetBoys. in a Complete Graph all verticies(nodes) are connected to all other vertices. 

Connected Graphs: 

easily mistaken for molecular models, vertices in a connected graph all share at least one edge with another vertex.

Disconnected Graphs:

like an archipelago where some of the islands are connected by moss-covered rope-bridges and others are near but not easy to get to so is our disconnected graph, some vertices may not have a common edge with any other vertex but they are still part of the graph archipelago. 


# Traversal and usage:

graphs are traversed in a similar manner to trees and the implementation resembles a queue. Nodes in a Graph also include a propertie `visited` other methods of `<class 'Graph'>` include Push, Peek, and Pop. 
it may be useful to add a `contains` method as well. 

Graphs are used in applications involving GPS, Mapping, Social networks and targeted suggestion algorithms. it is interesting to note that graphs also resemble neural-network structures and I suspect are heavily used in machine-learning and AI developments. 



#### [Return to Main index of Notes](./README.md)