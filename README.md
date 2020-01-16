# addlicense

The program ensures source code files have copyright license headers
by scanning directory patterns recursively.

It modifies all source files in place and avoids adding a license header
to any file that already has one.

## install

    go get -u github.com/google/addlicense

## usage

    addlicense [flags] pattern [pattern ...]

    -c copyright holder (defaults to "Google LLC")
    -f custom license file (no default)
    -l license type: netgain, apache, bsd, mit (defaults to "netgain")
    -p purpose of file: inserts a string for later replacement, "purposereplace", or inserts purpose statement of code
    -a author of file: inserts a string for later replacement, "authorreplace", or inserts author name
    -y year (defaults to current year)
    -v verbose, prints names of all files modifed

The pattern argument can be provided multiple times, and may also refer
to single files.  The pattern arg is either an individual filename or a directory.

## license

Apache 2.0

This is not an official Google product.
