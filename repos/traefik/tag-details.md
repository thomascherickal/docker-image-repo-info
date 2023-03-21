<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `traefik`

-	[`traefik:1.7`](#traefik17)
-	[`traefik:1.7-alpine`](#traefik17-alpine)
-	[`traefik:1.7-windowsservercore-1809`](#traefik17-windowsservercore-1809)
-	[`traefik:1.7.34`](#traefik1734)
-	[`traefik:1.7.34-alpine`](#traefik1734-alpine)
-	[`traefik:1.7.34-windowsservercore-1809`](#traefik1734-windowsservercore-1809)
-	[`traefik:2.9`](#traefik29)
-	[`traefik:2.9-windowsservercore-1809`](#traefik29-windowsservercore-1809)
-	[`traefik:2.9.9`](#traefik299)
-	[`traefik:2.9.9-windowsservercore-1809`](#traefik299-windowsservercore-1809)
-	[`traefik:3.0`](#traefik30)
-	[`traefik:3.0-windowsservercore-1809`](#traefik30-windowsservercore-1809)
-	[`traefik:3.0.0-beta2`](#traefik300-beta2)
-	[`traefik:3.0.0-beta2-windowsservercore-1809`](#traefik300-beta2-windowsservercore-1809)
-	[`traefik:banon`](#traefikbanon)
-	[`traefik:banon-windowsservercore-1809`](#traefikbanon-windowsservercore-1809)
-	[`traefik:beaufort`](#traefikbeaufort)
-	[`traefik:beaufort-windowsservercore-1809`](#traefikbeaufort-windowsservercore-1809)
-	[`traefik:latest`](#traefiklatest)
-	[`traefik:maroilles`](#traefikmaroilles)
-	[`traefik:maroilles-alpine`](#traefikmaroilles-alpine)
-	[`traefik:maroilles-windowsservercore-1809`](#traefikmaroilles-windowsservercore-1809)
-	[`traefik:v1.7`](#traefikv17)
-	[`traefik:v1.7-alpine`](#traefikv17-alpine)
-	[`traefik:v1.7-windowsservercore-1809`](#traefikv17-windowsservercore-1809)
-	[`traefik:v1.7.34`](#traefikv1734)
-	[`traefik:v1.7.34-alpine`](#traefikv1734-alpine)
-	[`traefik:v1.7.34-windowsservercore-1809`](#traefikv1734-windowsservercore-1809)
-	[`traefik:v2.9`](#traefikv29)
-	[`traefik:v2.9-windowsservercore-1809`](#traefikv29-windowsservercore-1809)
-	[`traefik:v2.9.9`](#traefikv299)
-	[`traefik:v2.9.9-windowsservercore-1809`](#traefikv299-windowsservercore-1809)
-	[`traefik:v3.0`](#traefikv30)
-	[`traefik:v3.0-windowsservercore-1809`](#traefikv30-windowsservercore-1809)
-	[`traefik:v3.0.0-beta2`](#traefikv300-beta2)
-	[`traefik:v3.0.0-beta2-windowsservercore-1809`](#traefikv300-beta2-windowsservercore-1809)
-	[`traefik:windowsservercore-1809`](#traefikwindowsservercore-1809)

## `traefik:1.7`

```console
$ docker pull traefik@sha256:fc9a03a8a58c18c573451455172d31b8d85119da6c57b2b200fbea546b1161ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7` - linux; amd64

```console
$ docker pull traefik@sha256:a37a3469b7bd1e58d95ab5918f31f3a8aada1bdfa90f8d963eb78e8bae37d025
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22594315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b06305d2e0eca68d66088b5290a28c31dd73722f3f8e33c764bd60faf17edd7`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Sat, 11 Feb 2023 14:05:58 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Sat, 11 Feb 2023 14:05:59 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Sat, 11 Feb 2023 14:05:59 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:59 GMT
VOLUME [/tmp]
# Sat, 11 Feb 2023 14:05:59 GMT
ENTRYPOINT ["/traefik"]
# Sat, 11 Feb 2023 14:05:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b232dbde1f095d758c59886ecc24a42610dd35fd72116f3bf04738104e1cfa`  
		Last Modified: Sat, 11 Feb 2023 14:07:25 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066ff3631f4c0a13ebb72826195f8332b28aa6c9945865b1c07076fad46fb81b`  
		Last Modified: Sat, 11 Feb 2023 14:07:29 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7d30df83fa81bb480812fb04384c340a5414a90b3ef139ed06b11db2629ab6d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1a3efa227e28dd72fe4fe204cfc7a77441567e522b5aec07bea603efcf3767`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 14 Mar 2023 01:31:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Tue, 14 Mar 2023 01:31:59 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Tue, 14 Mar 2023 01:32:01 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Tue, 14 Mar 2023 01:32:01 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:32:01 GMT
VOLUME [/tmp]
# Tue, 14 Mar 2023 01:32:01 GMT
ENTRYPOINT ["/traefik"]
# Tue, 14 Mar 2023 01:32:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:68a2bb2e7a38ecc0a394b8fde6e116d903af0a9081c1816df304ab9a95b081da`  
		Last Modified: Tue, 14 Mar 2023 01:34:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abcbdf883582fff78fa64c20ff3783c94c68cbdc4b3c199fc94e53b5094e4e6`  
		Last Modified: Tue, 14 Mar 2023 01:34:17 GMT  
		Size: 308.9 KB (308851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8772ce58379f8b2532ee1b93c4220cd99b6e6c0c6a5ccad7ff67de5849bc65e`  
		Last Modified: Tue, 14 Mar 2023 01:34:22 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ac5b287132e97dc27bbd96791a25701e051ddce973d6ee70eda1c87138e3c299
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d5da1bea8e1a3e20b83ceca6e486a1e881451b1e304a0281d936d5e51f418d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:00:57 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:00:58 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 11 Nov 2022 11:00:58 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:58 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:00:58 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:00:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f6a6b590d30fda524213974a86d6ca01981b3ab4154a359b9c2e3fa3262c6`  
		Last Modified: Fri, 11 Nov 2022 11:02:04 GMT  
		Size: 308.8 KB (308813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af8a7d805d81cf74f58f3793659f76132259201bea15bbb7a0edc6191f8edfa`  
		Last Modified: Fri, 11 Nov 2022 11:02:07 GMT  
		Size: 20.1 MB (20131346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-alpine`

```console
$ docker pull traefik@sha256:dae77187506098f71a878261bde8207a34ec77e283bfcce446e8a5332c54992f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:6a5bf0d59212a73927e18da4a5b85ff7d02fb566283bcd10b3c307b8a39627a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25653523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:299327139165b0025a883c7a11747b5d04c4bc72f053601c0f763fee0ed761a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:51 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:52 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fab313a1ca0ee79d027587c5edad5ff243a08e1cbd263abe2a17503c316d8b`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 661.5 KB (661461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e550be36e43026c7c9214cf16b3b866de5ce1da12f14fcef46658c0def1d4a7`  
		Last Modified: Sat, 11 Feb 2023 14:07:12 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4561714fba29bd0d410fa9813afc75479ffef93714ffdad849a7943771d73544`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9b251f4e7f9ac30ecbca3b12d2e03cbb774df99d708e61e84e23a5e6ed53f08d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01eaf16e6615e6646fa59fb368b61c5a55cad7eef251093d04c76f2529a135d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:54 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Mon, 13 Mar 2023 16:12:54 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:51 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:51 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:51 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d811b603dbe15ba6438e580f10afa348eb213b791a9252642521f986fd77e0d`  
		Last Modified: Tue, 14 Mar 2023 01:33:53 GMT  
		Size: 666.4 KB (666440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b099a3d2655c5ee12dfd7e0cd01338c6305193d9e7329186ba998a100afae1`  
		Last Modified: Tue, 14 Mar 2023 01:33:57 GMT  
		Size: 20.6 MB (20623429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a10f592ec7cdfd0ff7a0f1c3a8473de24a82068b80b9239b3436398f7c1af5`  
		Last Modified: Tue, 14 Mar 2023 01:33:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e23b8edb3c8a7f4a5ce7b2697e304f8e31d845474dccdbcd15b86e831c7bc69b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72dbaffc2f8e74c9ed9aa7a99d590e792ba2b318e8562992180335ba122958e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:46 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:46 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:46 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c8dd85906c92d3445ffeb0481950055e77c854095c4cbbd854f6951242a3c`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 663.2 KB (663163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0994ad8baa5503f4c667ced5bb36b643eba7642f9791e4bf7975527de9f2c2ed`  
		Last Modified: Sat, 11 Feb 2023 06:41:57 GMT  
		Size: 20.1 MB (20131363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6a5a822a3369f9999a4da4bcb9718729d386c2dbf108fb8a8a52056eacc8d2`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f643d6e3857163a610f6ee48dcedefc4ae1c6957968b821a132c45dad295521d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:1.7-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:eb030d1415b37297490d0d042c132510d0592f8158bb80f98328bebe132c71c7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036484756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd883fc0a81df58f398881ad9a26665e14af2ff944186704211ca53de351d281`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:48:48 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 16 Mar 2023 08:48:49 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:48:50 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:48:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c40e4a974e18ba73f3964c77bafb530b44a02b157bff67d57d80b50a37d306`  
		Last Modified: Thu, 16 Mar 2023 08:50:12 GMT  
		Size: 23.0 MB (22970100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b8a1819bca4f2eb81e780d11f83ab69e9c936aeaddbd31803a9949cf487145`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5590048d6ec03d383585a24a3e40df19cce710181b483bb92abd200c87c856`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbdbd264f1bd9f178ca6c87b2073841bac0e4226b3fed4145bbdb0c46e98ca1`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34`

```console
$ docker pull traefik@sha256:fc9a03a8a58c18c573451455172d31b8d85119da6c57b2b200fbea546b1161ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:a37a3469b7bd1e58d95ab5918f31f3a8aada1bdfa90f8d963eb78e8bae37d025
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22594315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b06305d2e0eca68d66088b5290a28c31dd73722f3f8e33c764bd60faf17edd7`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Sat, 11 Feb 2023 14:05:58 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Sat, 11 Feb 2023 14:05:59 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Sat, 11 Feb 2023 14:05:59 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:59 GMT
VOLUME [/tmp]
# Sat, 11 Feb 2023 14:05:59 GMT
ENTRYPOINT ["/traefik"]
# Sat, 11 Feb 2023 14:05:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b232dbde1f095d758c59886ecc24a42610dd35fd72116f3bf04738104e1cfa`  
		Last Modified: Sat, 11 Feb 2023 14:07:25 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066ff3631f4c0a13ebb72826195f8332b28aa6c9945865b1c07076fad46fb81b`  
		Last Modified: Sat, 11 Feb 2023 14:07:29 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7d30df83fa81bb480812fb04384c340a5414a90b3ef139ed06b11db2629ab6d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1a3efa227e28dd72fe4fe204cfc7a77441567e522b5aec07bea603efcf3767`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 14 Mar 2023 01:31:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Tue, 14 Mar 2023 01:31:59 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Tue, 14 Mar 2023 01:32:01 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Tue, 14 Mar 2023 01:32:01 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:32:01 GMT
VOLUME [/tmp]
# Tue, 14 Mar 2023 01:32:01 GMT
ENTRYPOINT ["/traefik"]
# Tue, 14 Mar 2023 01:32:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:68a2bb2e7a38ecc0a394b8fde6e116d903af0a9081c1816df304ab9a95b081da`  
		Last Modified: Tue, 14 Mar 2023 01:34:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abcbdf883582fff78fa64c20ff3783c94c68cbdc4b3c199fc94e53b5094e4e6`  
		Last Modified: Tue, 14 Mar 2023 01:34:17 GMT  
		Size: 308.9 KB (308851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8772ce58379f8b2532ee1b93c4220cd99b6e6c0c6a5ccad7ff67de5849bc65e`  
		Last Modified: Tue, 14 Mar 2023 01:34:22 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ac5b287132e97dc27bbd96791a25701e051ddce973d6ee70eda1c87138e3c299
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d5da1bea8e1a3e20b83ceca6e486a1e881451b1e304a0281d936d5e51f418d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:00:57 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:00:58 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 11 Nov 2022 11:00:58 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:58 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:00:58 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:00:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f6a6b590d30fda524213974a86d6ca01981b3ab4154a359b9c2e3fa3262c6`  
		Last Modified: Fri, 11 Nov 2022 11:02:04 GMT  
		Size: 308.8 KB (308813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af8a7d805d81cf74f58f3793659f76132259201bea15bbb7a0edc6191f8edfa`  
		Last Modified: Fri, 11 Nov 2022 11:02:07 GMT  
		Size: 20.1 MB (20131346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-alpine`

```console
$ docker pull traefik@sha256:dae77187506098f71a878261bde8207a34ec77e283bfcce446e8a5332c54992f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:6a5bf0d59212a73927e18da4a5b85ff7d02fb566283bcd10b3c307b8a39627a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25653523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:299327139165b0025a883c7a11747b5d04c4bc72f053601c0f763fee0ed761a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:51 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:52 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fab313a1ca0ee79d027587c5edad5ff243a08e1cbd263abe2a17503c316d8b`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 661.5 KB (661461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e550be36e43026c7c9214cf16b3b866de5ce1da12f14fcef46658c0def1d4a7`  
		Last Modified: Sat, 11 Feb 2023 14:07:12 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4561714fba29bd0d410fa9813afc75479ffef93714ffdad849a7943771d73544`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9b251f4e7f9ac30ecbca3b12d2e03cbb774df99d708e61e84e23a5e6ed53f08d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01eaf16e6615e6646fa59fb368b61c5a55cad7eef251093d04c76f2529a135d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:54 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Mon, 13 Mar 2023 16:12:54 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:51 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:51 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:51 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d811b603dbe15ba6438e580f10afa348eb213b791a9252642521f986fd77e0d`  
		Last Modified: Tue, 14 Mar 2023 01:33:53 GMT  
		Size: 666.4 KB (666440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b099a3d2655c5ee12dfd7e0cd01338c6305193d9e7329186ba998a100afae1`  
		Last Modified: Tue, 14 Mar 2023 01:33:57 GMT  
		Size: 20.6 MB (20623429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a10f592ec7cdfd0ff7a0f1c3a8473de24a82068b80b9239b3436398f7c1af5`  
		Last Modified: Tue, 14 Mar 2023 01:33:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e23b8edb3c8a7f4a5ce7b2697e304f8e31d845474dccdbcd15b86e831c7bc69b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72dbaffc2f8e74c9ed9aa7a99d590e792ba2b318e8562992180335ba122958e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:46 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:46 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:46 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c8dd85906c92d3445ffeb0481950055e77c854095c4cbbd854f6951242a3c`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 663.2 KB (663163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0994ad8baa5503f4c667ced5bb36b643eba7642f9791e4bf7975527de9f2c2ed`  
		Last Modified: Sat, 11 Feb 2023 06:41:57 GMT  
		Size: 20.1 MB (20131363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6a5a822a3369f9999a4da4bcb9718729d386c2dbf108fb8a8a52056eacc8d2`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f643d6e3857163a610f6ee48dcedefc4ae1c6957968b821a132c45dad295521d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:1.7.34-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:eb030d1415b37297490d0d042c132510d0592f8158bb80f98328bebe132c71c7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036484756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd883fc0a81df58f398881ad9a26665e14af2ff944186704211ca53de351d281`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:48:48 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 16 Mar 2023 08:48:49 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:48:50 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:48:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c40e4a974e18ba73f3964c77bafb530b44a02b157bff67d57d80b50a37d306`  
		Last Modified: Thu, 16 Mar 2023 08:50:12 GMT  
		Size: 23.0 MB (22970100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b8a1819bca4f2eb81e780d11f83ab69e9c936aeaddbd31803a9949cf487145`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5590048d6ec03d383585a24a3e40df19cce710181b483bb92abd200c87c856`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbdbd264f1bd9f178ca6c87b2073841bac0e4226b3fed4145bbdb0c46e98ca1`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9`

```console
$ docker pull traefik@sha256:a29972da395acf3f186b01bca023985dd736545d1bccc55a33a7376adeee3495
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:2.9` - linux; amd64

```console
$ docker pull traefik@sha256:553239e27c4614d0477651415205b9b119f7a98f698e6562ef383c9d8ff3b6e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38777669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85dec640e68e655f5cf95c8ce8671da1194710b38a539166ca080ba0c93e1d4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 23:22:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 23:22:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 23:22:09 GMT
EXPOSE 80
# Wed, 15 Feb 2023 23:22:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 23:22:09 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 23:22:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3655af1bbd56df1bcfec44686273a57d30cc0b69f6e501f87ec67712913b8b55`  
		Last Modified: Sat, 11 Feb 2023 14:06:23 GMT  
		Size: 662.0 KB (662047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f984ad6ecbda363b2ce6487b63b68f4f9f68741c7a7c2e50c3e68e1faf9aec5`  
		Last Modified: Wed, 15 Feb 2023 23:22:46 GMT  
		Size: 35.3 MB (35289107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823d14d881861f99e9db87cb68a06cdead6f070c4920274ac6a0d173432a0043`  
		Last Modified: Wed, 15 Feb 2023 23:22:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b45f882e5a6c1229a285aa460569aa45c487c878ff713c9d038d012a9ea7cf74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36629054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a42eaf1d53da78868c01e06a4c4b2fa9dde5d9aa210460f2948fb6f13f1781b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:35 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:36 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937713bf36e8ddb19f4d3861767039861708c7cc2a83e388aa80b6981bd0dc3a`  
		Last Modified: Tue, 14 Mar 2023 01:32:58 GMT  
		Size: 666.5 KB (666511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bc1d14d49fdac439a68245e1142963cd97f387ff68c5eb42604d4fc03e324`  
		Last Modified: Tue, 14 Mar 2023 01:33:29 GMT  
		Size: 33.3 MB (33328526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331609b39766af505ef55a69602b8ceac4018a6aca9937efac165e7296ba860c`  
		Last Modified: Tue, 14 Mar 2023 01:33:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9c79fa649e5cbe903c4815a112e8bd370a27492589550418e20ac5dfa1ca0879
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35760765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4616f42b3ac2a862ba6e9bdf25bd690efbacb8961960a681ac25f0d3ae3f128`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 22:49:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 22:49:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 22:49:07 GMT
EXPOSE 80
# Wed, 15 Feb 2023 22:49:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 22:49:07 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 22:49:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57456bf9239ae8d2b09ba33d1227b60a493b664b0a0558a09a614e08aedf0438`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 663.2 KB (663152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92b39b3528b8dd48de9d16db14bfda9c6a0094d2fa75eafa29f6b1c1c168a11`  
		Last Modified: Wed, 15 Feb 2023 22:49:43 GMT  
		Size: 32.4 MB (32375688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c984c91836ae71200fb885d8fe5477ff6718e55e16d0d1d03e20b925a1107906`  
		Last Modified: Wed, 15 Feb 2023 22:49:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:2.9` - linux; s390x

```console
$ docker pull traefik@sha256:e1440b2606e72909deec6ca7bee86ea2081864c320c28651dca4644ee581325d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37438024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ffd4bc9101c8ac43816d439afeedbc3fe84e411a98c5237e8c28019dd53af6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:37 GMT
ADD file:8a7d887c96c361c6ae19ca804030a0d79a1984b9e32b6c3767ede695c6613909 in / 
# Fri, 10 Feb 2023 21:41:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:21:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 22:46:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 22:46:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 22:46:13 GMT
EXPOSE 80
# Wed, 15 Feb 2023 22:46:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 22:46:14 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 22:46:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0d71e9a79f477719291f0a25b6a2462917f2e396325883144c1f1e59fbc56f21`  
		Last Modified: Fri, 10 Feb 2023 21:42:33 GMT  
		Size: 2.6 MB (2610267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e10f8aa3cb11731ad3d5cea5740b9baa80c4652f810b4efd47d507984fa8d8`  
		Last Modified: Sat, 11 Feb 2023 05:22:25 GMT  
		Size: 666.4 KB (666384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595453c84153d4d6b45b74c510ea02485c73813554c2753e704ac2a3ee5075e`  
		Last Modified: Wed, 15 Feb 2023 22:46:55 GMT  
		Size: 34.2 MB (34161005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c6f65f8083b617d701bc732b372962e6aa9b9f620a349ef3ce2191e197a7f`  
		Last Modified: Wed, 15 Feb 2023 22:46:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1d23dcfba19d25a7db7e5cd85cfcb48ecc50e88cd0ada6101f1f125b5a69e87f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:2.9-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:09d2d0195ec592feca5562747351e547f37853ef9400af79664398ad0e67df8f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2756d6e358452d2bdb882cda3b649d92fc7edef462e0d4d4268b1b78d2fde2f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 21 Mar 2023 19:17:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.9/traefik_v2.9.9_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 21 Mar 2023 19:17:08 GMT
EXPOSE 80
# Tue, 21 Mar 2023 19:17:09 GMT
ENTRYPOINT ["/traefik"]
# Tue, 21 Mar 2023 19:17:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.9 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa99ce6cd34b6eec9c095cd7936aeed038d0e89f07b98e0854b8d40625b3d844`  
		Last Modified: Tue, 21 Mar 2023 19:18:05 GMT  
		Size: 36.3 MB (36264213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e291ba8ae74eee25775851ef3eca803d2166e1606f542c53019340d6f5930bc`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1b936795c1df1230fc4fef82f77463356552d7296c59ee6dc3410c2d81303e`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38befdb3655c93aebc9c7975e6bb46d591fb7e4785d6fe33725d3fe2b89d8105`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:2.9.9`

```console
$ docker pull traefik@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `traefik:2.9.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1d23dcfba19d25a7db7e5cd85cfcb48ecc50e88cd0ada6101f1f125b5a69e87f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:2.9.9-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:09d2d0195ec592feca5562747351e547f37853ef9400af79664398ad0e67df8f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2756d6e358452d2bdb882cda3b649d92fc7edef462e0d4d4268b1b78d2fde2f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 21 Mar 2023 19:17:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.9/traefik_v2.9.9_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 21 Mar 2023 19:17:08 GMT
EXPOSE 80
# Tue, 21 Mar 2023 19:17:09 GMT
ENTRYPOINT ["/traefik"]
# Tue, 21 Mar 2023 19:17:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.9 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa99ce6cd34b6eec9c095cd7936aeed038d0e89f07b98e0854b8d40625b3d844`  
		Last Modified: Tue, 21 Mar 2023 19:18:05 GMT  
		Size: 36.3 MB (36264213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e291ba8ae74eee25775851ef3eca803d2166e1606f542c53019340d6f5930bc`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1b936795c1df1230fc4fef82f77463356552d7296c59ee6dc3410c2d81303e`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38befdb3655c93aebc9c7975e6bb46d591fb7e4785d6fe33725d3fe2b89d8105`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0`

```console
$ docker pull traefik@sha256:1f88c068865e68dde18a29aec644a1c92432e4d4279abfb9c80df845f8019173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0` - linux; amd64

```console
$ docker pull traefik@sha256:bf822393b55095bc13f7699ae1fa1b56bbe2e072bc2ae283bffd3a4dadd98d7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40563449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e32ad70784035ddea0808eeb76e7f8a6bc64e2cb867b63c6513f8f4e853f1133`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:33 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:33 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3655af1bbd56df1bcfec44686273a57d30cc0b69f6e501f87ec67712913b8b55`  
		Last Modified: Sat, 11 Feb 2023 14:06:23 GMT  
		Size: 662.0 KB (662047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cc32ef302c3bee4df8ba7b31c8717d000beefd7e66fbdcc07450792441ad67`  
		Last Modified: Sat, 11 Feb 2023 14:06:28 GMT  
		Size: 37.1 MB (37074888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f96cb39092b375e76e59ca53f161a1777975c9c58ea5d46e480812addb564`  
		Last Modified: Sat, 11 Feb 2023 14:06:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c6eb90c1a642c95756e04f947caee3baaed18ea1e02780df54b15240795df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a352a59877646edd78a3c6c811509111a92cd686212c584e5a5ee4845aed3818`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:21 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:22 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:23 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937713bf36e8ddb19f4d3861767039861708c7cc2a83e388aa80b6981bd0dc3a`  
		Last Modified: Tue, 14 Mar 2023 01:32:58 GMT  
		Size: 666.5 KB (666511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09007fbe2ec6b465a9c6d24d737b5f27c316d90aaae93757efb986a68a59acf9`  
		Last Modified: Tue, 14 Mar 2023 01:33:03 GMT  
		Size: 35.0 MB (34989328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50ac3be21a5d5b5b332f61de0380a4216157129e1668df6f68dde1d969fb098`  
		Last Modified: Tue, 14 Mar 2023 01:32:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:49b2e1db6ca60eae983dab7632ed2ea3997c698d05dd6789eeac4de13c94ea14
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0b18449b8e63bade321e2c66ff5674dd5d7e3a36154f012db7b37c3c668a53`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:29 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:30 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:30 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57456bf9239ae8d2b09ba33d1227b60a493b664b0a0558a09a614e08aedf0438`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 663.2 KB (663152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e1381066f019ec8bedc5c9e8c8dcae4ed86e75cb46d22c461d5a87a060f23a`  
		Last Modified: Sat, 11 Feb 2023 06:41:17 GMT  
		Size: 34.0 MB (34023515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac00a09db30fc81aca200d38461e38fcc368b57e9878c1f51bb832b235e287d`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0` - linux; s390x

```console
$ docker pull traefik@sha256:c50bbeaf64f9b8a1d4a6f4ec10ff476e2066ac2dc59230bf8f02ce77f9cb4f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d71fc91baad09e19cde42a2c649d7dc4a303b86b94d97f988e69e7da9222d76`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:37 GMT
ADD file:8a7d887c96c361c6ae19ca804030a0d79a1984b9e32b6c3767ede695c6613909 in / 
# Fri, 10 Feb 2023 21:41:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:21:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 05:21:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 05:21:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 05:21:37 GMT
EXPOSE 80
# Sat, 11 Feb 2023 05:21:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 05:21:37 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 05:21:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0d71e9a79f477719291f0a25b6a2462917f2e396325883144c1f1e59fbc56f21`  
		Last Modified: Fri, 10 Feb 2023 21:42:33 GMT  
		Size: 2.6 MB (2610267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e10f8aa3cb11731ad3d5cea5740b9baa80c4652f810b4efd47d507984fa8d8`  
		Last Modified: Sat, 11 Feb 2023 05:22:25 GMT  
		Size: 666.4 KB (666384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1f663552d308b8665c6af4376a263f91e8bf072db5dce19d544e897af5aa9`  
		Last Modified: Sat, 11 Feb 2023 05:22:30 GMT  
		Size: 35.9 MB (35855467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6a80fe50e1182c4db36fc9b9c0c0ed898c4e2745f7b16e7a2654fa5a403a2d`  
		Last Modified: Sat, 11 Feb 2023 05:22:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2eb0d945da364a274f76288295b9120086404be2c7606fe340ac2ee6f1d64ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:3.0-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:62e9db8356188c92dbce1706a8c2af3702993ee762b34d398fc7921eb03a3629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051205802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648f7c4938c24c605c3f3cbf0b16d4a5767ce075cd407fa9c6ab93e256035917`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:45:29 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Mar 2023 08:45:30 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:45:31 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:45:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eafb0300ea614e208e5052cfdd0941f2ad90a341c5b337ab489e223bb31e88`  
		Last Modified: Thu, 16 Mar 2023 08:49:24 GMT  
		Size: 37.7 MB (37691161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec0dc51e5d37193b3e6ebdd21f1bb94e44f593af5691b32af00720bb4548bbc`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28da668ed65b21bb734a5ba72dd5262a27de001c56a64bebf1db5e9244aaad4c`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6138998225adfde27a93f621c64ba53c628511ce9209f16661fd0c3619ff3e3`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta2`

```console
$ docker pull traefik@sha256:1f88c068865e68dde18a29aec644a1c92432e4d4279abfb9c80df845f8019173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:3.0.0-beta2` - linux; amd64

```console
$ docker pull traefik@sha256:bf822393b55095bc13f7699ae1fa1b56bbe2e072bc2ae283bffd3a4dadd98d7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40563449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e32ad70784035ddea0808eeb76e7f8a6bc64e2cb867b63c6513f8f4e853f1133`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:33 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:33 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3655af1bbd56df1bcfec44686273a57d30cc0b69f6e501f87ec67712913b8b55`  
		Last Modified: Sat, 11 Feb 2023 14:06:23 GMT  
		Size: 662.0 KB (662047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cc32ef302c3bee4df8ba7b31c8717d000beefd7e66fbdcc07450792441ad67`  
		Last Modified: Sat, 11 Feb 2023 14:06:28 GMT  
		Size: 37.1 MB (37074888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f96cb39092b375e76e59ca53f161a1777975c9c58ea5d46e480812addb564`  
		Last Modified: Sat, 11 Feb 2023 14:06:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c6eb90c1a642c95756e04f947caee3baaed18ea1e02780df54b15240795df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a352a59877646edd78a3c6c811509111a92cd686212c584e5a5ee4845aed3818`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:21 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:22 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:23 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937713bf36e8ddb19f4d3861767039861708c7cc2a83e388aa80b6981bd0dc3a`  
		Last Modified: Tue, 14 Mar 2023 01:32:58 GMT  
		Size: 666.5 KB (666511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09007fbe2ec6b465a9c6d24d737b5f27c316d90aaae93757efb986a68a59acf9`  
		Last Modified: Tue, 14 Mar 2023 01:33:03 GMT  
		Size: 35.0 MB (34989328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50ac3be21a5d5b5b332f61de0380a4216157129e1668df6f68dde1d969fb098`  
		Last Modified: Tue, 14 Mar 2023 01:32:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:49b2e1db6ca60eae983dab7632ed2ea3997c698d05dd6789eeac4de13c94ea14
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0b18449b8e63bade321e2c66ff5674dd5d7e3a36154f012db7b37c3c668a53`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:29 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:30 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:30 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57456bf9239ae8d2b09ba33d1227b60a493b664b0a0558a09a614e08aedf0438`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 663.2 KB (663152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e1381066f019ec8bedc5c9e8c8dcae4ed86e75cb46d22c461d5a87a060f23a`  
		Last Modified: Sat, 11 Feb 2023 06:41:17 GMT  
		Size: 34.0 MB (34023515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac00a09db30fc81aca200d38461e38fcc368b57e9878c1f51bb832b235e287d`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:3.0.0-beta2` - linux; s390x

```console
$ docker pull traefik@sha256:c50bbeaf64f9b8a1d4a6f4ec10ff476e2066ac2dc59230bf8f02ce77f9cb4f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d71fc91baad09e19cde42a2c649d7dc4a303b86b94d97f988e69e7da9222d76`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:37 GMT
ADD file:8a7d887c96c361c6ae19ca804030a0d79a1984b9e32b6c3767ede695c6613909 in / 
# Fri, 10 Feb 2023 21:41:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:21:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 05:21:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 05:21:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 05:21:37 GMT
EXPOSE 80
# Sat, 11 Feb 2023 05:21:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 05:21:37 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 05:21:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0d71e9a79f477719291f0a25b6a2462917f2e396325883144c1f1e59fbc56f21`  
		Last Modified: Fri, 10 Feb 2023 21:42:33 GMT  
		Size: 2.6 MB (2610267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e10f8aa3cb11731ad3d5cea5740b9baa80c4652f810b4efd47d507984fa8d8`  
		Last Modified: Sat, 11 Feb 2023 05:22:25 GMT  
		Size: 666.4 KB (666384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1f663552d308b8665c6af4376a263f91e8bf072db5dce19d544e897af5aa9`  
		Last Modified: Sat, 11 Feb 2023 05:22:30 GMT  
		Size: 35.9 MB (35855467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6a80fe50e1182c4db36fc9b9c0c0ed898c4e2745f7b16e7a2654fa5a403a2d`  
		Last Modified: Sat, 11 Feb 2023 05:22:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:3.0.0-beta2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2eb0d945da364a274f76288295b9120086404be2c7606fe340ac2ee6f1d64ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:3.0.0-beta2-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:62e9db8356188c92dbce1706a8c2af3702993ee762b34d398fc7921eb03a3629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051205802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648f7c4938c24c605c3f3cbf0b16d4a5767ce075cd407fa9c6ab93e256035917`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:45:29 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Mar 2023 08:45:30 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:45:31 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:45:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eafb0300ea614e208e5052cfdd0941f2ad90a341c5b337ab489e223bb31e88`  
		Last Modified: Thu, 16 Mar 2023 08:49:24 GMT  
		Size: 37.7 MB (37691161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec0dc51e5d37193b3e6ebdd21f1bb94e44f593af5691b32af00720bb4548bbc`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28da668ed65b21bb734a5ba72dd5262a27de001c56a64bebf1db5e9244aaad4c`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6138998225adfde27a93f621c64ba53c628511ce9209f16661fd0c3619ff3e3`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:banon`

```console
$ docker pull traefik@sha256:a29972da395acf3f186b01bca023985dd736545d1bccc55a33a7376adeee3495
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:banon` - linux; amd64

```console
$ docker pull traefik@sha256:553239e27c4614d0477651415205b9b119f7a98f698e6562ef383c9d8ff3b6e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38777669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85dec640e68e655f5cf95c8ce8671da1194710b38a539166ca080ba0c93e1d4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 23:22:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 23:22:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 23:22:09 GMT
EXPOSE 80
# Wed, 15 Feb 2023 23:22:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 23:22:09 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 23:22:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3655af1bbd56df1bcfec44686273a57d30cc0b69f6e501f87ec67712913b8b55`  
		Last Modified: Sat, 11 Feb 2023 14:06:23 GMT  
		Size: 662.0 KB (662047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f984ad6ecbda363b2ce6487b63b68f4f9f68741c7a7c2e50c3e68e1faf9aec5`  
		Last Modified: Wed, 15 Feb 2023 23:22:46 GMT  
		Size: 35.3 MB (35289107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823d14d881861f99e9db87cb68a06cdead6f070c4920274ac6a0d173432a0043`  
		Last Modified: Wed, 15 Feb 2023 23:22:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b45f882e5a6c1229a285aa460569aa45c487c878ff713c9d038d012a9ea7cf74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36629054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a42eaf1d53da78868c01e06a4c4b2fa9dde5d9aa210460f2948fb6f13f1781b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:35 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:36 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937713bf36e8ddb19f4d3861767039861708c7cc2a83e388aa80b6981bd0dc3a`  
		Last Modified: Tue, 14 Mar 2023 01:32:58 GMT  
		Size: 666.5 KB (666511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bc1d14d49fdac439a68245e1142963cd97f387ff68c5eb42604d4fc03e324`  
		Last Modified: Tue, 14 Mar 2023 01:33:29 GMT  
		Size: 33.3 MB (33328526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331609b39766af505ef55a69602b8ceac4018a6aca9937efac165e7296ba860c`  
		Last Modified: Tue, 14 Mar 2023 01:33:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9c79fa649e5cbe903c4815a112e8bd370a27492589550418e20ac5dfa1ca0879
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35760765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4616f42b3ac2a862ba6e9bdf25bd690efbacb8961960a681ac25f0d3ae3f128`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 22:49:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 22:49:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 22:49:07 GMT
EXPOSE 80
# Wed, 15 Feb 2023 22:49:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 22:49:07 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 22:49:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57456bf9239ae8d2b09ba33d1227b60a493b664b0a0558a09a614e08aedf0438`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 663.2 KB (663152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92b39b3528b8dd48de9d16db14bfda9c6a0094d2fa75eafa29f6b1c1c168a11`  
		Last Modified: Wed, 15 Feb 2023 22:49:43 GMT  
		Size: 32.4 MB (32375688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c984c91836ae71200fb885d8fe5477ff6718e55e16d0d1d03e20b925a1107906`  
		Last Modified: Wed, 15 Feb 2023 22:49:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:banon` - linux; s390x

```console
$ docker pull traefik@sha256:e1440b2606e72909deec6ca7bee86ea2081864c320c28651dca4644ee581325d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37438024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ffd4bc9101c8ac43816d439afeedbc3fe84e411a98c5237e8c28019dd53af6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:37 GMT
ADD file:8a7d887c96c361c6ae19ca804030a0d79a1984b9e32b6c3767ede695c6613909 in / 
# Fri, 10 Feb 2023 21:41:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:21:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 22:46:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 22:46:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 22:46:13 GMT
EXPOSE 80
# Wed, 15 Feb 2023 22:46:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 22:46:14 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 22:46:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0d71e9a79f477719291f0a25b6a2462917f2e396325883144c1f1e59fbc56f21`  
		Last Modified: Fri, 10 Feb 2023 21:42:33 GMT  
		Size: 2.6 MB (2610267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e10f8aa3cb11731ad3d5cea5740b9baa80c4652f810b4efd47d507984fa8d8`  
		Last Modified: Sat, 11 Feb 2023 05:22:25 GMT  
		Size: 666.4 KB (666384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595453c84153d4d6b45b74c510ea02485c73813554c2753e704ac2a3ee5075e`  
		Last Modified: Wed, 15 Feb 2023 22:46:55 GMT  
		Size: 34.2 MB (34161005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c6f65f8083b617d701bc732b372962e6aa9b9f620a349ef3ce2191e197a7f`  
		Last Modified: Wed, 15 Feb 2023 22:46:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:banon-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1d23dcfba19d25a7db7e5cd85cfcb48ecc50e88cd0ada6101f1f125b5a69e87f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:banon-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:09d2d0195ec592feca5562747351e547f37853ef9400af79664398ad0e67df8f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2756d6e358452d2bdb882cda3b649d92fc7edef462e0d4d4268b1b78d2fde2f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 21 Mar 2023 19:17:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.9/traefik_v2.9.9_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 21 Mar 2023 19:17:08 GMT
EXPOSE 80
# Tue, 21 Mar 2023 19:17:09 GMT
ENTRYPOINT ["/traefik"]
# Tue, 21 Mar 2023 19:17:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.9 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa99ce6cd34b6eec9c095cd7936aeed038d0e89f07b98e0854b8d40625b3d844`  
		Last Modified: Tue, 21 Mar 2023 19:18:05 GMT  
		Size: 36.3 MB (36264213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e291ba8ae74eee25775851ef3eca803d2166e1606f542c53019340d6f5930bc`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1b936795c1df1230fc4fef82f77463356552d7296c59ee6dc3410c2d81303e`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38befdb3655c93aebc9c7975e6bb46d591fb7e4785d6fe33725d3fe2b89d8105`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort`

```console
$ docker pull traefik@sha256:1f88c068865e68dde18a29aec644a1c92432e4d4279abfb9c80df845f8019173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:beaufort` - linux; amd64

```console
$ docker pull traefik@sha256:bf822393b55095bc13f7699ae1fa1b56bbe2e072bc2ae283bffd3a4dadd98d7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40563449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e32ad70784035ddea0808eeb76e7f8a6bc64e2cb867b63c6513f8f4e853f1133`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:33 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:33 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3655af1bbd56df1bcfec44686273a57d30cc0b69f6e501f87ec67712913b8b55`  
		Last Modified: Sat, 11 Feb 2023 14:06:23 GMT  
		Size: 662.0 KB (662047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cc32ef302c3bee4df8ba7b31c8717d000beefd7e66fbdcc07450792441ad67`  
		Last Modified: Sat, 11 Feb 2023 14:06:28 GMT  
		Size: 37.1 MB (37074888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f96cb39092b375e76e59ca53f161a1777975c9c58ea5d46e480812addb564`  
		Last Modified: Sat, 11 Feb 2023 14:06:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c6eb90c1a642c95756e04f947caee3baaed18ea1e02780df54b15240795df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a352a59877646edd78a3c6c811509111a92cd686212c584e5a5ee4845aed3818`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:21 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:22 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:23 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937713bf36e8ddb19f4d3861767039861708c7cc2a83e388aa80b6981bd0dc3a`  
		Last Modified: Tue, 14 Mar 2023 01:32:58 GMT  
		Size: 666.5 KB (666511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09007fbe2ec6b465a9c6d24d737b5f27c316d90aaae93757efb986a68a59acf9`  
		Last Modified: Tue, 14 Mar 2023 01:33:03 GMT  
		Size: 35.0 MB (34989328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50ac3be21a5d5b5b332f61de0380a4216157129e1668df6f68dde1d969fb098`  
		Last Modified: Tue, 14 Mar 2023 01:32:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:49b2e1db6ca60eae983dab7632ed2ea3997c698d05dd6789eeac4de13c94ea14
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0b18449b8e63bade321e2c66ff5674dd5d7e3a36154f012db7b37c3c668a53`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:29 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:30 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:30 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57456bf9239ae8d2b09ba33d1227b60a493b664b0a0558a09a614e08aedf0438`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 663.2 KB (663152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e1381066f019ec8bedc5c9e8c8dcae4ed86e75cb46d22c461d5a87a060f23a`  
		Last Modified: Sat, 11 Feb 2023 06:41:17 GMT  
		Size: 34.0 MB (34023515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac00a09db30fc81aca200d38461e38fcc368b57e9878c1f51bb832b235e287d`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:beaufort` - linux; s390x

```console
$ docker pull traefik@sha256:c50bbeaf64f9b8a1d4a6f4ec10ff476e2066ac2dc59230bf8f02ce77f9cb4f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d71fc91baad09e19cde42a2c649d7dc4a303b86b94d97f988e69e7da9222d76`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:37 GMT
ADD file:8a7d887c96c361c6ae19ca804030a0d79a1984b9e32b6c3767ede695c6613909 in / 
# Fri, 10 Feb 2023 21:41:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:21:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 05:21:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 05:21:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 05:21:37 GMT
EXPOSE 80
# Sat, 11 Feb 2023 05:21:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 05:21:37 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 05:21:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0d71e9a79f477719291f0a25b6a2462917f2e396325883144c1f1e59fbc56f21`  
		Last Modified: Fri, 10 Feb 2023 21:42:33 GMT  
		Size: 2.6 MB (2610267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e10f8aa3cb11731ad3d5cea5740b9baa80c4652f810b4efd47d507984fa8d8`  
		Last Modified: Sat, 11 Feb 2023 05:22:25 GMT  
		Size: 666.4 KB (666384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1f663552d308b8665c6af4376a263f91e8bf072db5dce19d544e897af5aa9`  
		Last Modified: Sat, 11 Feb 2023 05:22:30 GMT  
		Size: 35.9 MB (35855467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6a80fe50e1182c4db36fc9b9c0c0ed898c4e2745f7b16e7a2654fa5a403a2d`  
		Last Modified: Sat, 11 Feb 2023 05:22:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:beaufort-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2eb0d945da364a274f76288295b9120086404be2c7606fe340ac2ee6f1d64ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:beaufort-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:62e9db8356188c92dbce1706a8c2af3702993ee762b34d398fc7921eb03a3629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051205802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648f7c4938c24c605c3f3cbf0b16d4a5767ce075cd407fa9c6ab93e256035917`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:45:29 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Mar 2023 08:45:30 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:45:31 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:45:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eafb0300ea614e208e5052cfdd0941f2ad90a341c5b337ab489e223bb31e88`  
		Last Modified: Thu, 16 Mar 2023 08:49:24 GMT  
		Size: 37.7 MB (37691161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec0dc51e5d37193b3e6ebdd21f1bb94e44f593af5691b32af00720bb4548bbc`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28da668ed65b21bb734a5ba72dd5262a27de001c56a64bebf1db5e9244aaad4c`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6138998225adfde27a93f621c64ba53c628511ce9209f16661fd0c3619ff3e3`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:latest`

```console
$ docker pull traefik@sha256:a29972da395acf3f186b01bca023985dd736545d1bccc55a33a7376adeee3495
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:latest` - linux; amd64

```console
$ docker pull traefik@sha256:553239e27c4614d0477651415205b9b119f7a98f698e6562ef383c9d8ff3b6e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38777669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85dec640e68e655f5cf95c8ce8671da1194710b38a539166ca080ba0c93e1d4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 23:22:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 23:22:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 23:22:09 GMT
EXPOSE 80
# Wed, 15 Feb 2023 23:22:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 23:22:09 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 23:22:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3655af1bbd56df1bcfec44686273a57d30cc0b69f6e501f87ec67712913b8b55`  
		Last Modified: Sat, 11 Feb 2023 14:06:23 GMT  
		Size: 662.0 KB (662047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f984ad6ecbda363b2ce6487b63b68f4f9f68741c7a7c2e50c3e68e1faf9aec5`  
		Last Modified: Wed, 15 Feb 2023 23:22:46 GMT  
		Size: 35.3 MB (35289107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823d14d881861f99e9db87cb68a06cdead6f070c4920274ac6a0d173432a0043`  
		Last Modified: Wed, 15 Feb 2023 23:22:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b45f882e5a6c1229a285aa460569aa45c487c878ff713c9d038d012a9ea7cf74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36629054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a42eaf1d53da78868c01e06a4c4b2fa9dde5d9aa210460f2948fb6f13f1781b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:35 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:36 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937713bf36e8ddb19f4d3861767039861708c7cc2a83e388aa80b6981bd0dc3a`  
		Last Modified: Tue, 14 Mar 2023 01:32:58 GMT  
		Size: 666.5 KB (666511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bc1d14d49fdac439a68245e1142963cd97f387ff68c5eb42604d4fc03e324`  
		Last Modified: Tue, 14 Mar 2023 01:33:29 GMT  
		Size: 33.3 MB (33328526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331609b39766af505ef55a69602b8ceac4018a6aca9937efac165e7296ba860c`  
		Last Modified: Tue, 14 Mar 2023 01:33:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9c79fa649e5cbe903c4815a112e8bd370a27492589550418e20ac5dfa1ca0879
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35760765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4616f42b3ac2a862ba6e9bdf25bd690efbacb8961960a681ac25f0d3ae3f128`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 22:49:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 22:49:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 22:49:07 GMT
EXPOSE 80
# Wed, 15 Feb 2023 22:49:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 22:49:07 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 22:49:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57456bf9239ae8d2b09ba33d1227b60a493b664b0a0558a09a614e08aedf0438`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 663.2 KB (663152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92b39b3528b8dd48de9d16db14bfda9c6a0094d2fa75eafa29f6b1c1c168a11`  
		Last Modified: Wed, 15 Feb 2023 22:49:43 GMT  
		Size: 32.4 MB (32375688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c984c91836ae71200fb885d8fe5477ff6718e55e16d0d1d03e20b925a1107906`  
		Last Modified: Wed, 15 Feb 2023 22:49:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:latest` - linux; s390x

```console
$ docker pull traefik@sha256:e1440b2606e72909deec6ca7bee86ea2081864c320c28651dca4644ee581325d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37438024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ffd4bc9101c8ac43816d439afeedbc3fe84e411a98c5237e8c28019dd53af6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:37 GMT
ADD file:8a7d887c96c361c6ae19ca804030a0d79a1984b9e32b6c3767ede695c6613909 in / 
# Fri, 10 Feb 2023 21:41:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:21:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 22:46:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 22:46:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 22:46:13 GMT
EXPOSE 80
# Wed, 15 Feb 2023 22:46:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 22:46:14 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 22:46:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0d71e9a79f477719291f0a25b6a2462917f2e396325883144c1f1e59fbc56f21`  
		Last Modified: Fri, 10 Feb 2023 21:42:33 GMT  
		Size: 2.6 MB (2610267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e10f8aa3cb11731ad3d5cea5740b9baa80c4652f810b4efd47d507984fa8d8`  
		Last Modified: Sat, 11 Feb 2023 05:22:25 GMT  
		Size: 666.4 KB (666384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595453c84153d4d6b45b74c510ea02485c73813554c2753e704ac2a3ee5075e`  
		Last Modified: Wed, 15 Feb 2023 22:46:55 GMT  
		Size: 34.2 MB (34161005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c6f65f8083b617d701bc732b372962e6aa9b9f620a349ef3ce2191e197a7f`  
		Last Modified: Wed, 15 Feb 2023 22:46:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles`

```console
$ docker pull traefik@sha256:fc9a03a8a58c18c573451455172d31b8d85119da6c57b2b200fbea546b1161ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles` - linux; amd64

```console
$ docker pull traefik@sha256:a37a3469b7bd1e58d95ab5918f31f3a8aada1bdfa90f8d963eb78e8bae37d025
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22594315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b06305d2e0eca68d66088b5290a28c31dd73722f3f8e33c764bd60faf17edd7`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Sat, 11 Feb 2023 14:05:58 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Sat, 11 Feb 2023 14:05:59 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Sat, 11 Feb 2023 14:05:59 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:59 GMT
VOLUME [/tmp]
# Sat, 11 Feb 2023 14:05:59 GMT
ENTRYPOINT ["/traefik"]
# Sat, 11 Feb 2023 14:05:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b232dbde1f095d758c59886ecc24a42610dd35fd72116f3bf04738104e1cfa`  
		Last Modified: Sat, 11 Feb 2023 14:07:25 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066ff3631f4c0a13ebb72826195f8332b28aa6c9945865b1c07076fad46fb81b`  
		Last Modified: Sat, 11 Feb 2023 14:07:29 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7d30df83fa81bb480812fb04384c340a5414a90b3ef139ed06b11db2629ab6d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1a3efa227e28dd72fe4fe204cfc7a77441567e522b5aec07bea603efcf3767`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 14 Mar 2023 01:31:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Tue, 14 Mar 2023 01:31:59 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Tue, 14 Mar 2023 01:32:01 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Tue, 14 Mar 2023 01:32:01 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:32:01 GMT
VOLUME [/tmp]
# Tue, 14 Mar 2023 01:32:01 GMT
ENTRYPOINT ["/traefik"]
# Tue, 14 Mar 2023 01:32:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:68a2bb2e7a38ecc0a394b8fde6e116d903af0a9081c1816df304ab9a95b081da`  
		Last Modified: Tue, 14 Mar 2023 01:34:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abcbdf883582fff78fa64c20ff3783c94c68cbdc4b3c199fc94e53b5094e4e6`  
		Last Modified: Tue, 14 Mar 2023 01:34:17 GMT  
		Size: 308.9 KB (308851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8772ce58379f8b2532ee1b93c4220cd99b6e6c0c6a5ccad7ff67de5849bc65e`  
		Last Modified: Tue, 14 Mar 2023 01:34:22 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ac5b287132e97dc27bbd96791a25701e051ddce973d6ee70eda1c87138e3c299
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d5da1bea8e1a3e20b83ceca6e486a1e881451b1e304a0281d936d5e51f418d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:00:57 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:00:58 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 11 Nov 2022 11:00:58 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:58 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:00:58 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:00:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f6a6b590d30fda524213974a86d6ca01981b3ab4154a359b9c2e3fa3262c6`  
		Last Modified: Fri, 11 Nov 2022 11:02:04 GMT  
		Size: 308.8 KB (308813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af8a7d805d81cf74f58f3793659f76132259201bea15bbb7a0edc6191f8edfa`  
		Last Modified: Fri, 11 Nov 2022 11:02:07 GMT  
		Size: 20.1 MB (20131346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-alpine`

```console
$ docker pull traefik@sha256:dae77187506098f71a878261bde8207a34ec77e283bfcce446e8a5332c54992f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:maroilles-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:6a5bf0d59212a73927e18da4a5b85ff7d02fb566283bcd10b3c307b8a39627a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25653523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:299327139165b0025a883c7a11747b5d04c4bc72f053601c0f763fee0ed761a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:51 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:52 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fab313a1ca0ee79d027587c5edad5ff243a08e1cbd263abe2a17503c316d8b`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 661.5 KB (661461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e550be36e43026c7c9214cf16b3b866de5ce1da12f14fcef46658c0def1d4a7`  
		Last Modified: Sat, 11 Feb 2023 14:07:12 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4561714fba29bd0d410fa9813afc75479ffef93714ffdad849a7943771d73544`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9b251f4e7f9ac30ecbca3b12d2e03cbb774df99d708e61e84e23a5e6ed53f08d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01eaf16e6615e6646fa59fb368b61c5a55cad7eef251093d04c76f2529a135d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:54 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Mon, 13 Mar 2023 16:12:54 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:51 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:51 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:51 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d811b603dbe15ba6438e580f10afa348eb213b791a9252642521f986fd77e0d`  
		Last Modified: Tue, 14 Mar 2023 01:33:53 GMT  
		Size: 666.4 KB (666440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b099a3d2655c5ee12dfd7e0cd01338c6305193d9e7329186ba998a100afae1`  
		Last Modified: Tue, 14 Mar 2023 01:33:57 GMT  
		Size: 20.6 MB (20623429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a10f592ec7cdfd0ff7a0f1c3a8473de24a82068b80b9239b3436398f7c1af5`  
		Last Modified: Tue, 14 Mar 2023 01:33:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:maroilles-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e23b8edb3c8a7f4a5ce7b2697e304f8e31d845474dccdbcd15b86e831c7bc69b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72dbaffc2f8e74c9ed9aa7a99d590e792ba2b318e8562992180335ba122958e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:46 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:46 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:46 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c8dd85906c92d3445ffeb0481950055e77c854095c4cbbd854f6951242a3c`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 663.2 KB (663163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0994ad8baa5503f4c667ced5bb36b643eba7642f9791e4bf7975527de9f2c2ed`  
		Last Modified: Sat, 11 Feb 2023 06:41:57 GMT  
		Size: 20.1 MB (20131363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6a5a822a3369f9999a4da4bcb9718729d386c2dbf108fb8a8a52056eacc8d2`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:maroilles-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f643d6e3857163a610f6ee48dcedefc4ae1c6957968b821a132c45dad295521d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:maroilles-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:eb030d1415b37297490d0d042c132510d0592f8158bb80f98328bebe132c71c7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036484756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd883fc0a81df58f398881ad9a26665e14af2ff944186704211ca53de351d281`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:48:48 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 16 Mar 2023 08:48:49 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:48:50 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:48:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c40e4a974e18ba73f3964c77bafb530b44a02b157bff67d57d80b50a37d306`  
		Last Modified: Thu, 16 Mar 2023 08:50:12 GMT  
		Size: 23.0 MB (22970100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b8a1819bca4f2eb81e780d11f83ab69e9c936aeaddbd31803a9949cf487145`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5590048d6ec03d383585a24a3e40df19cce710181b483bb92abd200c87c856`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbdbd264f1bd9f178ca6c87b2073841bac0e4226b3fed4145bbdb0c46e98ca1`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7`

```console
$ docker pull traefik@sha256:fc9a03a8a58c18c573451455172d31b8d85119da6c57b2b200fbea546b1161ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7` - linux; amd64

```console
$ docker pull traefik@sha256:a37a3469b7bd1e58d95ab5918f31f3a8aada1bdfa90f8d963eb78e8bae37d025
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22594315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b06305d2e0eca68d66088b5290a28c31dd73722f3f8e33c764bd60faf17edd7`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Sat, 11 Feb 2023 14:05:58 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Sat, 11 Feb 2023 14:05:59 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Sat, 11 Feb 2023 14:05:59 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:59 GMT
VOLUME [/tmp]
# Sat, 11 Feb 2023 14:05:59 GMT
ENTRYPOINT ["/traefik"]
# Sat, 11 Feb 2023 14:05:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b232dbde1f095d758c59886ecc24a42610dd35fd72116f3bf04738104e1cfa`  
		Last Modified: Sat, 11 Feb 2023 14:07:25 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066ff3631f4c0a13ebb72826195f8332b28aa6c9945865b1c07076fad46fb81b`  
		Last Modified: Sat, 11 Feb 2023 14:07:29 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7d30df83fa81bb480812fb04384c340a5414a90b3ef139ed06b11db2629ab6d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1a3efa227e28dd72fe4fe204cfc7a77441567e522b5aec07bea603efcf3767`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 14 Mar 2023 01:31:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Tue, 14 Mar 2023 01:31:59 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Tue, 14 Mar 2023 01:32:01 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Tue, 14 Mar 2023 01:32:01 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:32:01 GMT
VOLUME [/tmp]
# Tue, 14 Mar 2023 01:32:01 GMT
ENTRYPOINT ["/traefik"]
# Tue, 14 Mar 2023 01:32:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:68a2bb2e7a38ecc0a394b8fde6e116d903af0a9081c1816df304ab9a95b081da`  
		Last Modified: Tue, 14 Mar 2023 01:34:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abcbdf883582fff78fa64c20ff3783c94c68cbdc4b3c199fc94e53b5094e4e6`  
		Last Modified: Tue, 14 Mar 2023 01:34:17 GMT  
		Size: 308.9 KB (308851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8772ce58379f8b2532ee1b93c4220cd99b6e6c0c6a5ccad7ff67de5849bc65e`  
		Last Modified: Tue, 14 Mar 2023 01:34:22 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ac5b287132e97dc27bbd96791a25701e051ddce973d6ee70eda1c87138e3c299
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d5da1bea8e1a3e20b83ceca6e486a1e881451b1e304a0281d936d5e51f418d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:00:57 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:00:58 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 11 Nov 2022 11:00:58 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:58 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:00:58 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:00:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f6a6b590d30fda524213974a86d6ca01981b3ab4154a359b9c2e3fa3262c6`  
		Last Modified: Fri, 11 Nov 2022 11:02:04 GMT  
		Size: 308.8 KB (308813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af8a7d805d81cf74f58f3793659f76132259201bea15bbb7a0edc6191f8edfa`  
		Last Modified: Fri, 11 Nov 2022 11:02:07 GMT  
		Size: 20.1 MB (20131346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-alpine`

```console
$ docker pull traefik@sha256:dae77187506098f71a878261bde8207a34ec77e283bfcce446e8a5332c54992f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:6a5bf0d59212a73927e18da4a5b85ff7d02fb566283bcd10b3c307b8a39627a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25653523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:299327139165b0025a883c7a11747b5d04c4bc72f053601c0f763fee0ed761a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:51 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:52 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fab313a1ca0ee79d027587c5edad5ff243a08e1cbd263abe2a17503c316d8b`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 661.5 KB (661461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e550be36e43026c7c9214cf16b3b866de5ce1da12f14fcef46658c0def1d4a7`  
		Last Modified: Sat, 11 Feb 2023 14:07:12 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4561714fba29bd0d410fa9813afc75479ffef93714ffdad849a7943771d73544`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9b251f4e7f9ac30ecbca3b12d2e03cbb774df99d708e61e84e23a5e6ed53f08d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01eaf16e6615e6646fa59fb368b61c5a55cad7eef251093d04c76f2529a135d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:54 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Mon, 13 Mar 2023 16:12:54 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:51 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:51 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:51 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d811b603dbe15ba6438e580f10afa348eb213b791a9252642521f986fd77e0d`  
		Last Modified: Tue, 14 Mar 2023 01:33:53 GMT  
		Size: 666.4 KB (666440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b099a3d2655c5ee12dfd7e0cd01338c6305193d9e7329186ba998a100afae1`  
		Last Modified: Tue, 14 Mar 2023 01:33:57 GMT  
		Size: 20.6 MB (20623429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a10f592ec7cdfd0ff7a0f1c3a8473de24a82068b80b9239b3436398f7c1af5`  
		Last Modified: Tue, 14 Mar 2023 01:33:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e23b8edb3c8a7f4a5ce7b2697e304f8e31d845474dccdbcd15b86e831c7bc69b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72dbaffc2f8e74c9ed9aa7a99d590e792ba2b318e8562992180335ba122958e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:46 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:46 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:46 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c8dd85906c92d3445ffeb0481950055e77c854095c4cbbd854f6951242a3c`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 663.2 KB (663163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0994ad8baa5503f4c667ced5bb36b643eba7642f9791e4bf7975527de9f2c2ed`  
		Last Modified: Sat, 11 Feb 2023 06:41:57 GMT  
		Size: 20.1 MB (20131363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6a5a822a3369f9999a4da4bcb9718729d386c2dbf108fb8a8a52056eacc8d2`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f643d6e3857163a610f6ee48dcedefc4ae1c6957968b821a132c45dad295521d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v1.7-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:eb030d1415b37297490d0d042c132510d0592f8158bb80f98328bebe132c71c7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036484756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd883fc0a81df58f398881ad9a26665e14af2ff944186704211ca53de351d281`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:48:48 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 16 Mar 2023 08:48:49 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:48:50 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:48:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c40e4a974e18ba73f3964c77bafb530b44a02b157bff67d57d80b50a37d306`  
		Last Modified: Thu, 16 Mar 2023 08:50:12 GMT  
		Size: 23.0 MB (22970100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b8a1819bca4f2eb81e780d11f83ab69e9c936aeaddbd31803a9949cf487145`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5590048d6ec03d383585a24a3e40df19cce710181b483bb92abd200c87c856`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbdbd264f1bd9f178ca6c87b2073841bac0e4226b3fed4145bbdb0c46e98ca1`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34`

```console
$ docker pull traefik@sha256:fc9a03a8a58c18c573451455172d31b8d85119da6c57b2b200fbea546b1161ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34` - linux; amd64

```console
$ docker pull traefik@sha256:a37a3469b7bd1e58d95ab5918f31f3a8aada1bdfa90f8d963eb78e8bae37d025
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **22.6 MB (22594315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b06305d2e0eca68d66088b5290a28c31dd73722f3f8e33c764bd60faf17edd7`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Fri, 07 Oct 2022 04:21:33 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Sat, 11 Feb 2023 14:05:58 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Sat, 11 Feb 2023 14:05:59 GMT
COPY file:36217e5a6056bef26cfff395c8af8c1010a61dbe8d62b2c7869ca221e2a6302c in / 
# Sat, 11 Feb 2023 14:05:59 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:59 GMT
VOLUME [/tmp]
# Sat, 11 Feb 2023 14:05:59 GMT
ENTRYPOINT ["/traefik"]
# Sat, 11 Feb 2023 14:05:59 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:39006e619508cd8a1ace2dcb57ecaa3a206fc01c9b72018e30b538ba58b0f45a`  
		Last Modified: Fri, 07 Oct 2022 04:22:39 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b232dbde1f095d758c59886ecc24a42610dd35fd72116f3bf04738104e1cfa`  
		Last Modified: Sat, 11 Feb 2023 14:07:25 GMT  
		Size: 308.8 KB (308823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066ff3631f4c0a13ebb72826195f8332b28aa6c9945865b1c07076fad46fb81b`  
		Last Modified: Sat, 11 Feb 2023 14:07:29 GMT  
		Size: 22.2 MB (22161952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm variant v6

```console
$ docker pull traefik@sha256:7d30df83fa81bb480812fb04384c340a5414a90b3ef139ed06b11db2629ab6d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.1 MB (21055672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1a3efa227e28dd72fe4fe204cfc7a77441567e522b5aec07bea603efcf3767`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Tue, 14 Mar 2023 01:31:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Tue, 14 Mar 2023 01:31:59 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Tue, 14 Mar 2023 01:32:01 GMT
COPY file:5d1e7e81e8b77b4f8828eeaf0d30a0f135a949b51396f12ae22af376c36d3129 in / 
# Tue, 14 Mar 2023 01:32:01 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:32:01 GMT
VOLUME [/tmp]
# Tue, 14 Mar 2023 01:32:01 GMT
ENTRYPOINT ["/traefik"]
# Tue, 14 Mar 2023 01:32:01 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:68a2bb2e7a38ecc0a394b8fde6e116d903af0a9081c1816df304ab9a95b081da`  
		Last Modified: Tue, 14 Mar 2023 01:34:18 GMT  
		Size: 123.5 KB (123540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2abcbdf883582fff78fa64c20ff3783c94c68cbdc4b3c199fc94e53b5094e4e6`  
		Last Modified: Tue, 14 Mar 2023 01:34:17 GMT  
		Size: 308.9 KB (308851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8772ce58379f8b2532ee1b93c4220cd99b6e6c0c6a5ccad7ff67de5849bc65e`  
		Last Modified: Tue, 14 Mar 2023 01:34:22 GMT  
		Size: 20.6 MB (20623281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:ac5b287132e97dc27bbd96791a25701e051ddce973d6ee70eda1c87138e3c299
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.6 MB (20563697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9d5da1bea8e1a3e20b83ceca6e486a1e881451b1e304a0281d936d5e51f418d`
-	Entrypoint: `["\/traefik"]`

```dockerfile
# Thu, 27 Oct 2022 23:00:59 GMT
COPY file:48964762d0c961c28f59ebd3ea194fb6486cf2bd9a9cf1780f6702d88bd7b7d9 in /etc/ssl/certs/ 
# Fri, 11 Nov 2022 11:00:57 GMT
COPY dir:3b1b1d8650d4180b42ead5fd074947c16b0405195b425df367fbf007be68841d in /usr/share/ 
# Fri, 11 Nov 2022 11:00:58 GMT
COPY file:60330593b6644f3f519fd13ce8ee34c2c7ab9994a1420afabbc01926dd1230dd in / 
# Fri, 11 Nov 2022 11:00:58 GMT
EXPOSE 80
# Fri, 11 Nov 2022 11:00:58 GMT
VOLUME [/tmp]
# Fri, 11 Nov 2022 11:00:58 GMT
ENTRYPOINT ["/traefik"]
# Fri, 11 Nov 2022 11:00:58 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:384a668e636c3a58c260d7eacd140f07b0727673d5ba128334cbcedd184a99f2`  
		Last Modified: Thu, 27 Oct 2022 23:02:00 GMT  
		Size: 123.5 KB (123538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3f6a6b590d30fda524213974a86d6ca01981b3ab4154a359b9c2e3fa3262c6`  
		Last Modified: Fri, 11 Nov 2022 11:02:04 GMT  
		Size: 308.8 KB (308813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af8a7d805d81cf74f58f3793659f76132259201bea15bbb7a0edc6191f8edfa`  
		Last Modified: Fri, 11 Nov 2022 11:02:07 GMT  
		Size: 20.1 MB (20131346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-alpine`

```console
$ docker pull traefik@sha256:dae77187506098f71a878261bde8207a34ec77e283bfcce446e8a5332c54992f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `traefik:v1.7.34-alpine` - linux; amd64

```console
$ docker pull traefik@sha256:6a5bf0d59212a73927e18da4a5b85ff7d02fb566283bcd10b3c307b8a39627a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25653523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:299327139165b0025a883c7a11747b5d04c4bc72f053601c0f763fee0ed761a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:46 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:51 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:51 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:51 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:52 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:52 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fab313a1ca0ee79d027587c5edad5ff243a08e1cbd263abe2a17503c316d8b`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 661.5 KB (661461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e550be36e43026c7c9214cf16b3b866de5ce1da12f14fcef46658c0def1d4a7`  
		Last Modified: Sat, 11 Feb 2023 14:07:12 GMT  
		Size: 22.2 MB (22162062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4561714fba29bd0d410fa9813afc75479ffef93714ffdad849a7943771d73544`  
		Last Modified: Sat, 11 Feb 2023 14:07:08 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm variant v6

```console
$ docker pull traefik@sha256:9b251f4e7f9ac30ecbca3b12d2e03cbb774df99d708e61e84e23a5e6ed53f08d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.9 MB (23928389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01eaf16e6615e6646fa59fb368b61c5a55cad7eef251093d04c76f2529a135d3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:54 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Mon, 13 Mar 2023 16:12:54 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:44 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:50 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:50 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:51 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:51 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:51 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d811b603dbe15ba6438e580f10afa348eb213b791a9252642521f986fd77e0d`  
		Last Modified: Tue, 14 Mar 2023 01:33:53 GMT  
		Size: 666.4 KB (666440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b099a3d2655c5ee12dfd7e0cd01338c6305193d9e7329186ba998a100afae1`  
		Last Modified: Tue, 14 Mar 2023 01:33:57 GMT  
		Size: 20.6 MB (20623429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a10f592ec7cdfd0ff7a0f1c3a8473de24a82068b80b9239b3436398f7c1af5`  
		Last Modified: Tue, 14 Mar 2023 01:33:53 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v1.7.34-alpine` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:e23b8edb3c8a7f4a5ce7b2697e304f8e31d845474dccdbcd15b86e831c7bc69b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23519920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72dbaffc2f8e74c9ed9aa7a99d590e792ba2b318e8562992180335ba122958e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:42 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:45 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='arm' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /usr/local/bin/traefik "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_linux-$arch"; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:46 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:46 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:46 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:46 GMT
LABEL org.opencontainers.image.vendor=traefik org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5c8dd85906c92d3445ffeb0481950055e77c854095c4cbbd854f6951242a3c`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 663.2 KB (663163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0994ad8baa5503f4c667ced5bb36b643eba7642f9791e4bf7975527de9f2c2ed`  
		Last Modified: Sat, 11 Feb 2023 06:41:57 GMT  
		Size: 20.1 MB (20131363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6a5a822a3369f9999a4da4bcb9718729d386c2dbf108fb8a8a52056eacc8d2`  
		Last Modified: Sat, 11 Feb 2023 06:41:54 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v1.7.34-windowsservercore-1809`

```console
$ docker pull traefik@sha256:f643d6e3857163a610f6ee48dcedefc4ae1c6957968b821a132c45dad295521d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v1.7.34-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:eb030d1415b37297490d0d042c132510d0592f8158bb80f98328bebe132c71c7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2036484756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd883fc0a81df58f398881ad9a26665e14af2ff944186704211ca53de351d281`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:48:48 GMT
RUN Invoke-WebRequest     -Uri "https://github.com/traefik/traefik/releases/download/v1.7.34/traefik_windows-amd64.exe"     -OutFile "/traefik.exe"
# Thu, 16 Mar 2023 08:48:49 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:48:50 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:48:51 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v1.7.34 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c40e4a974e18ba73f3964c77bafb530b44a02b157bff67d57d80b50a37d306`  
		Last Modified: Thu, 16 Mar 2023 08:50:12 GMT  
		Size: 23.0 MB (22970100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b8a1819bca4f2eb81e780d11f83ab69e9c936aeaddbd31803a9949cf487145`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5590048d6ec03d383585a24a3e40df19cce710181b483bb92abd200c87c856`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbdbd264f1bd9f178ca6c87b2073841bac0e4226b3fed4145bbdb0c46e98ca1`  
		Last Modified: Thu, 16 Mar 2023 08:50:06 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9`

```console
$ docker pull traefik@sha256:a29972da395acf3f186b01bca023985dd736545d1bccc55a33a7376adeee3495
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v2.9` - linux; amd64

```console
$ docker pull traefik@sha256:553239e27c4614d0477651415205b9b119f7a98f698e6562ef383c9d8ff3b6e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38777669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85dec640e68e655f5cf95c8ce8671da1194710b38a539166ca080ba0c93e1d4d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 23:22:08 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 23:22:09 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 23:22:09 GMT
EXPOSE 80
# Wed, 15 Feb 2023 23:22:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 23:22:09 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 23:22:09 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3655af1bbd56df1bcfec44686273a57d30cc0b69f6e501f87ec67712913b8b55`  
		Last Modified: Sat, 11 Feb 2023 14:06:23 GMT  
		Size: 662.0 KB (662047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f984ad6ecbda363b2ce6487b63b68f4f9f68741c7a7c2e50c3e68e1faf9aec5`  
		Last Modified: Wed, 15 Feb 2023 23:22:46 GMT  
		Size: 35.3 MB (35289107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823d14d881861f99e9db87cb68a06cdead6f070c4920274ac6a0d173432a0043`  
		Last Modified: Wed, 15 Feb 2023 23:22:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; arm variant v6

```console
$ docker pull traefik@sha256:b45f882e5a6c1229a285aa460569aa45c487c878ff713c9d038d012a9ea7cf74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36629054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a42eaf1d53da78868c01e06a4c4b2fa9dde5d9aa210460f2948fb6f13f1781b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:34 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:35 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:35 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:36 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:36 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937713bf36e8ddb19f4d3861767039861708c7cc2a83e388aa80b6981bd0dc3a`  
		Last Modified: Tue, 14 Mar 2023 01:32:58 GMT  
		Size: 666.5 KB (666511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930bc1d14d49fdac439a68245e1142963cd97f387ff68c5eb42604d4fc03e324`  
		Last Modified: Tue, 14 Mar 2023 01:33:29 GMT  
		Size: 33.3 MB (33328526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331609b39766af505ef55a69602b8ceac4018a6aca9937efac165e7296ba860c`  
		Last Modified: Tue, 14 Mar 2023 01:33:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:9c79fa649e5cbe903c4815a112e8bd370a27492589550418e20ac5dfa1ca0879
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35760765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4616f42b3ac2a862ba6e9bdf25bd690efbacb8961960a681ac25f0d3ae3f128`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 22:49:07 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 22:49:07 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 22:49:07 GMT
EXPOSE 80
# Wed, 15 Feb 2023 22:49:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 22:49:07 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 22:49:08 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57456bf9239ae8d2b09ba33d1227b60a493b664b0a0558a09a614e08aedf0438`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 663.2 KB (663152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92b39b3528b8dd48de9d16db14bfda9c6a0094d2fa75eafa29f6b1c1c168a11`  
		Last Modified: Wed, 15 Feb 2023 22:49:43 GMT  
		Size: 32.4 MB (32375688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c984c91836ae71200fb885d8fe5477ff6718e55e16d0d1d03e20b925a1107906`  
		Last Modified: Wed, 15 Feb 2023 22:49:40 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v2.9` - linux; s390x

```console
$ docker pull traefik@sha256:e1440b2606e72909deec6ca7bee86ea2081864c320c28651dca4644ee581325d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37438024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ffd4bc9101c8ac43816d439afeedbc3fe84e411a98c5237e8c28019dd53af6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:37 GMT
ADD file:8a7d887c96c361c6ae19ca804030a0d79a1984b9e32b6c3767ede695c6613909 in / 
# Fri, 10 Feb 2023 21:41:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:21:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Wed, 15 Feb 2023 22:46:09 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v2.9.8/traefik_v2.9.8_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Wed, 15 Feb 2023 22:46:13 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Wed, 15 Feb 2023 22:46:13 GMT
EXPOSE 80
# Wed, 15 Feb 2023 22:46:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 15 Feb 2023 22:46:14 GMT
CMD ["traefik"]
# Wed, 15 Feb 2023 22:46:14 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.8 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0d71e9a79f477719291f0a25b6a2462917f2e396325883144c1f1e59fbc56f21`  
		Last Modified: Fri, 10 Feb 2023 21:42:33 GMT  
		Size: 2.6 MB (2610267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e10f8aa3cb11731ad3d5cea5740b9baa80c4652f810b4efd47d507984fa8d8`  
		Last Modified: Sat, 11 Feb 2023 05:22:25 GMT  
		Size: 666.4 KB (666384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9595453c84153d4d6b45b74c510ea02485c73813554c2753e704ac2a3ee5075e`  
		Last Modified: Wed, 15 Feb 2023 22:46:55 GMT  
		Size: 34.2 MB (34161005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7c6f65f8083b617d701bc732b372962e6aa9b9f620a349ef3ce2191e197a7f`  
		Last Modified: Wed, 15 Feb 2023 22:46:50 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1d23dcfba19d25a7db7e5cd85cfcb48ecc50e88cd0ada6101f1f125b5a69e87f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v2.9-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:09d2d0195ec592feca5562747351e547f37853ef9400af79664398ad0e67df8f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2756d6e358452d2bdb882cda3b649d92fc7edef462e0d4d4268b1b78d2fde2f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 21 Mar 2023 19:17:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.9/traefik_v2.9.9_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 21 Mar 2023 19:17:08 GMT
EXPOSE 80
# Tue, 21 Mar 2023 19:17:09 GMT
ENTRYPOINT ["/traefik"]
# Tue, 21 Mar 2023 19:17:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.9 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa99ce6cd34b6eec9c095cd7936aeed038d0e89f07b98e0854b8d40625b3d844`  
		Last Modified: Tue, 21 Mar 2023 19:18:05 GMT  
		Size: 36.3 MB (36264213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e291ba8ae74eee25775851ef3eca803d2166e1606f542c53019340d6f5930bc`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1b936795c1df1230fc4fef82f77463356552d7296c59ee6dc3410c2d81303e`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38befdb3655c93aebc9c7975e6bb46d591fb7e4785d6fe33725d3fe2b89d8105`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v2.9.9`

```console
$ docker pull traefik@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `traefik:v2.9.9-windowsservercore-1809`

```console
$ docker pull traefik@sha256:1d23dcfba19d25a7db7e5cd85cfcb48ecc50e88cd0ada6101f1f125b5a69e87f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v2.9.9-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:09d2d0195ec592feca5562747351e547f37853ef9400af79664398ad0e67df8f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2756d6e358452d2bdb882cda3b649d92fc7edef462e0d4d4268b1b78d2fde2f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 21 Mar 2023 19:17:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.9/traefik_v2.9.9_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 21 Mar 2023 19:17:08 GMT
EXPOSE 80
# Tue, 21 Mar 2023 19:17:09 GMT
ENTRYPOINT ["/traefik"]
# Tue, 21 Mar 2023 19:17:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.9 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa99ce6cd34b6eec9c095cd7936aeed038d0e89f07b98e0854b8d40625b3d844`  
		Last Modified: Tue, 21 Mar 2023 19:18:05 GMT  
		Size: 36.3 MB (36264213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e291ba8ae74eee25775851ef3eca803d2166e1606f542c53019340d6f5930bc`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1b936795c1df1230fc4fef82f77463356552d7296c59ee6dc3410c2d81303e`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38befdb3655c93aebc9c7975e6bb46d591fb7e4785d6fe33725d3fe2b89d8105`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0`

```console
$ docker pull traefik@sha256:1f88c068865e68dde18a29aec644a1c92432e4d4279abfb9c80df845f8019173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0` - linux; amd64

```console
$ docker pull traefik@sha256:bf822393b55095bc13f7699ae1fa1b56bbe2e072bc2ae283bffd3a4dadd98d7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40563449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e32ad70784035ddea0808eeb76e7f8a6bc64e2cb867b63c6513f8f4e853f1133`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:33 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:33 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3655af1bbd56df1bcfec44686273a57d30cc0b69f6e501f87ec67712913b8b55`  
		Last Modified: Sat, 11 Feb 2023 14:06:23 GMT  
		Size: 662.0 KB (662047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cc32ef302c3bee4df8ba7b31c8717d000beefd7e66fbdcc07450792441ad67`  
		Last Modified: Sat, 11 Feb 2023 14:06:28 GMT  
		Size: 37.1 MB (37074888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f96cb39092b375e76e59ca53f161a1777975c9c58ea5d46e480812addb564`  
		Last Modified: Sat, 11 Feb 2023 14:06:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c6eb90c1a642c95756e04f947caee3baaed18ea1e02780df54b15240795df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a352a59877646edd78a3c6c811509111a92cd686212c584e5a5ee4845aed3818`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:21 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:22 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:23 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937713bf36e8ddb19f4d3861767039861708c7cc2a83e388aa80b6981bd0dc3a`  
		Last Modified: Tue, 14 Mar 2023 01:32:58 GMT  
		Size: 666.5 KB (666511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09007fbe2ec6b465a9c6d24d737b5f27c316d90aaae93757efb986a68a59acf9`  
		Last Modified: Tue, 14 Mar 2023 01:33:03 GMT  
		Size: 35.0 MB (34989328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50ac3be21a5d5b5b332f61de0380a4216157129e1668df6f68dde1d969fb098`  
		Last Modified: Tue, 14 Mar 2023 01:32:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:49b2e1db6ca60eae983dab7632ed2ea3997c698d05dd6789eeac4de13c94ea14
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0b18449b8e63bade321e2c66ff5674dd5d7e3a36154f012db7b37c3c668a53`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:29 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:30 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:30 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57456bf9239ae8d2b09ba33d1227b60a493b664b0a0558a09a614e08aedf0438`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 663.2 KB (663152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e1381066f019ec8bedc5c9e8c8dcae4ed86e75cb46d22c461d5a87a060f23a`  
		Last Modified: Sat, 11 Feb 2023 06:41:17 GMT  
		Size: 34.0 MB (34023515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac00a09db30fc81aca200d38461e38fcc368b57e9878c1f51bb832b235e287d`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0` - linux; s390x

```console
$ docker pull traefik@sha256:c50bbeaf64f9b8a1d4a6f4ec10ff476e2066ac2dc59230bf8f02ce77f9cb4f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d71fc91baad09e19cde42a2c649d7dc4a303b86b94d97f988e69e7da9222d76`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:37 GMT
ADD file:8a7d887c96c361c6ae19ca804030a0d79a1984b9e32b6c3767ede695c6613909 in / 
# Fri, 10 Feb 2023 21:41:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:21:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 05:21:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 05:21:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 05:21:37 GMT
EXPOSE 80
# Sat, 11 Feb 2023 05:21:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 05:21:37 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 05:21:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0d71e9a79f477719291f0a25b6a2462917f2e396325883144c1f1e59fbc56f21`  
		Last Modified: Fri, 10 Feb 2023 21:42:33 GMT  
		Size: 2.6 MB (2610267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e10f8aa3cb11731ad3d5cea5740b9baa80c4652f810b4efd47d507984fa8d8`  
		Last Modified: Sat, 11 Feb 2023 05:22:25 GMT  
		Size: 666.4 KB (666384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1f663552d308b8665c6af4376a263f91e8bf072db5dce19d544e897af5aa9`  
		Last Modified: Sat, 11 Feb 2023 05:22:30 GMT  
		Size: 35.9 MB (35855467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6a80fe50e1182c4db36fc9b9c0c0ed898c4e2745f7b16e7a2654fa5a403a2d`  
		Last Modified: Sat, 11 Feb 2023 05:22:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2eb0d945da364a274f76288295b9120086404be2c7606fe340ac2ee6f1d64ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v3.0-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:62e9db8356188c92dbce1706a8c2af3702993ee762b34d398fc7921eb03a3629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051205802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648f7c4938c24c605c3f3cbf0b16d4a5767ce075cd407fa9c6ab93e256035917`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:45:29 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Mar 2023 08:45:30 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:45:31 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:45:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eafb0300ea614e208e5052cfdd0941f2ad90a341c5b337ab489e223bb31e88`  
		Last Modified: Thu, 16 Mar 2023 08:49:24 GMT  
		Size: 37.7 MB (37691161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec0dc51e5d37193b3e6ebdd21f1bb94e44f593af5691b32af00720bb4548bbc`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28da668ed65b21bb734a5ba72dd5262a27de001c56a64bebf1db5e9244aaad4c`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6138998225adfde27a93f621c64ba53c628511ce9209f16661fd0c3619ff3e3`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta2`

```console
$ docker pull traefik@sha256:1f88c068865e68dde18a29aec644a1c92432e4d4279abfb9c80df845f8019173
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; s390x

### `traefik:v3.0.0-beta2` - linux; amd64

```console
$ docker pull traefik@sha256:bf822393b55095bc13f7699ae1fa1b56bbe2e072bc2ae283bffd3a4dadd98d7e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40563449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e32ad70784035ddea0808eeb76e7f8a6bc64e2cb867b63c6513f8f4e853f1133`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:05:27 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 14:05:32 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 14:05:33 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 14:05:33 GMT
EXPOSE 80
# Sat, 11 Feb 2023 14:05:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:05:33 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 14:05:33 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3655af1bbd56df1bcfec44686273a57d30cc0b69f6e501f87ec67712913b8b55`  
		Last Modified: Sat, 11 Feb 2023 14:06:23 GMT  
		Size: 662.0 KB (662047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cc32ef302c3bee4df8ba7b31c8717d000beefd7e66fbdcc07450792441ad67`  
		Last Modified: Sat, 11 Feb 2023 14:06:28 GMT  
		Size: 37.1 MB (37074888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f96cb39092b375e76e59ca53f161a1777975c9c58ea5d46e480812addb564`  
		Last Modified: Sat, 11 Feb 2023 14:06:22 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; arm variant v6

```console
$ docker pull traefik@sha256:c6eb90c1a642c95756e04f947caee3baaed18ea1e02780df54b15240795df9ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38289856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a352a59877646edd78a3c6c811509111a92cd686212c584e5a5ee4845aed3818`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:51 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Mon, 13 Mar 2023 16:12:51 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:31:15 GMT
RUN apk --no-cache add ca-certificates tzdata
# Tue, 14 Mar 2023 01:31:21 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Tue, 14 Mar 2023 01:31:22 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Tue, 14 Mar 2023 01:31:22 GMT
EXPOSE 80
# Tue, 14 Mar 2023 01:31:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Mar 2023 01:31:23 GMT
CMD ["traefik"]
# Tue, 14 Mar 2023 01:31:23 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937713bf36e8ddb19f4d3861767039861708c7cc2a83e388aa80b6981bd0dc3a`  
		Last Modified: Tue, 14 Mar 2023 01:32:58 GMT  
		Size: 666.5 KB (666511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09007fbe2ec6b465a9c6d24d737b5f27c316d90aaae93757efb986a68a59acf9`  
		Last Modified: Tue, 14 Mar 2023 01:33:03 GMT  
		Size: 35.0 MB (34989328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50ac3be21a5d5b5b332f61de0380a4216157129e1668df6f68dde1d969fb098`  
		Last Modified: Tue, 14 Mar 2023 01:32:57 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; arm64 variant v8

```console
$ docker pull traefik@sha256:49b2e1db6ca60eae983dab7632ed2ea3997c698d05dd6789eeac4de13c94ea14
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37408591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0b18449b8e63bade321e2c66ff5674dd5d7e3a36154f012db7b37c3c668a53`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:40:24 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 06:40:29 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 06:40:30 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 06:40:30 GMT
EXPOSE 80
# Sat, 11 Feb 2023 06:40:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 06:40:30 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 06:40:30 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57456bf9239ae8d2b09ba33d1227b60a493b664b0a0558a09a614e08aedf0438`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 663.2 KB (663152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e1381066f019ec8bedc5c9e8c8dcae4ed86e75cb46d22c461d5a87a060f23a`  
		Last Modified: Sat, 11 Feb 2023 06:41:17 GMT  
		Size: 34.0 MB (34023515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac00a09db30fc81aca200d38461e38fcc368b57e9878c1f51bb832b235e287d`  
		Last Modified: Sat, 11 Feb 2023 06:41:13 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `traefik:v3.0.0-beta2` - linux; s390x

```console
$ docker pull traefik@sha256:c50bbeaf64f9b8a1d4a6f4ec10ff476e2066ac2dc59230bf8f02ce77f9cb4f5d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39132486 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d71fc91baad09e19cde42a2c649d7dc4a303b86b94d97f988e69e7da9222d76`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["traefik"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:37 GMT
ADD file:8a7d887c96c361c6ae19ca804030a0d79a1984b9e32b6c3767ede695c6613909 in / 
# Fri, 10 Feb 2023 21:41:37 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:21:30 GMT
RUN apk --no-cache add ca-certificates tzdata
# Sat, 11 Feb 2023 05:21:35 GMT
RUN set -ex; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) arch='armv6' ;; 		aarch64) arch='arm64' ;; 		x86_64) arch='amd64' ;; 		s390x) arch='s390x' ;; 		*) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;; 	esac; 	wget --quiet -O /tmp/traefik.tar.gz "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_linux_$arch.tar.gz"; 	tar xzvf /tmp/traefik.tar.gz -C /usr/local/bin traefik; 	rm -f /tmp/traefik.tar.gz; 	chmod +x /usr/local/bin/traefik
# Sat, 11 Feb 2023 05:21:37 GMT
COPY file:59a219a1fb7a9dc894a7a9a4718fa97fd24adb0a4a6455240ec2ab0183da796e in / 
# Sat, 11 Feb 2023 05:21:37 GMT
EXPOSE 80
# Sat, 11 Feb 2023 05:21:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 05:21:37 GMT
CMD ["traefik"]
# Sat, 11 Feb 2023 05:21:37 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:0d71e9a79f477719291f0a25b6a2462917f2e396325883144c1f1e59fbc56f21`  
		Last Modified: Fri, 10 Feb 2023 21:42:33 GMT  
		Size: 2.6 MB (2610267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e10f8aa3cb11731ad3d5cea5740b9baa80c4652f810b4efd47d507984fa8d8`  
		Last Modified: Sat, 11 Feb 2023 05:22:25 GMT  
		Size: 666.4 KB (666384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f1f663552d308b8665c6af4376a263f91e8bf072db5dce19d544e897af5aa9`  
		Last Modified: Sat, 11 Feb 2023 05:22:30 GMT  
		Size: 35.9 MB (35855467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6a80fe50e1182c4db36fc9b9c0c0ed898c4e2745f7b16e7a2654fa5a403a2d`  
		Last Modified: Sat, 11 Feb 2023 05:22:24 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:v3.0.0-beta2-windowsservercore-1809`

```console
$ docker pull traefik@sha256:2eb0d945da364a274f76288295b9120086404be2c7606fe340ac2ee6f1d64ed1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:v3.0.0-beta2-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:62e9db8356188c92dbce1706a8c2af3702993ee762b34d398fc7921eb03a3629
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2051205802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648f7c4938c24c605c3f3cbf0b16d4a5767ce075cd407fa9c6ab93e256035917`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 08:45:29 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v3.0.0-beta2/traefik_v3.0.0-beta2_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Thu, 16 Mar 2023 08:45:30 GMT
EXPOSE 80
# Thu, 16 Mar 2023 08:45:31 GMT
ENTRYPOINT ["/traefik"]
# Thu, 16 Mar 2023 08:45:32 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v3.0.0-beta2 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eafb0300ea614e208e5052cfdd0941f2ad90a341c5b337ab489e223bb31e88`  
		Last Modified: Thu, 16 Mar 2023 08:49:24 GMT  
		Size: 37.7 MB (37691161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec0dc51e5d37193b3e6ebdd21f1bb94e44f593af5691b32af00720bb4548bbc`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28da668ed65b21bb734a5ba72dd5262a27de001c56a64bebf1db5e9244aaad4c`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6138998225adfde27a93f621c64ba53c628511ce9209f16661fd0c3619ff3e3`  
		Last Modified: Thu, 16 Mar 2023 08:49:15 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `traefik:windowsservercore-1809`

```console
$ docker pull traefik@sha256:1d23dcfba19d25a7db7e5cd85cfcb48ecc50e88cd0ada6101f1f125b5a69e87f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `traefik:windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull traefik@sha256:09d2d0195ec592feca5562747351e547f37853ef9400af79664398ad0e67df8f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2049778848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2756d6e358452d2bdb882cda3b649d92fc7edef462e0d4d4268b1b78d2fde2f`
-	Entrypoint: `["\/traefik"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 21 Mar 2023 19:17:07 GMT
RUN Invoke-WebRequest         -Uri "https://github.com/traefik/traefik/releases/download/v2.9.9/traefik_v2.9.9_windows_amd64.zip"         -OutFile "/traefik.zip";     Expand-Archive -Path "/traefik.zip" -DestinationPath "/" -Force;     Remove-Item "/traefik.zip" -Force
# Tue, 21 Mar 2023 19:17:08 GMT
EXPOSE 80
# Tue, 21 Mar 2023 19:17:09 GMT
ENTRYPOINT ["/traefik"]
# Tue, 21 Mar 2023 19:17:10 GMT
LABEL org.opencontainers.image.vendor=Traefik Labs org.opencontainers.image.url=https://traefik.io org.opencontainers.image.source=https://github.com/traefik/traefik org.opencontainers.image.title=Traefik org.opencontainers.image.description=A modern reverse-proxy org.opencontainers.image.version=v2.9.9 org.opencontainers.image.documentation=https://docs.traefik.io
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa99ce6cd34b6eec9c095cd7936aeed038d0e89f07b98e0854b8d40625b3d844`  
		Last Modified: Tue, 21 Mar 2023 19:18:05 GMT  
		Size: 36.3 MB (36264213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e291ba8ae74eee25775851ef3eca803d2166e1606f542c53019340d6f5930bc`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1b936795c1df1230fc4fef82f77463356552d7296c59ee6dc3410c2d81303e`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38befdb3655c93aebc9c7975e6bb46d591fb7e4785d6fe33725d3fe2b89d8105`  
		Last Modified: Tue, 21 Mar 2023 19:17:57 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
