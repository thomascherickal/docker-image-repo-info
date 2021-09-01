<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kapacitor`

-	[`kapacitor:1.5`](#kapacitor15)
-	[`kapacitor:1.5-alpine`](#kapacitor15-alpine)
-	[`kapacitor:1.5.9`](#kapacitor159)
-	[`kapacitor:1.5.9-alpine`](#kapacitor159-alpine)
-	[`kapacitor:1.6`](#kapacitor16)
-	[`kapacitor:1.6-alpine`](#kapacitor16-alpine)
-	[`kapacitor:1.6.1`](#kapacitor161)
-	[`kapacitor:1.6.1-alpine`](#kapacitor161-alpine)
-	[`kapacitor:alpine`](#kapacitoralpine)
-	[`kapacitor:latest`](#kapacitorlatest)

## `kapacitor:1.5`

```console
$ docker pull kapacitor@sha256:09ebd896a0b3ed3f47d74ee9146545591664277ea20b2ce8b276a485843391ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5` - linux; amd64

```console
$ docker pull kapacitor@sha256:bb089931dbaad2ef28526cd2c40a839e8c5995cd8265be3fb7e306e205191ef2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111563379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9184cdbff2473fc42ca22d4759d13be78d12c72a5f5f69d5a52dba423840cf4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:56 GMT
ADD file:0d0aa1ebd07b0f301aaf1077d1e9f2e9be1859510dd8535e143571b347a2a379 in / 
# Tue, 17 Aug 2021 01:25:56 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:24:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 07:01:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 07:01:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 07:01:29 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 18 Aug 2021 07:01:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 07:01:33 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 07:01:34 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 07:01:34 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 07:01:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 07:01:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 07:01:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:eb18d230e067c240479c6a3f842e7f9d4ff1088e3072d0a3245829c4e356623f`  
		Last Modified: Tue, 17 Aug 2021 01:33:03 GMT  
		Size: 45.4 MB (45379966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83600c1b4583abb5830c6d4a039cbab9a102ac1a7b3b779854638a371bb7128f`  
		Last Modified: Tue, 17 Aug 2021 09:33:12 GMT  
		Size: 11.3 MB (11295906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae15c65bfa0fdc9053dcb734e6c034f5394ea0481dee3277f6e3e9fa07702d0`  
		Last Modified: Tue, 17 Aug 2021 09:33:11 GMT  
		Size: 4.3 MB (4342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df9a81a6e6330b08dc4ea9322d4dbc9131ceb336f4f48222299992bee24d20c`  
		Last Modified: Wed, 18 Aug 2021 07:02:07 GMT  
		Size: 13.3 MB (13322522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ac9e7ace861b8fefc86ece32a745d3860247036ec12dca6a51e6436f64cfe6`  
		Last Modified: Wed, 18 Aug 2021 07:02:05 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51074876d326021dd844c3542120b88fe5845cec7e06e7631eda29afa627d7`  
		Last Modified: Wed, 18 Aug 2021 07:02:10 GMT  
		Size: 37.2 MB (37219290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fd780d2c50b816d5db46a42f0c3070bcc223cb2aefb6fda90f693beed3a258`  
		Last Modified: Wed, 18 Aug 2021 07:02:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba2e7f59ac966696e08fada5b63ed25da9d0d601dc818ce4c230146eef21ac4`  
		Last Modified: Wed, 18 Aug 2021 07:02:05 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:ab6bbc7d7030a12cc1de1253a7c2a42e2cf2bc998774f959ed3303a41af521b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104285309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46b57dd609214fefb28989704b619b335631d6e9d77611f11433dd507253d0a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 02:19:00 GMT
ADD file:5e5e5a4e13ae8e36740009c29111838a32d9901b28809b485c841d25d550698b in / 
# Tue, 17 Aug 2021 02:19:01 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:28:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 22:45:26 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 22:45:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 22:45:31 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 18 Aug 2021 22:45:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 22:45:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 22:45:41 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 22:45:42 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 22:45:42 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 22:45:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 22:45:43 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:30d3c67f4f95a7d99559389477234b45c05024484d59cec2d66264610a623fe9`  
		Last Modified: Tue, 17 Aug 2021 02:36:17 GMT  
		Size: 42.1 MB (42119745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e002433047948d255f28ba7ee556c302875d03d4d84f4b30b34ed9aeb481ef27`  
		Last Modified: Tue, 17 Aug 2021 15:46:54 GMT  
		Size: 10.0 MB (9951645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a501430415711f6cdd553e589abddd926f28b6f57669a8fafbbc06811a06d`  
		Last Modified: Tue, 17 Aug 2021 15:46:51 GMT  
		Size: 3.9 MB (3921237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd054fb54a132cb9e7f19bc9764a9434703dc3a2ee15a1d2f7ea39650eb3a411`  
		Last Modified: Wed, 18 Aug 2021 22:46:13 GMT  
		Size: 13.5 MB (13502661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d67efd24b51630c96bff1df01a207a55064c1eb3b987e15f1e7b8d6d080885`  
		Last Modified: Wed, 18 Aug 2021 22:46:08 GMT  
		Size: 2.9 KB (2857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b52f7d82af8ae34d00fe2994cfc18a978adf02d2547e2bd399cd386e77dbea`  
		Last Modified: Wed, 18 Aug 2021 22:46:25 GMT  
		Size: 34.8 MB (34786705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf01a5a9514a4bb4487c25036d80c6c3a2777407caec70697b1b2d7f296a0ed`  
		Last Modified: Wed, 18 Aug 2021 22:46:08 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf907a72c945feb1985ba745dc00c3d2bbc091b0cc0041bee18cfd3ac193787`  
		Last Modified: Wed, 18 Aug 2021 22:46:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:68a7b35baa283c4865d5e980280b0276c4d6d14a489f59aea0771babcf3f60d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105079408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b8be3152db041ae15a56f9525aa82925eeeac4e8b4f1e83b6911f9da104c50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:17 GMT
ADD file:79e0d0ec943ec405612e2310514d8f0c72cf83483eea6d5f1a7c28b36fa21cf8 in / 
# Tue, 17 Aug 2021 01:48:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:56:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:56:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 03:04:28 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 03:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 03:04:32 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 18 Aug 2021 03:04:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 03:04:36 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 03:04:37 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 03:04:37 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 03:04:37 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 03:04:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 03:04:37 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a410f7a7fb8af899e64ef008ec59cc8062766e91abbf21ba5cee65faac7ba3fa`  
		Last Modified: Tue, 17 Aug 2021 01:57:32 GMT  
		Size: 43.2 MB (43177652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e420ab67f91937cc8165f5fb2e94bdab905576eadca5515be250bc6212fe50`  
		Last Modified: Tue, 17 Aug 2021 08:04:49 GMT  
		Size: 10.2 MB (10215748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce4bbd3804fd1154090db6722050023d8242e910e02ed7d2c09b9795a9d5ac`  
		Last Modified: Tue, 17 Aug 2021 08:04:48 GMT  
		Size: 4.1 MB (4096582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151ac1cfab8790dc49973599fa396ed1be6d7c7941973b59135f515444b730be`  
		Last Modified: Wed, 18 Aug 2021 03:05:10 GMT  
		Size: 13.0 MB (13025171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918b8c0940b453d44ba7db5d3637f4123eb859a3817e86d547b0a677ec9bb051`  
		Last Modified: Wed, 18 Aug 2021 03:05:08 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39479fb4a2cddd3ed9efab594360312005a73c1cda58b6f94d8480b9a4a80cdf`  
		Last Modified: Wed, 18 Aug 2021 03:05:13 GMT  
		Size: 34.6 MB (34560947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b292b729814b071d5e0c0a7f4a22bdfb6f81a76482c197a075352b364cbeb66`  
		Last Modified: Wed, 18 Aug 2021 03:05:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe27079a3de6524ec3c861601187a9acb6ebf2e7a9b0802eb1ab1215628444a`  
		Last Modified: Wed, 18 Aug 2021 03:05:08 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5-alpine`

```console
$ docker pull kapacitor@sha256:2cdcab2a7797521e528a0a87065180d4f73c7822018996006320ef2b3e08b071
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:aec3c23ef7bc93b5791141f8fe2793404aad85a1a11f6b8d7ee2fdc62d40b781
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22625231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8f5a6c0287e53b4889d011df8971ef0630dce5ec50329c524d70043cf339cd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:23:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:23:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 01 Sep 2021 03:04:15 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 01 Sep 2021 03:04:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 01 Sep 2021 03:04:20 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 01 Sep 2021 03:04:20 GMT
EXPOSE 9092
# Wed, 01 Sep 2021 03:04:21 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 01 Sep 2021 03:04:21 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Wed, 01 Sep 2021 03:04:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 03:04:21 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69cd3502d3b453e253ea48e4ff56f5af4e25895a1bfa5e84cda59eaefce23be`  
		Last Modified: Wed, 01 Sep 2021 00:25:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7087df4b29e442773e368f72aa50cd7765fd6e6b43879c83880b0038e62b9077`  
		Last Modified: Wed, 01 Sep 2021 00:25:29 GMT  
		Size: 280.9 KB (280879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c781830543db249e742723c9ae5bdc70eb4c663278c7c28add837b5b20bc61e`  
		Last Modified: Wed, 01 Sep 2021 03:05:06 GMT  
		Size: 19.5 MB (19542013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec0599af5a04b1b7dad3ff6168e9fdb159c02e3149f99abafd7819204a5fca`  
		Last Modified: Wed, 01 Sep 2021 03:05:02 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f39527004d52de4b800959b812c0cbc9c2167b67ac327f7416d90afbf6d1b7d`  
		Last Modified: Wed, 01 Sep 2021 03:05:02 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9`

```console
$ docker pull kapacitor@sha256:09ebd896a0b3ed3f47d74ee9146545591664277ea20b2ce8b276a485843391ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `kapacitor:1.5.9` - linux; amd64

```console
$ docker pull kapacitor@sha256:bb089931dbaad2ef28526cd2c40a839e8c5995cd8265be3fb7e306e205191ef2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.6 MB (111563379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9184cdbff2473fc42ca22d4759d13be78d12c72a5f5f69d5a52dba423840cf4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:56 GMT
ADD file:0d0aa1ebd07b0f301aaf1077d1e9f2e9be1859510dd8535e143571b347a2a379 in / 
# Tue, 17 Aug 2021 01:25:56 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:24:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 07:01:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 07:01:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 07:01:29 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 18 Aug 2021 07:01:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 07:01:33 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 07:01:34 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 07:01:34 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 07:01:34 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 07:01:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 07:01:34 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:eb18d230e067c240479c6a3f842e7f9d4ff1088e3072d0a3245829c4e356623f`  
		Last Modified: Tue, 17 Aug 2021 01:33:03 GMT  
		Size: 45.4 MB (45379966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83600c1b4583abb5830c6d4a039cbab9a102ac1a7b3b779854638a371bb7128f`  
		Last Modified: Tue, 17 Aug 2021 09:33:12 GMT  
		Size: 11.3 MB (11295906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae15c65bfa0fdc9053dcb734e6c034f5394ea0481dee3277f6e3e9fa07702d0`  
		Last Modified: Tue, 17 Aug 2021 09:33:11 GMT  
		Size: 4.3 MB (4342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df9a81a6e6330b08dc4ea9322d4dbc9131ceb336f4f48222299992bee24d20c`  
		Last Modified: Wed, 18 Aug 2021 07:02:07 GMT  
		Size: 13.3 MB (13322522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ac9e7ace861b8fefc86ece32a745d3860247036ec12dca6a51e6436f64cfe6`  
		Last Modified: Wed, 18 Aug 2021 07:02:05 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51074876d326021dd844c3542120b88fe5845cec7e06e7631eda29afa627d7`  
		Last Modified: Wed, 18 Aug 2021 07:02:10 GMT  
		Size: 37.2 MB (37219290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fd780d2c50b816d5db46a42f0c3070bcc223cb2aefb6fda90f693beed3a258`  
		Last Modified: Wed, 18 Aug 2021 07:02:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba2e7f59ac966696e08fada5b63ed25da9d0d601dc818ce4c230146eef21ac4`  
		Last Modified: Wed, 18 Aug 2021 07:02:05 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm variant v7

```console
$ docker pull kapacitor@sha256:ab6bbc7d7030a12cc1de1253a7c2a42e2cf2bc998774f959ed3303a41af521b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104285309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46b57dd609214fefb28989704b619b335631d6e9d77611f11433dd507253d0a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 02:19:00 GMT
ADD file:5e5e5a4e13ae8e36740009c29111838a32d9901b28809b485c841d25d550698b in / 
# Tue, 17 Aug 2021 02:19:01 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 15:28:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 15:28:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 22:45:26 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 22:45:31 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 22:45:31 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 18 Aug 2021 22:45:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 22:45:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 22:45:41 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 22:45:42 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 22:45:42 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 22:45:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 22:45:43 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:30d3c67f4f95a7d99559389477234b45c05024484d59cec2d66264610a623fe9`  
		Last Modified: Tue, 17 Aug 2021 02:36:17 GMT  
		Size: 42.1 MB (42119745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e002433047948d255f28ba7ee556c302875d03d4d84f4b30b34ed9aeb481ef27`  
		Last Modified: Tue, 17 Aug 2021 15:46:54 GMT  
		Size: 10.0 MB (9951645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9a501430415711f6cdd553e589abddd926f28b6f57669a8fafbbc06811a06d`  
		Last Modified: Tue, 17 Aug 2021 15:46:51 GMT  
		Size: 3.9 MB (3921237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd054fb54a132cb9e7f19bc9764a9434703dc3a2ee15a1d2f7ea39650eb3a411`  
		Last Modified: Wed, 18 Aug 2021 22:46:13 GMT  
		Size: 13.5 MB (13502661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d67efd24b51630c96bff1df01a207a55064c1eb3b987e15f1e7b8d6d080885`  
		Last Modified: Wed, 18 Aug 2021 22:46:08 GMT  
		Size: 2.9 KB (2857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b52f7d82af8ae34d00fe2994cfc18a978adf02d2547e2bd399cd386e77dbea`  
		Last Modified: Wed, 18 Aug 2021 22:46:25 GMT  
		Size: 34.8 MB (34786705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf01a5a9514a4bb4487c25036d80c6c3a2777407caec70697b1b2d7f296a0ed`  
		Last Modified: Wed, 18 Aug 2021 22:46:08 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf907a72c945feb1985ba745dc00c3d2bbc091b0cc0041bee18cfd3ac193787`  
		Last Modified: Wed, 18 Aug 2021 22:46:08 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.5.9` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:68a7b35baa283c4865d5e980280b0276c4d6d14a489f59aea0771babcf3f60d3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.1 MB (105079408 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b8be3152db041ae15a56f9525aa82925eeeac4e8b4f1e83b6911f9da104c50`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:17 GMT
ADD file:79e0d0ec943ec405612e2310514d8f0c72cf83483eea6d5f1a7c28b36fa21cf8 in / 
# Tue, 17 Aug 2021 01:48:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:56:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:56:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 03:04:28 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 03:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 03:04:32 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 18 Aug 2021 03:04:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 03:04:36 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 03:04:37 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 03:04:37 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 03:04:37 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 03:04:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 03:04:37 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a410f7a7fb8af899e64ef008ec59cc8062766e91abbf21ba5cee65faac7ba3fa`  
		Last Modified: Tue, 17 Aug 2021 01:57:32 GMT  
		Size: 43.2 MB (43177652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e420ab67f91937cc8165f5fb2e94bdab905576eadca5515be250bc6212fe50`  
		Last Modified: Tue, 17 Aug 2021 08:04:49 GMT  
		Size: 10.2 MB (10215748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce4bbd3804fd1154090db6722050023d8242e910e02ed7d2c09b9795a9d5ac`  
		Last Modified: Tue, 17 Aug 2021 08:04:48 GMT  
		Size: 4.1 MB (4096582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151ac1cfab8790dc49973599fa396ed1be6d7c7941973b59135f515444b730be`  
		Last Modified: Wed, 18 Aug 2021 03:05:10 GMT  
		Size: 13.0 MB (13025171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918b8c0940b453d44ba7db5d3637f4123eb859a3817e86d547b0a677ec9bb051`  
		Last Modified: Wed, 18 Aug 2021 03:05:08 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39479fb4a2cddd3ed9efab594360312005a73c1cda58b6f94d8480b9a4a80cdf`  
		Last Modified: Wed, 18 Aug 2021 03:05:13 GMT  
		Size: 34.6 MB (34560947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b292b729814b071d5e0c0a7f4a22bdfb6f81a76482c197a075352b364cbeb66`  
		Last Modified: Wed, 18 Aug 2021 03:05:08 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe27079a3de6524ec3c861601187a9acb6ebf2e7a9b0802eb1ab1215628444a`  
		Last Modified: Wed, 18 Aug 2021 03:05:08 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.5.9-alpine`

```console
$ docker pull kapacitor@sha256:2cdcab2a7797521e528a0a87065180d4f73c7822018996006320ef2b3e08b071
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.5.9-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:aec3c23ef7bc93b5791141f8fe2793404aad85a1a11f6b8d7ee2fdc62d40b781
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22625231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c8f5a6c0287e53b4889d011df8971ef0630dce5ec50329c524d70043cf339cd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:23:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:23:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 01 Sep 2021 03:04:15 GMT
ENV KAPACITOR_VERSION=1.5.9
# Wed, 01 Sep 2021 03:04:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 01 Sep 2021 03:04:20 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 01 Sep 2021 03:04:20 GMT
EXPOSE 9092
# Wed, 01 Sep 2021 03:04:21 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 01 Sep 2021 03:04:21 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Wed, 01 Sep 2021 03:04:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 03:04:21 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69cd3502d3b453e253ea48e4ff56f5af4e25895a1bfa5e84cda59eaefce23be`  
		Last Modified: Wed, 01 Sep 2021 00:25:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7087df4b29e442773e368f72aa50cd7765fd6e6b43879c83880b0038e62b9077`  
		Last Modified: Wed, 01 Sep 2021 00:25:29 GMT  
		Size: 280.9 KB (280879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c781830543db249e742723c9ae5bdc70eb4c663278c7c28add837b5b20bc61e`  
		Last Modified: Wed, 01 Sep 2021 03:05:06 GMT  
		Size: 19.5 MB (19542013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec0599af5a04b1b7dad3ff6168e9fdb159c02e3149f99abafd7819204a5fca`  
		Last Modified: Wed, 01 Sep 2021 03:05:02 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f39527004d52de4b800959b812c0cbc9c2167b67ac327f7416d90afbf6d1b7d`  
		Last Modified: Wed, 01 Sep 2021 03:05:02 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6`

```console
$ docker pull kapacitor@sha256:214f7ab2493e72e0c690e2911b2b5ad25284d6459baf54a6f5f78316283eb67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6` - linux; amd64

```console
$ docker pull kapacitor@sha256:7153c14ce9004d4389fc69f407311389e848df2e044c7c699b25ff1e9fa0b4fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133606214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc13f62beab87315296150a800a4e1ba8dfc6bc1bf53ad6e6774cf958a1401a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:56 GMT
ADD file:0d0aa1ebd07b0f301aaf1077d1e9f2e9be1859510dd8535e143571b347a2a379 in / 
# Tue, 17 Aug 2021 01:25:56 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:24:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 07:01:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 07:01:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 07:01:40 GMT
ENV KAPACITOR_VERSION=1.6.1
# Wed, 18 Aug 2021 07:01:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 07:01:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 07:01:45 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 07:01:45 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 07:01:45 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 07:01:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 07:01:46 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:eb18d230e067c240479c6a3f842e7f9d4ff1088e3072d0a3245829c4e356623f`  
		Last Modified: Tue, 17 Aug 2021 01:33:03 GMT  
		Size: 45.4 MB (45379966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83600c1b4583abb5830c6d4a039cbab9a102ac1a7b3b779854638a371bb7128f`  
		Last Modified: Tue, 17 Aug 2021 09:33:12 GMT  
		Size: 11.3 MB (11295906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae15c65bfa0fdc9053dcb734e6c034f5394ea0481dee3277f6e3e9fa07702d0`  
		Last Modified: Tue, 17 Aug 2021 09:33:11 GMT  
		Size: 4.3 MB (4342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df9a81a6e6330b08dc4ea9322d4dbc9131ceb336f4f48222299992bee24d20c`  
		Last Modified: Wed, 18 Aug 2021 07:02:07 GMT  
		Size: 13.3 MB (13322522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ac9e7ace861b8fefc86ece32a745d3860247036ec12dca6a51e6436f64cfe6`  
		Last Modified: Wed, 18 Aug 2021 07:02:05 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1cc761767c20764cf1890fd66d9fe9b0c73793ffd089bb7010d856e3379946`  
		Last Modified: Wed, 18 Aug 2021 07:02:29 GMT  
		Size: 59.3 MB (59262125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c31ea119f5e5d39540a41d2bd75569c0967d85b58e6af5592701e382cf3603`  
		Last Modified: Wed, 18 Aug 2021 07:02:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fb14f03d554baca4f313ccbaddb34e22c9da8d46e6a3aa2ff345503b0d9d06`  
		Last Modified: Wed, 18 Aug 2021 07:02:21 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:bb3c234e66dfa59d248b87cee4296683b657746d08d662675aa83d300aaf5957
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126412617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2d82c3b2c970a55952ec9459906b48548ebfe5e31952e7027918bc433967e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:17 GMT
ADD file:79e0d0ec943ec405612e2310514d8f0c72cf83483eea6d5f1a7c28b36fa21cf8 in / 
# Tue, 17 Aug 2021 01:48:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:56:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:56:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 03:04:28 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 03:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 03:04:43 GMT
ENV KAPACITOR_VERSION=1.6.1
# Wed, 18 Aug 2021 03:04:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 03:04:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 03:04:47 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 03:04:48 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 03:04:48 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 03:04:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 03:04:48 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a410f7a7fb8af899e64ef008ec59cc8062766e91abbf21ba5cee65faac7ba3fa`  
		Last Modified: Tue, 17 Aug 2021 01:57:32 GMT  
		Size: 43.2 MB (43177652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e420ab67f91937cc8165f5fb2e94bdab905576eadca5515be250bc6212fe50`  
		Last Modified: Tue, 17 Aug 2021 08:04:49 GMT  
		Size: 10.2 MB (10215748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce4bbd3804fd1154090db6722050023d8242e910e02ed7d2c09b9795a9d5ac`  
		Last Modified: Tue, 17 Aug 2021 08:04:48 GMT  
		Size: 4.1 MB (4096582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151ac1cfab8790dc49973599fa396ed1be6d7c7941973b59135f515444b730be`  
		Last Modified: Wed, 18 Aug 2021 03:05:10 GMT  
		Size: 13.0 MB (13025171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918b8c0940b453d44ba7db5d3637f4123eb859a3817e86d547b0a677ec9bb051`  
		Last Modified: Wed, 18 Aug 2021 03:05:08 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b545f7a05e164a6464596480ab593368549e63552f2c253130589d7a69dffa3`  
		Last Modified: Wed, 18 Aug 2021 03:05:33 GMT  
		Size: 55.9 MB (55894157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22483778e68af06d02517e68ca78f872bcdd3558272fe774717854d2e191693`  
		Last Modified: Wed, 18 Aug 2021 03:05:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98f8758a8b6b71214bc116749a3a506c46efa2a44a7655f0cc6e97aef2c9221`  
		Last Modified: Wed, 18 Aug 2021 03:05:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6-alpine`

```console
$ docker pull kapacitor@sha256:7896801d6eeb35bbcbed36310760a3b1ff3120d16b23aaf20267a3e927b8936d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:b3c9c70bdad340a180f54ab64c17a420e8ea6544513bb86d1d5ee61c980c1f16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62282802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c171de764c09f16e4ce559429bf58d7f552765083dabe7eeaff600d961ba3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:23:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:23:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 01 Sep 2021 03:04:27 GMT
ENV KAPACITOR_VERSION=1.6.1
# Wed, 01 Sep 2021 03:04:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 01 Sep 2021 03:04:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 01 Sep 2021 03:04:41 GMT
EXPOSE 9092
# Wed, 01 Sep 2021 03:04:41 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 01 Sep 2021 03:04:42 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Wed, 01 Sep 2021 03:04:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 03:04:42 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69cd3502d3b453e253ea48e4ff56f5af4e25895a1bfa5e84cda59eaefce23be`  
		Last Modified: Wed, 01 Sep 2021 00:25:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7087df4b29e442773e368f72aa50cd7765fd6e6b43879c83880b0038e62b9077`  
		Last Modified: Wed, 01 Sep 2021 00:25:29 GMT  
		Size: 280.9 KB (280879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7cb5b6248de8e40cb59c8a172882bcf139b97f02ea65ba88919ed2aadef1e9`  
		Last Modified: Wed, 01 Sep 2021 03:05:26 GMT  
		Size: 59.2 MB (59199583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e72ce875cf5d94b0730927e9e97d3df95bdfb5651c544f52ac5c124f2f43e5`  
		Last Modified: Wed, 01 Sep 2021 03:05:17 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0b546e47c7e79bda5d79a7be609e9c46eedd0801b11be06c36d4c4bfde1b39`  
		Last Modified: Wed, 01 Sep 2021 03:05:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.1`

```console
$ docker pull kapacitor@sha256:214f7ab2493e72e0c690e2911b2b5ad25284d6459baf54a6f5f78316283eb67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:1.6.1` - linux; amd64

```console
$ docker pull kapacitor@sha256:7153c14ce9004d4389fc69f407311389e848df2e044c7c699b25ff1e9fa0b4fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133606214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc13f62beab87315296150a800a4e1ba8dfc6bc1bf53ad6e6774cf958a1401a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:56 GMT
ADD file:0d0aa1ebd07b0f301aaf1077d1e9f2e9be1859510dd8535e143571b347a2a379 in / 
# Tue, 17 Aug 2021 01:25:56 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:24:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 07:01:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 07:01:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 07:01:40 GMT
ENV KAPACITOR_VERSION=1.6.1
# Wed, 18 Aug 2021 07:01:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 07:01:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 07:01:45 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 07:01:45 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 07:01:45 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 07:01:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 07:01:46 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:eb18d230e067c240479c6a3f842e7f9d4ff1088e3072d0a3245829c4e356623f`  
		Last Modified: Tue, 17 Aug 2021 01:33:03 GMT  
		Size: 45.4 MB (45379966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83600c1b4583abb5830c6d4a039cbab9a102ac1a7b3b779854638a371bb7128f`  
		Last Modified: Tue, 17 Aug 2021 09:33:12 GMT  
		Size: 11.3 MB (11295906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae15c65bfa0fdc9053dcb734e6c034f5394ea0481dee3277f6e3e9fa07702d0`  
		Last Modified: Tue, 17 Aug 2021 09:33:11 GMT  
		Size: 4.3 MB (4342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df9a81a6e6330b08dc4ea9322d4dbc9131ceb336f4f48222299992bee24d20c`  
		Last Modified: Wed, 18 Aug 2021 07:02:07 GMT  
		Size: 13.3 MB (13322522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ac9e7ace861b8fefc86ece32a745d3860247036ec12dca6a51e6436f64cfe6`  
		Last Modified: Wed, 18 Aug 2021 07:02:05 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1cc761767c20764cf1890fd66d9fe9b0c73793ffd089bb7010d856e3379946`  
		Last Modified: Wed, 18 Aug 2021 07:02:29 GMT  
		Size: 59.3 MB (59262125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c31ea119f5e5d39540a41d2bd75569c0967d85b58e6af5592701e382cf3603`  
		Last Modified: Wed, 18 Aug 2021 07:02:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fb14f03d554baca4f313ccbaddb34e22c9da8d46e6a3aa2ff345503b0d9d06`  
		Last Modified: Wed, 18 Aug 2021 07:02:21 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:1.6.1` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:bb3c234e66dfa59d248b87cee4296683b657746d08d662675aa83d300aaf5957
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126412617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2d82c3b2c970a55952ec9459906b48548ebfe5e31952e7027918bc433967e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:17 GMT
ADD file:79e0d0ec943ec405612e2310514d8f0c72cf83483eea6d5f1a7c28b36fa21cf8 in / 
# Tue, 17 Aug 2021 01:48:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:56:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:56:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 03:04:28 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 03:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 03:04:43 GMT
ENV KAPACITOR_VERSION=1.6.1
# Wed, 18 Aug 2021 03:04:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 03:04:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 03:04:47 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 03:04:48 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 03:04:48 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 03:04:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 03:04:48 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a410f7a7fb8af899e64ef008ec59cc8062766e91abbf21ba5cee65faac7ba3fa`  
		Last Modified: Tue, 17 Aug 2021 01:57:32 GMT  
		Size: 43.2 MB (43177652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e420ab67f91937cc8165f5fb2e94bdab905576eadca5515be250bc6212fe50`  
		Last Modified: Tue, 17 Aug 2021 08:04:49 GMT  
		Size: 10.2 MB (10215748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce4bbd3804fd1154090db6722050023d8242e910e02ed7d2c09b9795a9d5ac`  
		Last Modified: Tue, 17 Aug 2021 08:04:48 GMT  
		Size: 4.1 MB (4096582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151ac1cfab8790dc49973599fa396ed1be6d7c7941973b59135f515444b730be`  
		Last Modified: Wed, 18 Aug 2021 03:05:10 GMT  
		Size: 13.0 MB (13025171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918b8c0940b453d44ba7db5d3637f4123eb859a3817e86d547b0a677ec9bb051`  
		Last Modified: Wed, 18 Aug 2021 03:05:08 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b545f7a05e164a6464596480ab593368549e63552f2c253130589d7a69dffa3`  
		Last Modified: Wed, 18 Aug 2021 03:05:33 GMT  
		Size: 55.9 MB (55894157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22483778e68af06d02517e68ca78f872bcdd3558272fe774717854d2e191693`  
		Last Modified: Wed, 18 Aug 2021 03:05:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98f8758a8b6b71214bc116749a3a506c46efa2a44a7655f0cc6e97aef2c9221`  
		Last Modified: Wed, 18 Aug 2021 03:05:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:1.6.1-alpine`

```console
$ docker pull kapacitor@sha256:7896801d6eeb35bbcbed36310760a3b1ff3120d16b23aaf20267a3e927b8936d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:1.6.1-alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:b3c9c70bdad340a180f54ab64c17a420e8ea6544513bb86d1d5ee61c980c1f16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62282802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c171de764c09f16e4ce559429bf58d7f552765083dabe7eeaff600d961ba3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:23:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:23:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 01 Sep 2021 03:04:27 GMT
ENV KAPACITOR_VERSION=1.6.1
# Wed, 01 Sep 2021 03:04:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 01 Sep 2021 03:04:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 01 Sep 2021 03:04:41 GMT
EXPOSE 9092
# Wed, 01 Sep 2021 03:04:41 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 01 Sep 2021 03:04:42 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Wed, 01 Sep 2021 03:04:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 03:04:42 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69cd3502d3b453e253ea48e4ff56f5af4e25895a1bfa5e84cda59eaefce23be`  
		Last Modified: Wed, 01 Sep 2021 00:25:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7087df4b29e442773e368f72aa50cd7765fd6e6b43879c83880b0038e62b9077`  
		Last Modified: Wed, 01 Sep 2021 00:25:29 GMT  
		Size: 280.9 KB (280879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7cb5b6248de8e40cb59c8a172882bcf139b97f02ea65ba88919ed2aadef1e9`  
		Last Modified: Wed, 01 Sep 2021 03:05:26 GMT  
		Size: 59.2 MB (59199583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e72ce875cf5d94b0730927e9e97d3df95bdfb5651c544f52ac5c124f2f43e5`  
		Last Modified: Wed, 01 Sep 2021 03:05:17 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0b546e47c7e79bda5d79a7be609e9c46eedd0801b11be06c36d4c4bfde1b39`  
		Last Modified: Wed, 01 Sep 2021 03:05:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:alpine`

```console
$ docker pull kapacitor@sha256:7896801d6eeb35bbcbed36310760a3b1ff3120d16b23aaf20267a3e927b8936d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kapacitor:alpine` - linux; amd64

```console
$ docker pull kapacitor@sha256:b3c9c70bdad340a180f54ab64c17a420e8ea6544513bb86d1d5ee61c980c1f16
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.3 MB (62282802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c171de764c09f16e4ce559429bf58d7f552765083dabe7eeaff600d961ba3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:23 GMT
ADD file:e3d2013df9d58cd9255c749dbd62e7b1b1bdf1c2ee644c17bb93e67d859f0815 in / 
# Tue, 31 Aug 2021 23:18:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:23:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:23:43 GMT
RUN apk add --no-cache ca-certificates &&     update-ca-certificates
# Wed, 01 Sep 2021 03:04:27 GMT
ENV KAPACITOR_VERSION=1.6.1
# Wed, 01 Sep 2021 03:04:40 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     gpg --batch --verify kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz.asc kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf kapacitor-${KAPACITOR_VERSION}_linux_amd64.tar.gz &&     rm -f /usr/src/kapacitor-*/kapacitor.conf &&     chmod +x /usr/src/kapacitor-*/* &&     cp -a /usr/src/kapacitor-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 01 Sep 2021 03:04:41 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 01 Sep 2021 03:04:41 GMT
EXPOSE 9092
# Wed, 01 Sep 2021 03:04:41 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 01 Sep 2021 03:04:42 GMT
COPY file:a64543022a380a96e18ddc4e841e034238df340064743d570fa109d5086b123a in /entrypoint.sh 
# Wed, 01 Sep 2021 03:04:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Sep 2021 03:04:42 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:e519532ddf75bafbbb0ad01d3fb678ef9395cd8554fa25bef4695bb6e11f39f1`  
		Last Modified: Tue, 31 Aug 2021 23:19:05 GMT  
		Size: 2.8 MB (2801707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69cd3502d3b453e253ea48e4ff56f5af4e25895a1bfa5e84cda59eaefce23be`  
		Last Modified: Wed, 01 Sep 2021 00:25:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7087df4b29e442773e368f72aa50cd7765fd6e6b43879c83880b0038e62b9077`  
		Last Modified: Wed, 01 Sep 2021 00:25:29 GMT  
		Size: 280.9 KB (280879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e7cb5b6248de8e40cb59c8a172882bcf139b97f02ea65ba88919ed2aadef1e9`  
		Last Modified: Wed, 01 Sep 2021 03:05:26 GMT  
		Size: 59.2 MB (59199583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e72ce875cf5d94b0730927e9e97d3df95bdfb5651c544f52ac5c124f2f43e5`  
		Last Modified: Wed, 01 Sep 2021 03:05:17 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0b546e47c7e79bda5d79a7be609e9c46eedd0801b11be06c36d4c4bfde1b39`  
		Last Modified: Wed, 01 Sep 2021 03:05:17 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kapacitor:latest`

```console
$ docker pull kapacitor@sha256:214f7ab2493e72e0c690e2911b2b5ad25284d6459baf54a6f5f78316283eb67e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kapacitor:latest` - linux; amd64

```console
$ docker pull kapacitor@sha256:7153c14ce9004d4389fc69f407311389e848df2e044c7c699b25ff1e9fa0b4fd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133606214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc13f62beab87315296150a800a4e1ba8dfc6bc1bf53ad6e6774cf958a1401a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 01:25:56 GMT
ADD file:0d0aa1ebd07b0f301aaf1077d1e9f2e9be1859510dd8535e143571b347a2a379 in / 
# Tue, 17 Aug 2021 01:25:56 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:24:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 07:01:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 07:01:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 07:01:40 GMT
ENV KAPACITOR_VERSION=1.6.1
# Wed, 18 Aug 2021 07:01:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 07:01:45 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 07:01:45 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 07:01:45 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 07:01:45 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 07:01:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 07:01:46 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:eb18d230e067c240479c6a3f842e7f9d4ff1088e3072d0a3245829c4e356623f`  
		Last Modified: Tue, 17 Aug 2021 01:33:03 GMT  
		Size: 45.4 MB (45379966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83600c1b4583abb5830c6d4a039cbab9a102ac1a7b3b779854638a371bb7128f`  
		Last Modified: Tue, 17 Aug 2021 09:33:12 GMT  
		Size: 11.3 MB (11295906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae15c65bfa0fdc9053dcb734e6c034f5394ea0481dee3277f6e3e9fa07702d0`  
		Last Modified: Tue, 17 Aug 2021 09:33:11 GMT  
		Size: 4.3 MB (4342387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df9a81a6e6330b08dc4ea9322d4dbc9131ceb336f4f48222299992bee24d20c`  
		Last Modified: Wed, 18 Aug 2021 07:02:07 GMT  
		Size: 13.3 MB (13322522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ac9e7ace861b8fefc86ece32a745d3860247036ec12dca6a51e6436f64cfe6`  
		Last Modified: Wed, 18 Aug 2021 07:02:05 GMT  
		Size: 2.9 KB (2853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1cc761767c20764cf1890fd66d9fe9b0c73793ffd089bb7010d856e3379946`  
		Last Modified: Wed, 18 Aug 2021 07:02:29 GMT  
		Size: 59.3 MB (59262125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c31ea119f5e5d39540a41d2bd75569c0967d85b58e6af5592701e382cf3603`  
		Last Modified: Wed, 18 Aug 2021 07:02:21 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fb14f03d554baca4f313ccbaddb34e22c9da8d46e6a3aa2ff345503b0d9d06`  
		Last Modified: Wed, 18 Aug 2021 07:02:21 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kapacitor:latest` - linux; arm64 variant v8

```console
$ docker pull kapacitor@sha256:bb3c234e66dfa59d248b87cee4296683b657746d08d662675aa83d300aaf5957
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126412617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2d82c3b2c970a55952ec9459906b48548ebfe5e31952e7027918bc433967e9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["kapacitord"]`

```dockerfile
# Tue, 17 Aug 2021 01:48:17 GMT
ADD file:79e0d0ec943ec405612e2310514d8f0c72cf83483eea6d5f1a7c28b36fa21cf8 in / 
# Tue, 17 Aug 2021 01:48:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:56:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:56:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 03:04:28 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y bash-completion &&     awk 'f{if(sub(/^#/,"",$0)==0){f=0}};/^# enable bash completion/{f=1};{print;}' /etc/bash.bashrc > /etc/bash.bashrc.new &&     mv /etc/bash.bashrc.new /etc/bash.bashrc
# Wed, 18 Aug 2021 03:04:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 03:04:43 GMT
ENV KAPACITOR_VERSION=1.6.1
# Wed, 18 Aug 2021 03:04:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/kapacitor/releases/kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb.asc kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     dpkg -i kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb &&     rm -f kapacitor_${KAPACITOR_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 03:04:47 GMT
COPY file:9450c5dcbc0a583243f987f682dc6c44d9e4a3f1c31d1bb9957f313457e444ec in /etc/kapacitor/kapacitor.conf 
# Wed, 18 Aug 2021 03:04:47 GMT
EXPOSE 9092
# Wed, 18 Aug 2021 03:04:48 GMT
VOLUME [/var/lib/kapacitor]
# Wed, 18 Aug 2021 03:04:48 GMT
COPY file:a229567085df49450fcc70ed6d49efcbdfc41ca92b6c5bdb3b541cb803165dbc in /entrypoint.sh 
# Wed, 18 Aug 2021 03:04:48 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 03:04:48 GMT
CMD ["kapacitord"]
```

-	Layers:
	-	`sha256:a410f7a7fb8af899e64ef008ec59cc8062766e91abbf21ba5cee65faac7ba3fa`  
		Last Modified: Tue, 17 Aug 2021 01:57:32 GMT  
		Size: 43.2 MB (43177652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e420ab67f91937cc8165f5fb2e94bdab905576eadca5515be250bc6212fe50`  
		Last Modified: Tue, 17 Aug 2021 08:04:49 GMT  
		Size: 10.2 MB (10215748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ce4bbd3804fd1154090db6722050023d8242e910e02ed7d2c09b9795a9d5ac`  
		Last Modified: Tue, 17 Aug 2021 08:04:48 GMT  
		Size: 4.1 MB (4096582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151ac1cfab8790dc49973599fa396ed1be6d7c7941973b59135f515444b730be`  
		Last Modified: Wed, 18 Aug 2021 03:05:10 GMT  
		Size: 13.0 MB (13025171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918b8c0940b453d44ba7db5d3637f4123eb859a3817e86d547b0a677ec9bb051`  
		Last Modified: Wed, 18 Aug 2021 03:05:08 GMT  
		Size: 2.9 KB (2852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b545f7a05e164a6464596480ab593368549e63552f2c253130589d7a69dffa3`  
		Last Modified: Wed, 18 Aug 2021 03:05:33 GMT  
		Size: 55.9 MB (55894157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22483778e68af06d02517e68ca78f872bcdd3558272fe774717854d2e191693`  
		Last Modified: Wed, 18 Aug 2021 03:05:25 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98f8758a8b6b71214bc116749a3a506c46efa2a44a7655f0cc6e97aef2c9221`  
		Last Modified: Wed, 18 Aug 2021 03:05:25 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
