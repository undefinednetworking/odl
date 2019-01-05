FROM anapsix/alpine-java
ARG ODL_VER=0.9.1
ENV DOWNLOAD_URL_VAR="https://nexus.opendaylight.org/content/repositories/public/org/opendaylight/integration/opendaylight/$ODL_VER/opendaylight-$ODL_VER.tar.gz" 
RUN echo $DOWNLOAD_URL_VAR >test.txt
RUN mkdir -p /opt/odl && wget -O /opt/odl/opendaylight.tar.gz \
	$DOWNLOAD_URL_VAR && \
	tar zxf /opt/odl/opendaylight.tar.gz -C /opt/odl
#ADD ./opendaylight-0.9.1 /opt/opendaylight-0.9.1
WORKDIR /opt/odl
