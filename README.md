# rosscm.github.io

Source code for personal website [rosscm.github.io](rosscm.gihub.io)
built with [Beautiful Jekyll](https://beautifuljekyll.com/)

### :pencil2: Custom additions

* **_bibliography**
  * **articles.bib**: article info in `.bib` format for jekyll-scholar to build Publication page
  * **thesis.bib**: MSc info in `.bib` format
* **_layouts**:
  * **search.html**: search layout from [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) (still need to configure properly)
* **_pages**: folder for page markdown files (formerly located in parent folder)
* **assets**:
  * **css/custom-styles.css**: CSS code for custom font (family and size) and center align property
  * **img**: custom images for website
* **favicon.ico**: custom website icon
* **Rakefile**: Ruby Makefile to render website and push compiled sources to master branch (necessary due to custom Jekyll plugins like jekyll-scholar; Rakefile [code](http://ixti.net/software/2013/01/28/using-jekyll-plugins-on-github-pages.html))
