## `aerospike:ce-5.7.0.8`

```console
$ docker pull aerospike@sha256:d2e7cfc88f5188200c9d3b59d6793224f972cdc56368b5ad42fbaac3e0c4481f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-5.7.0.8` - linux; amd64

```console
$ docker pull aerospike@sha256:f3a88d3b138809b8cff6213886bc63a4ef292ef448e05f06c4a33d2a4d585545
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81533785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abb23481bdcf2ff1974788049f30ae661ee22fef4d61efb37aeb240b498994fb`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:48:22 GMT
ENV AEROSPIKE_VERSION=5.7.0.8
# Tue, 21 Dec 2021 01:48:49 GMT
ENV AEROSPIKE_SHA256=587baea6f9ff594ae168a1dd21becccfd9cf4298cb073bb6f13e0ca72b6c42c0
# Tue, 21 Dec 2021 01:49:11 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Tue, 21 Dec 2021 01:49:11 GMT
COPY file:1897c4aae07efbc61bf2d8c2c7b0dfb0990174e11cc787eac71d5adf767abaed in /etc/aerospike/aerospike.template.conf 
# Tue, 21 Dec 2021 01:49:12 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Tue, 21 Dec 2021 01:49:12 GMT
EXPOSE 3000 3001 3002
# Tue, 21 Dec 2021 01:49:12 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 21 Dec 2021 01:49:12 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70547a6da418da9005bbd22a71ffe94f3c93945d2fda607b6d44030b9692713d`  
		Last Modified: Tue, 21 Dec 2021 01:49:48 GMT  
		Size: 54.4 MB (54378043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ba0cd5ca18109d2174717938d7ff15d4917d95a762074836a99fb31545ef51`  
		Last Modified: Tue, 21 Dec 2021 01:49:40 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd8ebad6886301a17ceca3a960351215b721920aaa8b5b46ac41ae4e15bcf94`  
		Last Modified: Tue, 21 Dec 2021 01:49:40 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
