+++
reference = "Part for Claim 3 from ~ https://www3.nd.edu/%7eandyp/notes/AKS.pdf"
state = "Draft"
statement = """
cl3a.1 $e |- G = ( Z/nZ ` R ) $.
cl3a.2 $e |- O = ( od ` G ) $.
cl3a.3 $e |- F = ( GF_oo ` P ) $. // F is the algebraic closure of F_p
cl3a.4 $e |- A = ( ( ZRHom ` P ) ` a ) $. // ` A ` is the image of a by the canonical homomorphism from the integers to the ring ` F `
cl3a.5 $e |- .^ = ( .g ` ( mulGrp ` F ) ) $.
cl3a.6 $e |- .1. = ( 1r ` F ) $.
cl3a.7 $e |- +. = ( +g ` F ) $.
cl3a.8 $e |- .0. = ( 0g ` F ) $.
cl3a.9 $e |- ( ph -> N e. ( ZZ>= ` 2 ) ) $.
cl3a.10 $e |- ( ph -> P e. Prime ) $.
cl3a.11 $e |- ( ph -> P || N ) $.
cl3a.12 $e |- ( ph -> R e. ( ZZ>= ` 2 ) ) $.
cl3a.13 $e |- ( ph -> ( N gcd R ) = 1 ) $.
cl3a.14 $e |- ( ph -> ( ( 2 logb N ) ^ 2 ) < ( O ` N ) ) $.
cl3a.15 $e |- ( E = { x e. ZZ | ( K e. NN0 /\\ J e. NN0 /\\
( ( ( N / P ) ^ K ) x. ( P ^ J ) ) ) } ) $.
cl3a.16 $e |- ( M = ( ZRHom ` G ) ) $. //I think we need to define a map as in preparation for claim 3.
cl3a $e |- ( ph ->  ( M " E ) = ( Base ` G ) )
"""
dependencies = ["znzrhfo","cl3contnpows"]
+++

This is a necessary step for claim 3, essentially we want to show that
the restriction of the homomorphism of E -> Z/rZ is surjective.
This allows us to reason that the image contains r elements.
Assume it is not true, then there is an element in Z/rZ that is not hit by the homomorphism,
but this is a contradiction by our result. Thus we can replace ord_r(n) with barE
but by cl3a.14 claim 3 follows.

We also need to show that all powers of n are in E, but this should be trivial.
This should be proven in cl3contnpows.
