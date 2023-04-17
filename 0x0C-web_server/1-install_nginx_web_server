#!/bin/bash

# Update package list
apt update

# Install nginx
apt install -y nginx

# Configure nginx to listen on port 80
echo "server {
        listen 80;
        location / {
                echo \"Hello World!\";
        }
}" > /etc/nginx/sites-available/default

# Restart nginx
/etc/init.d/nginx restart
