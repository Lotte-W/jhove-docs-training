# JHOVE Docs Training
This repo is a playground for testing how to edit the jhove documentation website.

## How the site works
JHOVE use a thing called 'GitHub pages' to create the website.
This works by having a folder called 'docs' in the repository. And then we tell GitHub to enable pages onj the repository. It will confirm you mean the 'docs' folder, and then it will setup a webpage for you and use the docs folder to create it. 

## Whats in docs
GitHub Pages is a very versatile tool, that can support a range of technologies, but in the case of JHOVE it is a fairly straight forward HTML setup with a tiny bit of 'templating'
The templating is very minimal, it is hsed solely for the headers and footers, and you will see a tiny snippet like this:
```
{% include header.html %}
```
Where the ```{% ... %}``` lets you know that a snippet of HTML will be loaded from the template file.
In the 'docs' folder you will find an index.html and this is the 'Home Page' of JHOVE. other files at this level are int he 'root' of the website. There are folders in the 'docs' 'root' with more HTML files, and they will correspond with the URL structure of the website you see in the address bar. So the ```/docs/about``` folder in this project will correspond to the ```https://darrendignam.github.io/jhove-docs-training/about/``` public website.

## Making changes
If you make changes to these files and then push them to GitHub, a 'Workflow' will be initiated on GitHub to test and verify everything, and if those checks pass, the public website will be updated.
### Changes to the actual JHOVE documentation 
Any changes we make with our personal projects will only affect our personal website. If we want to change the actual JHOVE site we will need fork JHOVE, edit the docs, and then after we save our changes push them to GitHub, we would then have the opportunity to create a 'Push Request' - where we are trying to 'Push' our changes over to the parent project - for the maintainers of that project to choose to accept them into their project.