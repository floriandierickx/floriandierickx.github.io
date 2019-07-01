# Jekyll and website setup
## Run local site
- **Run local jekyll site:** 'bundle exec jekyll serve'
## Jekyll example sites
- Nice **jekyll example site**: https://amor.cms.hu-berlin.de/~jaeschkr/#
## Plugins
- Jekyll plugins overview: https://github.com/planetjekyll/awesome-jekyll-plugins
- **In-site citations**: see http://weinan.io/2017/03/06/using-papers-and-manuscripts-to-do-correct-citation.html
### RSS Feed with blogposts: Jekyll-feed & Jekyll-planet
- Atom feed inclusion: https://github.com/jekyll/jekyll-feed
	- OK
- Jekyll-planet (Planet Pluto) to included other RSSs in blog: https://github.com/feedreader/jekyll-planet
	- Usage (steps)
		- include/edit pluto.ini
		- bash: 'gem install pluto' to install
		- bash: **pluto update planet.ini** [original: pluto build planet.ini]
		- create blogposts: **ruby -r 'jekyll/planet' -e 'JekyllPlanet.main'**
	- Note on how to assign automatic tags to websites:
		1. input tag name in website title in 'planet.ini'
		2. add `tags:       [#{item.title}]` to line 52 of `tool.rb` in `/Users/florian/.rvm/gems/ruby-2.6.0/gems/jekyll-planet-0.2.1/lib/jekyll/planet/tool.rb` [=DONE]
- Tagging: according to https://codinfox.github.io/dev/2015/03/06/use-tags-and-categories-in-your-jekyll-based-github-pages/
	- Tag categories:
		- website: posts related to website
		- rss-repost: interesting blogposts from the internet (t-rss feed)
		- *twitter: twitter posts
		- *input-output:
- Find out where gems are installed (ruby): `gem environment`s
## Update and maintenance of Jekyll and Gems
- Gem (Ruby)
	- Update gem : 'gem update --system'
	- Update gems: 'bundle update --all' --> updates all gems in gemfile
	
# Annotation and comments of Website: hypothes.is
- Edit of '_layouts/default.html'. See https://github.com/floriandierickx/floriandierickx.github.io/commit/bc61aa0c4dedd016f086eda4e807ff2b196b88c9

# Conversion of twitter threads to HTML: TweetView

- https://github.com/hrbrmstr/tweetview/blob/master/README.md (R package)
	- Solution to error installing tidyverse: https://medium.com/@kadek/how-to-install-the-tidyverse-r-via-homebrew-macos-10-14-d749d2136cf1
- Thanks to @hrbrmstr for helping out with formatting and publishing ! -> https://github.com/hrbrmstr/tweetview/issues/1

# Comments integration: Discuss
- Add script to pages ('_layouts/default.html', ...)
- See commit https://github.com/floriandierickx/floriandierickx.github.io/commit/9823e711e56f555c64ff44d8f016296b9441bc81

# Publishing of markdown in dynamic html: bookdown in dynamic iframe
- Integration commit: https://github.com/floriandierickx/floriandierickx.github.io/commit/3f0528db235504020757c46bd8751769a2e9f207
- Inclusion of iframe: http://seankross.com/2016/11/17/How-to-Start-a-Bookdown-Book.html (for https://floriandierickx.github.io/library/copernicus/index.html)

# Online Library with Altmetric Badges [+ Annotation of Pdfs: not yet implemented, suggestions welcome] : bib-list.js [hypoethes.is and nextcloud upload]
## Online library: bib-list.js
- First integration: 
## Integration of altmetric badges in literature list
- See https://github.com/floriandierickx/floriandierickx.github.io/commit/faba83911807f5807d280c58afce5de2000fcef4

# General website formatting
## Find and replace fonts in css files
regex search and replace with font-family:(?:.*);
## Change spacing between menu items
change 'margin-right' in nav ul li, footer ul li {
## Icons (Font Awesome and Academicons)
- Start: https://fontawesome.com/start or https://jpswalsh.github.io/academicons/ 
- Look for icons: https://fontawesome.com/icons/ + include icons in html:
	- **Font Awesome**: Include href link, around icon: <a href="http://....." target="_blank">ICON <i> LINK </a>
	- **Academicons**: 
## Change formatting of library titles
- capture in '<b>' and '<\/b>' (see https://github.com/floriandierickx/floriandierickx.github.io/commit/3d79b96da69ef065bb88f0228e7e44cba38ddf8d)


		