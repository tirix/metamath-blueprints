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

Simply edit the files in this repository. They will be compiled and displayed in [https://tirix.github.io/metamath-blueprints](https://tirix.github.io/metamath-blueprints). You can contribute via commits or PRs.

One directory represents a project, and each file in that directory represents a definition or a theorem. Files are in the markdown format, with a TOML front-matter,  which might contain following optional fields as in:
```
+++
type = "Theorem"
reference = " Theorem 11.29 of [Schwabhauser] p. 102."
dependencies = ["isleag", "isinag"]
statement = "|- ( ph -> ( <\" A B C \"> ( leA ` G ) <\" D E F \"> <-> E. y e. P ( C ( inA ` G ) <\" A B y \"> /\\ <\" A B y \"> ( cgrA ` G ) <\" D E F \"> ) ) )"
state = "ReadyForProof"
hide = true
+++
```
The rest of the file can include e.g. an informal description of the proof or any useful hints.
