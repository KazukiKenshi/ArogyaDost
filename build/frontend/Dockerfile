# Use Nginx as the base image
FROM nginx:alpine

# Copy all files (including index.html, assets/) to the correct Nginx serving directory
COPY . /usr/share/nginx/html

COPY nginx.conf /etc/nginx/conf.d/default.conf

# Expose port 80
EXPOSE 80

# Start Nginx
CMD ["nginx", "-g", "daemon off;"]
