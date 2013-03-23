mkstatic
========

mkstatic is Perl-script wich creates a package (self-executable Shell-file) from given executable and it's libraries. Dependencies of libraries itself are also tracked.
The idea is to launch executable file on another machine even if it DOES NOT HAVE all the libraries installed.
The goal is similar to statically linked binaries, although it has nothing with actual linkage.

Your steps are very straightforward:

    - You call mkstatic binary_file
    - Copy result-file (binary_file.static) to target host
    - Launch your/binary_file.static (the same usage as using original binary_file)

You may see details and options using mkstatic --man
