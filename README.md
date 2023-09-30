[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=11754423&assignment_repo_type=AssignmentRepo)
# Asymptotic Equivalences

In the lectures, we said that logarithms with different bases don't affect the
asymptotic complexity of an algorithm. Prove that $O(\log_{2} n)$ is the same as
$O(\log_{5} n)$. Use the mathematical definition of $O$ -- do a formal proof,
not just the intuition.

I have started with the formal definition of $O$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$T(n) \in O(f(n)) \iff \exists c, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$


Using the definition of $O$, we can obtain:

$T(n) \leq c \cdot \log_{2}n$ for all $T(n) \in \log_{2}n$

$T(n) \leq c \cdot \log_{5}n$ for all $T(n) \in \log_{5}n$

Using change of base log rules, we can obtain

$T(n) \leq c \cdot \log_{5}(2)\log_{5}n$

$c \cdot \log_{5}(2)$ is a constant d

$T(n) \leq d \cdot \log_{5}n$ 

this means that $T(n) \in O(\log_{2}n) \iff \exists c, n_0: T(n) \leq d \cdot \log_{5}n$

this means that $T(n) \in \log_{2}$ is also in $\log_{5}$ and vice versa so logs with different bases don't affect asymptotically complxeity