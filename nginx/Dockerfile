# nginx/Dockerfile
FROM nginx:alpine

# Copy custom NGINX configuration file
COPY nginx.conf /etc/nginx/nginx.conf

# Copy the built application files to the nginx container
COPY --from=0 /app/dist /usr/share/nginx/html

# Expose the port the server runs on
EXPOSE 80

