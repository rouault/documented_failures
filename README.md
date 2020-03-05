# List of various unsuccessful attempts at software tasks

## C++: When qualifying a class with "final" actually hinders performance

Attempted on GEOS library in https://github.com/libgeos/geos/pull/279
Conclusion is that the addition of "final" resulted in measurable performance loss, whereas we at least hoped for identical performance : https://github.com/libgeos/geos/pull/279#issuecomment-586089698
The reason for this wasn't explored deeply. Woud likely require to look at generated assembly code. One explanation might be that this resulted in more inlining that could have negatively affected the instruction cache ?

## Humour section

### Brainfuck will not rule the world

The Turing-complete [Brainfuck](https://en.wikipedia.org/wiki/Brainfuck) language should normally have taken over all other programming languagues by its sheer simplicity, but it hasn't. Although it benefits from an advanced open source implementation, [libbf](https://savannah.nongnu.org/projects/libbf), the uptake has been close to none. No contributions from other developers have been received up-to-date. Reasons are not completely clear: lack of Javascript implementation, lack of gcc / clang frontend ?

We have also [prototyped](https://github.com/rouault/PROJ/commit/767c5c4e864b09e5000a5a72363a38daa2605735) an extension of the syntax of the [PROJ](https://proj.org) open source project with Brainfuck operators to give it Turing-completness, but this only caused shrugs. 

## License of this document

https://creativecommons.org/share-your-work/public-domain/cc0/
