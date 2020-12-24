# site-nginx

to allow hosting multiple docker sites in same droplet, we should create multiple sites exposed on port 80 [dockerhub link](https://hub.docker.com/repository/docker/nathanesau/site-clones)

docker instructions:

```bash
# build the image
docker build -t site-nginx .

# run the image
docker run -p 80:80 -p 443:443 --name site-nginx --restart always -d site-nginx

# push to docker hub
docker tag site-nginx nathanesau/site-clones:site-nginx
docker push nathanesau/site-clones:site-nginx
```

install nginx as service (for digital-ocean):

```bash
# install nginx
sudo apt-get install nginx

# start nginx
sudo systemctl enable nginx

# configuration
cp twitter-app /etc/nginx/sites-enabled/default

# check configuration
nginx -t 

# reload
service nginx reload
```
