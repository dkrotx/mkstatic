# mkstatic

mkstatic is Perl-script which creates a package (self-executable Shell-file) from given executable and it's libraries. Dependencies of libraries itself are also tracked.
The idea is to launch executable file on another machine even if it DOES NOT HAVE all the libraries installed.
The goal is similar to statically linked binaries, although it has nothing with actual linkage.

## INSTALLATION

````
$ sudo make install
````

## USAGE

Your steps are very straightforward:
- Run mkstatic with your binary: `$ mkstatic path/to/your/binary_file`
- Copy result-file (path/to/your/binary_file.static) to target host
- Launch your binary_file.static (the same usage as using original binary_file)

You may see details and options using `mkstatic --man`

## See Also
Original review: http://dkrotx-prg.blogspot.ru/2013/03/mkstatic.html
