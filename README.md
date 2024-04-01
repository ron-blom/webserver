# Webserver
This project is part of my [homeserver](https://github.com/ron-blom/homeserver) project and will deploy a nginx webserver with it's own ip address on my homeserver. Change address in values.yaml to fit your own network.

Using images: 

nginx

IP address used:
```
192.168.112.9
```

persistent storage:
```
/usr/share/nginx/html
```

# Deploy 

```
helm secrets upgrade --install webserver-chart ./webserver-chart -f webserver-chart/secrets.yaml
```