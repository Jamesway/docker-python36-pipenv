# Docker image with Python 3.6 and pipenv
Brings PHP composer style package management to Python

### Installing a package
```
# eg Django
docker run --rm -itv $(pwd):/code jamesway/python36-pipenv install django
```

### Installing a package for development
```
docker run --rm -itv $(pwd):/code jamesway/python36-pipenv install pytest --dev
```

### Installing all non-development packages from pipfile
```
docker run --rm -itv $(pwd):/code jamesway/python36-pipenv install
```

### Installing everything including dev packages from pipfile
```
docker run --rm -itv $(pwd):/code jamesway/python36-pipenv install --dev
```

### Generate a version lock file
```
docker run --rm -itv $(pwd):/code jamesway/python36-pipenv lock
```
