FROM httpd:2.4
COPY ./my-httpd.conf /usr/local/apache2/conf/httpd.conf
ARG UID=1001
ARG GID=1001
ENV UID=${UID}
ENV GID=${GID}
RUN usermod -u $UID www-data && groupmod -g $GID www-data && mkdir /app && chown 1001:1001 /app
