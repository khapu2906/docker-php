FROM devilbox/php-fpm:7.3-prod
LABEL Name=developer Version=0.0.1

# Install dependencies
RUN apt-get update && apt-get install -y \
    build-essential \
    libpng-dev \
    libjpeg62-turbo-dev \
    libfreetype6-dev \
    locales \
    zip \
    jpegoptim optipng pngquant gifsicle \
    vim \
    unzip \
    git \
    curl \
    # postgresql \ 
    # postgresql-contrib \
    libpq-dev \ 
    net-tools \
    iputils-ping

# Install composer
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer