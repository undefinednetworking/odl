FROM anapsix/alpine-java
ARG ODL_VER=0.9.1
ENV DOWNLOAD_URL_VAR="https://nexus.opendaylight.org/content/repositories/public/org/opendaylight/integration/opendaylight/$ODL_VER/opendaylight-$ODL_VER.tar.gz" 

RUN mkdir -p /opt/odl && wget -O /opt/odl/opendaylight.tar.gz \
	$DOWNLOAD_URL_VAR && \
	tar zxf /opt/odl/opendaylight.tar.gz -C /opt/odl

WORKDIR /opt/odl/opendaylight-$ODL_VER

# 8181 : API
# 6633 : Openflow
# 8101 : ODL cli

EXPOSE 8181 6633 8101

CMD ./bin/karaf

