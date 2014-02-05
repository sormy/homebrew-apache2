homebrew-apache2
----------------

[homebrew][h] + [Apache 2.4][a]

[h]: https://github.com/mxcl/homebrew
[a]: https://httpd.apache.org/

**Installation**

    brew tap bpresles/homebrew-apache2
    brew install bpresles/apache2/httpd24

**Configuration**

To use PHP with this apache formula, you must install (or reinstall) php55 with --homebrew-apxs option:

    brew install php55 --homebrew-apxs

or

    brew reinstall php55 --homebrew-apxs	

Also if you use a multithreaded mpm module in Apache, don't forget to build php55 with --with-thread-safety option:

    brew install php55 --homebrew-apxs --with-thread-safety

or

    brew reinstall php55 --homebrew-apxs --with-thread-safety
