# Hands-on-Linux-Command


## Docker 

### How many images in Docker 
```
docker images -q | wc -l
```
docker images -q: This command lists all Docker images. The -q option makes it only output the image IDs.

wc -l: This command counts the number of lines in the output. Since each image ID is on a separate line, this effectively counts the number of images.

PS: We must use -q, or if one container name is too long, one container will correspond to 2 lines.

### stop all containers
```
docker stop $(docker ps -aq)
```
The $() syntax in the commands above is called command substitution. It's a feature of Unix-like shells such as Bash, Zsh, and others.

Command substitution allows you to use the output of a command as an argument to another command. It's a way of connecting two commands together so that the output of one is the input to the other.
