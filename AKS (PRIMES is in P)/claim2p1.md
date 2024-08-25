+++
reference = "Part of Claim 2 from ~ https://www3.nd.edu/%7eandyp/notes/AKS.pdf"
state = "Draft"
statement = """
$e |- ( ph -> P e. Prime ) $.
$e |- X = ( GFoo ` P ) $.
$e |- B = ( Base ` X ) $.
$e |- ( ph -> R e. PrimRoot ) $.
$e |- ( ph -> CurlyPbar = { y e. B | E. f e. CurlyP y = ( f ` R ) } ) $.
$e |- ( ph -> T = ( ( X ^ M ) - ( X ^ N ) ) ) $.
$e |- ( ( ph /\ x e. CurlyPbar ) -> ( T ` x ) = 0 ) $.
$p |- ( ph -> ( # ` CurlyPBar ) <_ ( ( deg1 ` R ) ` T ) ) $.
"""
dependencies = ["fta1g"]
+++
If every element of CurlyPBar is a root of T, then the elements of CurlyPBar are bound by the degree of T.
Also, not as a statement, but the degree of T is greater equal than $N^{\sqrt{\bar \mathcal{R}\bar}}$
