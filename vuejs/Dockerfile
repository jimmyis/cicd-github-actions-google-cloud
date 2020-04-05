FROM nginx:stable-alpine

COPY ./nginx.conf /etc/nginx/nginx.conf

WORKDIR /app

COPY ./dist .

EXPOSE 80

CMD [ "nginx", "-g", "daemon off;" ]
