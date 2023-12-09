[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12802950&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ have the same number of nodes and are
completely connected, they must be isomorphic. I have started with the formal
definition of isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## My Implementation 

-> We consider two fully connected graphs graphs, $A = (V_1  , E_1)$ and $B = (V_2 , E_2)$, both having an equal number of nodes, the potential for a one-to-one bijection mapping. 

-> In the fully connected graphs, each node connects with every other node. This connectivity holds true for both A and B, ensuring that nodes within A are essentially equivalent, both in terms of edges and total node count. This means that for every node in A, there exists an edge connecting it to each and every other node in A, and the same holds for B. This connectivity equivalence, paired with an equal count of edges, sets the stage for establishing isomorphism

-> Bijective Mapping construction
  - Nodes of $A$ are randomly permuted, resulting in a unique order.
  - Similarly, nodes of $B$ has a random permutation, yielding a distinct order. 
  - Bijective mapping: $f: V_1$ $\rightarrow V_2$ by associating each node in $A$ with the corresponding node in $B$ without repetition.

-> For any node in $u$ $\in$ $V_1$ , its counterpart $f(u)$ $\in$ $V_2$ is unique. 

-> For each edge $(u , v)$ $\in$ $E_1$ , the corresponding edge $(f(u) , f(v))$ $\in$ $E_2$ is also present. 

-> In conclusion, the shared number of nodes, equivalent node structures, and the bijective mapping construction establish a one-to-one and onto mapping between the completely connected graphs $A$ and $B$. This ensures not only a matching of nodes but also an exact mapping of the connections (edges) between nodes in $A$ to $B$. Therefore, if two graphs have the same number of nodes and are completely connected, they must be isomorphic

-> Sources Used: TA
