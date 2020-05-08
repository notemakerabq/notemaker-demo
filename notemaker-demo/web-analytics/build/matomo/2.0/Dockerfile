FROM wonderfall/matomo 
MAINTAINER owner="Matthew Barker"
LABEL application="WebAnalytics"
LABEL tier="web"
LABEL appVersion==="2.0"
LABEL baseImage="wonderfall/matomo"

# update package manager
RUN apk update

# remove unnecessary packages
RUN apk del gcc g++ make git perl perl-net-ssleay perl-io-socket-ssl perl-libwww 

# upgrade entire OS and php7 due to OS level vulnerabilities
RUN apk upgrade
RUN apk add php7 php7-fpm php7-opcache 

# add and use a named user to limit attack surface
RUN adduser -D --uid=991 matomo
USER matomo










