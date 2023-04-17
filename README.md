# CSC Website – Dev Guide

_Eventually this guide will become part of the Handbook on the website._

_Please flag any issues with these instructions as I have mostly written from memory!_

## Install
1. First, install ruby, the Jekyll rubygem and other pre-requisities by following the instructions here: [MacOS](https://jekyllrb.com/docs/installation/macos/).
2. Clone this repo using `git clone` or GitHub Desktop.
   - The master branch is called `gh-pages`.
4. `bundle install`
   - This builds the website locally on your machine.
   - For Apple Silicon (ARM) e.g., M1 Mac users, you may need to run `arch -arch x86_64 bundle install` if the above does not work.
5. `bundle exec jekyll serve --livereload`
   - This runs the website locally on your machine.
   - For Apple Silicon (ARM) e.g., M1 Mac users, you may need to run `arch -arch x86_64 bundle exec jekyll serve` if the above does not work.
   - The `--livereload` option enables you to see changes to your code automatically in your browser, without rebuilding the code.
   - NB: the `--livereload` option does not work with changes to the `config.yml` file. In this case, you will need to re-run `bundle exec jekyll serve --livereload`.
6. View in your browser with the URL: [http://localhost:4000](http://localhost:4000/)

## Developer Guide

The CSC site is built on Jekyll and incorporates Bootstrap v5 for CSS and java. Useful links relating to these are in the [Resources](#Resources) section below.

### Website structure
For a thorough explanation of this, consult the Jekyll website. This is an abridged alternative. The directory structure of the website is approximately as follows:
```
.
├── _data
├── _layouts
├── _includes
├── _sass
├── _site
├── assets
│   ├── css
│   ├── img
│   └── js
│
├ ._config.yml
├ Gemfile
└ multiple .md files
```

`_data` – this folder contains .yml files which contain the actual 'data' within the website. i.e.: the content that goes into the calendar, info about team members, etc. Once we have designed the layouts of the pages, we should be able to just update the files in here with new content. In theory...

`_layouts` – this folder contains html files which determine different page layouts. The layouts can be called in the YAML frontmatter of a page, e.g.: `layout: platforms` applies the `_layouts/platforms.html`

`_includes` – this folder contains html snippets which can be 'included' in other pages, hence it's called "*_includes*". For instance, the code for the CSC calendar is in here which is used in two places: 1) the home page and 2) the actual dedicated Calendar page. This enables modular design and avoids code duplication.

`_sass` – this contains the CSS for the site, which determines colours, padding, background colours, etc. SASS is basically fancy, enhanced CSS. **Note:** styling is also controlled in some other files, such as the `_config.yml`, `assets/css/` and a few other places.

`_site` – Do **NOT** edit these files. Jekyll creates the website from the .md, .html, .css, etc. files and puts the compiled website in this folder.

`assets` – contains CSS, Javascript and image files. Can have subdirectories, such as `img/team` which contains all the photos of the CSC team.

`._config.yml` – The configuration file for the website. Determines various important things which propagate across the entire site. Can have lots of content.

`.md files` – Markdown files which form the basic building blocks of the website. In Jekyll, if you use the Liquid filter `{{ content }}` then the contents of the .md file are input. You can also call files from the `_includes` folder using the Liquid tag `{% include file-in-_includes.html %}`.

### Demo: How to Create a new page

Let's pretend to create the Team page on the website.

1. Create markdown file: `team.md`
   - NB: these are all currently created in the root dir. Might change this in future.
2. Specify the layout for the file. In this case, the Team page comes under the About Us section of the main navbar. We can also set the page title here. So, edit frontmatter of `team.md`:
    ```
    ---
    layout: aboutus
    title: Meet the Team
    ---
    ```
   - `layout: aboutus` calls the `_layout/aboutus.html` file, which in turn uses Liquid: `{% include subnav-aboutus.html %}`, hence we get the correct subnav bar.
   - `title: Meet the Team` is assigned a `<h1>` heading tag in the `aboutus.html`.
3. Create a file in `_includes` which contains the the structure of the Team page. I've already made one called `team.html`.
4. Create the content (or 'data') for the page in `_data/team.yml`. 
   - This shows how powerful Jekyll and Liquid can be because you can simply add a new CSC team member to this file and the html in `_includes/team.html` has already been configured to loop through however many team members exist in the `.yml` file!
   - NB: to call the fields in `_data/team.yml`, in your .html file, you need to use a [Liquid tag](https://jekyllrb.com/docs/liquid/tags/), a bit like this: `{% for name in site.data.team[site.locale].team.people.name %}`, which will loop over all the team member names.
5. View your changes at [http://localhost:4000](http://localhost:4000/)

If you're happy with your changes, push your feature branch to the repo on GitHub, submit a pull request and ask someone to review your changes.

## Resources

### Jekyll
The nuts and bolts of the website.
- [Quickstart guide](https://jekyllrb.com/docs/) – useful intro to installing Jekyll.
- [Step-by-step](https://jekyllrb.com/docs/step-by-step/01-setup/) – this is a good, quick tutorial for making a Jekyll site. Really digestible way of understanding the directory structure of a Jekyll site.
- [Guide to Liquid](https://jekyllrb.com/docs/liquid/) – Liquid is a templating language, used by Jekyll. It's really great for programming a website in an efficient way. Allows logic, for loops and such.

### Bootstrap
Determines the styling of the website, such as CSS and Java. 

**Important:** Bootstrap is designed to be responsive, which means that the website is optimised for both large computer screens and small mobile phone screens. 
- [Docs](https://getbootstrap.com/docs/5.0/getting-started/introduction/) – The lefthand bar contains links to all the different possibly classes contained in Bootstrap. This is _**really**_ useful, for instance if you want to design a page with different sized columns, add in buttons, layout images, etc, etc.
- [Page Layouts](https://getbootstrap.com/docs/5.1/layout/columns/) – specifically working with rows/columns.
- [Bootstrap Tutorial Video](https://www.youtube.com/watch?v=rQryOSyfXmI) – 1.5hr intro video on Bootstrap. Covers a lot of ground. I found this very helpful. You can skip through some bits, such as pop-ups and stuff, which we won't need.

### Useful Tools for Web Design
- [CSS Peeper](https://chrome.google.com/webstore/detail/css-peeper/mbnbehikldjhnfehhnaidhjhoofhpehk?hl=en) – a really handy Chrome plugin for investigating web page code structures. Like a lightweight version of your browsers in-built Dev Tools (which you can access by pressing `F12`).
- [coolers.co](https://coolors.co/) – Great website for choosing complementary colours.





