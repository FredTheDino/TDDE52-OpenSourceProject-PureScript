# Contribution Plan - PureScript, edvth289

# Sprint Planning

## Sprint 1
  - Setup the development environment
    - [x] Install and setup Stack and GHC
    - [x] Setup language servers and IDE support
    - [x] Try to compile the project
    - [x] Read trough PR about recent changes to error messages (https://github.com/purescript/purescript/pull/4383)
  - Bellow this is extra stuff
    - [x] Add unit tests to Erlang Map and add some more derives (https://github.com/purerl/purescript-erl-maps/pull/11)
    - [x] Formulate a simple change and propose it to the PureScript team
      - Say which fields mismatched in type errors with records?
      - Highlight which fields have matched successfully in the overview?

## Sprint 2
  - [x] Message the maintainers about merging the `Erl.Data.Map` changes
  - [x] Start making changes and see what I don't understand
    - Resulted in (https://github.com/purescript/purescript/pull/4411), is undergoing review but I think it's gonna get merged, it's getting some attention :D
  - [x] Learn something
  - [ ] See what needs doing and do it
    - Accidentally made (parts of a) treesitter module, needs more work though https://github.com/FredTheDino/tree-sitter-purescript/
    - Make PureScript into a real programming language: https://github.com/cat-milk/Anime-Girls-Holding-Programming-Books/pull/549
  - [x] Start looking at another improvement to the error messages

## For next week
  - [ ] Merge #4411 <- apparently won't be done?
  - [ ] Finish the tree sitter <- not done
  - [ ] More revisions on https://github.com/purescript/purescript/pull/4421 

## Technical difficulty

### Build and Test Environment
Build and test environment is already set up with a CI job that runs some tests and builds.
The entire project is built using `stack` (the currently hot build system for Haskell).
`stack` automatically installs dependencies and the like.

The build system is *easy* (tough `stack` is pretty bad...)

------------
After further consideration and feedback from the rest of my group, I'm
cindering the buildsystem to be *medium* in difficulty.

### Domain knowledge
The project is a compiler. Compilers are one of the most studied areas in computer science.
PureScript would require knowledge of compilers and strong fundamentals in computer science to work on.

I will classify the project as *hard* in domain knowledge.

### Project size
After running `cloc` on the PureScript repository.
```
--------------------------------------------------
Language       files     blank   comment      code
--------------------------------------------------
Haskell          220      5391      6901     34574
PureScript       965      3874       877      9170
Markdown          22      1648         0      4271
CSS                2        85       283       799
yacc               1       122         0       689
LESS               1       166       116       624
JavaScript        38        25        20       512
Bourne Shell       6        63        95       244
YAML               4        47       109       221
JSON              14         0         0       194
make               1        21        11        47
dhall              1         5        10        19
Text               1         6         0         9
XML                1         0         0         2
--------------------------------------------------
SUM:            1277     11453      8422     51375
--------------------------------------------------
```

the project is in total around ~51KLOC, but the project is also written in a
very high level language with a fair bit of dependencies. Therefore the code
base size doesn't clearly classify it's size compared to a similar project
written in `C`. There is also a myriad of backends for the PureScript compiler
and if I were to include those the project would be medium to large.

I'd classify the project size as *medium*.

## Process difficulty

### Issue tracker
The issues have no difficulty markers, though it's probably quite easy to ask in their Discord channel.

I'd guess the project is *medium* difficult with it's issue tracking since the community is quite active
and that issues don't really tell the full picture.

### Documentation
No clear introduction for new developers - some documented code and a lot of `todo`s for various errors.

The project is *hard* in this respect.

### Communications
PureScript has a Discord server with specific channels for developer (but nothing for new developers).

It'd therefore classify the project as *medium*.

## Development process

### Group contributions
I'll actively participate in project meetings since I don't know exactly how
much time and energy I have for this course.

I'll do the *easy*.

### Planning and reflection
Similar to the previous point, I'll do minimum effort.

I'll do the *easy*.

### Engineering practice
Similar to the previous point, I'll do minimum effort.

I'll do the *easy*.

## Contributions
### Quantity of code contributions
I'll aim to make one contribution that has been accepted by the project.

I'll do the *easy*.

### Complexity of code contributions
I'll aim to make a non-trivial code contribution.

I'll do the *easy*.

### External communications
I'll aim to communicate with at least one developer.

I'll do the *easy*.

