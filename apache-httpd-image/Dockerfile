FROM httpd:2.4

# LOAD MODIFIED CONFIG FILE
COPY ./httpd.conf /usr/local/apache2/conf/

# MAKE A FOLDER FOR EACH WEBSITE
RUN mkdir -p /usr/local/apache2/htdocs/zorionakana.tk/public_html
# COPY EACH WEBSITE TO THE SPECIFIC FOLDER
COPY ./website/ /usr/local/apache2/htdocs/zorionakana.tk/public_html

# LOAD VHOST CONFIG FILES (ADD NEW HOSTS HERE)
COPY httpd-vhosts.conf /usr/local/apache2/conf/extra
