Direkt SPEED - Dev2Production Replaced with Minify a PHP Version with Bookmarklets to Create even Static Versions
=================================================================================================================

https://github.com/mrclay/minify/blob/master/min_extras/cli/minify.php

Like rewrite-uris.php, it's not standalone: it autoloads from min/lib

Example usages:

./minify.php ../../min_unit_tests/_test_files/js/*.js

./minify.php -d../.. ../../min_unit_tests/_test_files/css/*.css

echo "var js = 'Awesome' && /cool/;" | ./minify.php -t js

echo "sel > ector { prop: 'value  '; }" | ./minify.php -t css

Basically, if you pump data in via STDIN, a type (-t) is required. And if you want URI
rewriting to work, you must supply your DOC_ROOT via -d.

To get help: ./minify.php -?



