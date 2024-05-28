+++
reference = "Theorem 2.2 from ~ https://www3.nd.edu/%7eandyp/notes/AKS.pdf"
state = "Draft"
statement = """
$e |- 
$e |- ( ph -> N e. ( ZZ>= ` 2 ) ) $.
$e |- ( ph -> R e. ( 1 ... ( |^ ` ( 5 log N ) ) ) ) $.
$e |- ( ph -> A e. ( 1 ... ( |_ ` ( ( sqrt ` ( phi ` R )  ) x. ( 2 log N )  )  ) ) ) $.
$e |- ( ph -> ( A gcd N ) = 1 ) $.
$e |- ( ph ->  = 1 ) $.
$p |- ( ph -> E. m e. NN ( P ^ m ) = N ) $.
"""
dependencies = ["odrlblem","rhmextex","aks61"]
+++
Consider some $n\geq 2$. For all $1 \leq r \leq \left\lceil log_5 n \right\rceil$ and $1 \leq a \leq \left\lfloor \sqrt{ \phi(r)} log n \right\lfloor$, assume that the following hold:
* gcd(a, n) = 1, and
* In $(\mathbb{Z}/n)[x]/(x^r − 1)$, we have $(x + a)^n \equiv x^n + a$.

Then $n$ is a power of a prime.
