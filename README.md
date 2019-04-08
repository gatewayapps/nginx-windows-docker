# nginx-windows-docker

Right now it is using a precompiled nginx 64 bit binary located in the nginx folder.

Mount your configuration files in c:/conf.

Remember to bind ports 80 and 443.

Example usage:

```
docker run --name nginx -p 80:80 -p 443:443 -v MY_CONF_DIR:c:/conf gatewayapps/nginx-windows:nano
```

In the future I will implement the build process for the nginx binary in the dockerfile itself.

