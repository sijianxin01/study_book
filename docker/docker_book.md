docker --version
docker run --rm hello-world
docker ps -a
docker ps

docker images
docker run --gpus all -it -p 8888:8888 -v /home/sjx:/workspace image:tag
ssh -L port:localhost:port destip

docker start id/name 
docker exec -it id/name
docker stop id/name
docker rm id/name

docker images
docker commit name img:tag
docker save imag:tag > xx.tar
docker rmi id
docker load < xx.tgz