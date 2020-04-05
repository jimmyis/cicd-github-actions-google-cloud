FROM nginx:stable-alpine

WORKDIR /app

COPY nginx.conf /etc/nginx/nginx.conf

COPY dist .

EXPOSE 80

CMD [ "nginx", "-g", "daemon off;" ]
