LLNW collectd port for FreeBSD 
==============================

* Upstream:  http://svn.FreeBSD.org/ports/head/net-mgmt/collectd5
* FreshPorts:  http://www.freshports.org/net-mgmt/collectd5/
* Our Port differences:  https://github.com/llnw/collectd-build-freebsd/compare/upstream...LLNW

We build [our branch of collectd][llnw collectd] 

Building the port:
------------------
* `make -DBATCH install clean`

Port maintenance:
-----------------

* Alter DISTVERSION, DISTVERSIONSUFFIX in Makefile
* Update the distinfo checksums:  `make makesum`

Repo maintanance:
-----------------

* Repo and branch **upstream** should be from

    ```git svn clone https://svn.FreeBSD.org/ports/head/net-mgmt/collectd5 collectd-build-freebsd```
* `git svn rebase` to update local branch **upstream** (follows ports svn HEAD)
* Use standard git merge to maintain other local branches

  [llnw collectd]: https://github.com/llnw/collectd/
