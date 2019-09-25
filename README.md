# docker-compose-awx
Docker compose file for AWX

The [awx installer](https://github.com/ansible/awx/blob/devel/installer/roles/local_docker/templates/docker-compose.yml.j2) has its own docker-compose thats run through ansible. 

However if you don't want to use the offical method of bootstrapping, here is a compose file.

# How to use:

## Execute the following commands
```
git clone https://github.com/arthurd2/docker-compose-awx.git awx
cd awx
sudo docker swarm init
docker stack deploy awx -c docker-compose.yml
echo "Enjoy life... =D"
```

# External DB?
Change variables in the following files:
1. docker-compose.yml
2. files/credentials.py
3. files/environment.sh
