# Instrukcja
Uruchamianie
```sh
docker swarm init
docker stack deploy -c docker-compose.yml images-app
docker-compose -f docker-compose.yml -f docker-compose.update.yml --log-level ERROR config > stack.yml
docker stack deploy -c stack.yml images-app
```
Usuwanie:
```sh
docker stack images-app
docker swarm leave --force 
``` 
