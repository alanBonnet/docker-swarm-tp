"# docker-swarm-tp" 

docker swarm init

docker stack deploy -c server-node.yml mystack

docker service ls

docker service ps mystack_web

docker service update --replicas=6 mystack_web

docker service scale mystack_web=6