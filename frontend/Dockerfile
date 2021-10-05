FROM nginx:1.13.3-alpine
COPY default.conf /etc/default.conf
CMD ["/bin/sh", "-c", "envsubst '$BACKEND_URL' </etc/default.conf >/etc/nginx/conf.d/default.conf ; nginx -g 'daemon off;'"]
