FROM wordpress:latest

# Install Git, Unzip (for Composer), and Composer
RUN apt-get update && \
    apt-get install -y git unzip && \
    curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer && \
    rm -rf /var/lib/apt/lists/*

# Set the default command to start Apache (same as the base image)
CMD ["apache2-foreground"]

