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
| site-clones | site-nginx (nginx) | 80 |

docker hub links:

* twitter-clone: https://hub.docker.com/repository/docker/nathanesau/twitter-clone
* site-clones: https://hub.docker.com/repository/docker/nathanesau/site-clones

site links:

* twitter-clone: http://siteclones.freeddns.org/twitter-clone
