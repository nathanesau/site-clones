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

site links:

* twitter-clone: http://siteclones.freeddns.org/twitter-clone
