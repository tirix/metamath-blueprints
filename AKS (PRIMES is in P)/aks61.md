+++
reference = "Theorem 6.1 from ~ https://www3.nd.edu/%7eandyp/notes/AKS.pdf"
state = "Draft"
statement = """
aks.1 $e |- G = ( Z/nZ ` R ) $.
aks.2 $e |- O = ( od ` G ) $.
aks.3 $e |- F = ( GF_oo ` P ) $. // F is the algebraic closure of F_p
aks.4 $e |- A = ( ( ZRHom ` P ) ` a ) $. // ` A ` is the image of a by the canonical homomorphism from the integers to the ring ` F `
aks.5 $e |- .^ = ( .g ` ( mulGrp ` F ) ) $.
aks.6 $e |- .1. = ( 1r ` F ) $.
aks.7 $e |- +. = ( +g ` F ) $.
aks.8 $e |- .0. = ( 0g ` F ) $.
aks.9 $e |- ( ph -> N e. ( ZZ>= ` 2 ) ) $.
aks.10 $e |- ( ph -> P e. Prime ) $.
aks.11 $e |- ( ph -> P || N ) $.
aks.12 $e |- ( ph -> R e. ( ZZ>= ` 2 ) ) $.
aks.13 $e |- ( ph -> ( N gcd R ) = 1 ) $.
aks.14 $e |- ( ph -> ( ( 2 logb N ) ^ 2 ) < ( O ` N ) ) $.
aks.15 $e |- ( ph -> M e. F ) // M is an element of the splitting field
aks.16 $e |- ( ph -> ( R .^ M ) = .1. ) $. // also state that R is minimal so that it is a primitive root?
aks.17 $e |- ( ( ph /\\ a e. ( 1 ... ( |_ ` ( ( sqrt ` ( phi ` R ) ) x. ( 2 logb N ) ) ) ) ) -> ( a gcd N ) = 1 ) $.
aks.18 $e |- ( ( ph /\\ a e. ( 1 ... ( |_ ` ( ( sqrt ` ( phi ` R ) ) x. ( 2 logb N ) ) ) ) ) -> ( N .^ ( M .+ A ) ) = ( ( N .^ M ) .+ A ) ) $.
aks $p |- ( ph -> E. m e. NN ( P ^ m ) = N ) $= ? $. // AKS Result, if 1-18 hold, then N is a power of P.
"""
dependencies = ["aks61c2","aks61c7"]
+++
