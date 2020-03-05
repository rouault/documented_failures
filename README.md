# List of various unsuccessful attempts at software tasks

## C++: When qualifying a class with "final" actually hinders performance

Attempted on GEOS library in https://github.com/libgeos/geos/pull/279
Conclusion is that the addition of "final" resulted in measurable performance loss, whereas we at least hoped for identical performance : https://github.com/libgeos/geos/pull/279#issuecomment-586089698
The reason for this wasn't explored deeply. Woud likely require to look at generated assembly code. One explanation might be that this resulted in more inlining that could have negatively affected the instruction cache ?
