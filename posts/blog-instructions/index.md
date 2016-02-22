<!-- 
.. title: blog-instructions
.. slug: blog-instructions
.. date: 2016-02-22 02:20:00 UTC-05:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

# Set up
- Install [Nikola](https://getnikola.com/getting-started.html)
- Install [git](https://desktop.github.com/)
- Clone the blog repository and checkout the develop branch:
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
Use "nikola new_post --help" for more options.
- Edit the post in "posts/my-first-post.md" with your favorite text editor. Try [SublimeText](https://www.sublimetext.com/)
- Build the site:
```
    nikola build
```
- View it locally:
```
    nikola server
    <open your browser, type "localhost:8000">
```
- Deploy on github so everyone can see:
```
    nikola github_deploy
```