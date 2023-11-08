[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12742746&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

## Proof

Considering two graphs A and B that are isomorphic but not connected: 

Graph A: $G_1 = (V_1, E_1)$

Vertices: $V_1 = {A, B, C}$,
Edges: $E_1 = {(A, B), (B, C)}$

Graph B: $G_2 = (V_2, E_2)$

Vertices: $V_2 = {X, Y, Z}$,
Edges: $E_2 = {(X, Y), (Y, Z)}$

Bijection function $f: V_1 \rightarrow V_2$ is as follows:

$f(A) = X$

$f(B) = Y$

$f(C) = Z$

It is clear that this function is a one-to-one and onto (bijection) function. Additionally, for any edge $(u, v) \in E_1$, we have $(f(u), f(v)) \in E_2$. For example, in Graph A, we have $(A, B) \in E_1$, and in Graph B, we have $(X, Y) \in E_2$, which satisfies the isomorphism condition.

However both Graph A and Graph B are not completely connected since they each have only two edges, not connecting all vertices. Therefore, we have shown that it is possible for isomorphic graphs to not be completely connected.

