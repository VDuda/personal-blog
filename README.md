# Pelican based personal blog

Using Pelican and Python 3.3+ to statically create a webpage at vlad-duda.me

### Writing Content
To write an article plop a markdown file into the content directory. Follow the specified metadata of the previous articles. In the future there will be more thought into categories and they will be listed under this readme. 

### Deploying
To deploy the static site you should take advantage of the Makefile within this repo. Currently deploying up to Github, with AWS R53 managing DNS routing. 

```
make github
``` 

### Testing locally 
To test locally you'll need to generate the html files and then serve up the content using a server.
```
make html  # Generates html, CSS, & JS 
make serve # Will serve up the content on localhost:8000
```