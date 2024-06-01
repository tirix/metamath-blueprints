+++
reference = "Theorem 3.1 from ~ https://www3.nd.edu/%7eandyp/notes/AKS.pdf"
state = "Formalized"
statement = """
    lcmineqlem.1 $e |- ( ph -> N e. NN ) $.
    lcmineqlem.2 $e |- ( ph -> 7 <_ N ) $.
    lcmineqlem $p |- ( ph -> ( 2 ^ N ) <_ ( _lcm ` ( 1 ... N ) ) ) $.
"""
+++
The least common multiple inequality lemma, a central result for future use.  
