# gup_docker_php_yii1
Docker image for Yii 1 applications of SPbGUP,  PHP 5.6

If you want to make changes in image, simply edit dockerfile, save it, then build new image and push it to dockerhub.

## To build and push docker image run:
```
docker build -t spbgup/php:5.6.yii1 . --no-cache
docker push spbgup/php:5.6.yii1
```
Explain:  
``` docker build ```  
`-t` is for tag `spbgup/php:5.6` without this img won't pushed  
`.` (DOT) is for build with Dockerfile located in current directory  
`-- no-cache` to force build docker  

`push spbgup/php:5.6` push img to docker hub repository

For login use `docker login` command with cridentials from KeePass.
