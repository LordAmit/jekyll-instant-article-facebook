# Facebook Instant Article for Jekyll ⚡ RSS Feed

Facebook instant article rss feed generator for Jekyll static site. It is based on liquid tags and insanely simple!

## Setup / Installation / Configuration
Installation requires downloading an XML file based on which `RSS Feed` will be generated. It is dependent on some `Jekyll-plugins` and some configurations in `_config.yml` file.

### 1. Downloading XML file

Please go to the [Releases](https://github.com/lordamit/jekyll-instant-article-facebook/releases) section,  download the latest release and extract it.

### 2. Installing jekyll-plugins
You need the following plugins:
- [jekyll-figure](https://github.com/paulrobertlloyd/jekyll-figure)

### 3. Configuring \_config.yml file
Based on the settings, your rss feed generator will be able to use default image as feature image, default titles and some other things.
```yaml
title: Your website title here
description: "Your Website description here"
# change it to your site address.
# depending on your configuration, you might have to add a / after the address.
url: http://lordamit.github.io
default_bg: sitelogo.png
baseurl: ""
owner:
  name:           Your name here
  avatar:         images/Your_image.jpg
```
That should be enough. I should emphasize on the fact that these are also dependent on your jekyll-configuration, so you might have to tweak around a bit.

## Customizing Instant Article based on Post
The Instant feed RSS generator is your post aware, and based on the YAML front matter, it will insert / replace values - making your article suitable for Facebook instant article publication.

```yaml
# image is used to specify an image for your article.
# If not used, it will use the default sitelogo specified in _config.yml
image: "ImageURL here"
# based on instantfeedback - it will show like buttons for feedback in your post.
# Enter true or false
instantfeedback: true|false
# if you have used any image or contents from others, please give it credit.
credit: "Credit text here"
```

That should do it! Please head over to the ["Sites using"](https://github.com/lordamit/jekyll-instant-article-facebook/wiki/Sites-using-jekyll-instant-article-facebook) section to include your site's address, so that I can know who are using it. :)

Thank you!

## References

- [Facebook instant article documentation](https://developers.facebook.com/docs/instant-articles/)
- [Instant article quick start](https://developers.facebook.com/docs/instant-articles/quickstart)
- [Instant Article publication through RSS](https://developers.facebook.com/docs/instant-articles/publishing/setup-rss-feed)
