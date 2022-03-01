# httpd - Servidor web
[Docker hub: image httpd](https://hub.docker.com/_/httpd "")
##Ejecutar el comando para contruir una imagen Docker

```batch
 $docker build -t my-apache2 .
```

## Ejecutar la imagen docker
```batch
  $ docker run -dit --name my-running-app -p 8080:80 my-apache2
  
  ```
  
## Ejecutar la imagen usando un directorio  compartido
```batch
docker run --rm -it -d -p 8000:80 -v ${PWD}\public-html:/usr/local/apache2/htdocs/ my-apache2
```