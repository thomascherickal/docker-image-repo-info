<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:4.6.0.12`](#aerospike46012)
-	[`aerospike:4.7.0.10`](#aerospike47010)
-	[`aerospike:4.8.0.5`](#aerospike4805)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:4.6.0.12`

```console
$ docker pull aerospike@sha256:ad6a10f4289f086341e6c670866295b153307622ad3efc0b63cb2ce7fa40df5a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.6.0.12` - linux; amd64

```console
$ docker pull aerospike@sha256:04b162689cf65e0aaae0fc447c109a1eff36730fecb55ef991cdc78043f475a1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51644850 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af232c729f8915ee60de9831b576bfedd3b81427afbd8901d4190e9ba80f1650`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:25:00 GMT
ENV AEROSPIKE_VERSION=4.6.0.12
# Wed, 26 Feb 2020 01:25:00 GMT
ENV AEROSPIKE_SHA256=3e4cfc8c3681091e5ba56042ad4d6a9fc1a69c6f732d08e917c4df05e5eb8d96
# Wed, 26 Feb 2020 01:25:19 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 26 Feb 2020 01:25:19 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Wed, 26 Feb 2020 01:25:19 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Wed, 26 Feb 2020 01:25:19 GMT
VOLUME [/opt/aerospike/data]
# Wed, 26 Feb 2020 01:25:19 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 26 Feb 2020 01:25:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:25:20 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbe7cf4e890f86f57feb5bca686de3d320ffa4245d3b2b873332ec0bda7f805`  
		Last Modified: Wed, 26 Feb 2020 01:26:24 GMT  
		Size: 29.1 MB (29129467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e11d920c875099099951f30d8f0fe8a17ca53905e91871213ee70bac235888`  
		Last Modified: Wed, 26 Feb 2020 01:26:18 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb8d082e6c204741ee39b6b73c360457cf565b23f9109e0f91b8f70c8fb585c`  
		Last Modified: Wed, 26 Feb 2020 01:26:18 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:4.7.0.10`

```console
$ docker pull aerospike@sha256:bf1025be4eb1694f9cff36b1d4c1e48c3c195078bd17f3a79dd2a0352606ad61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.7.0.10` - linux; amd64

```console
$ docker pull aerospike@sha256:b8e838cf668cb966cfdba1844ba3d34514b19e0f52cafd7b546dee0b8d98386e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51766677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1de137dd9628ffa0222e9ff95182284a4dbf76cb8c804e7b0a1c306060b3501`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:25:23 GMT
ENV AEROSPIKE_VERSION=4.7.0.10
# Wed, 26 Feb 2020 01:25:23 GMT
ENV AEROSPIKE_SHA256=cf96bf6e8dd85b57e0a2bba4446ae3a66b12f753c9d95af69e97f2ec0eea210d
# Wed, 26 Feb 2020 01:25:43 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 26 Feb 2020 01:25:44 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Wed, 26 Feb 2020 01:25:44 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Wed, 26 Feb 2020 01:25:44 GMT
VOLUME [/opt/aerospike/data]
# Wed, 26 Feb 2020 01:25:44 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 26 Feb 2020 01:25:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:25:45 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bde73fa52b42ffa6aa6d14e8b990c9ea1d39bf4863ed7f10d451e6cf61879a1`  
		Last Modified: Wed, 26 Feb 2020 01:26:33 GMT  
		Size: 29.3 MB (29251294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98f39d823735dcc9bd23eb5f3160f6d3b16fcbd383dde4c1f285632e7ff41e6`  
		Last Modified: Wed, 26 Feb 2020 01:26:27 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840f0e997f913f51a2f09dbe9ce47035ff05ea9e0007dd1c3d57c709c50a7033`  
		Last Modified: Wed, 26 Feb 2020 01:26:28 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:4.8.0.5`

```console
$ docker pull aerospike@sha256:7a56a9844788ecffa84015c9c39ae6a14f6a0e5073a12f87203573b52d541837
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.8.0.5` - linux; amd64

```console
$ docker pull aerospike@sha256:3206d71d79a6b418023ac435d9b79c3f825910451209351429ca4375235a17e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51844305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ff77adff3cbe4e62a381ce1de8e29be58531e210f38f095e81c577bd17a12c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:25:51 GMT
ENV AEROSPIKE_VERSION=4.8.0.5
# Wed, 26 Feb 2020 01:25:51 GMT
ENV AEROSPIKE_SHA256=b7082c51eee268992a55c5f0751b3de006cda857d93ed9d3e14624ca7118a1e8
# Wed, 26 Feb 2020 01:26:10 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 26 Feb 2020 01:26:11 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Wed, 26 Feb 2020 01:26:11 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Wed, 26 Feb 2020 01:26:11 GMT
VOLUME [/opt/aerospike/data]
# Wed, 26 Feb 2020 01:26:11 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 26 Feb 2020 01:26:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:26:12 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fc788786cb038dcbafaff5d99e6662bb74545a7c44cf28cc7bd068f68f57b6`  
		Last Modified: Wed, 26 Feb 2020 01:26:42 GMT  
		Size: 29.3 MB (29328922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96eef7ff4d848152ffdb5588ddfb58040e607554568dab40c2ecd8ec30f5743b`  
		Last Modified: Wed, 26 Feb 2020 01:26:36 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad93b59d4a01fb6ee0d5d109d89fb8e379283c38e257a7c5653d4cc22f0aa8b9`  
		Last Modified: Wed, 26 Feb 2020 01:26:37 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:7a56a9844788ecffa84015c9c39ae6a14f6a0e5073a12f87203573b52d541837
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:3206d71d79a6b418023ac435d9b79c3f825910451209351429ca4375235a17e3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51844305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ff77adff3cbe4e62a381ce1de8e29be58531e210f38f095e81c577bd17a12c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Wed, 26 Feb 2020 00:41:38 GMT
ADD file:1256c62f77a54c982fdb2790d682049b2ad64c8466466e846f3d33ad1ed4035d in / 
# Wed, 26 Feb 2020 00:41:38 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:25:51 GMT
ENV AEROSPIKE_VERSION=4.8.0.5
# Wed, 26 Feb 2020 01:25:51 GMT
ENV AEROSPIKE_SHA256=b7082c51eee268992a55c5f0751b3de006cda857d93ed9d3e14624ca7118a1e8
# Wed, 26 Feb 2020 01:26:10 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Wed, 26 Feb 2020 01:26:11 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Wed, 26 Feb 2020 01:26:11 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Wed, 26 Feb 2020 01:26:11 GMT
VOLUME [/opt/aerospike/data]
# Wed, 26 Feb 2020 01:26:11 GMT
EXPOSE 3000 3001 3002 3003
# Wed, 26 Feb 2020 01:26:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Feb 2020 01:26:12 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:6d28e14ab8c85bf8a4331de0667c27d19ef4092b12531eec0334b5c2a1012668`  
		Last Modified: Wed, 26 Feb 2020 00:47:21 GMT  
		Size: 22.5 MB (22513365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fc788786cb038dcbafaff5d99e6662bb74545a7c44cf28cc7bd068f68f57b6`  
		Last Modified: Wed, 26 Feb 2020 01:26:42 GMT  
		Size: 29.3 MB (29328922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96eef7ff4d848152ffdb5588ddfb58040e607554568dab40c2ecd8ec30f5743b`  
		Last Modified: Wed, 26 Feb 2020 01:26:36 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad93b59d4a01fb6ee0d5d109d89fb8e379283c38e257a7c5653d4cc22f0aa8b9`  
		Last Modified: Wed, 26 Feb 2020 01:26:37 GMT  
		Size: 883.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
