# es6-perlin-module

JavaScript port of Perlin noise (and Perlin periodic noise), ported directly from Stefan Gustavson's work at:

https://github.com/stegu/perlin-noise  
https://github.com/stegu/perlin-noise/blob/master/src/noise1234.c

Released into the public domain.

This port is implemented as an ES6 module. If you need to use in a non-ES6 environment, simply remove the export directives in the source.

Note that all return values are scaled to be between 0 and 1.

Individual APIs are exposed, and there is also a single `noise(x, y, z, w)` function that will call the appropriate perlin noise function depending on the number of arguments passed in. APIs include 1D, 2D, 3D, and 4D implementations of perlin noise and perlin periodic noise.

You can view some examples at: [here](https://github.com/mikechambers/CreativeCoding/tree/master/meshjs/perlin) and [here](https://github.com/mikechambers/CreativeCoding/tree/master/meshjs/flowfield).

Note, performance seems pretty good, and is faster than a number of other JavaScript perlin noise implementations I have looked at. However, I have not done any optimizations in the code, or any formal benchmarking.
