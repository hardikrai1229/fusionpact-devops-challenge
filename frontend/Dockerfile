# Use official Nginx image as base
FROM nginx:alpine

# Set working directory to Nginx HTML directory
WORKDIR /usr/share/nginx/html


RUN rm -rf ./*


COPY Devops_Intern.html index.html

# Expose port 5001 for the frontend
EXPOSE 5001

# Change Nginx to listen on port 5001 instead of 80
RUN sed -i 's/listen       80;/listen       5001;/' /etc/nginx/conf.d/default.conf


CMD ["nginx", "-g", "daemon off;"]
