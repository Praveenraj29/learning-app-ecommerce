# Use the official MariaDB image as the base
FROM mariadb

# Copy the database initialization script to the container
COPY db-load-script.sql /docker-entrypoint-initdb.d/

# Set environment variables for database initialization
ENV MYSQL_DATABASE ecomdb
ENV MYSQL_USER ecomuser
ENV MYSQL_PASSWORD ecompassword
ENV MYSQL_ROOT_PASSWORD rootpassword

# Expose MySQL port
EXPOSE 3306
