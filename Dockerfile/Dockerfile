FROM nginx:latest
RUN yum update

RUN yum add --no-cache nginx   

# nginx config
COPY nginx.conf /etc/nginx/nginx.conf
RUN mkdir  -p /usr/share/doc/nginx/html

COPY index.html /usr/share/doc/nginx/html/index.html

# nginx port
EXPOSE 80

# starting nginx
CMD ["nginx", "-g", "daemon off;"]

