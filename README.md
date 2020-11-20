# Python server

## prereqs
        
    criar novo ambiente python
        python3 -m venv clientes_venv
        
        
        pip3 install --upgrade pip
        source clientes_venv/bin/activate
        
        pip install flask flask_cors wheel connexion connexion connexion[swagger-ui]
        
        
    
## Docker
    
    https://hub.docker.com/repository/docker/gabrielltr/clientes_microservice
    
    docker run --name clientes-microservice -it -p 5000:5000 -d usuario/clientes_microservice
    