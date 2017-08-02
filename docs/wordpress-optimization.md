# WordPress Optimization
WordPress is the most popular CMS, powering around 25% of all websites in the world and responsible for over 76.5 million blogs. This guide provides a few basic ways to optimize your WordPress site!

### Installing & Setup WP Super Cache
WP Super Cache plugin is one of the best caching options. It is easy to install and configure.

1. **Install WP Super Cache** in WordPress
2. Go to **Plugin Admin Page**
3. Select **Caching** on and Click **Update Status**

>**Note**:The generated cache pages by WP Super Cache are stored as HTML or PHP files on your server. You can delete these cached pages from your server by clicking on Delete Cache button.

1. Click **Advanced Tab** in the Caching Section
2. Select **Simple** in the Cache Delivery Method
3. Under Miscellaneous click:
	1. **Don't cache pages for known users**
	2. **Don't cache pages with GET parameter**
	3. **Compress pages so they're served more quickly to visitors**
	4. **Cache rebuild. Serve a supercache file to anonymous users while a new file is being generated**
4. Under Advanced click:
	1. **Mobile device support**
	2. **Clear all cache files when a post or page is published or updated**
	3. **Extra homepage checks**
5. Click **Update Status**
6. Go to **CDN Tab**
7. Select **Enable CDN Supoort** and **Skip https URLs to avoid "mixed content" errors**
8. Go to **Preload Tab**
9. Then click **Preload Cache Now**

### Installing & Implement Smush Image Compression & Optimization
Smush resizes, optimizes and compresses all of your images. 

1. **Install Smush** in WordPress
2. **Activate Smush** in Plugin Tab
3. Go to the media tab and click **WP Smush**
3. Click the blue button **Bulk Smush Now**
4. **Repeat** this process until all your images have been Smushed

### Check Your Website

To check the overall load time of your website or see other ideas of how to improve, here are a few tools:

- GTmetrix
- Pingdom
- Google PageSpeed Insights