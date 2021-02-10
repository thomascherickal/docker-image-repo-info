## `telegraf:latest`

```console
$ docker pull telegraf@sha256:3927abad7b716d785a83af70b02a4c22f137f879221a499ac4beb4bfc25537b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:a05a950f2d426641b1f549806943ee1f7f862522a004aa5a1ff91bd0d662ee84
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.3 MB (108348187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fe56be3a20fc85dc845c8c73e677bb9c51a4757cb632af00f18c63b27a3ce05`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Jan 2021 04:53:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Jan 2021 04:53:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 29 Jan 2021 04:32:20 GMT
ENV TELEGRAF_VERSION=1.17.2
# Fri, 29 Jan 2021 04:32:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jan 2021 04:32:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jan 2021 04:32:24 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 29 Jan 2021 04:32:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jan 2021 04:32:25 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b1b9836397a1f6a8bcceaf48114f9358677f022f0872b44f5446fe6ac98590`  
		Last Modified: Wed, 13 Jan 2021 04:54:38 GMT  
		Size: 17.4 MB (17412160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d481d0989b3180f85249175a536a5497daf377815101a00b80ac6f3df31ba200`  
		Last Modified: Wed, 13 Jan 2021 04:54:32 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b755b74a2742266b814d5b3f189f8e1763c5138ddd24a6b2179e019925a4378`  
		Last Modified: Fri, 29 Jan 2021 04:33:11 GMT  
		Size: 22.7 MB (22725409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395a1e47e5e9b6e8ad986cfc21c216a8c86294cc0d34e0b13b0681af187bc85c`  
		Last Modified: Fri, 29 Jan 2021 04:33:06 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:b0223d3c0b2d6acc937a8299470515ce1efbb76a5d224a4740029515b88faac8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.7 MB (99730481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d9c338bde64304bb022b962cf79b96c4effb3a6d277c23b770c0f734bab3d6d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:29 GMT
ADD file:817a4ff41fcac0be44e95d3f0a51c9fa878d16dac7cdab68bfc445f630c43c22 in / 
# Tue, 09 Feb 2021 03:00:33 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:26:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 19:55:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 19:55:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Tue, 09 Feb 2021 19:56:28 GMT
ENV TELEGRAF_VERSION=1.17.2
# Tue, 09 Feb 2021 19:56:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 09 Feb 2021 19:56:38 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 09 Feb 2021 19:56:39 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Tue, 09 Feb 2021 19:56:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 09 Feb 2021 19:56:40 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4c2a0a79594a20b9c2f0bfbd535f875ca1b079625052cdd801afb1cc0362d6d0`  
		Last Modified: Tue, 09 Feb 2021 03:09:18 GMT  
		Size: 45.9 MB (45867053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c11c595f6421f88e1b10286a766ae8db88f67c2c0f41cedd170640aee498ab`  
		Last Modified: Tue, 09 Feb 2021 04:39:37 GMT  
		Size: 7.1 MB (7123173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cb22b679409f00e04b8d645444df7181f05cb2967ed73f1a377e7f774b6873`  
		Last Modified: Tue, 09 Feb 2021 04:39:37 GMT  
		Size: 9.3 MB (9343495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce5311dee3939b000b512866c837493d083bbc9994f6aa62ffa18d846437e86`  
		Last Modified: Tue, 09 Feb 2021 19:57:03 GMT  
		Size: 16.2 MB (16159030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cf43512439bd6f20c230833d5baee2af75a616363734c38ddb15deb7dcb7b2`  
		Last Modified: Tue, 09 Feb 2021 19:56:57 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024747a3817c30558ebffba6256cdb2c160e203b1e5680b9e77a24c391b1f7f9`  
		Last Modified: Tue, 09 Feb 2021 19:57:32 GMT  
		Size: 21.2 MB (21234647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9930b8f6e16d383afb16f3d49ef6129ced5451ee88131dd48417e8c88b106d34`  
		Last Modified: Tue, 09 Feb 2021 19:57:25 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f1e9729daf7a97ebd21b4f42cbff85c298af836433518defff43876fc6c5b723
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.0 MB (104963136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56313f68c41fb89b9e32c106745b9bd4e8332432126f549c798604deedeb1780`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Feb 2021 02:40:45 GMT
ADD file:78412ee35e3dc6fb5fdfce41eb05dd273ba1d49328ab327465639bfa4821aa51 in / 
# Tue, 09 Feb 2021 02:40:50 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:43:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:43:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 10 Feb 2021 01:34:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 10 Feb 2021 01:34:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 10 Feb 2021 01:34:57 GMT
ENV TELEGRAF_VERSION=1.17.2
# Wed, 10 Feb 2021 01:35:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 10 Feb 2021 01:35:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 10 Feb 2021 01:35:04 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 10 Feb 2021 01:35:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Feb 2021 01:35:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c78c297fb0d010ee085f95ae439636ecb167b050c1acb4273bd576998cf94a83`  
		Last Modified: Tue, 09 Feb 2021 02:47:03 GMT  
		Size: 49.2 MB (49183229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06af62193c25241eb123af8cf115c7a6298e834976fe148ac79ec11a7ca06ee5`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 7.7 MB (7694122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b846e1b73901174c506ae5e6219ac2f356ef71eaa5896dfbc238dc67ca4bf73`  
		Last Modified: Tue, 09 Feb 2021 04:57:24 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f612f69ce7b7ea13616165baa95712bc8fffcccb5edbad3e64092dbf3e553f9`  
		Last Modified: Wed, 10 Feb 2021 01:35:26 GMT  
		Size: 17.3 MB (17269513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d18ce172c92baee16f65c0b522d8bc636a36202351339897d05c4645a2d79f`  
		Last Modified: Wed, 10 Feb 2021 01:35:21 GMT  
		Size: 2.9 KB (2896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1194a7e65e5067f9f8a2ab8236eecd36c4042aff55c2c87fb41d17dc9a32eb4c`  
		Last Modified: Wed, 10 Feb 2021 01:35:55 GMT  
		Size: 20.8 MB (20828912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caedcd287509d831920291aab344faa08cbdb47d44ad9fba0379ba15105f4834`  
		Last Modified: Wed, 10 Feb 2021 01:35:51 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
