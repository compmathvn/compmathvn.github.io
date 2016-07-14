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
    <give it a title: "My first post">
```
__Note__: use ```nikola new_post --help``` for more options.  
__Note__: for ipython, simply copying an ipynb to the ```posts``` folder won't work. Need to use ```nikola new_post -f ipynb``` to generate the file with appropriate metadata.
<!-- TEASER_END -->

- Edit the new post ```posts/my-first-post.md``` with your favorite text editor. Try [SublimeText](https://www.sublimetext.com/)  
__Tip__: To break a line in markdown, end its with a double space \s\s.

- *(Optional)* Build the site and view it locally
```
    nikola build
    nikola server -b
```
- Deploy on github so everyone can see:
```
    nikola github_deploy
    <open your browser, type "compmathvn.github.io">
```
This will automatically push the change (new posts) to the develop branch on github, build the site, and push the new site to the master branch.

# Git setup
If you find it annoying to enter the username and password everytime you push to github, [generating a new ssh key and adding it to the ssh agent and your github account](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/). Also email ```comp.math.vn@gmail.com``` your github username to ask for the push access.
