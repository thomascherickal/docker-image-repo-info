<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:19`](#docker19)
-	[`docker:19.03`](#docker1903)
-	[`docker:19.03.5`](#docker19035)
-	[`docker:19.03.5-dind`](#docker19035-dind)
-	[`docker:19.03.5-dind-rootless`](#docker19035-dind-rootless)
-	[`docker:19.03.5-git`](#docker19035-git)
-	[`docker:19.03-dind`](#docker1903-dind)
-	[`docker:19.03-dind-rootless`](#docker1903-dind-rootless)
-	[`docker:19.03-git`](#docker1903-git)
-	[`docker:19-dind`](#docker19-dind)
-	[`docker:19-dind-rootless`](#docker19-dind-rootless)
-	[`docker:19-git`](#docker19-git)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:stable`](#dockerstable)
-	[`docker:stable-dind`](#dockerstable-dind)
-	[`docker:stable-dind-rootless`](#dockerstable-dind-rootless)
-	[`docker:stable-git`](#dockerstable-git)
-	[`docker:test`](#dockertest)
-	[`docker:test-dind`](#dockertest-dind)
-	[`docker:test-dind-rootless`](#dockertest-dind-rootless)
-	[`docker:test-git`](#dockertest-git)

## `docker:19`

```console
$ docker pull docker@sha256:f5ea831fc81d7a65d4220f4c90e3be2514d6f85646156ed5ca63ec54abf639d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19` - linux; amd64

```console
$ docker pull docker@sha256:b7736ba0a18b5b9dfe5393c7d07e220b84d0706432676956ff9d4bc17768d97f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69014678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e347affc72a211a0fa374a5a4b0cacc9bcdf83c3dedbceb971ea41f82d29eb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm variant v6

```console
$ docker pull docker@sha256:d1287d8bbc43b537b1b3fa5016466a39d1af71aa69221cbf9472350de1f7c8fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64446518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12399d6fd7868964589118cd4e6ada27e1b6d940d4157dbce7750280360fbf9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm variant v7

```console
$ docker pull docker@sha256:87726053d7c6ee7a6973b022c6b755ff92626d9a8714accc186a544e785bb215
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fed20cbea7e22fee5be15f851a1ad9ce75ef61b04f28aa16c78f418f5da8dca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9a56f700a8b852e33e1eb04618d355746c970263a7ed33bfbd5709bda1ab71d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62177304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518e90cb2dafcef0a36a8cedadaacbb1d4c918d9f13b330b228c0816f65fd0ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03`

```console
$ docker pull docker@sha256:f5ea831fc81d7a65d4220f4c90e3be2514d6f85646156ed5ca63ec54abf639d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03` - linux; amd64

```console
$ docker pull docker@sha256:b7736ba0a18b5b9dfe5393c7d07e220b84d0706432676956ff9d4bc17768d97f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69014678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e347affc72a211a0fa374a5a4b0cacc9bcdf83c3dedbceb971ea41f82d29eb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm variant v6

```console
$ docker pull docker@sha256:d1287d8bbc43b537b1b3fa5016466a39d1af71aa69221cbf9472350de1f7c8fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64446518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12399d6fd7868964589118cd4e6ada27e1b6d940d4157dbce7750280360fbf9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm variant v7

```console
$ docker pull docker@sha256:87726053d7c6ee7a6973b022c6b755ff92626d9a8714accc186a544e785bb215
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fed20cbea7e22fee5be15f851a1ad9ce75ef61b04f28aa16c78f418f5da8dca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9a56f700a8b852e33e1eb04618d355746c970263a7ed33bfbd5709bda1ab71d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62177304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518e90cb2dafcef0a36a8cedadaacbb1d4c918d9f13b330b228c0816f65fd0ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.5`

```console
$ docker pull docker@sha256:f5ea831fc81d7a65d4220f4c90e3be2514d6f85646156ed5ca63ec54abf639d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03.5` - linux; amd64

```console
$ docker pull docker@sha256:b7736ba0a18b5b9dfe5393c7d07e220b84d0706432676956ff9d4bc17768d97f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69014678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e347affc72a211a0fa374a5a4b0cacc9bcdf83c3dedbceb971ea41f82d29eb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5` - linux; arm variant v6

```console
$ docker pull docker@sha256:d1287d8bbc43b537b1b3fa5016466a39d1af71aa69221cbf9472350de1f7c8fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64446518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12399d6fd7868964589118cd4e6ada27e1b6d940d4157dbce7750280360fbf9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5` - linux; arm variant v7

```console
$ docker pull docker@sha256:87726053d7c6ee7a6973b022c6b755ff92626d9a8714accc186a544e785bb215
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fed20cbea7e22fee5be15f851a1ad9ce75ef61b04f28aa16c78f418f5da8dca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9a56f700a8b852e33e1eb04618d355746c970263a7ed33bfbd5709bda1ab71d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62177304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518e90cb2dafcef0a36a8cedadaacbb1d4c918d9f13b330b228c0816f65fd0ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.5-dind`

```console
$ docker pull docker@sha256:8f2b876b7410dc1209bec396088e4307d1dba73a75fbe9d66dbd0b6468689488
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03.5-dind` - linux; amd64

```console
$ docker pull docker@sha256:98320e6e491d3c0b7be603066175eaa6e23f3b4dffe3f493e7ccab86b6948a4b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74573729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba63cfbc76778322c00026aa3dd95002fb50da4312955b8a544269b9f8c0a2db`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:877e47979983570e53f851aa8fb41b17e902ef6d6620662eb37d412ecfe62cce
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67580864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf032d26bd6437dcb33784dfb7629082a2cb131aeb30415276d5a849895a533`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:50:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:50:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:50:30 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:50:32 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:50:33 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:50:34 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:50:35 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:50:37 GMT
CMD []
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a76b4f6e4121e7da80c4af4221d6d4c45f58180a2a612775425371f8cd1a05`  
		Last Modified: Wed, 11 Dec 2019 22:51:46 GMT  
		Size: 3.1 MB (3129714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f77cf40d4f1482950df90f7ab94549c4ccf3172e0f4070dee798f4b2747101`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca9067df88c1168f38e515013336c2beb2823499303e55490cc4a09e404eb86`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5dc55ddf941dd0b8d99b9b42f40856d8fd95b0e22b086d2c995cba76f06643`  
		Last Modified: Wed, 11 Dec 2019 22:51:45 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:b4550223e98a4bd2af4328fde6a0605e5642c21d7de1d6f9da1da6d7b2e64729
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66947676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:133f018416e59428748299bc3df1ba87ad4e586baf1a61197151e10d384ef6a8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:11 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:58:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:58:16 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:58:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:58:19 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:58:19 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:58:20 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:58:21 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:58:22 GMT
CMD []
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b110d429435f40b9d9f2541733f6668014dec2c9fa106ddf093f3421b239f065`  
		Last Modified: Wed, 11 Dec 2019 22:59:17 GMT  
		Size: 2.8 MB (2800896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e33e07071ce563e196747d8956056567a5a0aa79f1e038f40fca52ffcdc8c`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a125c9fb6d46759d72990c98b7df96efba4cfabd9578c84b7503b6f19a84b438`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c28f89e09bb9c7ac200b3bae5847571c4f7ab9899076deaabdae6cc3ba310f`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8003ebd5f122dc9d2c6cbd9039e69d0d13b602e904fda320641dbc7c5f87661f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67759986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08132b3cbd5d257416b6f79cc8a12f20d85cb41a4d40f097454b5e7fbbea6c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:07 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:40:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:40:12 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:40:17 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:40:22 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:40:23 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:40:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:40:33 GMT
CMD []
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b1c5f65ee755dd97182c2641d94eb393fc0496adf7f1b4bf78bf5b50944e1c`  
		Last Modified: Wed, 11 Dec 2019 23:41:44 GMT  
		Size: 5.6 MB (5578054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b8444b828db4cd92dfcaa796e6a15d1fc3377b030024a8b87c1087429c0762`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dd84dc8fd332bb6571553ec1bf4c65377a8924e867bf51c7f6ddfc4daa3efa`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee095995d2a1c5fe6eaf5e8ceaf7ae5a4ef428406c8e3f4b42a12b06af1db2`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.5-dind-rootless`

```console
$ docker pull docker@sha256:67383a2ae35bd7334ede473e4f7f2563342fc78dbfbf50d0787fb5f518603b74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03.5-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:7ccba991abe7af742b95bb74d9358fa2d329fcd03355867e0c325ebf9bac763d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96804016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c85bf7f5b44cdd293a12b5ad71cc24a083e7553d8adbe27efbbea38a3d79cd52`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
# Wed, 11 Dec 2019 23:21:12 GMT
RUN apk add --no-cache iproute2
# Wed, 11 Dec 2019 23:21:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 Dec 2019 23:21:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:15 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 20 Dec 2019 01:29:24 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 20 Dec 2019 01:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 20 Dec 2019 01:29:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 20 Dec 2019 01:29:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 20 Dec 2019 01:29:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10b23adfdb7b416b5b7eeca1659094e1aabebef346b33f16b26c547d52b5883`  
		Last Modified: Wed, 11 Dec 2019 23:22:21 GMT  
		Size: 782.2 KB (782240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4493bdb21cc998a479ae1f20098f52af6e955a07fff8b1b537bc2a5ebf34939e`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1dd53a02457cef93d7ea523326898d54554a0b24ac1ea9783b858e6168ebd2`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cfa48d52eb16b37a00fcf447455ed9bbb90d4efbb15930ce31bbd224e907e`  
		Last Modified: Wed, 11 Dec 2019 23:22:22 GMT  
		Size: 9.1 MB (9109470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bfbe5a8c5124939208a5805ea253058b2b92a1857b1fd3d5266d1d0990da97`  
		Last Modified: Fri, 20 Dec 2019 01:30:02 GMT  
		Size: 12.3 MB (12336935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c1cc8d056e3bf1d3b3badafd7fce2cf1884ae118484bf3cb52281d725c563c`  
		Last Modified: Fri, 20 Dec 2019 01:30:00 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03.5-git`

```console
$ docker pull docker@sha256:3141a9f66a8eaa90e74a0fbf999ab40e7cf3eb2890577ea17e688ead7e020641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03.5-git` - linux; amd64

```console
$ docker pull docker@sha256:e470d67889af90ea7d5008faaba9f8c6bc43de06304dab2b8b2fdd492eae39d3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76865996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6fefe517a89d818bcbdf3465b0bf9657cc4b3bc72f3cb9bc098ff9169ace33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:36 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fedb39903367c1422036ce9ec4d702341b70ad82cc01b6e76bffdc2642b1395`  
		Last Modified: Wed, 11 Dec 2019 23:22:36 GMT  
		Size: 7.9 MB (7851318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d109033468e4c2d3916676f30f34833313dc39a469c23b24dda9845a940b73af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71863615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1158e8b1b186b886304088df5c4a3e6dd590a351875f2051f206250d4e8ffe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:52 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0700c76dc28a7b907870ceaa7e72e7f65265a74a0582be0cfd5713b288d6fdb`  
		Last Modified: Wed, 11 Dec 2019 22:52:01 GMT  
		Size: 7.4 MB (7417097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:81fefdf9037cb7a9b65fc7e76bc4fd79fc3fb2011172b0a47ab4154698bb478a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70735384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84c951058f8f3b2ad0e89f4efb78fe2d0f7458ceb918af47a93fcde708e716c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b770b6bdd361810ea324b9adf28a24ebcbf0bb0520d3b6a4ee53e496bb1ad4`  
		Last Modified: Wed, 11 Dec 2019 22:59:30 GMT  
		Size: 6.6 MB (6593235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03.5-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8854ae5a4e1458fb0154a525ccc0893a13b9656d54ab27f2d582910a30dcaaf9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70263541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7f16c5d45e9719de4c144047b6384e359e4112fa93e439f12a8a82692e09a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:49 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06784639818de54df259278e50245d457fa0bf61002da027f39d8126a8956475`  
		Last Modified: Wed, 11 Dec 2019 23:41:58 GMT  
		Size: 8.1 MB (8086237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-dind`

```console
$ docker pull docker@sha256:8f2b876b7410dc1209bec396088e4307d1dba73a75fbe9d66dbd0b6468689488
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-dind` - linux; amd64

```console
$ docker pull docker@sha256:98320e6e491d3c0b7be603066175eaa6e23f3b4dffe3f493e7ccab86b6948a4b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74573729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba63cfbc76778322c00026aa3dd95002fb50da4312955b8a544269b9f8c0a2db`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:877e47979983570e53f851aa8fb41b17e902ef6d6620662eb37d412ecfe62cce
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67580864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf032d26bd6437dcb33784dfb7629082a2cb131aeb30415276d5a849895a533`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:50:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:50:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:50:30 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:50:32 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:50:33 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:50:34 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:50:35 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:50:37 GMT
CMD []
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a76b4f6e4121e7da80c4af4221d6d4c45f58180a2a612775425371f8cd1a05`  
		Last Modified: Wed, 11 Dec 2019 22:51:46 GMT  
		Size: 3.1 MB (3129714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f77cf40d4f1482950df90f7ab94549c4ccf3172e0f4070dee798f4b2747101`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca9067df88c1168f38e515013336c2beb2823499303e55490cc4a09e404eb86`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5dc55ddf941dd0b8d99b9b42f40856d8fd95b0e22b086d2c995cba76f06643`  
		Last Modified: Wed, 11 Dec 2019 22:51:45 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:b4550223e98a4bd2af4328fde6a0605e5642c21d7de1d6f9da1da6d7b2e64729
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66947676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:133f018416e59428748299bc3df1ba87ad4e586baf1a61197151e10d384ef6a8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:11 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:58:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:58:16 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:58:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:58:19 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:58:19 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:58:20 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:58:21 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:58:22 GMT
CMD []
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b110d429435f40b9d9f2541733f6668014dec2c9fa106ddf093f3421b239f065`  
		Last Modified: Wed, 11 Dec 2019 22:59:17 GMT  
		Size: 2.8 MB (2800896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e33e07071ce563e196747d8956056567a5a0aa79f1e038f40fca52ffcdc8c`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a125c9fb6d46759d72990c98b7df96efba4cfabd9578c84b7503b6f19a84b438`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c28f89e09bb9c7ac200b3bae5847571c4f7ab9899076deaabdae6cc3ba310f`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8003ebd5f122dc9d2c6cbd9039e69d0d13b602e904fda320641dbc7c5f87661f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67759986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08132b3cbd5d257416b6f79cc8a12f20d85cb41a4d40f097454b5e7fbbea6c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:07 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:40:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:40:12 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:40:17 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:40:22 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:40:23 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:40:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:40:33 GMT
CMD []
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b1c5f65ee755dd97182c2641d94eb393fc0496adf7f1b4bf78bf5b50944e1c`  
		Last Modified: Wed, 11 Dec 2019 23:41:44 GMT  
		Size: 5.6 MB (5578054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b8444b828db4cd92dfcaa796e6a15d1fc3377b030024a8b87c1087429c0762`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dd84dc8fd332bb6571553ec1bf4c65377a8924e867bf51c7f6ddfc4daa3efa`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee095995d2a1c5fe6eaf5e8ceaf7ae5a4ef428406c8e3f4b42a12b06af1db2`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-dind-rootless`

```console
$ docker pull docker@sha256:67383a2ae35bd7334ede473e4f7f2563342fc78dbfbf50d0787fb5f518603b74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19.03-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:7ccba991abe7af742b95bb74d9358fa2d329fcd03355867e0c325ebf9bac763d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96804016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c85bf7f5b44cdd293a12b5ad71cc24a083e7553d8adbe27efbbea38a3d79cd52`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
# Wed, 11 Dec 2019 23:21:12 GMT
RUN apk add --no-cache iproute2
# Wed, 11 Dec 2019 23:21:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 Dec 2019 23:21:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:15 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 20 Dec 2019 01:29:24 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 20 Dec 2019 01:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 20 Dec 2019 01:29:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 20 Dec 2019 01:29:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 20 Dec 2019 01:29:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10b23adfdb7b416b5b7eeca1659094e1aabebef346b33f16b26c547d52b5883`  
		Last Modified: Wed, 11 Dec 2019 23:22:21 GMT  
		Size: 782.2 KB (782240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4493bdb21cc998a479ae1f20098f52af6e955a07fff8b1b537bc2a5ebf34939e`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1dd53a02457cef93d7ea523326898d54554a0b24ac1ea9783b858e6168ebd2`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cfa48d52eb16b37a00fcf447455ed9bbb90d4efbb15930ce31bbd224e907e`  
		Last Modified: Wed, 11 Dec 2019 23:22:22 GMT  
		Size: 9.1 MB (9109470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bfbe5a8c5124939208a5805ea253058b2b92a1857b1fd3d5266d1d0990da97`  
		Last Modified: Fri, 20 Dec 2019 01:30:02 GMT  
		Size: 12.3 MB (12336935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c1cc8d056e3bf1d3b3badafd7fce2cf1884ae118484bf3cb52281d725c563c`  
		Last Modified: Fri, 20 Dec 2019 01:30:00 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19.03-git`

```console
$ docker pull docker@sha256:3141a9f66a8eaa90e74a0fbf999ab40e7cf3eb2890577ea17e688ead7e020641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19.03-git` - linux; amd64

```console
$ docker pull docker@sha256:e470d67889af90ea7d5008faaba9f8c6bc43de06304dab2b8b2fdd492eae39d3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76865996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6fefe517a89d818bcbdf3465b0bf9657cc4b3bc72f3cb9bc098ff9169ace33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:36 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fedb39903367c1422036ce9ec4d702341b70ad82cc01b6e76bffdc2642b1395`  
		Last Modified: Wed, 11 Dec 2019 23:22:36 GMT  
		Size: 7.9 MB (7851318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d109033468e4c2d3916676f30f34833313dc39a469c23b24dda9845a940b73af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71863615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1158e8b1b186b886304088df5c4a3e6dd590a351875f2051f206250d4e8ffe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:52 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0700c76dc28a7b907870ceaa7e72e7f65265a74a0582be0cfd5713b288d6fdb`  
		Last Modified: Wed, 11 Dec 2019 22:52:01 GMT  
		Size: 7.4 MB (7417097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:81fefdf9037cb7a9b65fc7e76bc4fd79fc3fb2011172b0a47ab4154698bb478a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70735384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84c951058f8f3b2ad0e89f4efb78fe2d0f7458ceb918af47a93fcde708e716c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b770b6bdd361810ea324b9adf28a24ebcbf0bb0520d3b6a4ee53e496bb1ad4`  
		Last Modified: Wed, 11 Dec 2019 22:59:30 GMT  
		Size: 6.6 MB (6593235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19.03-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8854ae5a4e1458fb0154a525ccc0893a13b9656d54ab27f2d582910a30dcaaf9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70263541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7f16c5d45e9719de4c144047b6384e359e4112fa93e439f12a8a82692e09a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:49 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06784639818de54df259278e50245d457fa0bf61002da027f39d8126a8956475`  
		Last Modified: Wed, 11 Dec 2019 23:41:58 GMT  
		Size: 8.1 MB (8086237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind`

```console
$ docker pull docker@sha256:8f2b876b7410dc1209bec396088e4307d1dba73a75fbe9d66dbd0b6468689488
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-dind` - linux; amd64

```console
$ docker pull docker@sha256:98320e6e491d3c0b7be603066175eaa6e23f3b4dffe3f493e7ccab86b6948a4b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74573729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba63cfbc76778322c00026aa3dd95002fb50da4312955b8a544269b9f8c0a2db`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:877e47979983570e53f851aa8fb41b17e902ef6d6620662eb37d412ecfe62cce
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67580864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf032d26bd6437dcb33784dfb7629082a2cb131aeb30415276d5a849895a533`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:50:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:50:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:50:30 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:50:32 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:50:33 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:50:34 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:50:35 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:50:37 GMT
CMD []
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a76b4f6e4121e7da80c4af4221d6d4c45f58180a2a612775425371f8cd1a05`  
		Last Modified: Wed, 11 Dec 2019 22:51:46 GMT  
		Size: 3.1 MB (3129714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f77cf40d4f1482950df90f7ab94549c4ccf3172e0f4070dee798f4b2747101`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca9067df88c1168f38e515013336c2beb2823499303e55490cc4a09e404eb86`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5dc55ddf941dd0b8d99b9b42f40856d8fd95b0e22b086d2c995cba76f06643`  
		Last Modified: Wed, 11 Dec 2019 22:51:45 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:b4550223e98a4bd2af4328fde6a0605e5642c21d7de1d6f9da1da6d7b2e64729
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66947676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:133f018416e59428748299bc3df1ba87ad4e586baf1a61197151e10d384ef6a8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:11 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:58:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:58:16 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:58:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:58:19 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:58:19 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:58:20 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:58:21 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:58:22 GMT
CMD []
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b110d429435f40b9d9f2541733f6668014dec2c9fa106ddf093f3421b239f065`  
		Last Modified: Wed, 11 Dec 2019 22:59:17 GMT  
		Size: 2.8 MB (2800896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e33e07071ce563e196747d8956056567a5a0aa79f1e038f40fca52ffcdc8c`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a125c9fb6d46759d72990c98b7df96efba4cfabd9578c84b7503b6f19a84b438`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c28f89e09bb9c7ac200b3bae5847571c4f7ab9899076deaabdae6cc3ba310f`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8003ebd5f122dc9d2c6cbd9039e69d0d13b602e904fda320641dbc7c5f87661f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67759986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08132b3cbd5d257416b6f79cc8a12f20d85cb41a4d40f097454b5e7fbbea6c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:07 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:40:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:40:12 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:40:17 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:40:22 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:40:23 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:40:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:40:33 GMT
CMD []
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b1c5f65ee755dd97182c2641d94eb393fc0496adf7f1b4bf78bf5b50944e1c`  
		Last Modified: Wed, 11 Dec 2019 23:41:44 GMT  
		Size: 5.6 MB (5578054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b8444b828db4cd92dfcaa796e6a15d1fc3377b030024a8b87c1087429c0762`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dd84dc8fd332bb6571553ec1bf4c65377a8924e867bf51c7f6ddfc4daa3efa`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee095995d2a1c5fe6eaf5e8ceaf7ae5a4ef428406c8e3f4b42a12b06af1db2`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-dind-rootless`

```console
$ docker pull docker@sha256:67383a2ae35bd7334ede473e4f7f2563342fc78dbfbf50d0787fb5f518603b74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:19-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:7ccba991abe7af742b95bb74d9358fa2d329fcd03355867e0c325ebf9bac763d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96804016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c85bf7f5b44cdd293a12b5ad71cc24a083e7553d8adbe27efbbea38a3d79cd52`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
# Wed, 11 Dec 2019 23:21:12 GMT
RUN apk add --no-cache iproute2
# Wed, 11 Dec 2019 23:21:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 Dec 2019 23:21:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:15 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 20 Dec 2019 01:29:24 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 20 Dec 2019 01:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 20 Dec 2019 01:29:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 20 Dec 2019 01:29:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 20 Dec 2019 01:29:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10b23adfdb7b416b5b7eeca1659094e1aabebef346b33f16b26c547d52b5883`  
		Last Modified: Wed, 11 Dec 2019 23:22:21 GMT  
		Size: 782.2 KB (782240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4493bdb21cc998a479ae1f20098f52af6e955a07fff8b1b537bc2a5ebf34939e`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1dd53a02457cef93d7ea523326898d54554a0b24ac1ea9783b858e6168ebd2`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cfa48d52eb16b37a00fcf447455ed9bbb90d4efbb15930ce31bbd224e907e`  
		Last Modified: Wed, 11 Dec 2019 23:22:22 GMT  
		Size: 9.1 MB (9109470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bfbe5a8c5124939208a5805ea253058b2b92a1857b1fd3d5266d1d0990da97`  
		Last Modified: Fri, 20 Dec 2019 01:30:02 GMT  
		Size: 12.3 MB (12336935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c1cc8d056e3bf1d3b3badafd7fce2cf1884ae118484bf3cb52281d725c563c`  
		Last Modified: Fri, 20 Dec 2019 01:30:00 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:19-git`

```console
$ docker pull docker@sha256:3141a9f66a8eaa90e74a0fbf999ab40e7cf3eb2890577ea17e688ead7e020641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:19-git` - linux; amd64

```console
$ docker pull docker@sha256:e470d67889af90ea7d5008faaba9f8c6bc43de06304dab2b8b2fdd492eae39d3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76865996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6fefe517a89d818bcbdf3465b0bf9657cc4b3bc72f3cb9bc098ff9169ace33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:36 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fedb39903367c1422036ce9ec4d702341b70ad82cc01b6e76bffdc2642b1395`  
		Last Modified: Wed, 11 Dec 2019 23:22:36 GMT  
		Size: 7.9 MB (7851318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d109033468e4c2d3916676f30f34833313dc39a469c23b24dda9845a940b73af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71863615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1158e8b1b186b886304088df5c4a3e6dd590a351875f2051f206250d4e8ffe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:52 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0700c76dc28a7b907870ceaa7e72e7f65265a74a0582be0cfd5713b288d6fdb`  
		Last Modified: Wed, 11 Dec 2019 22:52:01 GMT  
		Size: 7.4 MB (7417097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:81fefdf9037cb7a9b65fc7e76bc4fd79fc3fb2011172b0a47ab4154698bb478a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70735384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84c951058f8f3b2ad0e89f4efb78fe2d0f7458ceb918af47a93fcde708e716c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b770b6bdd361810ea324b9adf28a24ebcbf0bb0520d3b6a4ee53e496bb1ad4`  
		Last Modified: Wed, 11 Dec 2019 22:59:30 GMT  
		Size: 6.6 MB (6593235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:19-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8854ae5a4e1458fb0154a525ccc0893a13b9656d54ab27f2d582910a30dcaaf9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70263541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7f16c5d45e9719de4c144047b6384e359e4112fa93e439f12a8a82692e09a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:49 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06784639818de54df259278e50245d457fa0bf61002da027f39d8126a8956475`  
		Last Modified: Wed, 11 Dec 2019 23:41:58 GMT  
		Size: 8.1 MB (8086237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:8f2b876b7410dc1209bec396088e4307d1dba73a75fbe9d66dbd0b6468689488
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:98320e6e491d3c0b7be603066175eaa6e23f3b4dffe3f493e7ccab86b6948a4b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74573729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba63cfbc76778322c00026aa3dd95002fb50da4312955b8a544269b9f8c0a2db`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:877e47979983570e53f851aa8fb41b17e902ef6d6620662eb37d412ecfe62cce
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67580864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf032d26bd6437dcb33784dfb7629082a2cb131aeb30415276d5a849895a533`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:50:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:50:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:50:30 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:50:32 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:50:33 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:50:34 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:50:35 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:50:37 GMT
CMD []
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a76b4f6e4121e7da80c4af4221d6d4c45f58180a2a612775425371f8cd1a05`  
		Last Modified: Wed, 11 Dec 2019 22:51:46 GMT  
		Size: 3.1 MB (3129714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f77cf40d4f1482950df90f7ab94549c4ccf3172e0f4070dee798f4b2747101`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca9067df88c1168f38e515013336c2beb2823499303e55490cc4a09e404eb86`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5dc55ddf941dd0b8d99b9b42f40856d8fd95b0e22b086d2c995cba76f06643`  
		Last Modified: Wed, 11 Dec 2019 22:51:45 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:b4550223e98a4bd2af4328fde6a0605e5642c21d7de1d6f9da1da6d7b2e64729
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66947676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:133f018416e59428748299bc3df1ba87ad4e586baf1a61197151e10d384ef6a8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:11 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:58:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:58:16 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:58:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:58:19 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:58:19 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:58:20 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:58:21 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:58:22 GMT
CMD []
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b110d429435f40b9d9f2541733f6668014dec2c9fa106ddf093f3421b239f065`  
		Last Modified: Wed, 11 Dec 2019 22:59:17 GMT  
		Size: 2.8 MB (2800896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e33e07071ce563e196747d8956056567a5a0aa79f1e038f40fca52ffcdc8c`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a125c9fb6d46759d72990c98b7df96efba4cfabd9578c84b7503b6f19a84b438`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c28f89e09bb9c7ac200b3bae5847571c4f7ab9899076deaabdae6cc3ba310f`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8003ebd5f122dc9d2c6cbd9039e69d0d13b602e904fda320641dbc7c5f87661f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67759986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08132b3cbd5d257416b6f79cc8a12f20d85cb41a4d40f097454b5e7fbbea6c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:07 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:40:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:40:12 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:40:17 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:40:22 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:40:23 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:40:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:40:33 GMT
CMD []
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b1c5f65ee755dd97182c2641d94eb393fc0496adf7f1b4bf78bf5b50944e1c`  
		Last Modified: Wed, 11 Dec 2019 23:41:44 GMT  
		Size: 5.6 MB (5578054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b8444b828db4cd92dfcaa796e6a15d1fc3377b030024a8b87c1087429c0762`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dd84dc8fd332bb6571553ec1bf4c65377a8924e867bf51c7f6ddfc4daa3efa`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee095995d2a1c5fe6eaf5e8ceaf7ae5a4ef428406c8e3f4b42a12b06af1db2`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:67383a2ae35bd7334ede473e4f7f2563342fc78dbfbf50d0787fb5f518603b74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:7ccba991abe7af742b95bb74d9358fa2d329fcd03355867e0c325ebf9bac763d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96804016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c85bf7f5b44cdd293a12b5ad71cc24a083e7553d8adbe27efbbea38a3d79cd52`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
# Wed, 11 Dec 2019 23:21:12 GMT
RUN apk add --no-cache iproute2
# Wed, 11 Dec 2019 23:21:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 Dec 2019 23:21:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:15 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 20 Dec 2019 01:29:24 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 20 Dec 2019 01:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 20 Dec 2019 01:29:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 20 Dec 2019 01:29:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 20 Dec 2019 01:29:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10b23adfdb7b416b5b7eeca1659094e1aabebef346b33f16b26c547d52b5883`  
		Last Modified: Wed, 11 Dec 2019 23:22:21 GMT  
		Size: 782.2 KB (782240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4493bdb21cc998a479ae1f20098f52af6e955a07fff8b1b537bc2a5ebf34939e`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1dd53a02457cef93d7ea523326898d54554a0b24ac1ea9783b858e6168ebd2`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cfa48d52eb16b37a00fcf447455ed9bbb90d4efbb15930ce31bbd224e907e`  
		Last Modified: Wed, 11 Dec 2019 23:22:22 GMT  
		Size: 9.1 MB (9109470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bfbe5a8c5124939208a5805ea253058b2b92a1857b1fd3d5266d1d0990da97`  
		Last Modified: Fri, 20 Dec 2019 01:30:02 GMT  
		Size: 12.3 MB (12336935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c1cc8d056e3bf1d3b3badafd7fce2cf1884ae118484bf3cb52281d725c563c`  
		Last Modified: Fri, 20 Dec 2019 01:30:00 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:3141a9f66a8eaa90e74a0fbf999ab40e7cf3eb2890577ea17e688ead7e020641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:e470d67889af90ea7d5008faaba9f8c6bc43de06304dab2b8b2fdd492eae39d3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76865996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6fefe517a89d818bcbdf3465b0bf9657cc4b3bc72f3cb9bc098ff9169ace33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:36 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fedb39903367c1422036ce9ec4d702341b70ad82cc01b6e76bffdc2642b1395`  
		Last Modified: Wed, 11 Dec 2019 23:22:36 GMT  
		Size: 7.9 MB (7851318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d109033468e4c2d3916676f30f34833313dc39a469c23b24dda9845a940b73af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71863615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1158e8b1b186b886304088df5c4a3e6dd590a351875f2051f206250d4e8ffe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:52 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0700c76dc28a7b907870ceaa7e72e7f65265a74a0582be0cfd5713b288d6fdb`  
		Last Modified: Wed, 11 Dec 2019 22:52:01 GMT  
		Size: 7.4 MB (7417097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm variant v7

```console
$ docker pull docker@sha256:81fefdf9037cb7a9b65fc7e76bc4fd79fc3fb2011172b0a47ab4154698bb478a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70735384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84c951058f8f3b2ad0e89f4efb78fe2d0f7458ceb918af47a93fcde708e716c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b770b6bdd361810ea324b9adf28a24ebcbf0bb0520d3b6a4ee53e496bb1ad4`  
		Last Modified: Wed, 11 Dec 2019 22:59:30 GMT  
		Size: 6.6 MB (6593235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8854ae5a4e1458fb0154a525ccc0893a13b9656d54ab27f2d582910a30dcaaf9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70263541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7f16c5d45e9719de4c144047b6384e359e4112fa93e439f12a8a82692e09a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:49 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06784639818de54df259278e50245d457fa0bf61002da027f39d8126a8956475`  
		Last Modified: Wed, 11 Dec 2019 23:41:58 GMT  
		Size: 8.1 MB (8086237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:f5ea831fc81d7a65d4220f4c90e3be2514d6f85646156ed5ca63ec54abf639d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:b7736ba0a18b5b9dfe5393c7d07e220b84d0706432676956ff9d4bc17768d97f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69014678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e347affc72a211a0fa374a5a4b0cacc9bcdf83c3dedbceb971ea41f82d29eb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm variant v6

```console
$ docker pull docker@sha256:d1287d8bbc43b537b1b3fa5016466a39d1af71aa69221cbf9472350de1f7c8fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64446518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12399d6fd7868964589118cd4e6ada27e1b6d940d4157dbce7750280360fbf9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm variant v7

```console
$ docker pull docker@sha256:87726053d7c6ee7a6973b022c6b755ff92626d9a8714accc186a544e785bb215
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fed20cbea7e22fee5be15f851a1ad9ce75ef61b04f28aa16c78f418f5da8dca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9a56f700a8b852e33e1eb04618d355746c970263a7ed33bfbd5709bda1ab71d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62177304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518e90cb2dafcef0a36a8cedadaacbb1d4c918d9f13b330b228c0816f65fd0ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable`

```console
$ docker pull docker@sha256:f5ea831fc81d7a65d4220f4c90e3be2514d6f85646156ed5ca63ec54abf639d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:stable` - linux; amd64

```console
$ docker pull docker@sha256:b7736ba0a18b5b9dfe5393c7d07e220b84d0706432676956ff9d4bc17768d97f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69014678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e347affc72a211a0fa374a5a4b0cacc9bcdf83c3dedbceb971ea41f82d29eb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable` - linux; arm variant v6

```console
$ docker pull docker@sha256:d1287d8bbc43b537b1b3fa5016466a39d1af71aa69221cbf9472350de1f7c8fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64446518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12399d6fd7868964589118cd4e6ada27e1b6d940d4157dbce7750280360fbf9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable` - linux; arm variant v7

```console
$ docker pull docker@sha256:87726053d7c6ee7a6973b022c6b755ff92626d9a8714accc186a544e785bb215
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fed20cbea7e22fee5be15f851a1ad9ce75ef61b04f28aa16c78f418f5da8dca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9a56f700a8b852e33e1eb04618d355746c970263a7ed33bfbd5709bda1ab71d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62177304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518e90cb2dafcef0a36a8cedadaacbb1d4c918d9f13b330b228c0816f65fd0ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable-dind`

```console
$ docker pull docker@sha256:8f2b876b7410dc1209bec396088e4307d1dba73a75fbe9d66dbd0b6468689488
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:stable-dind` - linux; amd64

```console
$ docker pull docker@sha256:98320e6e491d3c0b7be603066175eaa6e23f3b4dffe3f493e7ccab86b6948a4b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74573729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba63cfbc76778322c00026aa3dd95002fb50da4312955b8a544269b9f8c0a2db`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:877e47979983570e53f851aa8fb41b17e902ef6d6620662eb37d412ecfe62cce
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67580864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf032d26bd6437dcb33784dfb7629082a2cb131aeb30415276d5a849895a533`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:50:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:50:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:50:30 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:50:32 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:50:33 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:50:34 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:50:35 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:50:37 GMT
CMD []
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a76b4f6e4121e7da80c4af4221d6d4c45f58180a2a612775425371f8cd1a05`  
		Last Modified: Wed, 11 Dec 2019 22:51:46 GMT  
		Size: 3.1 MB (3129714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f77cf40d4f1482950df90f7ab94549c4ccf3172e0f4070dee798f4b2747101`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca9067df88c1168f38e515013336c2beb2823499303e55490cc4a09e404eb86`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5dc55ddf941dd0b8d99b9b42f40856d8fd95b0e22b086d2c995cba76f06643`  
		Last Modified: Wed, 11 Dec 2019 22:51:45 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:b4550223e98a4bd2af4328fde6a0605e5642c21d7de1d6f9da1da6d7b2e64729
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66947676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:133f018416e59428748299bc3df1ba87ad4e586baf1a61197151e10d384ef6a8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:11 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:58:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:58:16 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:58:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:58:19 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:58:19 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:58:20 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:58:21 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:58:22 GMT
CMD []
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b110d429435f40b9d9f2541733f6668014dec2c9fa106ddf093f3421b239f065`  
		Last Modified: Wed, 11 Dec 2019 22:59:17 GMT  
		Size: 2.8 MB (2800896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e33e07071ce563e196747d8956056567a5a0aa79f1e038f40fca52ffcdc8c`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a125c9fb6d46759d72990c98b7df96efba4cfabd9578c84b7503b6f19a84b438`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c28f89e09bb9c7ac200b3bae5847571c4f7ab9899076deaabdae6cc3ba310f`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8003ebd5f122dc9d2c6cbd9039e69d0d13b602e904fda320641dbc7c5f87661f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67759986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08132b3cbd5d257416b6f79cc8a12f20d85cb41a4d40f097454b5e7fbbea6c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:07 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:40:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:40:12 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:40:17 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:40:22 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:40:23 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:40:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:40:33 GMT
CMD []
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b1c5f65ee755dd97182c2641d94eb393fc0496adf7f1b4bf78bf5b50944e1c`  
		Last Modified: Wed, 11 Dec 2019 23:41:44 GMT  
		Size: 5.6 MB (5578054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b8444b828db4cd92dfcaa796e6a15d1fc3377b030024a8b87c1087429c0762`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dd84dc8fd332bb6571553ec1bf4c65377a8924e867bf51c7f6ddfc4daa3efa`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee095995d2a1c5fe6eaf5e8ceaf7ae5a4ef428406c8e3f4b42a12b06af1db2`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable-dind-rootless`

```console
$ docker pull docker@sha256:67383a2ae35bd7334ede473e4f7f2563342fc78dbfbf50d0787fb5f518603b74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:stable-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:7ccba991abe7af742b95bb74d9358fa2d329fcd03355867e0c325ebf9bac763d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96804016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c85bf7f5b44cdd293a12b5ad71cc24a083e7553d8adbe27efbbea38a3d79cd52`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
# Wed, 11 Dec 2019 23:21:12 GMT
RUN apk add --no-cache iproute2
# Wed, 11 Dec 2019 23:21:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 Dec 2019 23:21:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:15 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 20 Dec 2019 01:29:24 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 20 Dec 2019 01:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 20 Dec 2019 01:29:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 20 Dec 2019 01:29:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 20 Dec 2019 01:29:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10b23adfdb7b416b5b7eeca1659094e1aabebef346b33f16b26c547d52b5883`  
		Last Modified: Wed, 11 Dec 2019 23:22:21 GMT  
		Size: 782.2 KB (782240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4493bdb21cc998a479ae1f20098f52af6e955a07fff8b1b537bc2a5ebf34939e`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1dd53a02457cef93d7ea523326898d54554a0b24ac1ea9783b858e6168ebd2`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cfa48d52eb16b37a00fcf447455ed9bbb90d4efbb15930ce31bbd224e907e`  
		Last Modified: Wed, 11 Dec 2019 23:22:22 GMT  
		Size: 9.1 MB (9109470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bfbe5a8c5124939208a5805ea253058b2b92a1857b1fd3d5266d1d0990da97`  
		Last Modified: Fri, 20 Dec 2019 01:30:02 GMT  
		Size: 12.3 MB (12336935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c1cc8d056e3bf1d3b3badafd7fce2cf1884ae118484bf3cb52281d725c563c`  
		Last Modified: Fri, 20 Dec 2019 01:30:00 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:stable-git`

```console
$ docker pull docker@sha256:3141a9f66a8eaa90e74a0fbf999ab40e7cf3eb2890577ea17e688ead7e020641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:stable-git` - linux; amd64

```console
$ docker pull docker@sha256:e470d67889af90ea7d5008faaba9f8c6bc43de06304dab2b8b2fdd492eae39d3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76865996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6fefe517a89d818bcbdf3465b0bf9657cc4b3bc72f3cb9bc098ff9169ace33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:36 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fedb39903367c1422036ce9ec4d702341b70ad82cc01b6e76bffdc2642b1395`  
		Last Modified: Wed, 11 Dec 2019 23:22:36 GMT  
		Size: 7.9 MB (7851318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d109033468e4c2d3916676f30f34833313dc39a469c23b24dda9845a940b73af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71863615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1158e8b1b186b886304088df5c4a3e6dd590a351875f2051f206250d4e8ffe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:52 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0700c76dc28a7b907870ceaa7e72e7f65265a74a0582be0cfd5713b288d6fdb`  
		Last Modified: Wed, 11 Dec 2019 22:52:01 GMT  
		Size: 7.4 MB (7417097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:81fefdf9037cb7a9b65fc7e76bc4fd79fc3fb2011172b0a47ab4154698bb478a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70735384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84c951058f8f3b2ad0e89f4efb78fe2d0f7458ceb918af47a93fcde708e716c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b770b6bdd361810ea324b9adf28a24ebcbf0bb0520d3b6a4ee53e496bb1ad4`  
		Last Modified: Wed, 11 Dec 2019 22:59:30 GMT  
		Size: 6.6 MB (6593235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:stable-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8854ae5a4e1458fb0154a525ccc0893a13b9656d54ab27f2d582910a30dcaaf9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70263541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7f16c5d45e9719de4c144047b6384e359e4112fa93e439f12a8a82692e09a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:49 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06784639818de54df259278e50245d457fa0bf61002da027f39d8126a8956475`  
		Last Modified: Wed, 11 Dec 2019 23:41:58 GMT  
		Size: 8.1 MB (8086237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test`

```console
$ docker pull docker@sha256:f5ea831fc81d7a65d4220f4c90e3be2514d6f85646156ed5ca63ec54abf639d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test` - linux; amd64

```console
$ docker pull docker@sha256:b7736ba0a18b5b9dfe5393c7d07e220b84d0706432676956ff9d4bc17768d97f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69014678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e347affc72a211a0fa374a5a4b0cacc9bcdf83c3dedbceb971ea41f82d29eb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm variant v6

```console
$ docker pull docker@sha256:d1287d8bbc43b537b1b3fa5016466a39d1af71aa69221cbf9472350de1f7c8fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64446518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12399d6fd7868964589118cd4e6ada27e1b6d940d4157dbce7750280360fbf9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm variant v7

```console
$ docker pull docker@sha256:87726053d7c6ee7a6973b022c6b755ff92626d9a8714accc186a544e785bb215
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.1 MB (64142149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fed20cbea7e22fee5be15f851a1ad9ce75ef61b04f28aa16c78f418f5da8dca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:9a56f700a8b852e33e1eb04618d355746c970263a7ed33bfbd5709bda1ab71d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62177304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518e90cb2dafcef0a36a8cedadaacbb1d4c918d9f13b330b228c0816f65fd0ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-dind`

```console
$ docker pull docker@sha256:8f2b876b7410dc1209bec396088e4307d1dba73a75fbe9d66dbd0b6468689488
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test-dind` - linux; amd64

```console
$ docker pull docker@sha256:98320e6e491d3c0b7be603066175eaa6e23f3b4dffe3f493e7ccab86b6948a4b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.6 MB (74573729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba63cfbc76778322c00026aa3dd95002fb50da4312955b8a544269b9f8c0a2db`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:877e47979983570e53f851aa8fb41b17e902ef6d6620662eb37d412ecfe62cce
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67580864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf032d26bd6437dcb33784dfb7629082a2cb131aeb30415276d5a849895a533`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:10 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:50:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:50:22 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:50:30 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:50:32 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:50:33 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:50:34 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:50:35 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:50:37 GMT
CMD []
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a76b4f6e4121e7da80c4af4221d6d4c45f58180a2a612775425371f8cd1a05`  
		Last Modified: Wed, 11 Dec 2019 22:51:46 GMT  
		Size: 3.1 MB (3129714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f77cf40d4f1482950df90f7ab94549c4ccf3172e0f4070dee798f4b2747101`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca9067df88c1168f38e515013336c2beb2823499303e55490cc4a09e404eb86`  
		Last Modified: Wed, 11 Dec 2019 22:51:44 GMT  
		Size: 758.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5dc55ddf941dd0b8d99b9b42f40856d8fd95b0e22b086d2c995cba76f06643`  
		Last Modified: Wed, 11 Dec 2019 22:51:45 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:b4550223e98a4bd2af4328fde6a0605e5642c21d7de1d6f9da1da6d7b2e64729
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66947676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:133f018416e59428748299bc3df1ba87ad4e586baf1a61197151e10d384ef6a8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:11 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 22:58:16 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 22:58:16 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 22:58:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 22:58:19 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:58:19 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 22:58:20 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 22:58:21 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 22:58:22 GMT
CMD []
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b110d429435f40b9d9f2541733f6668014dec2c9fa106ddf093f3421b239f065`  
		Last Modified: Wed, 11 Dec 2019 22:59:17 GMT  
		Size: 2.8 MB (2800896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1e33e07071ce563e196747d8956056567a5a0aa79f1e038f40fca52ffcdc8c`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 1.3 KB (1339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a125c9fb6d46759d72990c98b7df96efba4cfabd9578c84b7503b6f19a84b438`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 755.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c28f89e09bb9c7ac200b3bae5847571c4f7ab9899076deaabdae6cc3ba310f`  
		Last Modified: Wed, 11 Dec 2019 22:59:16 GMT  
		Size: 2.5 KB (2537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8003ebd5f122dc9d2c6cbd9039e69d0d13b602e904fda320641dbc7c5f87661f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67759986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c08132b3cbd5d257416b6f79cc8a12f20d85cb41a4d40f097454b5e7fbbea6c1`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:07 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:40:11 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:40:12 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:40:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:40:17 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:40:22 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:40:23 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:40:28 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:40:33 GMT
CMD []
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b1c5f65ee755dd97182c2641d94eb393fc0496adf7f1b4bf78bf5b50944e1c`  
		Last Modified: Wed, 11 Dec 2019 23:41:44 GMT  
		Size: 5.6 MB (5578054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b8444b828db4cd92dfcaa796e6a15d1fc3377b030024a8b87c1087429c0762`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0dd84dc8fd332bb6571553ec1bf4c65377a8924e867bf51c7f6ddfc4daa3efa`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 756.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee095995d2a1c5fe6eaf5e8ceaf7ae5a4ef428406c8e3f4b42a12b06af1db2`  
		Last Modified: Wed, 11 Dec 2019 23:41:41 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-dind-rootless`

```console
$ docker pull docker@sha256:67383a2ae35bd7334ede473e4f7f2563342fc78dbfbf50d0787fb5f518603b74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `docker:test-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:7ccba991abe7af742b95bb74d9358fa2d329fcd03355867e0c325ebf9bac763d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96804016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c85bf7f5b44cdd293a12b5ad71cc24a083e7553d8adbe27efbbea38a3d79cd52`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:04 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 Dec 2019 23:21:05 GMT
RUN set -x 	&& addgroup -S dockremap 	&& adduser -S -G dockremap dockremap 	&& echo 'dockremap:165536:65536' >> /etc/subuid 	&& echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:05 GMT
ENV DIND_COMMIT=37498f009d8bf25fbb6199e8ccd34bed84f2874b
# Wed, 11 Dec 2019 23:21:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 Dec 2019 23:21:06 GMT
COPY file:ecdfb2538258e3154663fab9321e96251276aff00fa2a01c2045656e10a627dd in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:21:07 GMT
VOLUME [/var/lib/docker]
# Wed, 11 Dec 2019 23:21:07 GMT
EXPOSE 2375 2376
# Wed, 11 Dec 2019 23:21:07 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 Dec 2019 23:21:07 GMT
CMD []
# Wed, 11 Dec 2019 23:21:12 GMT
RUN apk add --no-cache iproute2
# Wed, 11 Dec 2019 23:21:13 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 Dec 2019 23:21:13 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 Dec 2019 23:21:15 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O rootless.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-rootless-extras-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-rootless-extras-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		vpnkit --version
# Fri, 20 Dec 2019 01:29:24 GMT
ENV ROOTLESSKIT_VERSION=0.7.1
# Fri, 20 Dec 2019 01:29:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .rootlesskit-build-deps 		go 		libc-dev 	; 	wget -O rootlesskit.tgz "https://github.com/rootless-containers/rootlesskit/archive/v${ROOTLESSKIT_VERSION}.tar.gz"; 	export GOPATH='/go'; mkdir "$GOPATH"; 	mkdir -p "$GOPATH/src/github.com/rootless-containers/rootlesskit"; 	tar --extract --file rootlesskit.tgz --directory "$GOPATH/src/github.com/rootless-containers/rootlesskit" --strip-components 1; 	rm rootlesskit.tgz; 	go build -o /usr/local/bin/rootlesskit github.com/rootless-containers/rootlesskit/cmd/rootlesskit; 	go build -o /usr/local/bin/rootlesskit-docker-proxy github.com/rootless-containers/rootlesskit/cmd/rootlesskit-docker-proxy; 	rm -rf "$GOPATH"; 	apk del --no-network .rootlesskit-build-deps; 	rootlesskit --version
# Fri, 20 Dec 2019 01:29:39 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 20 Dec 2019 01:29:39 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 20 Dec 2019 01:29:39 GMT
USER rootless
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a48ac35fa1a35012549ab3b78195b6d45ffab0a9fcc72c5341c7ea2f01ed5b5`  
		Last Modified: Wed, 11 Dec 2019 23:22:12 GMT  
		Size: 5.6 MB (5554448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377809b0e452b76b024c01a892aa670bfbd9dfc9e9f7de75109590269ab9afeb`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e84307aacff590d2c328103b231f259707f8c1ecbbe0affce9ab3040d44b5cc`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 757.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a86070856a0fc818943d9c9372bc5ebc270f3e067223110bd570b35fecbc250d`  
		Last Modified: Wed, 11 Dec 2019 23:22:11 GMT  
		Size: 2.5 KB (2536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10b23adfdb7b416b5b7eeca1659094e1aabebef346b33f16b26c547d52b5883`  
		Last Modified: Wed, 11 Dec 2019 23:22:21 GMT  
		Size: 782.2 KB (782240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4493bdb21cc998a479ae1f20098f52af6e955a07fff8b1b537bc2a5ebf34939e`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1dd53a02457cef93d7ea523326898d54554a0b24ac1ea9783b858e6168ebd2`  
		Last Modified: Wed, 11 Dec 2019 23:22:19 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59cfa48d52eb16b37a00fcf447455ed9bbb90d4efbb15930ce31bbd224e907e`  
		Last Modified: Wed, 11 Dec 2019 23:22:22 GMT  
		Size: 9.1 MB (9109470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bfbe5a8c5124939208a5805ea253058b2b92a1857b1fd3d5266d1d0990da97`  
		Last Modified: Fri, 20 Dec 2019 01:30:02 GMT  
		Size: 12.3 MB (12336935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c1cc8d056e3bf1d3b3badafd7fce2cf1884ae118484bf3cb52281d725c563c`  
		Last Modified: Fri, 20 Dec 2019 01:30:00 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:test-git`

```console
$ docker pull docker@sha256:3141a9f66a8eaa90e74a0fbf999ab40e7cf3eb2890577ea17e688ead7e020641
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `docker:test-git` - linux; amd64

```console
$ docker pull docker@sha256:e470d67889af90ea7d5008faaba9f8c6bc43de06304dab2b8b2fdd492eae39d3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76865996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6fefe517a89d818bcbdf3465b0bf9657cc4b3bc72f3cb9bc098ff9169ace33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:20:49 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:20:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:20:50 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:20:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:20:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:20:57 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:20:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:20:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:20:58 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:21:36 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca718c007e090ea606c06ea2d0625898b7c360306699eb418b690c37a01d3e`  
		Last Modified: Wed, 11 Dec 2019 23:21:50 GMT  
		Size: 2.4 MB (2422634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cec70188224ea7ba22191c00accecaaf1b78e1f4fab18701e028cca51d3def4`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c248f2b1183d8e2e483bf7ae591bba5e4a4acd64f28896ea24ccf2bba09b9df9`  
		Last Modified: Wed, 11 Dec 2019 23:22:01 GMT  
		Size: 63.8 MB (63803076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2503d20971037b9a2d5a7c7ffb0bc2ed815dd4aed7ff70ea8ca55d87b85c2ca`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b0d619bd33ab28b4e8fe1717ca1f585c4b8fe378f75dba428d12e1a2363b0c`  
		Last Modified: Wed, 11 Dec 2019 23:21:48 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec7a6d53674b6e4eb41a4141aa72ac2894d0b720162d4def56525d374de64c5`  
		Last Modified: Wed, 11 Dec 2019 23:21:49 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fedb39903367c1422036ce9ec4d702341b70ad82cc01b6e76bffdc2642b1395`  
		Last Modified: Wed, 11 Dec 2019 23:22:36 GMT  
		Size: 7.9 MB (7851318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:d109033468e4c2d3916676f30f34833313dc39a469c23b24dda9845a940b73af
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71863615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf1158e8b1b186b886304088df5c4a3e6dd590a351875f2051f206250d4e8ffe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:49:36 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:49:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:49:39 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:49:40 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:49:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:49:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:49:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:49:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:49:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:49:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:50:52 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ff5944bdb7e9171cd9a0b4ff982e7f9f76bee3f40ac1a008ca4ef6a3fc27b`  
		Last Modified: Wed, 11 Dec 2019 22:51:15 GMT  
		Size: 2.3 MB (2336234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46de1899c6245f4aa2d837e9f7c82667f72436fcc7f851b6456f00a63952d93`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5467d422b56b61d8e91e846ad852dd7c79cdf05075198258733b2027d5f493c`  
		Last Modified: Wed, 11 Dec 2019 22:51:32 GMT  
		Size: 59.5 MB (59537105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57abdd7b742761c1733281558639e15c8c0451a6ec25fecee23119353c05b73`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8887fef07d0dab5b2fab086bf75186f5d24bc72b9c2e6ffce87a2391007c77cd`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ca6e031218cb5b93c4111cfec0b7f769837784da486b8aba989ca6b22acabb`  
		Last Modified: Wed, 11 Dec 2019 22:51:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0700c76dc28a7b907870ceaa7e72e7f65265a74a0582be0cfd5713b288d6fdb`  
		Last Modified: Wed, 11 Dec 2019 22:52:01 GMT  
		Size: 7.4 MB (7417097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:81fefdf9037cb7a9b65fc7e76bc4fd79fc3fb2011172b0a47ab4154698bb478a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.7 MB (70735384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84c951058f8f3b2ad0e89f4efb78fe2d0f7458ceb918af47a93fcde708e716c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 22:57:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 22:57:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 22:57:45 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 22:57:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 22:57:55 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 22:57:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 22:57:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 22:57:58 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 22:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 22:57:59 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 22:58:29 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d7fa3dbcd1426cadb6cb4b0846f206a8926d14baffbe8ad5aa852b787da0ef`  
		Last Modified: Wed, 11 Dec 2019 22:58:48 GMT  
		Size: 2.2 MB (2229557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85d9384eb6eca9f83454f40ab447e2eeacfea860348314b3d82ea82238d573`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1545409360129e2ae80d7b8f220f790c5b012b70972f8b64fd0a350483f10c`  
		Last Modified: Wed, 11 Dec 2019 22:59:04 GMT  
		Size: 59.5 MB (59532287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8be6d608ad31e1cc6ef04fd44189715e2bec7defbc9731e56af39548ce97abf`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9f1fb9da16c49cce339d24f699837384e3842493dd1a1d48a5904e6d04eebd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107ef206935890f5e3c8d6f7b13c9e231dd9fb87198c07b8b153679d3a07bcd`  
		Last Modified: Wed, 11 Dec 2019 22:58:45 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b770b6bdd361810ea324b9adf28a24ebcbf0bb0520d3b6a4ee53e496bb1ad4`  
		Last Modified: Wed, 11 Dec 2019 22:59:30 GMT  
		Size: 6.6 MB (6593235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:test-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:8854ae5a4e1458fb0154a525ccc0893a13b9656d54ab27f2d582910a30dcaaf9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70263541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c7f16c5d45e9719de4c144047b6384e359e4112fa93e439f12a8a82692e09a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Wed, 11 Dec 2019 23:39:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client
# Wed, 11 Dec 2019 23:39:41 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 11 Dec 2019 23:39:42 GMT
ENV DOCKER_CHANNEL=stable
# Wed, 11 Dec 2019 23:39:43 GMT
ENV DOCKER_VERSION=19.03.5
# Wed, 11 Dec 2019 23:39:51 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) dockerArch='x86_64' ;; 		armhf) dockerArch='armel' ;; 		armv7) dockerArch='armhf' ;; 		aarch64) dockerArch='aarch64' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 		if ! wget -O docker.tgz "https://download.docker.com/linux/static/${DOCKER_CHANNEL}/${dockerArch}/docker-${DOCKER_VERSION}.tgz"; then 		echo >&2 "error: failed to download 'docker-${DOCKER_VERSION}' from '${DOCKER_CHANNEL}' for '${dockerArch}'"; 		exit 1; 	fi; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 Dec 2019 23:39:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 Dec 2019 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 Dec 2019 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 Dec 2019 23:39:54 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 Dec 2019 23:39:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 Dec 2019 23:39:55 GMT
CMD ["sh"]
# Wed, 11 Dec 2019 23:40:49 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a4930edba01571f06733f51438ff75fd189643faaa974ecd081fe02c862f30`  
		Last Modified: Wed, 11 Dec 2019 23:41:12 GMT  
		Size: 2.5 MB (2451440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168cec15ea7d22d62052eca3277505f95f654ea420b93214e439c7bed4e67b95`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b561127bf77d73eae5e1ef05a721ee95b4049642c37de2926df6801485b285e`  
		Last Modified: Wed, 11 Dec 2019 23:41:28 GMT  
		Size: 57.0 MB (57006217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b14fc1df435300bb4cc734e1c5ec8835e63a6c4974878ae1df55a0138fbe393`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141662ea1213cce657fd7271df8105b45251ae241897b99143f1c4ecae5c4bd1`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b753173eaf4bfc3b344c536cebf062ddc0d56aa0ab88d30fc4e80cb23e96325`  
		Last Modified: Wed, 11 Dec 2019 23:41:09 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06784639818de54df259278e50245d457fa0bf61002da027f39d8126a8956475`  
		Last Modified: Wed, 11 Dec 2019 23:41:58 GMT  
		Size: 8.1 MB (8086237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
