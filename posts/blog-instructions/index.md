<!-- 
.. title: Blog instructions
.. slug: blog-instructions
.. date: 2016-02-22 02:20:00 UTC-05:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

# Set up
- Install [Nikola](https://getnikola.com/)
- Install [git](https://desktop.github.com/)
- Clone the blog repository and checkout the develop branch:
<!-- TEASER_END -->

```
    mkdir ~/git
    cd ~/git
    git clone https://github.com/compmathvn/compmathvn.github.io.git
    cd compmathvn.github.io
    git checkout develop
```
- Create your own post:
```
    nikola new_post -f markdown
    <give it a name: my-first-post>
```
__Note__: use "nikola new_post --help" for more options.

- Edit the post in "posts/my-first-post.md" with your favorite text editor. Try [SublimeText](https://www.sublimetext.com/)
- [Optional] Build the site and view it locally
```
    nikola build
    nikola server
    <open your browser, type "localhost:8000">
```
- Deploy on github so everyone can see:
```
    nikola github_deploy
    <open your browser, type "compmathvn.github.io"
```
This will automatically push the change (new posts) to the develop branch on github, build the site, and push the new site to the master branch.