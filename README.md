# can_R_learn_from_Julia
Data for a UserR! 2016 talk

This repository contains a UseR! talk that tries to show how 
Julia achieves performance. This is done by comparing an 
implementation of the colMeans function in Julia. 

colMeans(), in R, calls the do_colsums() function written in C.
To compute 1000 invocations of colMeans on a 100,000 element 
complex Vector takes 2 secs on my underpowered MacBook.

Implemented in pure R, and using the optimization level 3
of the GNU R bytecode compiler, the comptuation takes about
30 secs.

A straightforward Julia implementation takes .2 seconds.
