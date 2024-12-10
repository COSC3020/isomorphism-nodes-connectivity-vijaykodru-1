# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$. In other words, there is a one-to-one correspondence between the vertices of the two graphs that preserves the adjacency relation (i.e., if two vertices are connected by an edge in one graph, their corresponding vertices in the other graph must also be connected by an edge).

Given $G_1 = (V_1, E_1)$ and $G_2 = (V_2, E_2)$ be two completely connected graphs with the same number of nodes $n$. A graph to be completely connected it should have a edge connecting between every pair of nodes in that graph. Because the $G_1$ and $G_2$ are completely connected every pair of nodes in the graphs are connected with every other edge in that respective graph. 

Because the given graphs also have the same number of vertices we can take any vertex in Graph A and we can always find a corresponding vertex in graph B in any permutation. This is because all the nodes are connected to each other in both the graphs making it true that we always find a bijection between them. 

In a completely connected graph all vertices are connected to every other vertices in that graph with an edge between them. For $G_1$ this means that $E_1 = {u, v}$ such that $(u, v) \in V_1$ and $u \ne v$. This also the same for $G_2$ this means that $E_2 = {a, b}$ such that $(a, b) \in V_2$ and $a \ne b$.

with the bijection function f we can say that for any pair of ${u, v} \in E_1$ because it is a completely connected graph and the vertices $f(u), f(v) \in V_2$ and $(f(u), f(v)) \in E_2$ because $G_2$ is also completely connected graph. This satisafies the condition above where $(u,v) \in E_1 <=> (f(u),f(v)) \in E_2$. Therefore with this proof we can say that $G_1$ and $G_2$ are isomorphic.

References: I used my previous repository for correctness check, however it is not done properly with a proof to prove the mapping exits.