FROM nginx:latest

# Remove default configuration files
#RUN rm /etc/nginx/conf.d/default.conf; exit 0

RUN mkdir -p /etc/nginx/sites-enabled
RUN mkdir -p /etc/nginx/sites-available

# Copy our custom config files to Nginx Contatiner
COPY nginx.conf /etc/nginx

COPY tuxlab.org.in.conf /etc/nginx/sites-enabled
COPY tuxlab.org.in.conf /etc/nginx/sites-available
