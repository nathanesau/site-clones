# site-clones

use docker-compose to bring up all the projects:

```bash
# bring up projects
docker-compose up -d

# bring down projects
docker-compose down
```

ports list:

| project | service | port(s) |
| ------- | ------- | ------- |
| twitter-clone | twitter-search (elasticsearch) | 9200 |
| twitter-clone | twitter-app (flask) | 5000 |
| pastebin-clone | pastebin-app (flask) | 5001 | 
| site-clones | site-nginx (nginx) | 80 |

docker hub links:

* twitter-clone: https://hub.docker.com/repository/docker/nathanesau/twitter-clone
* pastebin-clone: https://hub.docker.com/repository/docker/nathanesau/pastebin-clone
* site-clones: https://hub.docker.com/repository/docker/nathanesau/site-clones

site links:

* twitter-clone: http://siteclones.freeddns.org/twitter-clone
* pastebin-clone: http://siteclones.freeddns.org/pastebin-clone
