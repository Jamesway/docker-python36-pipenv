# Docker image with Python 3.6 and pipenv
Brings PHP composer style package management to Python

### Usage with my 12 Factor django-admin docker image
https://github.com/jamesway/docker-12factor-django

### Installing packages
```
# install normally
docker run --rm -v $(pwd):/code jamesway/python36-pipenv install python-dotenv

# install a development package
docker run --rm -v $(pwd):/code jamesway/python36-pipenv install pytest --dev

# install all non-development packages from pipfile
docker run --rm -itv $(pwd):/code jamesway/python36-pipenv install

# installing everything including dev packages from pipfile
docker run --rm -itv $(pwd):/code jamesway/python36-pipenv install --dev
```
