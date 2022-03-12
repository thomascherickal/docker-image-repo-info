## `aerospike:ce-5.7.0.11`

```console
$ docker pull aerospike@sha256:0e4e24f00d2d27ae405d7e2a07c4c3d7ed1b9cebdd7170adb5a17cd5df37c1f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-5.7.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:ac84dc729d27cc83736acad7db696ee5fec46cc81ebbec09a03cd053711d22de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81536106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994326589d6c6d231806c03017c28977e23d89a3fe5d3a61a76910200da9a10d`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:56 GMT
ADD file:702017714ad3e1567b4f60b688750f8b631d91088e4dcf41351c4bb07749c579 in / 
# Tue, 01 Mar 2022 02:13:56 GMT
CMD ["bash"]
# Fri, 11 Mar 2022 18:19:21 GMT
ENV AEROSPIKE_VERSION=5.7.0.11
# Fri, 11 Mar 2022 18:19:49 GMT
ENV AEROSPIKE_SHA256=bd0d9962c8d068270746833df313d32117ef9e9c3e2367f8ac6902cf97d66142
# Fri, 11 Mar 2022 18:20:11 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Fri, 11 Mar 2022 18:20:12 GMT
COPY file:1897c4aae07efbc61bf2d8c2c7b0dfb0990174e11cc787eac71d5adf767abaed in /etc/aerospike/aerospike.template.conf 
# Fri, 11 Mar 2022 18:20:12 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Fri, 11 Mar 2022 18:20:12 GMT
EXPOSE 3000 3001 3002
# Fri, 11 Mar 2022 18:20:12 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Fri, 11 Mar 2022 18:20:12 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:15115158dd02a1bf2fd28724e3c1024394033fb0e9a5d3e451ed2715b6ae312d`  
		Last Modified: Tue, 01 Mar 2022 02:20:08 GMT  
		Size: 27.2 MB (27153737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe160033f12077907a2fdc9d220d250777e2add37acc98df2edb7d7d74e6037b`  
		Last Modified: Fri, 11 Mar 2022 18:20:49 GMT  
		Size: 54.4 MB (54380350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6acccb95222ee358b6be7ff4a483abb2468c1123cc752633812aa2e75e36b218`  
		Last Modified: Fri, 11 Mar 2022 18:20:41 GMT  
		Size: 1.1 KB (1139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b5240f71ce86c572d897867ad79dd8ea140b2b2cf55d5c2980c184c3a49b20`  
		Last Modified: Fri, 11 Mar 2022 18:20:41 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
