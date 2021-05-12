## `aerospike:ee-5.4.0.11`

```console
$ docker pull aerospike@sha256:9df903be9751f4a7a536f76050b27367a2f2873e198862d8e216a294bb5894a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:ee-5.4.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:da35b809db6387c977e197fe6c135cc1c575054198eaf4eae07040f37e0064f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76410761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d3beabf17fb9124a5facc145a39f6fcb18cccdc02c31cab69faec704aa6ff2e`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 12 May 2021 01:23:21 GMT
ADD file:a88164546613d1850e5c5494cccad7124d713187bfabf592a783eb9328de51eb in / 
# Wed, 12 May 2021 01:23:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:48:03 GMT
ENV AEROSPIKE_VERSION=5.4.0.11
# Wed, 12 May 2021 01:48:03 GMT
ENV AEROSPIKE_SHA256=a23c586ae4fdd31f916b2dda5b7c9f86a4a529cc32b110f13fda6fa393e5be93
# Wed, 12 May 2021 01:48:32 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libldap-dev libcurl4-openssl-dev   && wget "https://www.aerospike.com/enterprise/download/server/${AEROSPIKE_VERSION}/artifact/debian9" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y   && find /usr/bin/ -lname '/opt/aerospike/bin/*' -delete   && find /opt/aerospike/bin/ -user aerospike -group aerospike -exec chown root:root {} +   && mv /opt/aerospike/bin/* /usr/bin/   && rm -rf /opt/aerospike/bin
# Wed, 12 May 2021 01:48:33 GMT
COPY file:82161ba7b6e7d24ef9aeee8b19996114e9ff71c3928086ed1e58e01e82ee76a9 in /etc/aerospike/aerospike.template.conf 
# Wed, 12 May 2021 01:48:33 GMT
COPY file:11988df14ff2f0260ab7b8ccb322ee2d343b55791c51356df1d99639d16a6dbc in /entrypoint.sh 
# Wed, 12 May 2021 01:48:33 GMT
EXPOSE 3000 3001 3002
# Wed, 12 May 2021 01:48:34 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Wed, 12 May 2021 01:48:34 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:fa1690ae92289fb310aa27b793a164bf8bbedc7ddd00ca079a31bb8bb315b616`  
		Last Modified: Wed, 12 May 2021 01:30:20 GMT  
		Size: 22.5 MB (22528266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ff9e6860b0b1234399fe109db0458300a5743421671edcc167368c47ff1a4a`  
		Last Modified: Wed, 12 May 2021 01:51:54 GMT  
		Size: 53.9 MB (53880378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edf9bc1765e06f99e7dbc3c3db66a2c46045018f2c5f54db03e404eab9cec96`  
		Last Modified: Wed, 12 May 2021 01:51:43 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef3ddd04f606550dd2b4dbcacdfc8415de7938e5c915932fed1213a506f1265`  
		Last Modified: Wed, 12 May 2021 01:51:43 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
