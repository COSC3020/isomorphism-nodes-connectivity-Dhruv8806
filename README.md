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

-> We consider two graphs, $A$ and $B$, with the same number of nodes, and both are completely connected. To prove that they are isomorphic, we can establish a one-to-one and onto function between their node sets, $V_1$ and $V_2$

-> Since $A$ and $B$ have the same number of nodes, there exists a bijective function $f: V_1 \rightarrow V_2$ that maps each node in $A$ to a unique node in $B$. This one-to-one correspondence ensures that there are no extra or unmatched nodes in either graph

-> Now, let's examine the edges. Since both $A$ and $B$ are completely connected, every node in each graph is connected to every other node. This means that if two nodes, $u$ and $v$, are connected by an edge in $A$, their corresponding nodes, $f(u)$ and $f(v)$, must also be connected by an edge in B due to the bijective nature of the function $f$

-> Therefore, we've established a one-to-one and onto function f that preserves both the nodes and edges of $A$ and maps them to $B$, satisfying the definition of isomorphism. Hence, if two graphs have the same number of nodes and are completely connected, and they must be isomorphic.

-> Sources Used: TA
