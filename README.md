# clj-ns-name

Give Clojure/ClojureScript buffers the name of the Clojure namespace, rather
than the filename. E.g. if you open `clojure/core.clj` instead of the buffer
being called `core.clj` it will be called `clojure.core`.

To disambiguate the project name is added between angle brackets, determined by
Projectile, if necessary.

The name is taken from he `ns` form, which has to be first in the file. Changes
to the ns form are reflected upon save.

Run `(clj-ns-name-install)' to add function advice to activate this package. Run
`(clj-ns-name-uninstall)' to disable it again. Note that disabling will not
revert the buffer names.

<!-- license -->
## License

Copyright &copy; 2018-2022 Arne Brasseur and Contributors

Licensed under the term of the GNU General Public License, version 3. 
<!-- /license -->
