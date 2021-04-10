FROM alpine

USER root

# Copy the files
COPY src/install.sh /tmp/install.sh
COPY src/nginx.conf /etc/nginx/nginx.conf

# Run Install instructions
RUN sh /tmp/install.sh

EXPOSE 443 80

# Do the ENTRYPOINT for the Dockerfile
ENTRYPOINT nginx -g "daemon off;"
