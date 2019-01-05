FROM anapsix/alpine-java
ARG DOWNLOAD_URL
ENV DOWNLOAD_URL_VAR=$DOWNLOAD_URL
RUN echo $DOWNLOAD_URL_VAR >test.txt
RUN mkdir -p /opt/odl && wget -O /opt/odl/opendaylight.tar.gz \
	$DOWNLOAD_URL_VAR && \
	tar zxf /opt/odl/opendaylight.tar.gz -C /opt/odl
#ADD ./opendaylight-0.9.1 /opt/opendaylight-0.9.1
WORKDIR /opt/odl
