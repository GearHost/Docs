# WordPress Optimization
WordPress is the most popular CMS, powering around 25% of all websites in the world and responsible for over 76.5 million blogs. This guide provides a few basic ways to optimize your WordPress site!

#### A Simple Optimization Can Be Done in Your .htaccess File

Create a `.htaccess` file and place it in your /site/wwwroot/. Add the following code and restart your CloudSite.

### Browser Caching
	ExpiresActive On
	ExpiresByType image/jpg "access 1 year"
	ExpiresByType image/jpeg "access 1 year"
	ExpiresByType image/gif "access 1 year"
	ExpiresByType image/png "access 1 year"
	ExpiresByType text/css "access 1 month"
	ExpiresByType application/pdf "access 1 month"
	ExpiresByType text/x-javascript "access 1 month"
	ExpiresByType application/javascript "access 1 month"
	ExpiresByType application/x-javascript "access 1 month"
	ExpiresByType application/x-shockwave-flash "access 1 month"
	ExpiresByType image/x-icon "access 1 year"
	ExpiresDefault "access 2 days"

As you can see you are setting your expiration dates for specific content such as images (.jpg, .gif, .png, text, applications).

>**Note**: One mistake in .htaccess file can make your website unavailable, thus try these changes during off-hours. Also make sure you have a backup of the .htaccess file to restore if that happens.

### Another Optimization is GZip Compression

It’s common sense that smaller files transfer faster than larger ones. Gzip compression makes this possible. Gzip automatically compresses your site’s pages and stylesheets before serving them to the browser. Using this tool can definitely improve your site’s load time. To utilize gzip compression, add this code to your .htaccess file:

	# BEGIN gzip file compression
	# Compress HTML, CSS, JavaScript, Text, XML and fonts
	AddOutputFilterByType DEFLATE application/javascript
	AddOutputFilterByType DEFLATE application/rss+xml
	AddOutputFilterByType DEFLATE application/vnd.ms-fontobject
	AddOutputFilterByType DEFLATE application/x-font
	AddOutputFilterByType DEFLATE application/x-font-opentype
	AddOutputFilterByType DEFLATE application/x-font-otf
	AddOutputFilterByType DEFLATE application/x-font-truetype
	AddOutputFilterByType DEFLATE application/x-font-ttf
	AddOutputFilterByType DEFLATE application/x-javascript
	AddOutputFilterByType DEFLATE application/xhtml+xml
	AddOutputFilterByType DEFLATE application/xml
	AddOutputFilterByType DEFLATE font/opentype
	AddOutputFilterByType DEFLATE font/otf
	AddOutputFilterByType DEFLATE font/ttf
	AddOutputFilterByType DEFLATE image/svg+xml
	AddOutputFilterByType DEFLATE image/x-icon
	AddOutputFilterByType DEFLATE text/css
	AddOutputFilterByType DEFLATE text/html
	AddOutputFilterByType DEFLATE text/javascript
	AddOutputFilterByType DEFLATE text/plain
	AddOutputFilterByType DEFLATE text/xml
	# Remove browser bugs
	BrowserMatch ^Mozilla/4 gzip-only-text/html
	BrowserMatch ^Mozilla/4\.0[678] no-gzip
	BrowserMatch \bMSIE !no-gzip !gzip-only-text/html
	Header append Vary User-Agent
	# END gzip file compression


### The Last Simple Optimization is Image Compression
This can be as simple as resizing your images to the actual size needed to cleaning up any data that might be stored within your image.

If you don’t want to take the time to resize every image by hand, you can seek out WordPress plugins that will do the work for you.

There are also plugins that can optimize your images by takes the image file and removing any unnecessary data bytes stored within. This shrinks your images without any loss of image quality.

### Check Your Website

To check the overall load time of your website or see other ideas of how to improve, here are a few tools:

- GTmetrix
- Pingdom
- Google PageSpeed Insights