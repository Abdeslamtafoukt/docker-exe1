docker run -it --name myalpes -v /MontPoint alpine /bin/ash
docker commit myalpes myalpine:v12
docker images
docker ps -a
docker export myalpes > myalpes.tar
cat myalpes.tar | docker import - my_alpine:v12
docker images
docker history my_alpine:v12 
docker history myalpine:v12
docker login -u  abdeslamtafoukt -p 
docker image tag myalpine:v12 abdeslamtafoukt/my_alpine:v12
docker push abdeslamtafoukt/my_alpine:v12










---




