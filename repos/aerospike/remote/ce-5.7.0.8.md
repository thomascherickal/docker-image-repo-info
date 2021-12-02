## `aerospike:ce-5.7.0.8`

```console
$ docker pull aerospike@sha256:c65a6c6585b7ca010e3c7eb7ef989631389824e3f8848da164a83aead89c5600
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-5.7.0.8` - linux; amd64

```console
$ docker pull aerospike@sha256:556e2abbf91e09101bfdd3d5700c05502e988968dba9e6c0c70305215183ab9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81533895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a0f85503fc8f8eb46797ea8bf393730ba3d89e67e881b19ab8f6c1bcfd78bd9`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Thu, 02 Dec 2021 02:48:43 GMT
ADD file:70f893355b4ecf317b289874ea624aa52c30735086e26de45bad73f57d16757b in / 
# Thu, 02 Dec 2021 02:48:43 GMT
CMD ["bash"]
# Thu, 02 Dec 2021 03:37:23 GMT
ENV AEROSPIKE_VERSION=5.7.0.8
# Thu, 02 Dec 2021 03:37:57 GMT
ENV AEROSPIKE_SHA256=587baea6f9ff594ae168a1dd21becccfd9cf4298cb073bb6f13e0ca72b6c42c0
# Thu, 02 Dec 2021 03:38:27 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Thu, 02 Dec 2021 03:38:27 GMT
COPY file:1897c4aae07efbc61bf2d8c2c7b0dfb0990174e11cc787eac71d5adf767abaed in /etc/aerospike/aerospike.template.conf 
# Thu, 02 Dec 2021 03:38:28 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Thu, 02 Dec 2021 03:38:28 GMT
EXPOSE 3000 3001 3002
# Thu, 02 Dec 2021 03:38:28 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Thu, 02 Dec 2021 03:38:28 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:ffbb094f4f9e7c61d97c2b409f3e8154e2621a5074a0087d35f1849e665d0d34`  
		Last Modified: Thu, 02 Dec 2021 02:54:33 GMT  
		Size: 27.2 MB (27153729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2641913fef3ff48e0b716f3da3abdc0418181b717db26d2b90ca0e8fb43888`  
		Last Modified: Thu, 02 Dec 2021 03:39:05 GMT  
		Size: 54.4 MB (54378146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0432727ffe99db30cd57dfc509c7de12822a697665b68601c8edcb499916d36`  
		Last Modified: Thu, 02 Dec 2021 03:38:56 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1780ad4b4bb36a87083c4afa2d6cbaf4e979f729e2b706d8c0eaf062c4a2684`  
		Last Modified: Thu, 02 Dec 2021 03:38:56 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
