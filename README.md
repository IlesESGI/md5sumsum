# Pull request Ilès Benkoussa

I removed all the I/O operations made with the shell spawned process, instead I use a crate MD5 to compute the hash directly.

I also wanted to use per_iter from rayon to parallelize treatments but since the order is important I think we can't do it. The MD5 signature would be random each time we launch the program !