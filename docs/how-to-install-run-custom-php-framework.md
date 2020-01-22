...

# How To Install & Run Custom PHP Framework
PHP (Hypertext Preprocessor) is a widely-used open source general-purpose scripting language that is especially suited for web development and can be embedded into HTML. The purpose of this guide is to walk you through installing a custom PHP framework (oldest version to the newest).

### Read and Follow These Steps:
1. **Download** PHP from this link, this is our own compiled version of PHP 7.3 which includes wincache and other extensions that help with perormance: [PHP Download](https://github.com/GearHost/Docs/raw/master/docs/php.zip)
2. **Extract** the .zip file and **upload** its content into \site\bin\ via FTP you should have \site\bin\php\ after uploading the files
6. Go to **CloudSite > Configuration** tab
7. **Scroll** down and **Add** a `New Handler Mapping`
	1. Extension: ***.php**
	2. Script Processor Path: **C:\home\site\bin\php\php-cgi.exe**
	3. click on **Save Configuration** at the bottom
8. Create a [info.php](https://www.gearhost.com/documentation/create-php-info-page) page
9. Go ahead and **stop** your cloudSite
10. Then **start** it and go to {CloudSiteName}.gearhostpreview.com/info.php

If you have followed these steps, a page should up come with all the information about your PHP version.
