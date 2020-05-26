<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `aerospike`

-	[`aerospike:4.8.0.11`](#aerospike48011)
-	[`aerospike:4.9.0.8`](#aerospike4908)
-	[`aerospike:5.0.0.4`](#aerospike5004)
-	[`aerospike:latest`](#aerospikelatest)

## `aerospike:4.8.0.11`

```console
$ docker pull aerospike@sha256:67d2eef5d877c77597d8c93b0bf5e09bbc6726f0ee58615f0fa8bc27bc608c9d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.8.0.11` - linux; amd64

```console
$ docker pull aerospike@sha256:2630db6a4f020ff5a05bace63de13cc47b4ade2fc76c72c73740b8606025d12e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51853057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5a04bdece1e860c6499319c6dde2346b791bfdf6807c418f465849346bcd6c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Tue, 26 May 2020 22:19:21 GMT
ENV AEROSPIKE_VERSION=4.8.0.11
# Tue, 26 May 2020 22:19:21 GMT
ENV AEROSPIKE_SHA256=534f3ceb2da1e3914a62dff0cb4f876f7eacb9f30d029389dea1723387744aa3
# Tue, 26 May 2020 22:19:45 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 26 May 2020 22:19:45 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 26 May 2020 22:19:45 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 26 May 2020 22:19:45 GMT
VOLUME [/opt/aerospike/data]
# Tue, 26 May 2020 22:19:45 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 26 May 2020 22:19:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 May 2020 22:19:46 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea29733cfdd0b2b0c9af858e88d456564faeb5cf06ca28ee67a13feb8f9d67d2`  
		Last Modified: Tue, 26 May 2020 22:21:17 GMT  
		Size: 29.3 MB (29331114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e859d986239a046d2e1e411f8e7a029c54dfc50955e8ac2e23bd3f780fc16039`  
		Last Modified: Tue, 26 May 2020 22:21:10 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69be0285df80fd0699c0add90d9097201279bfabee80244493e9043239209a8`  
		Last Modified: Tue, 26 May 2020 22:21:09 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:4.9.0.8`

```console
$ docker pull aerospike@sha256:a87fd6b2fd5ba6e32cf10a803b948ea4f970f8383d10a733f7da734057b8d938
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:4.9.0.8` - linux; amd64

```console
$ docker pull aerospike@sha256:7d310817f4d7c830e4b5aadc62f42326e5df58bde5e2e78310890ba2a2dee5bf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53202990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8271a5c5eae8ed6f51f64c5e7d54b33a62c55de3ccbdd1df45f266c081827e00`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Tue, 26 May 2020 22:19:50 GMT
ENV AEROSPIKE_VERSION=4.9.0.8
# Tue, 26 May 2020 22:19:50 GMT
ENV AEROSPIKE_SHA256=dc41beb743ddc495c4c202897df8fc5000e764b659697beeb231e70f71005016
# Tue, 26 May 2020 22:20:14 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 26 May 2020 22:20:14 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 26 May 2020 22:20:15 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 26 May 2020 22:20:15 GMT
VOLUME [/opt/aerospike/data]
# Tue, 26 May 2020 22:20:16 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 26 May 2020 22:20:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 May 2020 22:20:16 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a86c888f371cd658b31b500217a71fb5f0c64988a7851796bc327d086852570`  
		Last Modified: Tue, 26 May 2020 22:21:27 GMT  
		Size: 30.7 MB (30681051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17a0538f1d082e5fac61c23ddf412a467a96fbf3bc71330d329fca7c049a1942`  
		Last Modified: Tue, 26 May 2020 22:21:21 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4be9d300e50c9f6562a04ced95843ab9f93e9a5758fcc76cf680e574e3c809`  
		Last Modified: Tue, 26 May 2020 22:21:21 GMT  
		Size: 900.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:5.0.0.4`

```console
$ docker pull aerospike@sha256:f146a121e6ba6e75cb306b8ea37f2770539a8da9a14a71c46b1c01e6de3224dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:5.0.0.4` - linux; amd64

```console
$ docker pull aerospike@sha256:bc2286efde1b20515a901f7df1fef3831ca4b2a04bd830d78583f328b26c1875
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53090683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:943526f108fcc376c7b5151a396f0a3330a41bb0362a0c4729deea8d761ef5b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Tue, 26 May 2020 22:20:26 GMT
ENV AEROSPIKE_VERSION=5.0.0.4
# Tue, 26 May 2020 22:20:26 GMT
ENV AEROSPIKE_SHA256=30638676e17a5918fcc91a5e1b93eec95823a465d1c68bdf8574241d5e68ea61
# Tue, 26 May 2020 22:20:54 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 26 May 2020 22:20:54 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 26 May 2020 22:20:55 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 26 May 2020 22:20:55 GMT
VOLUME [/opt/aerospike/data]
# Tue, 26 May 2020 22:20:55 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 26 May 2020 22:20:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 May 2020 22:20:56 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a14cf606a112b836e5f119002ec0b2334b0afd2d32323a3d72ee98ff25642f`  
		Last Modified: Tue, 26 May 2020 22:21:54 GMT  
		Size: 30.6 MB (30568742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72509580413e525dc37f23016b43051e3532005762c22361817ac601f5c24680`  
		Last Modified: Tue, 26 May 2020 22:21:30 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2d8a1c37f086f0bbbba02a8089f828ed0b7c0d2fb7ac179a1c4b5d6fb2013`  
		Last Modified: Tue, 26 May 2020 22:21:31 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `aerospike:latest`

```console
$ docker pull aerospike@sha256:f146a121e6ba6e75cb306b8ea37f2770539a8da9a14a71c46b1c01e6de3224dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `aerospike:latest` - linux; amd64

```console
$ docker pull aerospike@sha256:bc2286efde1b20515a901f7df1fef3831ca4b2a04bd830d78583f328b26c1875
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53090683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:943526f108fcc376c7b5151a396f0a3330a41bb0362a0c4729deea8d761ef5b5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["asd"]`

```dockerfile
# Fri, 15 May 2020 06:33:44 GMT
ADD file:ff87497c2a2fce1d776e432139030782373ac1549522a8366694786b45387306 in / 
# Fri, 15 May 2020 06:33:44 GMT
CMD ["bash"]
# Tue, 26 May 2020 22:20:26 GMT
ENV AEROSPIKE_VERSION=5.0.0.4
# Tue, 26 May 2020 22:20:26 GMT
ENV AEROSPIKE_SHA256=30638676e17a5918fcc91a5e1b93eec95823a465d1c68bdf8574241d5e68ea61
# Tue, 26 May 2020 22:20:54 GMT
RUN apt-get update -y   && apt-get install -y wget python lua5.2 gettext-base   && wget "https://www.aerospike.com/artifacts/aerospike-server-community/${AEROSPIKE_VERSION}/aerospike-server-community-${AEROSPIKE_VERSION}-debian9.tgz" -O aerospike-server.tgz   && echo "$AEROSPIKE_SHA256 *aerospike-server.tgz" | sha256sum -c -   && mkdir aerospike   && tar xzf aerospike-server.tgz --strip-components=1 -C aerospike   && dpkg -i aerospike/aerospike-server-*.deb   && dpkg -i aerospike/aerospike-tools-*.deb   && mkdir -p /var/log/aerospike/   && mkdir -p /var/run/aerospike/   && rm -rf aerospike-server.tgz aerospike /var/lib/apt/lists/*   && rm -rf /opt/aerospike/lib/java   && dpkg -r wget ca-certificates openssl xz-utils  && dpkg --purge wget ca-certificates openssl xz-utils  && apt-get purge -y   && apt autoremove -y
# Tue, 26 May 2020 22:20:54 GMT
COPY file:e804504afb5c4e22745b04c055979dfb9d5529cb7405e101861ade614def86f5 in /etc/aerospike/aerospike.template.conf 
# Tue, 26 May 2020 22:20:55 GMT
COPY file:51ea788984274d9d596ae7f174fc5d76048404a3be1d56d9df20cec477707497 in /entrypoint.sh 
# Tue, 26 May 2020 22:20:55 GMT
VOLUME [/opt/aerospike/data]
# Tue, 26 May 2020 22:20:55 GMT
EXPOSE 3000 3001 3002 3003
# Tue, 26 May 2020 22:20:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 May 2020 22:20:56 GMT
CMD ["asd"]
```

-	Layers:
	-	`sha256:e62d08fa1eb18131b4109c7cbece97f4f7e37d6ea09845a21beb3a899d0c963d`  
		Last Modified: Fri, 15 May 2020 06:40:45 GMT  
		Size: 22.5 MB (22519887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a14cf606a112b836e5f119002ec0b2334b0afd2d32323a3d72ee98ff25642f`  
		Last Modified: Tue, 26 May 2020 22:21:54 GMT  
		Size: 30.6 MB (30568742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72509580413e525dc37f23016b43051e3532005762c22361817ac601f5c24680`  
		Last Modified: Tue, 26 May 2020 22:21:30 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb2d8a1c37f086f0bbbba02a8089f828ed0b7c0d2fb7ac179a1c4b5d6fb2013`  
		Last Modified: Tue, 26 May 2020 22:21:31 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
