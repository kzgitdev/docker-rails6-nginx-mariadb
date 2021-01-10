ARG NGINX_TAG
FROM nginx:$NGINX_TAG

RUN rm -f /etc/nginx/conf.d/*
ADD default.conf /etc/nginx/conf.d/defualt.conf

# ビルド完了後にNginxを起動
CMD /usr/sbin/nginx -g 'daemon off;' -c /etc/nginx/nginx.conf
