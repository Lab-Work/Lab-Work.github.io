# README for website configuration and content modification
### Updated Feb. 2021

This document contains information for setting up this website and instructions for modifying its content. The original theme for this website is 'Massively' by HTML5 UP (html5up.net | @ajlkn). Free personal and commercial use under the CCA 3.0 [license](https://html5up.net/license) is permitted.

## Site hosting
This site is hosted using Github Pages. Mechanically, the publicly hosted version is compiled from the source code in this repository, only. When a commit is made to the repository, the site is regenerated and the updated version is immediately live.

This means that if updates are being made directly to the site with no local testing (see next section), they should be made incrementally and checked for correctness using the live version. Recent updates may not be immediately apparent because of browser content caching; it is recommended to open a new 'private browsing' window and navigate to the site to check recent updates. Updates can be rolled back easily by reverting commits to the repository.

## Site setup on local computer
In order to make more complex updates to the site, it is recommended to set up the site on a local computer. This allows better debugging and trial and error without interfering with the public version of the site. More instruction detail is provided [on the Github Pages Guide](https://docs.github.com/en/github/working-with-github-pages/testing-your-github-pages-site-locally-with-jekyll).

The very brief version of the instructions is as follows:
1) Just go ahead and read up on [how to install Jekyll](https://jekyllrb.com/). It's not too hard and particularly easy with a package manager like Homebrew.

2) Download the current version of [this repository](https://github.com/Lab-Work/Lab-Work.github.io/archive/master.zip), save it to any folder you want, and unzip it. Alternatively, you can [clone this repository](https://github.com/Lab-Work/Lab-Work.github.io.git) via ```git```. It is recommended to download the source files and construct a new repo for replicating the site, not forking this repo.

3) Open a terminal window or a command line and ```cd``` to that location.

4) Execute from the command line ```bundle exec jekyll serve```. You can now access the site at [http://127.0.0.1:4000/](http://127.0.0.1:4000/) in your browser.

## Source file structure
This section explains the repository's source file structure, including basic descriptions of the content of each directory or file. The structure may seem convoluted, but it is designed with modularity and easy updates in mind. A basic understanding of this structure is all that is needed to make minor updates to website content using a simple text editor (no HTML coding needed).

	Lab-Work.github.io
	|---- _bibliography				(ToDo) directory for publications bibliography
	|---- _data						YML data files for lists of things
	|---- _includes					HTML templates for page elements
		|---- foot.html					page footer (location, contact)
		|---- head.html					page title and some other stuff
		|---- nav.html					navigation bar
		|---- scripts-main.html			Javascript scrolling and animations
		|---- tracking.html				Google page analytics tracker
	|---- _layouts					HTML templates for page layouts
	    |---- blog.html					layout for blog full listing (see /blog.md)
		|---- page.html					layout for most site pages
		|---- post.html					blog post singular page layout
	|---- _pastprojects				(not used)
	|---- _people					MD files for each team member, past and present
	|---- _posts					MD files for blog updates
	|---- _projects					MD files for research projects, past and present
	|---- _research					MD list files for research project groupings
	|---- _site						auto-generated site backend files
	|---- _teams					MD list files for team member groupings
	|---- assets					style and element files for site
	|---- download					directory for site download files (papers, postings)
	|---- images					directory for all site images
	|---- papers					(not used)
	|---- therebound + similar		special site pages for article we wrote and hosted
	|- .gitignore					Git list for files to ignore when syncing repo
	|- _config.yml					site configuration file
	|- about.html					site page: Dan's "About" page
	|- blog.md						site page: blog main page/full listing
	|- data.html					site page: public datasets from past work
	|- elements.html				unlisted site page for style/element ref (useful)
	|- Gemfile + Gemfile.lock		site dependencies
	|- google...html				site-specific Google analytics indicator
	|- index.html					site page: home page (i.e., top level domain page)
	|- LICENSE.md					license file
	|- publications.html			site page: group publications
	|- README.md					this file
	|- robots.txt					tells site crawlers what pages/files not to index
	|- research.html				site page: research projects
	|- service.html					(ToDo) site page: Dan's service work
	|- sitemap.xml					(ToDo update?) site map that helps SEO + indexing
	|- teaching.html				site page: Dan's teaching work
	|- team.html					site page: group team members


## Routine site edits

The directories and files of note for small website updates are: `_people`, `_posts`, `_projects`, `_research`, and `_team`. Simple text changes or additions to files in these directories are automatically reflected by the site's HTML logic. The markdown files in `_people` correspond directly to the team member group lists in `_team`. The markdown files in `_projects` correspond directly to the project lists in `_research`. If a new person or project is added as a markdown file, its key value must be added to a corresponding list in order for the page to populate. Additions to the `_posts` directory automatically populate chronologically in the blog.

Both markdown and HTML syntax should work for .md files in the above referenced directories. A markdown syntax guide with complementary HTML syntax for most items is available [here](https://www.markdownguide.org/basic-syntax/). It is mostly recommended to copy existing files based on the elements and format desired in new files and edit the content. Some of the files are a strange mix of YML, MD, and HTML syntax. Of particular note are `<p>` paragraph tags, `<li>` list item tags, and quotation mark consistency (un-closed quotes can actually cause build errors for the whole site).


## More fundamental site edits

Many site settings are available in `_config.yml`. These should be changed with caution, but are important if replicating this site elsewhere.

Primary site pages are `index.html`, `about.html`, `data.html`, `publications.html`, `research.html`, `teaching.html`, `team.html`, and `blog.md`/`_layouts/blog.html`. Most of this content must be edited with HTML syntax. Pages can be added or removed from the navigation bar by editing `_includes/nav.html`.

The home page is `index.html`; the panels of content above the blog, below the navigation bar, are all static HTML-coded in this file. This is sort of the welcome area for the site, so it should introduce the content appropriately.

The linked pages from the navigation bar are controlled by the site page HTML files. But some of these (currently Research, Team, and Blog) are just structural code and have their content generated from the component files in other directories. The structural code should be edited with care.


## Future site enhancements

1. Bibtex file parser that auto-generates the publication page content so the Bibtex entries can be more easily organized for our internal use. Also, all paper pre-prints download from this site instead of link to external.
2. Making Dan's personal pages more clear in their purpose/organization.
3. Links to other relevant sites that we are affiliated with (e.g., Vanderbilt CEE).



## Other features

### Google analytics
This site is set up with anonymized Google analytics for the purpose of understanding its exposure on search. The `google...html` file in the top directory, along with the `{% include tracking.html %}` in the page layout accomplish these analytics.

### Auto-Generating Sitemap
The sitemap is supposed to be auto generated. Change the sitemap variable in front matter of each page, like so.
```
sitemap:
    priority: 0.7
    lastmod: 2017-11-02
    changefreq: weekly
```

## Credits
### Original README from HTML5 UP
```
Massively by HTML5 UP
html5up.net | @ajlkn
Free for personal and commercial use under the CCA 3.0 license (html5up.net/license)

This is Massively, a text-heavy, article-oriented design built around a huge background
image (with a new parallax implementation I'm testing) and scroll effects (powered by
Scrollex).

AJ: aj@lkn.io | @ajlkn


Credits:
	Demo Images: Unsplash (unsplash.com)
	Icons: Font Awesome (fortawesome.github.com/Font-Awesome)
	Other:
		jQuery (jquery.com)
		Misc. Sass functions (@HugoGiraudel)
		Skel (skel.io)
		Scrollex (github.com/ajlkn/jquery.scrollex)
```
