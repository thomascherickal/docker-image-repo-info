<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:5.3.0.9`](#aerospike5309)
-	[`aerospike:5.4.0.4`](#aerospike5404)
-	[`aerospike:5.5.0.2`](#aerospike5502)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:5.3.0.9`

```console
$ docker pull aerospike@sha256:391c4866783a28a640de589cb8ce3d92cb5dfa6685266fd5dc9771f52217fe1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.3.0.9` - linux; amd64

```console
$ docker pull aerospike@sha256:22ab92f4b5693b43364edffa9f114b8548d50d8cded9f9c6dc2c7e577200df2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74712040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e401332e4d9cd801ba3c77d8359f51877fc46d49b309e0a0de9858884c2bfa39`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:50:18 GMT
ENV AEROSPIKE_VERSION=5.3.0.9
# Tue, 09 Feb 2021 04:50:18 GMT
ENV AEROSPIKE_SHA256=2a1fac1fd86ed2eeec2d749dc6e4647a7b31d3d73f3d2fe7c238dbf52c6fe77e
# Tue, 09 Feb 2021 04:50:49 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 09 Feb 2021 04:50:49 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 09 Feb 2021 04:50:49 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 09 Feb 2021 04:50:49 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 09 Feb 2021 04:50:50 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 09 Feb 2021 04:50:50 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1468077646b8495fe5b55432620a5c9579f80bcc2cc99b92f8c4f80a005b771f`  
		Last Modified: Tue, 09 Feb 2021 04:52:56 GMT  
		Size: 52.2 MB (52181387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f82d3924c19a3c72982d484bdfb2ed878155eab13f94d28311719c7123e6ff7`  
		Last Modified: Tue, 09 Feb 2021 04:52:43 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a56e3f1e00fcadfaec4513f21046d0eedd65f082e13ff489e6f81a777a11e3`  
		Last Modified: Tue, 09 Feb 2021 04:52:43 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.4.0.4`

```console
$ docker pull aerospike@sha256:a6dde159fbd167806ddc85cf458c2d9b94769c13d39e9bd3f365ba064f023661
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.4.0.4` - linux; amd64

```console
$ docker pull aerospike@sha256:8e8610ae6d784dd4185d74869e0fae13414a493b4e8c220fb98a5f5b2dd28664
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74731406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e31017cc7d68a92aac0972a3b73fbeb5863045f530ccb63c1776bca132f790`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:50:59 GMT
ENV AEROSPIKE_VERSION=5.4.0.4
# Tue, 09 Feb 2021 04:51:00 GMT
ENV AEROSPIKE_SHA256=7222ef8414234f7a6d487aeffc6addcacdcd2d404a6654cafb8474313a193d9e
# Tue, 09 Feb 2021 04:51:34 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 09 Feb 2021 04:51:34 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 09 Feb 2021 04:51:35 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 09 Feb 2021 04:51:35 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 09 Feb 2021 04:51:35 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 09 Feb 2021 04:51:36 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ada0249e0b9596123176c663766d45af0e970811c5ba7eaab61f1d9ab455853`  
		Last Modified: Tue, 09 Feb 2021 04:53:13 GMT  
		Size: 52.2 MB (52200753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5c8160592e87c9647bb99f8d0b4c35cd5d523ca9e9cdb880611b4cb69bbc34`  
		Last Modified: Tue, 09 Feb 2021 04:53:00 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe3ac352cca94d3b318264110f46badbb0cce85967322a4925664c8f635d472`  
		Last Modified: Tue, 09 Feb 2021 04:53:00 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.5.0.2`

```console
$ docker pull aerospike@sha256:509f5019b57d87569dc55284f215b8776455a48b0a1c806b17137d5f330c41cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.5.0.2` - linux; amd64

```console
$ docker pull aerospike@sha256:dead9d39e313f414af0b188df07b672f167abb27febb580bf2ac92df86896949
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74770603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dda8faf276140484ab9154a4c3af89ea747dc8cfaad4249aab5612a0a4dfffa`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:51:47 GMT
ENV AEROSPIKE_VERSION=5.5.0.2
# Tue, 09 Feb 2021 04:51:48 GMT
ENV AEROSPIKE_SHA256=f09ef2ecbfcb6810d4a068f64a22b68f4bc0b770da7578edab616bacb0d8a576
# Tue, 09 Feb 2021 04:52:23 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 09 Feb 2021 04:52:23 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 09 Feb 2021 04:52:23 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 09 Feb 2021 04:52:24 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 09 Feb 2021 04:52:24 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 09 Feb 2021 04:52:24 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5612038084d3f99c1047c845fdcae5b1e693b6adf31504892e1e1c5c40f18c9e`  
		Last Modified: Tue, 09 Feb 2021 04:53:29 GMT  
		Size: 52.2 MB (52239950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4492ab08c5c439e50fbb95d40de277003c9a99735064ee6b9e7f4f0bfc9d72a`  
		Last Modified: Tue, 09 Feb 2021 04:53:17 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d551ae8cb06e668301f17f873c1ab175025144f5aa883bdfee0f12fdda6563`  
		Last Modified: Tue, 09 Feb 2021 04:53:17 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:509f5019b57d87569dc55284f215b8776455a48b0a1c806b17137d5f330c41cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:dead9d39e313f414af0b188df07b672f167abb27febb580bf2ac92df86896949
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74770603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dda8faf276140484ab9154a4c3af89ea747dc8cfaad4249aab5612a0a4dfffa`
-	Entrypoint: `["\/usr\/bin\/dumb-init","--","\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Tue, 09 Feb 2021 02:23:30 GMT
ADD file:da0c935ddc86ca9e44bdd5f61b46c7b43a115ee4bc356324265a7ad6323f61ae in / 
# Tue, 09 Feb 2021 02:23:30 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:51:47 GMT
ENV AEROSPIKE_VERSION=5.5.0.2
# Tue, 09 Feb 2021 04:51:48 GMT
ENV AEROSPIKE_SHA256=f09ef2ecbfcb6810d4a068f64a22b68f4bc0b770da7578edab616bacb0d8a576
# Tue, 09 Feb 2021 04:52:23 GMT
RUN apt-get update -y   && apt-get install -y iproute2 procps dumb-init wget python python3 lua5.2 gettext-base libcurl4-openssl-dev    && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 09 Feb 2021 04:52:23 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 09 Feb 2021 04:52:23 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 09 Feb 2021 04:52:24 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 09 Feb 2021 04:52:24 GMT
ENTRYPOINT ["/usr/bin/dumb-init" "--" "/entrypoint.sh"]
# Tue, 09 Feb 2021 04:52:24 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:cae7303ade7f17f84fe86b2a44880e9725cf7d6dcd17f79485360712b6af6dcd`  
		Last Modified: Tue, 09 Feb 2021 02:29:36 GMT  
		Size: 22.5 MB (22528600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5612038084d3f99c1047c845fdcae5b1e693b6adf31504892e1e1c5c40f18c9e`  
		Last Modified: Tue, 09 Feb 2021 04:53:29 GMT  
		Size: 52.2 MB (52239950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4492ab08c5c439e50fbb95d40de277003c9a99735064ee6b9e7f4f0bfc9d72a`  
		Last Modified: Tue, 09 Feb 2021 04:53:17 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d551ae8cb06e668301f17f873c1ab175025144f5aa883bdfee0f12fdda6563`  
		Last Modified: Tue, 09 Feb 2021 04:53:17 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
