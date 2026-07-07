# Use official lightweight Nginx image
FROM nginx:alpine

# Remove default nginx welcome page
RUN rm -rf /usr/share/nginx/html/*

# Copy our custom website into nginx's serving directory
COPY index.html /usr/share/nginx/html/

# Nginx listens on port 80 by default
EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
