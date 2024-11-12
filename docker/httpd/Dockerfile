FROM httpd:2.4
ARG REPO_URL=https://github.com/EstherCho-7/EstherCho-7.github.io.git
COPY ./my-httpd.conf /usr/local/apache2/conf/httpd.conf

RUN ["apt-get", "update"]
RUN ["apt-get", "install", "-y", "vim"]
RUN ["apt-get", "install", "-y", "git"]
RUN git clone -b 240829/firebase ${REPO_URL} /usr/local/apache2/blog
