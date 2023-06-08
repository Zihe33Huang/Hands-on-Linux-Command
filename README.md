# Hands-on-Linux-Command

### Docker 
* How many images in Docker 
```
docker images -q | wc -l
```
docker images -q: This command lists all Docker images. The -q option makes it only output the image IDs.

wc -l: This command counts the number of lines in the output. Since each image ID is on a separate line, this effectively counts the number of images.

PS: We must use -q, or if one container name is too long, one container will correspond to 2 lines.
