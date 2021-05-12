## `aerospike:ce-5.5.0.9`

```console
$ docker pull aerospike@sha256:2879252a6e61c02690153f84ddc32d2ae3e27c88604d46c721edfaf61d3a4e56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ce-5.5.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:355793c3c1ca5eec8d240f757f4953800882ee4ae81cc508afc97115d86aea00
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74778460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60ce4a9e712ba8b61e91b2d197e774f841592929c4e3e73a9c9fc67cfcc3ce06`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:48:39 GMT
ENV AEROSPIKE_VERSION=5.5.0.9
# Wed, 12 May 2021 01:49:15 GMT
ENV AEROSPIKE_SHA256=3e4e8f35c4607a465781e8f6b662494ca16717300746064ae7a1c09fd3b5ac90
# Wed, 12 May 2021 01:49:42 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:49:43 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:49:43 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 12 May 2021 01:49:44 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 12 May 2021 01:49:44 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:49:44 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66ab9f4217ba78f5a9eccccd54ebb0db2f3a19d27f6a3759ce96c0e3fe23f44`  
		Last Modified: Wed, 12 May 2021 01:52:38 GMT  
		Size: 52.2 MB (52248142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d93535340e8edcb9723e5093337d696021202e6909bd270ac4ae431b50ba641`  
		Last Modified: Wed, 12 May 2021 01:52:27 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a209082495bc63d19471fb0b7ea36b0455fe981213a41d9f9ccf46c7d49527`  
		Last Modified: Wed, 12 May 2021 01:52:27 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
