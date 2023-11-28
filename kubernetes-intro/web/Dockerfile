FROM ubuntu:20.04

WORKDIR /app

COPY ../* /app

RUN apt update && \
    apt install nginx -y && \
    rm -rf /var/lib/apt/lists/*

RUN useradd -s /bin/false nginx && \
    usermod -u 1001 nginx && groupmod -g 1001 nginx

COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 8000

CMD ["nginx", "-g", "daemon off;"]
