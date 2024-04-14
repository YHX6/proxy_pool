
# ProxyPool 

Original Github Repository: (https://github.com/jhao104/proxy_pool )[https://github.com/jhao104/proxy_pool]


# Setup
Use Docker to start this project (build locally might need to solve the issue of `imp` which is no longer supported after python3.9).

Run following command under project folder
``` bash
docker-compose up -d
```

# How to use

* Api

Start the project, default is api is: http://127.0.0.1:5010 :

| api | method | Description                 | params                                                     |
| ----| ---- |-----------------------------|------------------------------------------------------------|
| / | GET | api description             | None                                                       |
| /get | GET | randomly get a proxy        | optional parameters: `?type=https`  only get https proxies |
| /pop | GET | randomly get and delete a proxy | optional parameters: `?type=https`  only get https proxies                       |
| /all | GET | get all proxies             | optional parameters: `?type=https`  only get https proxies                       |
| /count | GET | check proxy number          | None                                                       |
| /delete | GET | delete a proxy              | `?proxy=host:ip`                                           |