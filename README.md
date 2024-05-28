# Metamath Blueprints

These are blueprints for Metamaths.

The `set.mm` database only includes fully validated and verified theorems. However, in many cases, it is interesting to discuss the path forward, and e.g. definition choices. This has been done using commented out theorems in the database, but blueprints might be an alternative.

In the Metamath community, there are both:
* people who are used to formalize proofs in `set.mm` or `iset.mm`, know the tools,
* people who are used to mathematics, have access to math litterature, and know the fundamentals.

In some cases people fall in both categories, but not always.

Blueprints is a way to help communication:
- explaining the path to complex theorems, and showing what's left to formalize, even for one single contributor, for the rest of the community,
- organizing, coordinating and e.g. splitting larger tasks between several contributors,
- communicating larger proofs and concepts between mathematicians and formalizers,
- viewing and tracking the progress made in a project,

## How to create and use blueprints

Simply edit the files in [this repository](https://github.com/tirix/metamath-blueprints). They will be compiled and displayed in [https://tirix.github.io/metamath-blueprints](https://tirix.github.io/metamath-blueprints). You can contribute via commits or PRs.

One directory represents a project, and each file in that directory represents a definition or a theorem. Files are in the markdown format, with a TOML front-matter,  which might contain following optional fields as in:
```
+++
type = "Theorem"
reference = " Theorem 11.29 of [Schwabhauser] p. 102."
dependencies = ["isleag", "isinag"]
statement = "|- ( ph -> ( <\" A B C \"> ( leA ` G ) <\" D E F \"> <-> E. y e. P ( C ( inA ` G ) <\" A B y \"> /\\ <\" A B y \"> ( cgrA ` G ) <\" D E F \"> ) ) )"
state = "ReadyForProof"
+++
```
The rest of the file can include e.g. an informal description of the proof or any useful hints.


## Definition of Key-Value pairs

### Type
A string giving the type of the statement. Possible values are:
- `Theorem`,
- `Definition`,
- `Axiom`

### Reference
An optional string giving the textbook reference for the statement. Usually a book, a url, with page and/or theorem number. This can be formatted as a [Metamath bibliographic reference](https://us.metamath.org/mpeuni/mmset.html#bib).

### Dependencies
An optional array of strings, either they exist already in the database which serves as a hint for the proof or they link to a lemma not in the database, with either statement or proof formalized or neither.

### Statement 
An optional string containing the Metamath statement. The quote symbol (`"`) and the backslash symbol have to be escaped with a backslash (resp. `\"` and `\\`).

### State
An optional string giving the current development state of the statement. The following state values are acceptable:
- `Draft`: This is to be used when the theorem is very much in its early stage and it is not clear whether the statement is of use yet or that necessary definitions are missing.
- `ReadyForStmt`: Once it is clear that the theorem is used in a proof we can try to formalize the statements and its hypotheses.
- `StmtFormalized`: The statement is formalized, this includes all hypotheses and its conclusion, yet the dependent theorems are not yet proven.
- `ReadyForProof`: The dependent theorems are proven and the statement is formalized. The proof step can begin now.
- `Formalized`: The proof and all its dependencies are proven. Good job to all contributors.
