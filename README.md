<img src="https://www.societyforscience.org/wp-content/uploads/2020/01/Regeneron-Logo-Tagline.png" width=300px />
<img src="https://github.com/zhouanbo/got_gene/raw/master/www/mp_logo.png" width=150px />

# got_gene

## Overview

Description

## Dependency

- Docker: https://docs.docker.com/get-docker/
- Git: https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

## Installation

To use it, clone it to your local machine by running:
```
git clone https://github.com/zhouanbo/got_gene.git
```
This will download all the codes and history to a folder called “got_gene”.
 
and then to build a docker image from the Dockerfile in the “got_gene” folder:
```
cd got_gene
docker build -t got_gene .
```

Once this is done, you can issue the command:
```
docker images
```
to see the got_gene image and it’s dependencies created.
 
To run the image, serving a shiny server on your local machine, you can issue this command:
```
docker run --rm -p 3838:3838 got_gene
```

Then open the browser and navigate to:
http://127.0.0.1:3838
you should see the project running!
