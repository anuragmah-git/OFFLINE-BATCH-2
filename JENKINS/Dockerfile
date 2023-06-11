# Pull the minimal Ubuntu image
FROM nginx

# update lib
RUN apt-get update && apt-get upgrade -y

# Copy the Nginx config
COPY index.html /usr/share/nginx/html

# Run the Nginx server
ENTRYPOINT service nginx start && bash
