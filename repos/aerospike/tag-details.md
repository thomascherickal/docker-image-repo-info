<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.3.0.9`](#aerospike5309)
-	[`aerospike:5.4.0.4`](#aerospike5404)
-	[`aerospike:5.5.0.2`](#aerospike5502)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.3.0.9`

```console
$ docker pull aerospike@sha256:5ca126a63666179d537f357c701feb0628f22c84e5fb9f6bbdce2f6a8815f7d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.3.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:3c3a434a70700e5eb0752f8f2545828dde6bf134ca872b2cb50c858b1347df5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74712880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d30f9187e004719144766d2c20d0f5035833458d9232915b43982f3d0575a09`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 01:19:43 GMT
ENV AEROSPIKE_VERSION=5.3.0.9
# Tue, 09 Feb 2021 01:19:43 GMT
ENV AEROSPIKE_SHA256=2a1fac1fd86ed2eeec2d749dc6e4647a7b31d3d73f3d2fe7c238dbf52c6fe77e
# Tue, 09 Feb 2021 01:20:06 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 09 Feb 2021 01:20:07 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 09 Feb 2021 01:20:07 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 09 Feb 2021 01:20:07 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 09 Feb 2021 01:20:07 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 09 Feb 2021 01:20:07 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd12550640f07791ef0413341543116b67ebab52f3f7f14d626a27f859a34cc9`  
		Last Modified: Tue, 09 Feb 2021 01:21:26 GMT  
		Size: 52.2 MB (52182219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3351e6d36f855a9b934bd8c020c9785ed113b973acf00b3eac5fe7c6869140a`  
		Last Modified: Tue, 09 Feb 2021 01:21:17 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b5aa064ae4cfa277be84437fc8644422f56f88c23b7c5f00042f3f38d2ae57`  
		Last Modified: Tue, 09 Feb 2021 01:21:17 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.4.0.4`

```console
$ docker pull aerospike@sha256:3d9cd3dbeee29f52f685c0137897218aef8815b5d90ea65a60caed4320236a18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.4.0.4` - linux; amd64

```console
$ docker pull aerospike@sha256:f2aabdc9ab9ecb163f7dc89bda7f002b703c8466d13f17da3f7459babf851de0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74730966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:092f45db7de5b76f7425485e5bcd7549fa0b8ba932c467d0afcea8cf43e230f2`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 01:20:12 GMT
ENV AEROSPIKE_VERSION=5.4.0.4
# Tue, 09 Feb 2021 01:20:12 GMT
ENV AEROSPIKE_SHA256=7222ef8414234f7a6d487aeffc6addcacdcd2d404a6654cafb8474313a193d9e
# Tue, 09 Feb 2021 01:20:35 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 09 Feb 2021 01:20:35 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 09 Feb 2021 01:20:36 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 09 Feb 2021 01:20:36 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 09 Feb 2021 01:20:36 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 09 Feb 2021 01:20:36 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a0afa45d9c046d652cc70a84a3ab6e3f09cd6aae4af805a3d0605e78e6669`  
		Last Modified: Tue, 09 Feb 2021 01:21:38 GMT  
		Size: 52.2 MB (52200303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57fb0ccf90434e67a29a339bb390de66e1bacee594f8aeb05f3ba002d785ddf8`  
		Last Modified: Tue, 09 Feb 2021 01:21:30 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096c4f61691cfbaed3bd3685cc074bb005b97fae24217d8c8ceab8c56037e99f`  
		Last Modified: Tue, 09 Feb 2021 01:21:30 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.5.0.2`

```console
$ docker pull aerospike@sha256:b362d0f69ee76b0b6e144923344713c99a6c6fddc5734569c7f7caf00d36bee0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.5.0.2` - linux; amd64

```console
$ docker pull aerospike@sha256:27fc86e5815721338c6580643a13a9e4a6b28cd3ddbef277fb0c1bf894c28918
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74770363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c7e19c3751c3af8f736074c49a948d947361db6104cfaf013b4c31ae5d26ec`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 01:20:42 GMT
ENV AEROSPIKE_VERSION=5.5.0.2
# Tue, 09 Feb 2021 01:20:42 GMT
ENV AEROSPIKE_SHA256=f09ef2ecbfcb6810d4a068f64a22b68f4bc0b770da7578edab616bacb0d8a576
# Tue, 09 Feb 2021 01:21:05 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 09 Feb 2021 01:21:05 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 09 Feb 2021 01:21:06 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 09 Feb 2021 01:21:06 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 09 Feb 2021 01:21:06 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 09 Feb 2021 01:21:06 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fd70b4c2f4e8ff4152b2a79bdaa29aed9fca83287d047e8e19b5e8dcd18043`  
		Last Modified: Tue, 09 Feb 2021 01:21:51 GMT  
		Size: 52.2 MB (52239701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca14792d322e284a5022c99d5b56ac4b4892a9ba9b4cffc56f5ca1d2fa1c0a96`  
		Last Modified: Tue, 09 Feb 2021 01:21:43 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9125ef29d24bef023f1a8e6891bcc6292e96e23ff79c7042dde6cf9805fddc5`  
		Last Modified: Tue, 09 Feb 2021 01:21:42 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:b362d0f69ee76b0b6e144923344713c99a6c6fddc5734569c7f7caf00d36bee0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:27fc86e5815721338c6580643a13a9e4a6b28cd3ddbef277fb0c1bf894c28918
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74770363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c7e19c3751c3af8f736074c49a948d947361db6104cfaf013b4c31ae5d26ec`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 12 Jan 2021 00:35:21 GMT
ADD file:f47757e25d3861a5c0180542919c21264323d4dace1f5a6761fc2f38b53a9003 in / 
# Tue, 12 Jan 2021 00:35:21 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 01:20:42 GMT
ENV AEROSPIKE_VERSION=5.5.0.2
# Tue, 09 Feb 2021 01:20:42 GMT
ENV AEROSPIKE_SHA256=f09ef2ecbfcb6810d4a068f64a22b68f4bc0b770da7578edab616bacb0d8a576
# Tue, 09 Feb 2021 01:21:05 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 09 Feb 2021 01:21:05 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 09 Feb 2021 01:21:06 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 09 Feb 2021 01:21:06 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 09 Feb 2021 01:21:06 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 09 Feb 2021 01:21:06 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:8aff230071c97ddc86b6d29fbbb7a4caae7a0183a83f08aa5a06e69e26ce2c81`  
		Last Modified: Tue, 12 Jan 2021 00:43:25 GMT  
		Size: 22.5 MB (22528609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46fd70b4c2f4e8ff4152b2a79bdaa29aed9fca83287d047e8e19b5e8dcd18043`  
		Last Modified: Tue, 09 Feb 2021 01:21:51 GMT  
		Size: 52.2 MB (52239701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca14792d322e284a5022c99d5b56ac4b4892a9ba9b4cffc56f5ca1d2fa1c0a96`  
		Last Modified: Tue, 09 Feb 2021 01:21:43 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9125ef29d24bef023f1a8e6891bcc6292e96e23ff79c7042dde6cf9805fddc5`  
		Last Modified: Tue, 09 Feb 2021 01:21:42 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
