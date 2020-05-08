FROM alpine 

LABEL maintainer="Matthew Barker"
LABEL application="NoteMaker" 
LABEL tier="database" 
LABEL appVersion="1.0"
LABEL baseImage="alpine:3.9"

RUN apk add mongodb-tools 

COPY collectStats.sh collectStats.sh

# collect stats every 300 seconds (5 minutes)
ENTRYPOINT ["collectStats.sh"]
CMD ["300"]



