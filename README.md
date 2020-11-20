# Python server

## prereqs
        
criar novo ambiente python
    python3 -m venv clientes_venv
    
    
    pip3 install --upgrade pip
    source clientes_venv/bin/activate
    
    pip install flask flask_cors wheel connexion connexion connexion[swagger-ui]
        
        
    
## Docker
    
https://hub.docker.com/repository/docker/gabrielltr/clientes_microservice
    docker push gabrielltr/clientes_microservice:latest
    
### crud in memory
    docker run --name clientes-microservice -it -p 5000:5000 -d gabrielltr/clientes_microservice

### crud mongodb
    docker run --name clientes-microservice-mongo -it -p 5050:5000 -d gabrielltr/clientes_microservice:mongo

## Mongo

    pip3 install pymongo

    docker run -d -p 27017:27017 --name mongodb mongo

