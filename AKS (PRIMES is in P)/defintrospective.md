+++
state = "Draft"
statement = "Let l be the homomorphism that maps the integer coefficents to Z mod p coefficients,
For two positive numbers p and r define a introspective relation, which is a binary relation 
on (positive numbers, Polynomials over Z), defined by
e ~ f, 
where f(X)^e is e-th iterate of p and
f(X^e) is the polynomial introduced by replacing the monomials X^0, X^1 ,... by X^e*0, X^e*1,...
Calculate l(f(X)^e-f(X^e)) and see if it divides (X^r)-1
"
df-intro $a |- INTRO = INTRO $.

"""
+++