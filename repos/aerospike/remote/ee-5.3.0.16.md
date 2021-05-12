## `aerospike:ee-5.3.0.16`

```console
$ docker pull aerospike@sha256:f37216310815da5ac5eda503f4059395566ff57424edbc58c1a2f5dbed904418
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ee-5.3.0.16` - linux; amd64

```console
$ docker pull aerospike@sha256:7e35adad5870b3b98090565d3da18c257630e5806aa236a3ebafba7713939854
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76373688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cb9027947820abdd32c7c6b3d49f7a3fbfc9b736822c309b36756adffe4f574`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:47:27 GMT
ENV AEROSPIKE_VERSION=5.3.0.16
# Wed, 12 May 2021 01:47:27 GMT
ENV AEROSPIKE_SHA256=1408e186da1d5bb225a7296091ad32330b6c39c89dc3a45077c7e869c6e80edd
# Wed, 12 May 2021 01:47:58 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian9" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:47:59 GMT
COPY file:82161ba7b6e7d24ef9aeee8b19996114e9ff71c3928086ed1e58e01e82ee76a9 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:47:59 GMT
COPY file:11988df14ff2f0260ab7b8ccb322ee2d343b55791c51356df1d99639d16a6dbc in /entrypoint.sh 
# Wed, 12 May 2021 01:47:59 GMT
EXPOSE 3000 3001 3002
# Wed, 12 May 2021 01:47:59 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:48:00 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5bf363b6f6b1130c20e27caeb84120b5cbb10769d5b9853dbcd81538249f9c`  
		Last Modified: Wed, 12 May 2021 01:51:35 GMT  
		Size: 53.8 MB (53843305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf8975fd92a01ac4b97d36d596d800084d03dd8edd44288189af65278de94c7`  
		Last Modified: Wed, 12 May 2021 01:51:25 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d74e43830856a4badf30dc29823b4ae93d79d1fae5d3d15bb539cf2907ffe3`  
		Last Modified: Wed, 12 May 2021 01:51:25 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
