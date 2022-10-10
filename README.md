# TNS-SHELL
===


TNS is a simple implementation of a shell in C.
It demonstrates the basics of how a shell works.
That is: read, parse, fork, exec, and wait.  Since its purpose is demonstration
(not feature completeness or even fitness for casual use), it has many
limitations, including:

* Commands must be on a single line.
* Arguments must be separated by whitespace.
* No quoting arguments or escaping whitespace.
* No piping or redirection.
* Only builtins are: `cd`, `help`, `exit`.

Running
-------

Use `gcc -o tns src/main.c` to compile, and then `./tns` to run. If you would
like to use the standard-library based implementation of `tns read_line()`, then
you can do: `gcc -DLSH_USE_STD_GETLINE -o tns src/main.c`.

Contributing
------------

Thanks to Stephen Brennam's tutorial on C and shell we are able to make this happen.
We looking to extend this shell with more features. we will be accepting any pull requests that has good features or that fixes bug. 
We hope to see more contributors to this program.

License
-------

This code is in the public domain (see [UNLICENSE](UNLICENSE) for more details).
This means you can use, modify, and distribute it without any restriction.  I
appreciate, but don't require, acknowledgement in derivative works.
