FROM openresty/openresty
COPY default.conf /etc/nginx/conf.d/
WORKDIR /build/app/
RUN apt-get update
RUN apt-get install -y php php-fpm vim
CMD ["tail", "-f", "/dev/null"]
# Move it to docker compose
# CMD ["nginx", "-g", "daemon off;"]