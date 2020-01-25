## `aerospike:latest`

```console
$ docker pull aerospike@sha256:c28a5051d0cc312bcb454c887be75e34a282ab151996d6156796e11076855419
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:66ae87a1ebf113feef40e3146c312d171fae99679641e5e9f9356b65049db9f3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51855506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e78a0704dd49093f5a1dee136196ca416e64cb792fb23623ead2a1fb4683de43`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Sat, 25 Jan 2020 02:20:03 GMT
ENV AEROSPIKE_VERSION=4.8.0.5
# Sat, 25 Jan 2020 02:20:03 GMT
ENV AEROSPIKE_SHA256=b7082c51eee268992a55c5f0751b3de006cda857d93ed9d3e14624ca7118a1e8
# Sat, 25 Jan 2020 02:20:19 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Sat, 25 Jan 2020 02:20:19 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Sat, 25 Jan 2020 02:20:20 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Sat, 25 Jan 2020 02:20:20 GMT
VOLUME [/opt/aerospike/data]
# Sat, 25 Jan 2020 02:20:20 GMT
EXPOSE 3000 3001 3002 3003
# Sat, 25 Jan 2020 02:20:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 25 Jan 2020 02:20:20 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16802e450df7d13a1426e0044519fd0bd4644a28a53718a6fddd42853a0b89d`  
		Last Modified: Sat, 25 Jan 2020 02:21:00 GMT  
		Size: 29.3 MB (29328880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6a54e1d32c88c8d9c1ec2e7b24d759f0d91c3483ac2953222f284ad9d38477`  
		Last Modified: Sat, 25 Jan 2020 02:20:46 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1abde99640f2b6cded6cc9f94e6ced07e1eef4e9bf9b4ee9c09809c3c3db7a85`  
		Last Modified: Sat, 25 Jan 2020 02:20:45 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
