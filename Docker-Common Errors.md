After installing docker, when we try to use any docker command it will give an error saying permission denied, if we give it with sudo it will work, 
so to add the ubuntu user to the docker group, we need to give the below command and then exit out and login back again for the change to be effective.

**Error:**
ubuntu@ip-172-31-91-205:~$ docker ps -a
Got permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.24/containers/json?all=1": dial unix /var/run/docker.sock: connect: permission denied

ubuntu@ip-172-31-91-205:~$ **sudo** docker images
REPOSITORY   TAG       IMAGE ID   CREATED   SIZE

**Solution:**
ubuntu@ip-172-31-91-205:~$ sudo usermod -aG docker ubuntu
ubuntu@ip-172-31-91-205:~$ docker images
Got permission denied while trying to connect to the Docker daemon socket at unix:///var/run/docker.sock: Get "http://%2Fvar%2Frun%2Fdocker.sock/v1.24/images/json": dial unix /var/run/docker.sock: connect: permission denied

ubuntu@ip-172-31-91-205:~$ sudo docker images
REPOSITORY   TAG       IMAGE ID   CREATED   SIZE
