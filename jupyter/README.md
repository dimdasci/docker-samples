# Jupyter Notebook Image

This is a starter image with Python 3.9.13 and Jupyter notebook.

To extend the modules needed for a project:

1.  fork the repo
2.  create a file with requirements 
3.  build an image 
4.  run a container with working directory mounted
5.  open a URL from terminal in your browser
6.  quit Jupyter notebook to stop the container. 

## How to build an image

    docker build --build-arg REQUIREMENTS=<REQUIREMENTS_FILE> -t <YOUR_TAG> .

Default value for `<REQUIREMENTS_FILE>` is `requirements.txt`.

Some sample requirements are provided:

- requirements.txt — just notebook and nb extensions,
- requirements-practucum.txt - modules for Yandex Practucum,
- jupyter/requirements-minds.txt — basic modules for data science projects. 

## How to run the container

    docker run -it --rm -p 8888:8888 -v "${PWD}":/home/dim/work <YOUR_TAG>

