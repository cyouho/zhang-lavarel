#
#--------------------------------------------------------------------------
# Image Setup (not finished)
#--------------------------------------------------------------------------
#

FROM centos
RUN yum install wget 

LABEL maintainer="zhang fan <my_mail@mail.com>"

#
#--------------------------------------------------------------------------
# Software's Installation (not finished)
#--------------------------------------------------------------------------
#

ENV LANGUAGE=en_US.UTF-8
ENV LC_ALL=en_US.UTF-8
ENV LC_CTYPE=en_US.UTF-8
ENV LANG=en_US.UTF-8
ENV TERM xterm

#
#--------------------------------------------------------------------------
# Composer Installation: Install composer and add its bin to the PATH.
#--------------------------------------------------------------------------
#

RUN curl -s http://getcomposer.org/installer | php && \
    echo "export PATH=${PATH}:/var/www/vendor/bin" >> ~/.bashrc && \
    mv composer.phar /usr/local/bin/composer


#
#--------------------------------------------------------------------------
# Source the bashn
#--------------------------------------------------------------------------
#

RUN . ~/.bashrc
