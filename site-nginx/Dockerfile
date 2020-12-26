FROM nginx:latest

# html files
COPY index.html /usr/share/nginx/html/index.html

# copy configuration files to the container
COPY default.conf /etc/nginx/conf.d/default.conf

EXPOSE 80

ENTRYPOINT ["nginx", "-g", "daemon off;"]
