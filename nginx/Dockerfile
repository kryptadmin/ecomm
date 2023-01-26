FROM nginx:latest
LABEL MAINTAINER "DD<dilip@kryptstreet.com>"

COPY nginx.default /etc/nginx/conf.d/default.conf
RUN ls -sf /dev/stdout /var/log/nginx/access.log && ln -sf /dev/stderr /var/log/nginx/error.log