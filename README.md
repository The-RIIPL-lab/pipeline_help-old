# RIIPL documentation builder

RIIPL documentation is generated quickly and easily using [SPHINX Autodoc](http://www.sphinx-doc.org/en/stable/ext/autodoc.html).

### Who creates documentation?
Anyone on the RIIPL Documentation team is able to clone, branch, and merge changes back into the help repo. The goal of this project is to help make useful documents for end users of the RIIPLXNAT system. :+1:

Advanced processing documentation, details about the RIIPL processing pipeline, and image processing techniques are beyond the scope of this help site.

### Who deploys the changes to the documentation site?
Currently, Richard only. However, a deploy script is on the way.

### What will I need to create documentation?
[SPHINX Autodoc](http://www.sphinx-doc.org/en/stable/ext/autodoc.html). creates html files based on rst files, which are written using [GitHub-Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

##### 1. Install [SPHINX Autodoc](http://www.sphinx-doc.org/en/stable/ext/autodoc.html).
```
$ pip install Sphinx
```
##### 2. Clone a copy of the help repo
```
$ git clone http://riiplcluster.medeng.wfubmc.edu:30000/docteam/help.git
```
##### 3. Create your own branch of changes
```
$ git checkout -b my_new_branch
```
##### 4. Make your changes
Writing great documentation with Markdown is easy. Here are some resources:
* [Markdown Editor](https://jbt.github.io/markdown-editor/)
* [Markdown Cheatsheat](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [Markdown docs](https://docs.gitlab.com/ee/user/markdown.html)

##### 5. Test your changes
Generate html documents in your \_build directory.
```
$ make html
```
Open your new html files in the browser to make sure they look correct.

##### 6. Commit your changes to your local repo
Git will not commit your build directory. That's just for your local testing. Only new rst files, images, and other resources will be added to the repo. Please do not add zip or executable files to the repo.

All files in your repo
```
$ git commit -a -m "I've made changes to all my files"
```
Or just a few
```
$ git add my_new_file.rst
$ git commit -m "Just commit my new file"
```

##### 6. Push to the repository
When everything looks good. You can push your new branch to the master repo and submit a [Merge Request](http://riiplcluster.medeng.wfubmc.edu:30000/docteam/help/merge_requests). This allows others in the group to review your changes, make notes or changes of the own.
```
$ git push
```
