FROM almalinux:9

# Install Nginx
RUN dnf install nginx -y

# Remove the default index.html file
RUN rm -rf /usr/share/nginx/html/index.html

# Add the new index.html file from the GitHub repository
ADD https://raw.githubusercontent.com/malurneelima/Docker/refs/heads/main/COPY/index.html /usr/share/nginx/html/index.html

# Set correct file and directory permissions
RUN chmod 644 /usr/share/nginx/html/index.html
RUN chmod 755 /usr/share/nginx/html

# Run Nginx in the foreground
CMD ["nginx", "-g", "daemon off;"]
