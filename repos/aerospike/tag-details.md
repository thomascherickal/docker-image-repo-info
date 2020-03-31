<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:4.6.0.13`](#aerospike46013)
-	[`aerospike:4.7.0.11`](#aerospike47011)
-	[`aerospike:4.8.0.6`](#aerospike4806)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:4.6.0.13`

```console
$ docker pull aerospike@sha256:6e91f0c054ffb845c6d2274a2febad13c07e9aacd487cf6a7fb67db225289a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.6.0.13` - linux; amd64

```console
$ docker pull aerospike@sha256:6eeefd4a40a65de875a7ba1f70b2b478d1ff7da65058fd37aac03cc17fa1a576
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51646138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:656c37fbc24fe942c4d26a3d1d175919105fd583f83f86af43ff664ebad5ff87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:51:28 GMT
ENV AEROSPIKE_VERSION=4.6.0.13
# Tue, 31 Mar 2020 01:51:28 GMT
ENV AEROSPIKE_SHA256=83b6c81922a4dbb17f979a3dd1810f11e4a1f1876093473e469500cde5fd89d6
# Tue, 31 Mar 2020 01:51:51 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 31 Mar 2020 01:51:51 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Tue, 31 Mar 2020 01:51:52 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Tue, 31 Mar 2020 01:51:52 GMT
VOLUME [/opt/aerospike/data]
# Tue, 31 Mar 2020 01:51:52 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 31 Mar 2020 01:51:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Mar 2020 01:51:52 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d50e08455824190c88718aaeeea7a9389f7270e6226b754a40849e5f7b4e35`  
		Last Modified: Tue, 31 Mar 2020 01:53:15 GMT  
		Size: 29.1 MB (29130746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e03c8a5707cadfb4bca3dcc178d577a672c699ff7a58576666e0d93e6607c5a`  
		Last Modified: Tue, 31 Mar 2020 01:53:10 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c6af049a3a1dd32a6e95fda33daa32359e69b72ac4564679110bd04b69a6a3`  
		Last Modified: Tue, 31 Mar 2020 01:53:10 GMT  
		Size: 885.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:4.7.0.11`

```console
$ docker pull aerospike@sha256:19246dab15c0548088b6134a0eff53548d3c7bba483114fab47f8149cded445b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.7.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:8f19b260ec0435ca7fb786399d1ac7467b8e812c9b9c36aa90570f2ca08b4728
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51770036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73397075757287813fc6785c0e88e2fa759f876dc2854cab414dba2ef79623da`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:52:00 GMT
ENV AEROSPIKE_VERSION=4.7.0.11
# Tue, 31 Mar 2020 01:52:00 GMT
ENV AEROSPIKE_SHA256=69585f4b519bf43cb7455360fd2fc81b5095533de59161be703f0658dc6d0c80
# Tue, 31 Mar 2020 01:52:19 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 31 Mar 2020 01:52:19 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Tue, 31 Mar 2020 01:52:20 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Tue, 31 Mar 2020 01:52:20 GMT
VOLUME [/opt/aerospike/data]
# Tue, 31 Mar 2020 01:52:21 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 31 Mar 2020 01:52:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Mar 2020 01:52:21 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0d387777264dc495e267207f05a372bbb8b749fbc7ee27b67c309bc38edf00`  
		Last Modified: Tue, 31 Mar 2020 01:53:24 GMT  
		Size: 29.3 MB (29254650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d545d008db872ebac6edfdaff0f25db55a0709d1bf9d51d2bf8dd8c2ce5f9bae`  
		Last Modified: Tue, 31 Mar 2020 01:53:18 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda5c4e5630f6e4003e79917dcfc50f1ec306f39d6002933ae2f0d598db0e598`  
		Last Modified: Tue, 31 Mar 2020 01:53:19 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:4.8.0.6`

```console
$ docker pull aerospike@sha256:0f531ee3f56f864effbc69bc85972583df85a9caf79ac523ab38b57f3b0a2e61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.8.0.6` - linux; amd64

```console
$ docker pull aerospike@sha256:c1ea27f677b11300376ae61e585a8e9703f6b726f1d66cf5ff36b743795005ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51845228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9cca18d05893bdb8a2ad91cbf9194d6013e54107f26ef0284615b911674c02a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:52:29 GMT
ENV AEROSPIKE_VERSION=4.8.0.6
# Tue, 31 Mar 2020 01:52:30 GMT
ENV AEROSPIKE_SHA256=8794e877abcc68faf3e2ccf461e3d9436343addcdccd3daba1c2e4e9154f8ef3
# Tue, 31 Mar 2020 01:52:57 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 31 Mar 2020 01:52:58 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Tue, 31 Mar 2020 01:52:59 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Tue, 31 Mar 2020 01:52:59 GMT
VOLUME [/opt/aerospike/data]
# Tue, 31 Mar 2020 01:52:59 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 31 Mar 2020 01:53:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Mar 2020 01:53:00 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b48c408db90cd8e7a145a8a17df40db7130de15002e081380506a636b64a7b1`  
		Last Modified: Tue, 31 Mar 2020 01:53:33 GMT  
		Size: 29.3 MB (29329835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f0119258f18ee529fca0bbee6ecefe1beb402c198901abd68486b117643198`  
		Last Modified: Tue, 31 Mar 2020 01:53:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd5138179ceed9f70748301d7d44161cedc8c4cbf3ba0e9262fed9be96f6d10`  
		Last Modified: Tue, 31 Mar 2020 01:53:28 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:0f531ee3f56f864effbc69bc85972583df85a9caf79ac523ab38b57f3b0a2e61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:c1ea27f677b11300376ae61e585a8e9703f6b726f1d66cf5ff36b743795005ba
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51845228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9cca18d05893bdb8a2ad91cbf9194d6013e54107f26ef0284615b911674c02a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:08 GMT
ADD file:e077f4d014ea0869fc4b3d5a3e6b3c8b792a97a8b4a328f33a994369225ff222 in / 
# Tue, 31 Mar 2020 01:24:08 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:52:29 GMT
ENV AEROSPIKE_VERSION=4.8.0.6
# Tue, 31 Mar 2020 01:52:30 GMT
ENV AEROSPIKE_SHA256=8794e877abcc68faf3e2ccf461e3d9436343addcdccd3daba1c2e4e9154f8ef3
# Tue, 31 Mar 2020 01:52:57 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 31 Mar 2020 01:52:58 GMT
COPY file:b2afebdf574a22640dc0687630172a267f2dc7857e8cd93254039deab3b62213 in /etc/aerospike/aerospike.template.conf 
# Tue, 31 Mar 2020 01:52:59 GMT
COPY file:688bc1b7dea55c1dc5575a99640936049823d07bac5c920bbace2369fbb27428 in /entrypoint.sh 
# Tue, 31 Mar 2020 01:52:59 GMT
VOLUME [/opt/aerospike/data]
# Tue, 31 Mar 2020 01:52:59 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 31 Mar 2020 01:53:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 31 Mar 2020 01:53:00 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:48839397421a64189661c2b86a34eb515d09a28204587a2b06b59df9f6e2d786`  
		Last Modified: Tue, 31 Mar 2020 01:29:28 GMT  
		Size: 22.5 MB (22513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b48c408db90cd8e7a145a8a17df40db7130de15002e081380506a636b64a7b1`  
		Last Modified: Tue, 31 Mar 2020 01:53:33 GMT  
		Size: 29.3 MB (29329835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f0119258f18ee529fca0bbee6ecefe1beb402c198901abd68486b117643198`  
		Last Modified: Tue, 31 Mar 2020 01:53:28 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd5138179ceed9f70748301d7d44161cedc8c4cbf3ba0e9262fed9be96f6d10`  
		Last Modified: Tue, 31 Mar 2020 01:53:28 GMT  
		Size: 884.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
