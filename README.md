# Pull request Ilès Benkoussa

I removed all the I/O operations made with the shell spawned process, instead I use a crate MD5 to compute the hash directly.

I also useed par_iter from rayon to parallelize treatments.
