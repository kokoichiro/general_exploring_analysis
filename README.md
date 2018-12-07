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