# hadoop_with_docker
Для сборки и старта контейнера необходимо выполнить docker.sh
При этом получим:
Build the image
If you'd like to try directly from the Dockerfile you can build the image as:

docker build  -t sequenceiq/hadoop-docker:2.7.0 .
Pull the image
The image is also released as an official Docker image from Docker's automated build repository - you can always pull or refer the image when launching containers.

docker pull sequenceiq/hadoop-docker:2.7.0
Start a container
In order to use the Docker image you have just build or pulled use:

Make sure that SELinux is disabled on the host. If you are using boot2docker you don't need to do anything.

docker run -it sequenceiq/hadoop-docker:2.7.0 /etc/bootstrap.sh -bash
Далее используем run-mapreduce.sh для запуска
