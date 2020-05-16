## `telegraf:latest`

```console
$ docker pull telegraf@sha256:4230c34d1f72ce7a427acecc2d74e1735f04b3c41157c818459008ccd1f26d60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:1db0840b1e240edffe9283bba13e2ba8b8e85ff4da74159b7f2496245c8ed007
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97897312 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6828ec3da942d2dec646b1f30af5ee86447ce87f136dbc16093f54378087221a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 15 May 2020 06:33:25 GMT
ADD file:13031623172f5c5857e27de93553adedf17d955fa370882f850bb6ed6fb8cee7 in / 
# Fri, 15 May 2020 06:33:25 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:43:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:43:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 May 2020 09:30:09 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 May 2020 09:30:12 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Sat, 16 May 2020 09:30:35 GMT
ENV TELEGRAF_VERSION=1.14.2
# Sat, 16 May 2020 09:30:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 16 May 2020 09:30:38 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 16 May 2020 09:30:38 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Sat, 16 May 2020 09:30:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 May 2020 09:30:39 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1c6172af85ee14a8db5a3a51d406b768dfa94d196c06d0d06d591507cf8199f0`  
		Last Modified: Fri, 15 May 2020 06:40:31 GMT  
		Size: 45.4 MB (45375207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b194b0e3c928807cfabf081055a117585ba5bf6697f65b2fede02225a5d73ad2`  
		Last Modified: Fri, 15 May 2020 17:55:27 GMT  
		Size: 10.8 MB (10797475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec00f35d5b2d1db6b8e925a3005c1a285365775028db0339903ddaeec4763`  
		Last Modified: Fri, 15 May 2020 17:55:29 GMT  
		Size: 4.3 MB (4340139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2ff79628f92ee47ce852ddfaa8aa614813357006710928b2045000f400f65e`  
		Last Modified: Sat, 16 May 2020 09:30:55 GMT  
		Size: 16.0 MB (15964693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232b2e3770a921b5ed3597d33cc9fbfa9146ec870cda52c3d48089e8d762e8d9`  
		Last Modified: Sat, 16 May 2020 09:30:52 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bed5708aeb95e7a2278c56a3861c186f953ecf1b4721e87bbb60b465b177a95`  
		Last Modified: Sat, 16 May 2020 09:31:13 GMT  
		Size: 21.4 MB (21416842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08483e242e4c44b807108b6bdd6b7014b65ba67cde23a1f0c48eb594e358801`  
		Last Modified: Sat, 16 May 2020 09:31:08 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:84b649d55c3eae444e692561562ebd3d994cad112ad11032fd618491d35b972f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90493270 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd94503327a88f7950fc568e8701dfb7cce0969ab87fe82681fe6bac5172be2b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 15 May 2020 01:06:22 GMT
ADD file:89db8453485648b09e63411b6e2ad84f08844ee55cb115e59cdc8c8cb1c29a1f in / 
# Fri, 15 May 2020 01:06:23 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:48:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:49:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 21:59:41 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 22:00:52 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Fri, 15 May 2020 22:04:22 GMT
ENV TELEGRAF_VERSION=1.14.2
# Fri, 15 May 2020 22:05:04 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 15 May 2020 22:05:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 15 May 2020 22:05:23 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 15 May 2020 22:05:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 22:05:39 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:11acdea2de14253903f5970d63a2076ff08912929430d1c33afe617c9fa6bf8f`  
		Last Modified: Fri, 15 May 2020 01:14:46 GMT  
		Size: 42.1 MB (42104346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99452f66748f5df5d89d2287e42b5c3d87c9d5e1e20c16ef729e87d463840cf7`  
		Last Modified: Fri, 15 May 2020 11:01:44 GMT  
		Size: 9.5 MB (9498344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cef06b7abe4487657829b47c97bd2992f14a34349e0bcf60a47de9c647bd3fb`  
		Last Modified: Fri, 15 May 2020 11:01:43 GMT  
		Size: 3.9 MB (3918713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e491a78695052b3ccb2badf6ed2c7ab7b37f87e0e943d9cc2957cce60b2331`  
		Last Modified: Fri, 15 May 2020 22:06:06 GMT  
		Size: 14.8 MB (14839243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f637ecae920d2d210a37ac6fbb04b0ff574a49c399b6e1e6837cb948f347e1cd`  
		Last Modified: Fri, 15 May 2020 22:06:04 GMT  
		Size: 2.8 KB (2800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07f8795a3e08cf8f94543f5b3a166bfc9f9066023555c576c5e3c77c5491df4`  
		Last Modified: Fri, 15 May 2020 22:06:50 GMT  
		Size: 20.1 MB (20129638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1294097e810b7810ff93a5ef76516d94b8f654b50f54ca75b344c195a98df6d`  
		Last Modified: Fri, 15 May 2020 22:06:43 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:07d78854ed7bcdec532a3fe34fc1a6c2dd7e38a7cd366badb4534e31b05402b5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92258898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378d588d2281110d16df2180a73bc2f2fd01f51606a3928ebe829b5be4aa9aa7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:23:37 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:23:42 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 29 Apr 2020 04:16:47 GMT
ENV TELEGRAF_VERSION=1.14.2
# Wed, 29 Apr 2020 04:16:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 29 Apr 2020 04:16:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 29 Apr 2020 04:16:58 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 29 Apr 2020 04:16:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 29 Apr 2020 04:17:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e063050434db1728e621506c3cfad2c7c247fe84e03b3c33470cb1027d09a6`  
		Last Modified: Thu, 23 Apr 2020 21:24:40 GMT  
		Size: 15.5 MB (15530251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a6bf49b82384126f8c9969d6fd716c5ee05b38147cdd2abc4d6599541de512`  
		Last Modified: Thu, 23 Apr 2020 21:24:35 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1926eb91dfdf94748bac8b240efdccec06386a292ea9f911353d84d09718472`  
		Last Modified: Wed, 29 Apr 2020 04:17:19 GMT  
		Size: 19.7 MB (19723662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9228e8cece76cbd8c5454cdf0e71113a653fdf8676487b0c373760aa27de2d7c`  
		Last Modified: Wed, 29 Apr 2020 04:17:13 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
