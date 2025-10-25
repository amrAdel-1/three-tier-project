FROM nginx:alpine
COPY nginx.conf /etc/nginx/nginx.conf
COPY certs/server.crt /etc/nginx/server.crt
COPY certs/server.key /etc/nginx/server.key
EXPOSE 443
CMD ["nginx", "-g", "daemon off;"]
