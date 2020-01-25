<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:4.6.0.12`](#aerospike46012)
-	[`aerospike:4.7.0.10`](#aerospike47010)
-	[`aerospike:4.8.0.5`](#aerospike4805)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:4.6.0.12`

```console
$ docker pull aerospike@sha256:d4302191519d7314b119689870b59195a86057d4bda461f987d46d129bca10df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.6.0.12` - linux; amd64

```console
$ docker pull aerospike@sha256:1a2000976c7ab1f7042480504d439d29b138a602341f4984568aa802c3919a73
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51655889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992cac721addefcf7d4adecf7d4ae700c9cfa8d9393cf67a3fba22a1dea8c460`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Sat, 25 Jan 2020 02:19:15 GMT
ENV AEROSPIKE_VERSION=4.6.0.12
# Sat, 25 Jan 2020 02:19:15 GMT
ENV AEROSPIKE_SHA256=3e4cfc8c3681091e5ba56042ad4d6a9fc1a69c6f732d08e917c4df05e5eb8d96
# Sat, 25 Jan 2020 02:19:32 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Sat, 25 Jan 2020 02:19:32 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Sat, 25 Jan 2020 02:19:32 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Sat, 25 Jan 2020 02:19:33 GMT
VOLUME [/opt/aerospike/data]
# Sat, 25 Jan 2020 02:19:33 GMT
EXPOSE 3000 3001 3002 3003
# Sat, 25 Jan 2020 02:19:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 25 Jan 2020 02:19:33 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36448e38be2fc3da5b449e4202f13d98c0620d11ef22340ffd809314579ea0e8`  
		Last Modified: Sat, 25 Jan 2020 02:20:34 GMT  
		Size: 29.1 MB (29129265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52aac67adb43be99ff848084b9e7a4b7adb546c4e20c8b02e97d9f2a655ae734`  
		Last Modified: Sat, 25 Jan 2020 02:20:30 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b683b77a56853f813c36649c75aee34a8c54bb49ebcac30573d31baf0e41964`  
		Last Modified: Sat, 25 Jan 2020 02:20:29 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:4.7.0.10`

```console
$ docker pull aerospike@sha256:d58bdfd85ab775c730c58b527b056f463fc9031328500139ed50bc1bb2cb24b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.7.0.10` - linux; amd64

```console
$ docker pull aerospike@sha256:b94ef42c1e378e4bda4393f85c40541ee1250fe9f49a7d5b040ff234c7b476ea
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51778617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:085c878f6719c5dd3718febd789c33c34d34c952da452713297e10dcfb068bf9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:47 GMT
ADD file:90a2c81769a336bed3f731f44a385f2a65b0916f517a0b77c06c224579bf9a9a in / 
# Sat, 28 Dec 2019 04:23:47 GMT
CMD ["bash"]
# Sat, 25 Jan 2020 02:19:39 GMT
ENV AEROSPIKE_VERSION=4.7.0.10
# Sat, 25 Jan 2020 02:19:39 GMT
ENV AEROSPIKE_SHA256=cf96bf6e8dd85b57e0a2bba4446ae3a66b12f753c9d95af69e97f2ec0eea210d
# Sat, 25 Jan 2020 02:19:55 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Sat, 25 Jan 2020 02:19:55 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Sat, 25 Jan 2020 02:19:56 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Sat, 25 Jan 2020 02:19:56 GMT
VOLUME [/opt/aerospike/data]
# Sat, 25 Jan 2020 02:19:56 GMT
EXPOSE 3000 3001 3002 3003
# Sat, 25 Jan 2020 02:19:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 25 Jan 2020 02:19:56 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:804555ee037604c40de144f9f8da0d826d38db82f15d74cded32790fe279a8f6`  
		Last Modified: Sat, 28 Dec 2019 04:28:38 GMT  
		Size: 22.5 MB (22524609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beeada3467e226b96eb46fcba48a712b069cbd095ba8ed56e8d230f6633a31e8`  
		Last Modified: Sat, 25 Jan 2020 02:20:42 GMT  
		Size: 29.3 MB (29251990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0a26a367b97f41185301a9faa22135a99fa812261d7597682bf81873d785d3`  
		Last Modified: Sat, 25 Jan 2020 02:20:37 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322cded8db4a5ade1336179ebe6656ad518d97ea47e16c1726528e416f3762ee`  
		Last Modified: Sat, 25 Jan 2020 02:20:38 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:4.8.0.5`

```console
$ docker pull aerospike@sha256:c28a5051d0cc312bcb454c887be75e34a282ab151996d6156796e11076855419
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.8.0.5` - linux; amd64

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
