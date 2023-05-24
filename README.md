## How to start 
```python
uvicorn main:app --reload
```
- [swagger](http://127.0.0.1:8000/docs)
- [another-doc](http://127.0.0.1:8000/redoc)

######

- [api-helloworld](http://127.0.0.1:8000/)
- [api1](http://127.0.0.1:8000/items/5?q=somequery)
## How to build docker image
docker build -t fastapi:1.0.0 .

## How to login ACR
- az login
- az acr login --name omsdevops
- [tutorial](https://learn.microsoft.com/en-us/azure/container-registry/container-registry-authentication?tabs=azure-cli)

## How to build tag
- docker tag fastapi:1.0.0 omsdevops.azurecr.io/fastapi:1.0.0
- docker tag fastapi:1.0.0 omsdevops.azurecr.io/fastapi

## How to push to ACR
- docker push omsdevops.azurecr.io/fastapi:1.0.0