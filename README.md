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

-> We consider two graphs, $A = (V_A  , E_A)$ and $B = (V_B , E_B)$, with $|V_A| = |V_B|$ as they same number of nodes, and both are completely connected. 

To prove that $A$ and $B$ are isomorphic, we need to establish a bijective function $f$ : $A$ $\leftrightarrow$ $B$ such that each node $v$ $\in$  $V_A$, there exists a unique corresponding node $u$ $\in$ $V_B$

$\forall_v$ $\in$ $V_A$ : $v$ $\leftrightarrow$ $f(v)$ 


-> For any edge: $(x, y)$ $\in$ $E_A$, there must exist a corresponding edge $(f(x), f(y))$ $\in$ $E_B$ . This means that if there's any connection between nodes $x$ and $y$ in $A$ , the same connection must exist between their counterparts $f(x)$ and $f(y)$ in $B$ . The rule applying to all edges in $A$ . 

$\forall$ $(x,y)$ $\in$ $E_A$ : $(f(x), f(y))$ $\in$ $E_B$

-> For each Edge: It's looking for each individual connection, so for each individual edge $e$ = $(x, y)$ $\in$ $E_A$ , it's corresponding edge $f(e) = (f(x), f(y))$ must exist in $E_B$ . And we consider specific connection in $A$ ensuring it's counterpart in $B$. 

$\forall_e$ = $(x, y)$ $\in$ $E_A$ : $e$ $\leftrightarrow$ $f(e)$ = $(f(x) , f(y))$ $\in$ $E_B$

-> Overall, isomorphism ensures that not only are nodes matched up, but the connections between those nodes (edges) in $A$ are exactly mapped to $B$.  Hence, if two graphs have the same number of nodes and are completely connected, they must be isomorphic.


-> Sources Used: TA
