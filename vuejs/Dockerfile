FROM nginx:stable-alpine

WORKDIR /app

RUN ls -la

# COPY nginx.conf /etc/nginx/nginx.conf

COPY dist .

RUN ls -la

EXPOSE 80

CMD [ "nginx", "-g", "daemon off;" ]
