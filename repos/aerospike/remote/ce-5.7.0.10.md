## `aerospike:ce-5.7.0.10`

```console
$ docker pull aerospike@sha256:b558ceddba90298ac76d9b7188ebbfbf08d30d7827a032e4a3e06c537b655a8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `aerospike:ce-5.7.0.10` - linux; amd64

```console
$ docker pull aerospike@sha256:07103bc6876f77275637b3835496888cb33500cf7c876b99ed315802b44cb3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81534520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d69c234484e22dfe56ca776ee3d49578cd1db0f149328872148b2a304e97f0ef`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 25 Jan 2022 20:19:22 GMT
ENV AEROSPIKE_VERSION=5.7.0.10
# Tue, 25 Jan 2022 20:19:50 GMT
ENV AEROSPIKE_SHA256=6c17caabf03094c284c28406145447165ce7c40b954427879b8bd38d2824902b
# Tue, 25 Jan 2022 20:20:09 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 python3-distutils lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian10.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Tue, 25 Jan 2022 20:20:10 GMT
COPY file:1897c4aae07efbc61bf2d8c2c7b0dfb0990174e11cc787eac71d5adf767abaed in /etc/aerospike/aerospike.template.conf 
# Tue, 25 Jan 2022 20:20:10 GMT
COPY file:e1d47057fdb4c34c118f7ba5898161c386b475cba70907a4ae483866cf07335b in /entrypoint.sh 
# Tue, 25 Jan 2022 20:20:10 GMT
EXPOSE 3000 3001 3002
# Tue, 25 Jan 2022 20:20:10 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 25 Jan 2022 20:20:11 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0979cd37b2688267c6d857ffb4f03a82f8da389861b46d2dc55e52ac3f4f80`  
		Last Modified: Tue, 25 Jan 2022 20:20:42 GMT  
		Size: 54.4 MB (54378775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2077766bc06b621f0cb48d88d8df667254260ab5369b9e960af784e985de29a2`  
		Last Modified: Tue, 25 Jan 2022 20:20:34 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e304e8f604b3397d257c7f162ed531146bcb88ee410f048f1cff8be1d1ed991d`  
		Last Modified: Tue, 25 Jan 2022 20:20:34 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
