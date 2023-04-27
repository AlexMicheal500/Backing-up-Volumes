# Backing-up-Volumes

1. Create a new volume using: 

$ docker volume create ubuntu_alex_volume

2. Check if the volume exists using:

$ docker volume ls

3. Make sure the volume also exixts in the volume directory using:

$ cd /volume/lib/docker/volumes

4. Make sure to copy everything in your exixting volume to the new volume called ubuntu_alex_volume using:

$ cp -r -p _data ../ubuntu_alex_volume

5. Create a new docker compose file because of backup:

$ cp docker-compose-ce.yaml New_docker-compose-ce.yaml

This is where we now edit.

6. In docker compose file, change database name, app name, port and change the colume to the one created above.

![image](https://user-images.githubusercontent.com/99332618/234854339-9cb16d01-7b6b-4d69-9e15-b73c4e02397c.png)

![image](https://user-images.githubusercontent.com/99332618/234854572-f6763710-f420-422e-a6f7-a8b9732aaf69.png)
