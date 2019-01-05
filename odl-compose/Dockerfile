FROM anapsix/alpine-java
RUN mkdir -p /opt/odl && wget -O /opt/odl/opendaylight.tar.gz \
	$DownloadURL && \
	tar zxf /opt/odl/opendaylight.tar.gz -C /opt/odl
#ADD ./opendaylight-0.9.1 /opt/opendaylight-0.9.1
WORKDIR /opt/odl
