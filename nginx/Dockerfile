FROM nginx:1.19.1-alpine

RUN echo "\033[0;31mBuilding PROD Nginx Service\n\033[0m" \
    && rm /etc/nginx/conf.d/default.conf

COPY ./nginx.conf /etc/nginx/conf.d/

RUN ln -sf /dev/stdout /var/log/nginx/access.log \
    && ln -sf /dev/stderr /var/log/nginx/error.log
