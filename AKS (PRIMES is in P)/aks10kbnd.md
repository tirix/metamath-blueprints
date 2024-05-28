+++
reference = "Lemma 2.3 from ~ https://www3.nd.edu/%7eandyp/notes/AKS.pdf"
state = "Draft"
statement = """
$e |- 
$e |- ( ph -> N e. RR ) $.
$e |- ( ph -> 10000 <_ N ) $.
$p |- ( ph -> ( ( 2 logb N ) ^ ( 7 / 2 ) ) < N ) $.
"""
dependencies = ["taylconcavebnd"]
+++
Use Taylor's expansion for $f(x) = (log_2(x))^{\frac{7}{2}}$ at $x = 10000$.
Then observe that $f^{\prime\prime}(x) < 0 $, $f^{\prime}(x)<1 $ and $f(x) < 10000$ for 
$x\geq 10000$.

This suffices, as $f(x)\leq f(10000)+(x-10000) f^{\prime}(x)\leq 
10000 + ( x-10000)f^{\prime}(10000)\leq
10000+(x-10000)=x
