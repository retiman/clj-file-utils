DESCRIPTION
===========

Unix-like filesystem manipulation utilities for Clojure, wrapping Apache
Commons IO.

Includes a `pchmod` function which changes file permissions in a portable
way.

Please consider upgrading to Clojure 1.3.0 and using the file manipulation functions in the standard library.

IMPLEMENTED FUNCTIONS
=====================

    cp
    cp-r
    directory?
    exists?
    file
    file?
    ls
    mv
    rm
    rm-f
    rm-r
    rm-rf
    size
    touch
    mkdir-p
    chmod

USAGE
=====

    user=> (use 'clj-file-utils.core)
    nil
    user=> (exists? "foo.txt")
    false
    user=> (touch "foo.txt")
    nil
    user=> (exists? "foo.txt")
    true
    user=> (rm "foo.txt")
    nil
    user=> (.getParent (file "/path/to/foo.txt"))
    "/path/to"

AUTHORS
=======

Extracted from <http://github.com/mmcgrana/clj-garden> by Mark McGranaghan <mmcgrana@gmail.com>

Updates by Nate Murray <nate@natemurray.com>, Min Huang <min.huang@alumni.usc.edu>
