#About PHP 7
We're very excited to announce that PHP 7 is now supported on your CloudSite! These are things you need to be know before you upgrade your [PHP version](https://www.gearhost.com/documentation/change-php-version).

##Speed
Most PHP applications will be much faster! Zend released an [infographic](https://pages.zend.com/rs/zendtechnologies/images/PHP7-Performance%20Infographic.pdf) that includes performance benchmarks among popular content management systems and PHP 7 is definitely king. We've done comparisons for WordPress websites and most were reduced by a couple of seconds, making it a big deal for SEO.
<img src="https://raw.githubusercontent.com/GearHost/docs/master/Images/wp_benchmark.PNG" width="75%"/>

##Compatibility
If you're running WordPress, you're likely wondering if your website will still work after upgrading your PHP version. For this concern we recommend installing [PHP Compatibility Checker](https://wordpress.org/plugins/php-compatibility-checker/). It will check if your plugins and themes are compatible with the newer version of PHP. Out of multiple WordPress websites we've tested, we didn't have an issue with the upgrade and did notice much faster load times.

##64-Bit Windows Systems Support
PHP 7 introduces consistent 64-bit support which means both native 64-bit integers and large files will be supported.

##PHP#NG(Next Generation)
While PHP 5.x currently uses Zend Engine II, PHP 7 is running on a faster engine under the name of [PHP#NG](https://wiki.php.net/phpng).

##Spaceship Operator
The spaceship operator is used for comparing two expressions. It returns -1, 0 or 1 when `$a` is respectively less than, equal to, or greater than `$b`.

    <?php
    // Integers
    echo 1 <=> 1; // 0
    echo 1 <=> 2; // -1
    echo 2 <=> 1; // 1
    
    // Floats
    echo 1.5 <=> 1.5; // 0
    echo 1.5 <=> 2.5; // -1
    echo 2.5 <=> 1.5; // 1
     
    // Strings
    echo "a" <=> "a"; // 0
    echo "a" <=> "b"; // -1
    echo "b" <=> "a"; // 1
    ?>


##Removed Extensions and SAPIs
Several extensions and SAPIs are being removed, we provide the list here.
 
**Extensions:**

- ereg
- mssql
- mysql
- sybase_ct

**SAPIs:**

- aolserver
- apache
- apache_hooks
- apache2filter
- caudium
- continuity
- isapi
- milter
- nsapi
- phttpd
- pi3web
- roxen
- thttpd
- tux
- webjames

**Extensions not yet ported to PHP 7:**

- interbase
- mssql
- oci8
- pdo_dblib
- pdo_oci
- sybase_ct



>**Tip:** For additional information regarding PHP 7 or assistance with migrating to this new environment we recommend checking out this [guide](http://php.net/manual/en/migration70.php).