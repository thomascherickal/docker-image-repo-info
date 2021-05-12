## `aerospike:ce-5.4.0.11`

```console
$ docker pull aerospike@sha256:91b8a389ed0b61318a0428674b71399de3679c911a920109ccf4a67cb3521c59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ce-5.4.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:203166448e747048708ea23997c878fc858da2c21f90edb68ed7fb1a4bf7e9ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74723752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9966e71ce43521461e5cd25d17060fb4d38f30205f476ff1f18652967f4749`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:48:03 GMT
ENV AEROSPIKE_VERSION=5.4.0.11
# Wed, 12 May 2021 01:49:51 GMT
ENV AEROSPIKE_SHA256=8ce655f36b18bf89f2f0c687c594d222371c2330ffaaa9509697051d7994ebc7
# Wed, 12 May 2021 01:50:20 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:50:20 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:50:20 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Wed, 12 May 2021 01:50:21 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 12 May 2021 01:50:21 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:50:21 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f9d8d34f6e7a63749b41787ca2cd60a1787ff6bf77c269c159fa67dc828d9f`  
		Last Modified: Wed, 12 May 2021 01:52:57 GMT  
		Size: 52.2 MB (52193432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a0021d5420968da43e64ad1f64ab8d4abaaa393384331bff93e2600a810f50`  
		Last Modified: Wed, 12 May 2021 01:52:46 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0648cc3934d5d791489c14346b0aa12354d4c6a6d196e7788ad71961fc80c5`  
		Last Modified: Wed, 12 May 2021 01:52:46 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
