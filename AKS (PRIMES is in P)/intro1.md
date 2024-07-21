+++
state = "Draft"
statement = "Closure statement of introspective relation"
$e |- ( ph -> P e. NN ) $.
$e |- ( ph -> R e. NN ) $.
$e |- I = ( P INTRO R ) $.
$e |- ( ph -> E e. NN ) $.
$e |- A = ( Base ` ( poly1 ` ZZ ) ) $.
$e |- ( ph -> F e. A ) $.
$e |- ( ph -> G e. A ) $.
$e |- ( ph -> E I F ) $.
$e |- ( ph -> E I G ) $.
$p |- ( ph -> E I ( F x. G ) ) $. // TODO Replace x. with polynomial multiplication.
"""
dependencies = ["defintrospective"]
+++

