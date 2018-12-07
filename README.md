# Replicatble analysis environment
This documentation shows you how to replicate your analysis environment with Docker and pipenv.
***


## Understand your environment
What kind of operating system are you using now? 
```
uname -a 
```
You can use this information for 'FROM' section of Dockerfile.


What kind of python modules are you using now? 
```
pipenv run pip freeze
```
You can use this information for understanding dependencies of your python modules.



## Use docker

1. Create Dockerfile
```
vim Dockerfile
```


2. Generate docker image from Dockerfile
```
docker build -t $your_container_image_name
```


3. Check your docker images
```
docker images
```


4. Run your new docker
```
docker run $your_container_image_name
```