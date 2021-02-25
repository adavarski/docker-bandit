# bandit
Bandit docker SAST (Static Application Security Testing) for python projects

# build

   docker build -t davarski/bandit -f Dockerfile .
   
   docker push davarski/bandit

docker-bandit
=============

Simple bandit docker to run static security tests on python project in stand-alone mode, ideal for integration into a DEVSECOPS pipeline: [Jenkinsfile-example-pipeline](https://github.com/adavarski/docker-bandit/blob/master/Jenkinsfile-SAST-Bandit-PYTHON_PROJECT-example)

Use
===
    docker run -u root --rm -v YOUR_PYTHON_PROJECT_PATH:/app davarski/bandit bandit -r ./
    //help
    docker run -u root --rm -v YOUR_PYTHON_PROJECT_PATH:/app davarski/bandit bandit -h
