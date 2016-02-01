There were two main areas where I spent the majority of time optimizing the pizza code.

1. In the background pizza loop.
2. In the pizza resizing function.

Breakdown

1. In the pizza background loop, expensive DOM manipulations and searches were being done too frequently and often. I reduced these and use the least expensive versions to perform the same action. There were also unnecessary calculations being performed inside of loops that have been moved out and optimized to increase speed.

2. In the pizza resizing function there were a number of additional DOM manipulations and searches being performed as well as the inefficient method of applying the styles. DOM manipulation has been optimized and the general method of changing the styles of the pizza elements was changed to rely on addClassList and removeClassList.
