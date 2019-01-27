FROM ubuntu
LABEL maintainer="Alina Baktybekova (alinkab312@gmail.com)"
RUN apt-get update && apt-get install -y nginx
RUN ln -sf /dev/stdout /var/log/nginx/access.log && ln -sf /dev/stderr /var/log/nginx/error.log
EXPOSE 80 8081
ENTRYPOINT ["/usr/sbin/nginx", "-g", "daemon off;"]
