### bandit
Bandit docker SAST (Static Application Security Testing) for python projects

#### docker-bandit
=============

Simple bandit docker image/container to run static security tests on python project in stand-alone mode, ideal for integration into a DEVSECOPS pipelines: 

#### build
```
   docker build -t davarski/bandit -f Dockerfile .
   docker login
   docker push davarski/bandit
```


#### use
```
    docker run -u root --rm -v YOUR_PYTHON_PROJECT_PATH:/app davarski/bandit bandit -r ./
    //help
    docker run -u root --rm -v YOUR_PYTHON_PROJECT_PATH:/app davarski/bandit bandit -h
```
#### Example DevSecOps J.pipeline:
