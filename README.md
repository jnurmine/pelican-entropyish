# Entropyish for Pelican

This is Entropyish. It's a somewhat stripped-down remix of Entropy Wordpress
theme by Timothy Long.

## Not Implemented

Not all features of Pelican are supported. This is because I made the remix for my own site
where I don't need all features.

The basic HTML exists but it's not properly using the CSS i.e. likely looks fugly:

-    archives
-    article_infos
-    period_archives
-    authors
-    categories
-    category
-    tags
-    taglist

The HTML templates, including the unworking ones, were simply copied from a
Pelican example theme.

Google analytics might or might not work. Basic implementation is included via
whatever was in the Pelican example theme. I don't use Google analytics myself
so I didn't waste time with those parts.

## Settings Used by This Theme

* `FOOTER_TEXT = 'Whatever you want` : the footer text
* `SITESUBTITLE = 'Your awesome blog'` : subtitle, appears under the name

### Recommended Settings

I recommend to use the following in settings.py:

```python
DISPLAY_CATEGORIES_ON_MENU = False
DIRECT_TEMPLATES = ([('index')])
DEFAULT_PAGINATION = 10

# Disable archives, authors, etc.
ARCHIVES_SAVE_AS = ''
AUTHORS_SAVE_AS = ''
CATEGORIES_SAVE_AS = ''
TAGS_SAVE_AS = ''
```

## Other Notes

The latest post is displayed in whole. Older articles are shown with the
title, a oneliner summary (from the "Summary"-tag) and a "read more" link.
Pagination is provided to access even older posts.

The graphics are as-is from Entropy.

There probably are bugs, such as bold or italic not working in a certain place.
When I encounter those I'll fix them. In the meanwhile, patches are welcome!

## Credits

### Authors

* [Jani Nurminen](http://kippura.org) (Porcini for Pelican)
* [Timothy Long](http://timothy-long.com) (Entropy for WordPress)

## License

CC-BY-SA, that's the way Timothy wanted it so who am I to argue.

