# Docker Volumes

There are 2 ways by which we can persists the data in Docker

- Bind Mounts
- Volumes

## Bind mount

directly binding host folder with container

```
$ docker run -itd --name <cotainer_name> -v <host_file_path>:<container_path> <image_name>
```

</br>

![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/6092ce96-1b23-450c-a104-87d0bba98208)

</br>

### data is persisting between host and container

</br>

![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/7a305ee0-cdd9-4565-b117-85366bbfe5e8)

</br>

## Docker create volume
```
$ docker volume create <volume_name>
```
</br>

![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/a85a8263-2ade-4d8b-98fe-78c2af87b82c)

</br>

## Attaching volume to containers with mount

```
$ docker run -itd --name <container_name> --mount source=<volume_name>,target=<by_what_name> <image_name>
```
</br>

![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/b18253c2-8948-4630-a329-a6f8d9ed2189)

</br>

### docker volume rohit atached to 2 containers

</br>

![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/ff460e3d-32e3-4d37-84aa-7bd336fe972a)

</br>

## Removing docker volume will give error if any container is attached to it
```
$ docker volume rm <volume_name>
```

</br>

![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/bc45ce34-8a1d-417b-8364-44cb607a3dd3)
</br>

## Docker volume through Dockerfile

</br>

![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/36af27df-80a2-45a4-b686-12201670714a)

</br>

### mount that volume to container

![image](https://github.com/suryaadev/DevOps-Projects/assets/47253310/072b02a1-4029-4be7-b3cb-3165f772944b)
