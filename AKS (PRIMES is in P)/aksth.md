+++
reference = "https://www3.nd.edu/%7eandyp/notes/AKS.pdf"
state = "Draft"
dependencies = ["aksthr","aks22","akslb"]
+++
Given an integer $n\geq 2$ and integer $a$ coprime to $n$, $n$ is prime if and only if the polynomial congruence relation
$$(X+a)^{n}\equiv X^{n}+a{\pmod {n}}$$
holds within the polynomial ring $(\mathbb{Z}/n\mathbb{Z})[X]$.

It is sufficient to evaluate that equality in a polynomial ring $(\mathbb{Z}/r\mathbb{Z})[X]$, and the number of $a$'s to test and the appropriate $r$ are both bounded by a polynomial in $log n$ and therefore, there is a deterministic polynomial time algorithm for testing primality.