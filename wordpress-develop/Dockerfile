FROM mattrayner/lamp:latest-2004-php8

# Your custom commands
# install wpcli
RUN curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar && \
    php wp-cli.phar --info && \
    chmod +x wp-cli.phar && \
    mv wp-cli.phar /usr/local/bin/wp
CMD ["/run.sh"]
