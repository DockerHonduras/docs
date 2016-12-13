Resolved issues
=================

###1. How to Remove multiple docker images with the same IMAGE ID ?

**Example**  

`tomcat 8.0 c6cfe59eb987 3 weeks ago 357 MB`  
`tomcat latest c6cfe59eb987 3 weeks ago 357 MB`

**answer**

`docker images | grep c6cfe59eb987 | awk '{print $1 ":" $2}' | xargs docker rmi`

[stackoverflow 32944391] - how-to-remove-multiple-docker-images-with-the-same-imageid
[stackoverflow 32944391]: <http://stackoverflow.com/questions/32944391/how-to-remove-multiple-docker-images-with-the-same-imageid>
