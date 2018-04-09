# dockerized-nginx

Official build of Nginx with dockerize preinstalled. [dockerize](https://github.com/jwilder/dockerize) is a utility to simplify running applications in docker containers. It allows you to:

* generate application configuration files at container startup time from templates and container environment variables
* Tail multiple log files to stdout and/or stderr
* Wait for other services to be available using TCP, HTTP(S), unix before starting the main process.

## Usage

```shell
docker run --name some-nginx -v $(pwd)/nginx.tmpl:/etc/nginx/nginx.tmpl -v $(pwd)/html:/usr/share/nginx/html:ro -d nginx
```
