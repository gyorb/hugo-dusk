Simple minimalistic dark theme for [Hugo](https://gohugo.io/).

![screenshot](https://github.com/gyorb/hugo-dusk/blob/master/images/tn.png "screenshot")

For more images check out the [images directory](https://github.com/gyorb/hugo-dusk/blob/master/images/).

Features
--------------------

* Responsive minimalistic design
* Configurable theme colors (with custom css file)
* Syntax highlight with builtin [Chroma](http://gohugo.io/content-management/syntax-highlighting/)
* [OpenGraph](http://ogp.me/), [Twitter cards](https://dev.twitter.com/cards/overview) support
  * Optionally generate opengraph images for the posts
* [Mastodon](https://joinmastodon.org/) [verification](https://joinmastodon.org/verification)
* [Fediverse creator tag](https://blog.joinmastodon.org/2024/07/highlighting-journalism-on-mastodon/)
* [Disqus](https://disqus.com/) comments support
* [Utterances](https://utteranc.es/) comments support
* [Google analytics](https://www.google.com/analytics/)
* Configurable pagination for posts
* Lazy menu
* Custom 404 page

Installation
--------------------

~~~sh
$ mkdir themes
$ cd themes
$ git clone https://github.com/gyorb/hugo-dusk
~~~

Configuration
--------------------

Example configuration:

~~~~toml
baseurl = "/"
title = "My site."
copyright = "Copyright (c) 2017, all rights reserved."
canonifyurls = true
languageCode = "en-US"
paginate = 3
theme = "hugo-dusk"

googleAnalytics = ""
disqusShortname = ""

[params.author]
  name = "Author name"
  intro = """\
    'hugo-dusk' theme for [hugo](https://gohugo.io/) an open-source static site generator.\
  """

SectionPagesMenu = "main"

[taxonomies]
  archive = "archive"
  blog = "blog"
  category = "categories"
  series = "series"
  tag = "tags"

# Configure syntax highlight
[markup]
  [markup.highlight]
    style = "gruvbox"  # dark themes: monokai, api, fruity, native, rrt, swapoff ... https://xyproto.github.io/splash/docs/longer/all.html

[[menu.main]]
  name = "Blog"
  weight = -120
  identifier = "blog"
  url = "/blog/"

[[menu.main]]
  name = "Tags"
  weight = -110
  identifier = "tag"
  url = "/tags/"

[[menu.main]]
  name = "Archive"
  weight = -100
  identifier = "archive"
  url = "/archive/"

[params.meta]
  keywords = "blog, tech"
  description = "Personal blog."
[params.meta.fediverse]
  creator = "@username@mastodon.server" # https://blog.joinmastodon.org/2024/07/highlighting-journalism-on-mastodon/

[params]
  mainSections = ['blog']
  github = "github id"
  gitlab = "gitlab id"
  twitter = "twitter id"
  linkedin = "linkedin id"
  email = "myemail"
  theme_colors = "default-dark" # uses color css file under static/css/default-dark.css
  enable_separate_main_page = false # enable a separate main page with author intro and recent posts instead of the list of posts
  generate_opengraph_image = false # enable opengraph image auto generation
  utterancesRepo="REPO_NAME" # Utterances is enabled when this param is set
  utterancesTheme="github-dark" # Default: github-dark
  utterancesIssueTerm="pathname" # Default: pathname
[params.mastodon] # https://joinmastodon.org/verification
  username = "username"
  server = "https://example.com"
~~~~

Automatic opengraph image generation
--------------------

Generating opengraph images for the posts can be enabled with the
generate_opengraph_image config value.

The generated opengraph image contains the site baseURL and the page title
for a post.
Two images are required in the assets directory use this feature:
  - "opengraph-post-blank.png" 1200x630px this will contain the baseURL and the title
  - "opengraph-logo.png" 400x400px a general logo for pages which are not posts

Example base images can be found in the assets directory which were created from the
svg files in the images directory.
A generated example image looks like this:
![opengraph exampe](https://github.com/gyorb/hugo-dusk/blob/master/images/opengraph.png "opengraph example")

