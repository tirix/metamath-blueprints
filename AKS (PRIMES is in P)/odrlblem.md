+++
reference = "Theorem 4.1 from ~ https://www3.nd.edu/%7eandyp/notes/AKS.pdf"
state = "ReadyForStmt"
statement = """
$e |- G = ( Z/nZ ` r ) $.
$e |- B = ( |^ ` ( ( 2 logb N ) ^ 5 ) ) $.
$p |- ( N e. ( ZZ>= ` 3 ) -> E. r e. ( 1 ... B ) ( ( r gcd N ) = 1 /\\ ( 2 logb N ) < ( od ` G ) ) ) $.
"""
dependencies = ["lcmineqlem"]
+++
### Making $n$ have high order modulo $r$.

For $n \geq 3$, there exists some $r \leq \left\lceil log_5 n \right\rceil$ such that $gcd(n, r) = 1$ and $od_r(n) > log_2 n$.

