FROM anapsix/alpine-java
RUN mkdir -p /opt/odl && wget -O /opt/odl/opendaylight-0.9.1.tar.gz \
	https://nexus.opendaylight.org/content/repositories/public/org/opendaylight/integration/opendaylight/0.9.1/opendaylight-0.9.1.tar.gz && \
	tar zxv /opt/odl/opendaylight-0.9.1.tar.gz -C /opt/odl
#ADD ./opendaylight-0.9.1 /opt/opendaylight-0.9.1
WORKDIR /opt/odl/opendaylight-0.9.1
