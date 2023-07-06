<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:23`](#docker23)
-	[`docker:23-cli`](#docker23-cli)
-	[`docker:23-dind`](#docker23-dind)
-	[`docker:23-dind-rootless`](#docker23-dind-rootless)
-	[`docker:23-git`](#docker23-git)
-	[`docker:23-windowsservercore`](#docker23-windowsservercore)
-	[`docker:23-windowsservercore-1809`](#docker23-windowsservercore-1809)
-	[`docker:23-windowsservercore-ltsc2022`](#docker23-windowsservercore-ltsc2022)
-	[`docker:23.0`](#docker230)
-	[`docker:23.0-cli`](#docker230-cli)
-	[`docker:23.0-dind`](#docker230-dind)
-	[`docker:23.0-dind-rootless`](#docker230-dind-rootless)
-	[`docker:23.0-git`](#docker230-git)
-	[`docker:23.0-windowsservercore`](#docker230-windowsservercore)
-	[`docker:23.0-windowsservercore-1809`](#docker230-windowsservercore-1809)
-	[`docker:23.0-windowsservercore-ltsc2022`](#docker230-windowsservercore-ltsc2022)
-	[`docker:23.0.6`](#docker2306)
-	[`docker:23.0.6-alpine3.18`](#docker2306-alpine318)
-	[`docker:23.0.6-cli`](#docker2306-cli)
-	[`docker:23.0.6-cli-alpine3.18`](#docker2306-cli-alpine318)
-	[`docker:23.0.6-dind`](#docker2306-dind)
-	[`docker:23.0.6-dind-alpine3.18`](#docker2306-dind-alpine318)
-	[`docker:23.0.6-dind-rootless`](#docker2306-dind-rootless)
-	[`docker:23.0.6-git`](#docker2306-git)
-	[`docker:23.0.6-windowsservercore`](#docker2306-windowsservercore)
-	[`docker:23.0.6-windowsservercore-1809`](#docker2306-windowsservercore-1809)
-	[`docker:23.0.6-windowsservercore-ltsc2022`](#docker2306-windowsservercore-ltsc2022)
-	[`docker:24`](#docker24)
-	[`docker:24-cli`](#docker24-cli)
-	[`docker:24-dind`](#docker24-dind)
-	[`docker:24-dind-rootless`](#docker24-dind-rootless)
-	[`docker:24-git`](#docker24-git)
-	[`docker:24-windowsservercore`](#docker24-windowsservercore)
-	[`docker:24-windowsservercore-1809`](#docker24-windowsservercore-1809)
-	[`docker:24-windowsservercore-ltsc2022`](#docker24-windowsservercore-ltsc2022)
-	[`docker:24.0`](#docker240)
-	[`docker:24.0-cli`](#docker240-cli)
-	[`docker:24.0-dind`](#docker240-dind)
-	[`docker:24.0-dind-rootless`](#docker240-dind-rootless)
-	[`docker:24.0-git`](#docker240-git)
-	[`docker:24.0-windowsservercore`](#docker240-windowsservercore)
-	[`docker:24.0-windowsservercore-1809`](#docker240-windowsservercore-1809)
-	[`docker:24.0-windowsservercore-ltsc2022`](#docker240-windowsservercore-ltsc2022)
-	[`docker:24.0.3`](#docker2403)
-	[`docker:24.0.3-alpine3.18`](#docker2403-alpine318)
-	[`docker:24.0.3-cli`](#docker2403-cli)
-	[`docker:24.0.3-cli-alpine3.18`](#docker2403-cli-alpine318)
-	[`docker:24.0.3-dind`](#docker2403-dind)
-	[`docker:24.0.3-dind-alpine3.18`](#docker2403-dind-alpine318)
-	[`docker:24.0.3-dind-rootless`](#docker2403-dind-rootless)
-	[`docker:24.0.3-git`](#docker2403-git)
-	[`docker:24.0.3-windowsservercore`](#docker2403-windowsservercore)
-	[`docker:24.0.3-windowsservercore-1809`](#docker2403-windowsservercore-1809)
-	[`docker:24.0.3-windowsservercore-ltsc2022`](#docker2403-windowsservercore-ltsc2022)
-	[`docker:cli`](#dockercli)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)
-	[`docker:windowsservercore-ltsc2022`](#dockerwindowsservercore-ltsc2022)

## `docker:23`

```console
$ docker pull docker@sha256:46cc6beebfd6fe2726e1e01f3dc80f5a73296c7e99efc06aadd23fb54b32375b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23` - linux; amd64

```console
$ docker pull docker@sha256:cf6466dfbe0fa1a46a973419da12278a3bf8f210f5b4679c56bea02f6c6c9c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115839183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dbe6391354f44e7b4237c2f65bcd6df95def9b18bc7af704eb9fa51fa8984a6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1978ec6acd84e4dbded4f5b7d647f01f17cc22e5b92afb29c512619965d48dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107101587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1ac3343b21336e4cf574c81ec5382eab04e1eb5284a1c2f53f0336b7958b3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-cli`

```console
$ docker pull docker@sha256:4c7e1aa002fbcc736df5cece6753b86bb516d7a10e59a662e003a6a376088c4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-cli` - linux; amd64

```console
$ docker pull docker@sha256:bf2a78137b4e1ed6f56941ed3b67d00e780d9acd933131d90009f95fe2b1828e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57095751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a1ce85150bff461f224eb003a761e9ec20e6f8de1f535123b735735e29bfa3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:928cef5ba7a6619883f006b42da615107e3a895a131772eca34426af182f156c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52751691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57ca1d0ab4becc6e1b93cd5f95b9b7ffc6727467bb8d317bb271e45e9e383231`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-dind`

```console
$ docker pull docker@sha256:46cc6beebfd6fe2726e1e01f3dc80f5a73296c7e99efc06aadd23fb54b32375b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-dind` - linux; amd64

```console
$ docker pull docker@sha256:cf6466dfbe0fa1a46a973419da12278a3bf8f210f5b4679c56bea02f6c6c9c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115839183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dbe6391354f44e7b4237c2f65bcd6df95def9b18bc7af704eb9fa51fa8984a6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1978ec6acd84e4dbded4f5b7d647f01f17cc22e5b92afb29c512619965d48dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107101587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1ac3343b21336e4cf574c81ec5382eab04e1eb5284a1c2f53f0336b7958b3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-dind-rootless`

```console
$ docker pull docker@sha256:552e8dd18c44b76090d5a6e3711dbb72f24fcd9b098e4a634fb256270582f127
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:e70af0dbeeac5d4b25c5c6ab1ec5f169dcb9092f3865ebb10603f05252f82c54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137550398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bb61285133e2037fe648fe1d7ab3b11e2ddf13659aaf48b463b040e8e13a2ad`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7b056009a58f5469167be072e412cbb1500cf7ce2e43eb204f01ea57cf6c32`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 1.4 MB (1362390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7daa59d1c75354a034dfbcfbe981e3663e4059c87a37cac12c784b10e6a701`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d995acd89cc9bab5de02def4fb4605edff397000b56b458c57f60c1b1514bd7`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b64edc94af7118d6a35ce31a73abee456015c79d28bc87f9cf571d6b7557c`  
		Last Modified: Tue, 04 Jul 2023 01:34:01 GMT  
		Size: 20.3 MB (20347087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63251170bd185825ef6f1f9993f3c686c668973c6a6fc5d3956a31ebaebbd2ed`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:3bab2e9c5eafb583f0be1659798a80f3f6929ea001c68855cb7cfda69cf08bfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130757536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cea1ffd3562b0a4f10fd22bfe1fc1d57d96c30421856cc90917cd55d4003c40`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb95cb6f89ebc6eeda7d6edd5a1d11e982363da94d17ec6eb20034b37d73273`  
		Last Modified: Tue, 04 Jul 2023 00:42:33 GMT  
		Size: 1.4 MB (1413230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096d6d013f761b0e48a145232b58544dfce1dd723f0c6fd10b712aa29684a299`  
		Last Modified: Tue, 04 Jul 2023 00:42:32 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c227cf32dfcd8bbfb4b00157ecff60e750875572ad1d51f3f73ac7107ddc8c2`  
		Last Modified: Tue, 04 Jul 2023 00:42:32 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1274d3c7d85f226b87bdfe5eafe8b63dad09d0f2cd8914513d0a63b8427c693`  
		Last Modified: Tue, 04 Jul 2023 00:42:36 GMT  
		Size: 22.2 MB (22240980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a5d7e3c761b86c806f388ab393a3343d912c29b402cb56e3294873e09ebfb9`  
		Last Modified: Tue, 04 Jul 2023 00:42:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-git`

```console
$ docker pull docker@sha256:43ef6ca30703b21ec031a1c1abf935c0d60511e5c110aa21ba62772d1128d3cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-git` - linux; amd64

```console
$ docker pull docker@sha256:650ec490f33a873e272161d631830181a0f4db7030fb11ccb7d8748eff52dd22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.8 MB (120773928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c49cc8d84a3397f07fd531be3a78af6f0b948026c70ae98d3df181978564164`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37bb0381f31821739ffcc42cffd870a6aa14895be165928d5ad49f72fcbe77`  
		Last Modified: Tue, 04 Jul 2023 01:34:13 GMT  
		Size: 4.9 MB (4934745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4d8f9537914221ed9a2c8979b6d5895bbde7ae6df58c5f24fe2bce3fa71a1958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112122687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:554c8b0d3a3dc5cd4365799c2ff56abe07a40f1d542463f55f149075c4b0da21`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bfbd724bb6b24fe4ead1511532394e222311c398f8e02125247eeed7759cf5`  
		Last Modified: Tue, 04 Jul 2023 00:42:48 GMT  
		Size: 5.0 MB (5021100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore`

```console
$ docker pull docker@sha256:487c6f6d2b2d9632e6c0eb53e84c7c7de46b13b705f863ed58fb27a2392817e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `docker:23-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:e16a9f4d6529304ae75e5e87b9676cf9de5698456bedc4791f0cf7a09420a56d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480280953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8419ea824aa11c888a44bb0ea52f5d804c08f13ff9828f5d8f125ffa44eb0c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:37:22 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:37:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:37:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:37:51 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:37:52 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:37:53 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:38:20 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:16:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:56 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e4d934aedb3408d39924086e00ca7aaad6ba9093494927ec3193aafd92a20f`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d47816062ca7fccecb96be7bf6468c4f36ffddd3115cf4d9bf244c0379bf7c`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520b4152b36536d9d6e0fbb761f4d738b989c5b9bc20fdcb54002f3531479b5`  
		Last Modified: Sat, 24 Jun 2023 03:42:18 GMT  
		Size: 17.3 MB (17325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29907b163c6b32e00b8763615b85445316f0e6cb7cd8c84e9e27ef2d3f409a1e`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99329c21e6a062ffac537c99b986885a8362333c37717e126cb5d88df72bfca3`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ff267e35546ccc351184e91eb2272e461f812168c1c315fbc2ff57b7408600`  
		Last Modified: Sat, 24 Jun 2023 03:42:13 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6b99421718086797da2255cb6dc64b1c37da7f21897b880a0e613168d72ce5`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 17.9 MB (17867625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020919e393d62b234026651fe526978a97e7497d89f3729492f3845ccffa0ba1`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea00cd1e900add94d978485461ef3689853aa4df28a37aa9f323b472a6331d0`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9856084393b0037c77765698dc88b22c99e6245a2f4491290959963bb9f6cacc`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13781f9f6fb0ab46635807dd978bb80fe0a32078b7942c0cc76b7aae45492698`  
		Last Modified: Tue, 04 Jul 2023 01:18:44 GMT  
		Size: 18.5 MB (18450181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:6e0b433184a45352544aaf4fd7d47bd7948d6113df04508d58bd94723ff122de
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704687111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6e5dc354031de16fdb42eef9f33197a8cf2a865cfc2f2cc7444159eeb0dc7b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:39:11 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:39:12 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:39:46 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:39:47 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:39:48 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:40:21 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:17:07 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:17:37 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabd176de44496cc60e08f954b7d47c99eb8d47e8a4338216815756e4e9659db`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b649bbc9bc70f0249f614bd545fd46c7cae1690a92cc79ea5befcd92cdcbdaa`  
		Last Modified: Sat, 24 Jun 2023 03:42:33 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f0093a3b9ea484ba6ea7db9214d3bc0d379d6ecdd7ee3a7fdecb30b09cde0`  
		Last Modified: Sat, 24 Jun 2023 03:42:36 GMT  
		Size: 17.3 MB (17317987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d15fecfe4327fa2649e3f89e72313f0422c9437822bd74b524549b42db8b71d`  
		Last Modified: Sat, 24 Jun 2023 03:42:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e5df5c643dd2fedeee943bc8960602ba9ad5380bfca064d0a5172a881cf6ee`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a32c51db291cc48fecb9640f7f516872275591d2c22cc3a8936a86ad45dc7e3`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b397682ddc1d0a0b22c92691691e7a787b2b7ac52eee263f47d7447edc8e336`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 17.9 MB (17857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415e61d7b47f78b19cafe15f8ec23830bbfd3cc09ba32b574c8b3709f9d9c73c`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250a626d9b7c309298042f6e5caa22099a134d01adf912982d92f40673f21ac5`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5e1fbabe536045bfb6179fb5a5f0a06799b9c4708f70d00df7b03848ea0ffe`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1205d9c3f51c766ca715b96f2836a9a0a9178124ea20c0f037f7d384e959a66a`  
		Last Modified: Tue, 04 Jul 2023 01:18:58 GMT  
		Size: 18.5 MB (18456783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore-1809`

```console
$ docker pull docker@sha256:5a44a5290d7055f171d743debcc74ef98264ec41bb37a1bbb5cce44cd0f90364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `docker:23-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:6e0b433184a45352544aaf4fd7d47bd7948d6113df04508d58bd94723ff122de
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704687111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6e5dc354031de16fdb42eef9f33197a8cf2a865cfc2f2cc7444159eeb0dc7b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:39:11 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:39:12 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:39:46 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:39:47 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:39:48 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:40:21 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:17:07 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:17:37 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabd176de44496cc60e08f954b7d47c99eb8d47e8a4338216815756e4e9659db`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b649bbc9bc70f0249f614bd545fd46c7cae1690a92cc79ea5befcd92cdcbdaa`  
		Last Modified: Sat, 24 Jun 2023 03:42:33 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f0093a3b9ea484ba6ea7db9214d3bc0d379d6ecdd7ee3a7fdecb30b09cde0`  
		Last Modified: Sat, 24 Jun 2023 03:42:36 GMT  
		Size: 17.3 MB (17317987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d15fecfe4327fa2649e3f89e72313f0422c9437822bd74b524549b42db8b71d`  
		Last Modified: Sat, 24 Jun 2023 03:42:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e5df5c643dd2fedeee943bc8960602ba9ad5380bfca064d0a5172a881cf6ee`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a32c51db291cc48fecb9640f7f516872275591d2c22cc3a8936a86ad45dc7e3`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b397682ddc1d0a0b22c92691691e7a787b2b7ac52eee263f47d7447edc8e336`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 17.9 MB (17857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415e61d7b47f78b19cafe15f8ec23830bbfd3cc09ba32b574c8b3709f9d9c73c`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250a626d9b7c309298042f6e5caa22099a134d01adf912982d92f40673f21ac5`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5e1fbabe536045bfb6179fb5a5f0a06799b9c4708f70d00df7b03848ea0ffe`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1205d9c3f51c766ca715b96f2836a9a0a9178124ea20c0f037f7d384e959a66a`  
		Last Modified: Tue, 04 Jul 2023 01:18:58 GMT  
		Size: 18.5 MB (18456783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:9eebb50b9d3133014ca7138f450cdbe0d43901e15c71d0895a8b09751fcc22a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `docker:23-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:e16a9f4d6529304ae75e5e87b9676cf9de5698456bedc4791f0cf7a09420a56d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480280953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8419ea824aa11c888a44bb0ea52f5d804c08f13ff9828f5d8f125ffa44eb0c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:37:22 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:37:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:37:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:37:51 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:37:52 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:37:53 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:38:20 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:16:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:56 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e4d934aedb3408d39924086e00ca7aaad6ba9093494927ec3193aafd92a20f`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d47816062ca7fccecb96be7bf6468c4f36ffddd3115cf4d9bf244c0379bf7c`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520b4152b36536d9d6e0fbb761f4d738b989c5b9bc20fdcb54002f3531479b5`  
		Last Modified: Sat, 24 Jun 2023 03:42:18 GMT  
		Size: 17.3 MB (17325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29907b163c6b32e00b8763615b85445316f0e6cb7cd8c84e9e27ef2d3f409a1e`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99329c21e6a062ffac537c99b986885a8362333c37717e126cb5d88df72bfca3`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ff267e35546ccc351184e91eb2272e461f812168c1c315fbc2ff57b7408600`  
		Last Modified: Sat, 24 Jun 2023 03:42:13 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6b99421718086797da2255cb6dc64b1c37da7f21897b880a0e613168d72ce5`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 17.9 MB (17867625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020919e393d62b234026651fe526978a97e7497d89f3729492f3845ccffa0ba1`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea00cd1e900add94d978485461ef3689853aa4df28a37aa9f323b472a6331d0`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9856084393b0037c77765698dc88b22c99e6245a2f4491290959963bb9f6cacc`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13781f9f6fb0ab46635807dd978bb80fe0a32078b7942c0cc76b7aae45492698`  
		Last Modified: Tue, 04 Jul 2023 01:18:44 GMT  
		Size: 18.5 MB (18450181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0`

```console
$ docker pull docker@sha256:46cc6beebfd6fe2726e1e01f3dc80f5a73296c7e99efc06aadd23fb54b32375b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0` - linux; amd64

```console
$ docker pull docker@sha256:cf6466dfbe0fa1a46a973419da12278a3bf8f210f5b4679c56bea02f6c6c9c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115839183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dbe6391354f44e7b4237c2f65bcd6df95def9b18bc7af704eb9fa51fa8984a6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1978ec6acd84e4dbded4f5b7d647f01f17cc22e5b92afb29c512619965d48dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107101587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1ac3343b21336e4cf574c81ec5382eab04e1eb5284a1c2f53f0336b7958b3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-cli`

```console
$ docker pull docker@sha256:4c7e1aa002fbcc736df5cece6753b86bb516d7a10e59a662e003a6a376088c4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-cli` - linux; amd64

```console
$ docker pull docker@sha256:bf2a78137b4e1ed6f56941ed3b67d00e780d9acd933131d90009f95fe2b1828e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57095751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a1ce85150bff461f224eb003a761e9ec20e6f8de1f535123b735735e29bfa3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:928cef5ba7a6619883f006b42da615107e3a895a131772eca34426af182f156c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52751691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57ca1d0ab4becc6e1b93cd5f95b9b7ffc6727467bb8d317bb271e45e9e383231`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-dind`

```console
$ docker pull docker@sha256:46cc6beebfd6fe2726e1e01f3dc80f5a73296c7e99efc06aadd23fb54b32375b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-dind` - linux; amd64

```console
$ docker pull docker@sha256:cf6466dfbe0fa1a46a973419da12278a3bf8f210f5b4679c56bea02f6c6c9c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115839183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dbe6391354f44e7b4237c2f65bcd6df95def9b18bc7af704eb9fa51fa8984a6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1978ec6acd84e4dbded4f5b7d647f01f17cc22e5b92afb29c512619965d48dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107101587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1ac3343b21336e4cf574c81ec5382eab04e1eb5284a1c2f53f0336b7958b3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-dind-rootless`

```console
$ docker pull docker@sha256:552e8dd18c44b76090d5a6e3711dbb72f24fcd9b098e4a634fb256270582f127
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:e70af0dbeeac5d4b25c5c6ab1ec5f169dcb9092f3865ebb10603f05252f82c54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137550398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bb61285133e2037fe648fe1d7ab3b11e2ddf13659aaf48b463b040e8e13a2ad`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7b056009a58f5469167be072e412cbb1500cf7ce2e43eb204f01ea57cf6c32`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 1.4 MB (1362390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7daa59d1c75354a034dfbcfbe981e3663e4059c87a37cac12c784b10e6a701`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d995acd89cc9bab5de02def4fb4605edff397000b56b458c57f60c1b1514bd7`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b64edc94af7118d6a35ce31a73abee456015c79d28bc87f9cf571d6b7557c`  
		Last Modified: Tue, 04 Jul 2023 01:34:01 GMT  
		Size: 20.3 MB (20347087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63251170bd185825ef6f1f9993f3c686c668973c6a6fc5d3956a31ebaebbd2ed`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:3bab2e9c5eafb583f0be1659798a80f3f6929ea001c68855cb7cfda69cf08bfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130757536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cea1ffd3562b0a4f10fd22bfe1fc1d57d96c30421856cc90917cd55d4003c40`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb95cb6f89ebc6eeda7d6edd5a1d11e982363da94d17ec6eb20034b37d73273`  
		Last Modified: Tue, 04 Jul 2023 00:42:33 GMT  
		Size: 1.4 MB (1413230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096d6d013f761b0e48a145232b58544dfce1dd723f0c6fd10b712aa29684a299`  
		Last Modified: Tue, 04 Jul 2023 00:42:32 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c227cf32dfcd8bbfb4b00157ecff60e750875572ad1d51f3f73ac7107ddc8c2`  
		Last Modified: Tue, 04 Jul 2023 00:42:32 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1274d3c7d85f226b87bdfe5eafe8b63dad09d0f2cd8914513d0a63b8427c693`  
		Last Modified: Tue, 04 Jul 2023 00:42:36 GMT  
		Size: 22.2 MB (22240980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a5d7e3c761b86c806f388ab393a3343d912c29b402cb56e3294873e09ebfb9`  
		Last Modified: Tue, 04 Jul 2023 00:42:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-git`

```console
$ docker pull docker@sha256:43ef6ca30703b21ec031a1c1abf935c0d60511e5c110aa21ba62772d1128d3cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-git` - linux; amd64

```console
$ docker pull docker@sha256:650ec490f33a873e272161d631830181a0f4db7030fb11ccb7d8748eff52dd22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.8 MB (120773928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c49cc8d84a3397f07fd531be3a78af6f0b948026c70ae98d3df181978564164`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37bb0381f31821739ffcc42cffd870a6aa14895be165928d5ad49f72fcbe77`  
		Last Modified: Tue, 04 Jul 2023 01:34:13 GMT  
		Size: 4.9 MB (4934745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4d8f9537914221ed9a2c8979b6d5895bbde7ae6df58c5f24fe2bce3fa71a1958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112122687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:554c8b0d3a3dc5cd4365799c2ff56abe07a40f1d542463f55f149075c4b0da21`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bfbd724bb6b24fe4ead1511532394e222311c398f8e02125247eeed7759cf5`  
		Last Modified: Tue, 04 Jul 2023 00:42:48 GMT  
		Size: 5.0 MB (5021100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore`

```console
$ docker pull docker@sha256:487c6f6d2b2d9632e6c0eb53e84c7c7de46b13b705f863ed58fb27a2392817e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `docker:23.0-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:e16a9f4d6529304ae75e5e87b9676cf9de5698456bedc4791f0cf7a09420a56d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480280953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8419ea824aa11c888a44bb0ea52f5d804c08f13ff9828f5d8f125ffa44eb0c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:37:22 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:37:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:37:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:37:51 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:37:52 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:37:53 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:38:20 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:16:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:56 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e4d934aedb3408d39924086e00ca7aaad6ba9093494927ec3193aafd92a20f`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d47816062ca7fccecb96be7bf6468c4f36ffddd3115cf4d9bf244c0379bf7c`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520b4152b36536d9d6e0fbb761f4d738b989c5b9bc20fdcb54002f3531479b5`  
		Last Modified: Sat, 24 Jun 2023 03:42:18 GMT  
		Size: 17.3 MB (17325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29907b163c6b32e00b8763615b85445316f0e6cb7cd8c84e9e27ef2d3f409a1e`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99329c21e6a062ffac537c99b986885a8362333c37717e126cb5d88df72bfca3`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ff267e35546ccc351184e91eb2272e461f812168c1c315fbc2ff57b7408600`  
		Last Modified: Sat, 24 Jun 2023 03:42:13 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6b99421718086797da2255cb6dc64b1c37da7f21897b880a0e613168d72ce5`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 17.9 MB (17867625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020919e393d62b234026651fe526978a97e7497d89f3729492f3845ccffa0ba1`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea00cd1e900add94d978485461ef3689853aa4df28a37aa9f323b472a6331d0`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9856084393b0037c77765698dc88b22c99e6245a2f4491290959963bb9f6cacc`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13781f9f6fb0ab46635807dd978bb80fe0a32078b7942c0cc76b7aae45492698`  
		Last Modified: Tue, 04 Jul 2023 01:18:44 GMT  
		Size: 18.5 MB (18450181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:6e0b433184a45352544aaf4fd7d47bd7948d6113df04508d58bd94723ff122de
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704687111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6e5dc354031de16fdb42eef9f33197a8cf2a865cfc2f2cc7444159eeb0dc7b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:39:11 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:39:12 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:39:46 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:39:47 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:39:48 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:40:21 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:17:07 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:17:37 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabd176de44496cc60e08f954b7d47c99eb8d47e8a4338216815756e4e9659db`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b649bbc9bc70f0249f614bd545fd46c7cae1690a92cc79ea5befcd92cdcbdaa`  
		Last Modified: Sat, 24 Jun 2023 03:42:33 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f0093a3b9ea484ba6ea7db9214d3bc0d379d6ecdd7ee3a7fdecb30b09cde0`  
		Last Modified: Sat, 24 Jun 2023 03:42:36 GMT  
		Size: 17.3 MB (17317987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d15fecfe4327fa2649e3f89e72313f0422c9437822bd74b524549b42db8b71d`  
		Last Modified: Sat, 24 Jun 2023 03:42:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e5df5c643dd2fedeee943bc8960602ba9ad5380bfca064d0a5172a881cf6ee`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a32c51db291cc48fecb9640f7f516872275591d2c22cc3a8936a86ad45dc7e3`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b397682ddc1d0a0b22c92691691e7a787b2b7ac52eee263f47d7447edc8e336`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 17.9 MB (17857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415e61d7b47f78b19cafe15f8ec23830bbfd3cc09ba32b574c8b3709f9d9c73c`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250a626d9b7c309298042f6e5caa22099a134d01adf912982d92f40673f21ac5`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5e1fbabe536045bfb6179fb5a5f0a06799b9c4708f70d00df7b03848ea0ffe`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1205d9c3f51c766ca715b96f2836a9a0a9178124ea20c0f037f7d384e959a66a`  
		Last Modified: Tue, 04 Jul 2023 01:18:58 GMT  
		Size: 18.5 MB (18456783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore-1809`

```console
$ docker pull docker@sha256:5a44a5290d7055f171d743debcc74ef98264ec41bb37a1bbb5cce44cd0f90364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `docker:23.0-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:6e0b433184a45352544aaf4fd7d47bd7948d6113df04508d58bd94723ff122de
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704687111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6e5dc354031de16fdb42eef9f33197a8cf2a865cfc2f2cc7444159eeb0dc7b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:39:11 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:39:12 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:39:46 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:39:47 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:39:48 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:40:21 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:17:07 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:17:37 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabd176de44496cc60e08f954b7d47c99eb8d47e8a4338216815756e4e9659db`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b649bbc9bc70f0249f614bd545fd46c7cae1690a92cc79ea5befcd92cdcbdaa`  
		Last Modified: Sat, 24 Jun 2023 03:42:33 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f0093a3b9ea484ba6ea7db9214d3bc0d379d6ecdd7ee3a7fdecb30b09cde0`  
		Last Modified: Sat, 24 Jun 2023 03:42:36 GMT  
		Size: 17.3 MB (17317987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d15fecfe4327fa2649e3f89e72313f0422c9437822bd74b524549b42db8b71d`  
		Last Modified: Sat, 24 Jun 2023 03:42:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e5df5c643dd2fedeee943bc8960602ba9ad5380bfca064d0a5172a881cf6ee`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a32c51db291cc48fecb9640f7f516872275591d2c22cc3a8936a86ad45dc7e3`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b397682ddc1d0a0b22c92691691e7a787b2b7ac52eee263f47d7447edc8e336`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 17.9 MB (17857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415e61d7b47f78b19cafe15f8ec23830bbfd3cc09ba32b574c8b3709f9d9c73c`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250a626d9b7c309298042f6e5caa22099a134d01adf912982d92f40673f21ac5`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5e1fbabe536045bfb6179fb5a5f0a06799b9c4708f70d00df7b03848ea0ffe`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1205d9c3f51c766ca715b96f2836a9a0a9178124ea20c0f037f7d384e959a66a`  
		Last Modified: Tue, 04 Jul 2023 01:18:58 GMT  
		Size: 18.5 MB (18456783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:9eebb50b9d3133014ca7138f450cdbe0d43901e15c71d0895a8b09751fcc22a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `docker:23.0-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:e16a9f4d6529304ae75e5e87b9676cf9de5698456bedc4791f0cf7a09420a56d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480280953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8419ea824aa11c888a44bb0ea52f5d804c08f13ff9828f5d8f125ffa44eb0c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:37:22 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:37:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:37:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:37:51 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:37:52 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:37:53 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:38:20 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:16:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:56 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e4d934aedb3408d39924086e00ca7aaad6ba9093494927ec3193aafd92a20f`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d47816062ca7fccecb96be7bf6468c4f36ffddd3115cf4d9bf244c0379bf7c`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520b4152b36536d9d6e0fbb761f4d738b989c5b9bc20fdcb54002f3531479b5`  
		Last Modified: Sat, 24 Jun 2023 03:42:18 GMT  
		Size: 17.3 MB (17325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29907b163c6b32e00b8763615b85445316f0e6cb7cd8c84e9e27ef2d3f409a1e`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99329c21e6a062ffac537c99b986885a8362333c37717e126cb5d88df72bfca3`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ff267e35546ccc351184e91eb2272e461f812168c1c315fbc2ff57b7408600`  
		Last Modified: Sat, 24 Jun 2023 03:42:13 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6b99421718086797da2255cb6dc64b1c37da7f21897b880a0e613168d72ce5`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 17.9 MB (17867625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020919e393d62b234026651fe526978a97e7497d89f3729492f3845ccffa0ba1`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea00cd1e900add94d978485461ef3689853aa4df28a37aa9f323b472a6331d0`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9856084393b0037c77765698dc88b22c99e6245a2f4491290959963bb9f6cacc`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13781f9f6fb0ab46635807dd978bb80fe0a32078b7942c0cc76b7aae45492698`  
		Last Modified: Tue, 04 Jul 2023 01:18:44 GMT  
		Size: 18.5 MB (18450181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6`

```console
$ docker pull docker@sha256:46cc6beebfd6fe2726e1e01f3dc80f5a73296c7e99efc06aadd23fb54b32375b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6` - linux; amd64

```console
$ docker pull docker@sha256:cf6466dfbe0fa1a46a973419da12278a3bf8f210f5b4679c56bea02f6c6c9c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115839183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dbe6391354f44e7b4237c2f65bcd6df95def9b18bc7af704eb9fa51fa8984a6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1978ec6acd84e4dbded4f5b7d647f01f17cc22e5b92afb29c512619965d48dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107101587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1ac3343b21336e4cf574c81ec5382eab04e1eb5284a1c2f53f0336b7958b3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-alpine3.18`

```console
$ docker pull docker@sha256:46cc6beebfd6fe2726e1e01f3dc80f5a73296c7e99efc06aadd23fb54b32375b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-alpine3.18` - linux; amd64

```console
$ docker pull docker@sha256:cf6466dfbe0fa1a46a973419da12278a3bf8f210f5b4679c56bea02f6c6c9c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115839183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dbe6391354f44e7b4237c2f65bcd6df95def9b18bc7af704eb9fa51fa8984a6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1978ec6acd84e4dbded4f5b7d647f01f17cc22e5b92afb29c512619965d48dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107101587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1ac3343b21336e4cf574c81ec5382eab04e1eb5284a1c2f53f0336b7958b3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-cli`

```console
$ docker pull docker@sha256:4c7e1aa002fbcc736df5cece6753b86bb516d7a10e59a662e003a6a376088c4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-cli` - linux; amd64

```console
$ docker pull docker@sha256:bf2a78137b4e1ed6f56941ed3b67d00e780d9acd933131d90009f95fe2b1828e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57095751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a1ce85150bff461f224eb003a761e9ec20e6f8de1f535123b735735e29bfa3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:928cef5ba7a6619883f006b42da615107e3a895a131772eca34426af182f156c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52751691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57ca1d0ab4becc6e1b93cd5f95b9b7ffc6727467bb8d317bb271e45e9e383231`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-cli-alpine3.18`

```console
$ docker pull docker@sha256:4c7e1aa002fbcc736df5cece6753b86bb516d7a10e59a662e003a6a376088c4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-cli-alpine3.18` - linux; amd64

```console
$ docker pull docker@sha256:bf2a78137b4e1ed6f56941ed3b67d00e780d9acd933131d90009f95fe2b1828e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57095751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a1ce85150bff461f224eb003a761e9ec20e6f8de1f535123b735735e29bfa3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-cli-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:928cef5ba7a6619883f006b42da615107e3a895a131772eca34426af182f156c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52751691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57ca1d0ab4becc6e1b93cd5f95b9b7ffc6727467bb8d317bb271e45e9e383231`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-dind`

```console
$ docker pull docker@sha256:46cc6beebfd6fe2726e1e01f3dc80f5a73296c7e99efc06aadd23fb54b32375b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-dind` - linux; amd64

```console
$ docker pull docker@sha256:cf6466dfbe0fa1a46a973419da12278a3bf8f210f5b4679c56bea02f6c6c9c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115839183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dbe6391354f44e7b4237c2f65bcd6df95def9b18bc7af704eb9fa51fa8984a6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1978ec6acd84e4dbded4f5b7d647f01f17cc22e5b92afb29c512619965d48dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107101587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1ac3343b21336e4cf574c81ec5382eab04e1eb5284a1c2f53f0336b7958b3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-dind-alpine3.18`

```console
$ docker pull docker@sha256:46cc6beebfd6fe2726e1e01f3dc80f5a73296c7e99efc06aadd23fb54b32375b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-dind-alpine3.18` - linux; amd64

```console
$ docker pull docker@sha256:cf6466dfbe0fa1a46a973419da12278a3bf8f210f5b4679c56bea02f6c6c9c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115839183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dbe6391354f44e7b4237c2f65bcd6df95def9b18bc7af704eb9fa51fa8984a6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-dind-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1978ec6acd84e4dbded4f5b7d647f01f17cc22e5b92afb29c512619965d48dc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107101587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1ac3343b21336e4cf574c81ec5382eab04e1eb5284a1c2f53f0336b7958b3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-dind-rootless`

```console
$ docker pull docker@sha256:552e8dd18c44b76090d5a6e3711dbb72f24fcd9b098e4a634fb256270582f127
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:e70af0dbeeac5d4b25c5c6ab1ec5f169dcb9092f3865ebb10603f05252f82c54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137550398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bb61285133e2037fe648fe1d7ab3b11e2ddf13659aaf48b463b040e8e13a2ad`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7b056009a58f5469167be072e412cbb1500cf7ce2e43eb204f01ea57cf6c32`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 1.4 MB (1362390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7daa59d1c75354a034dfbcfbe981e3663e4059c87a37cac12c784b10e6a701`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d995acd89cc9bab5de02def4fb4605edff397000b56b458c57f60c1b1514bd7`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318b64edc94af7118d6a35ce31a73abee456015c79d28bc87f9cf571d6b7557c`  
		Last Modified: Tue, 04 Jul 2023 01:34:01 GMT  
		Size: 20.3 MB (20347087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63251170bd185825ef6f1f9993f3c686c668973c6a6fc5d3956a31ebaebbd2ed`  
		Last Modified: Tue, 04 Jul 2023 01:33:58 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:3bab2e9c5eafb583f0be1659798a80f3f6929ea001c68855cb7cfda69cf08bfc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.8 MB (130757536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cea1ffd3562b0a4f10fd22bfe1fc1d57d96c30421856cc90917cd55d4003c40`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 16 May 2023 17:59:38 GMT
USER rootless
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb95cb6f89ebc6eeda7d6edd5a1d11e982363da94d17ec6eb20034b37d73273`  
		Last Modified: Tue, 04 Jul 2023 00:42:33 GMT  
		Size: 1.4 MB (1413230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:096d6d013f761b0e48a145232b58544dfce1dd723f0c6fd10b712aa29684a299`  
		Last Modified: Tue, 04 Jul 2023 00:42:32 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c227cf32dfcd8bbfb4b00157ecff60e750875572ad1d51f3f73ac7107ddc8c2`  
		Last Modified: Tue, 04 Jul 2023 00:42:32 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1274d3c7d85f226b87bdfe5eafe8b63dad09d0f2cd8914513d0a63b8427c693`  
		Last Modified: Tue, 04 Jul 2023 00:42:36 GMT  
		Size: 22.2 MB (22240980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a5d7e3c761b86c806f388ab393a3343d912c29b402cb56e3294873e09ebfb9`  
		Last Modified: Tue, 04 Jul 2023 00:42:32 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-git`

```console
$ docker pull docker@sha256:43ef6ca30703b21ec031a1c1abf935c0d60511e5c110aa21ba62772d1128d3cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.6-git` - linux; amd64

```console
$ docker pull docker@sha256:650ec490f33a873e272161d631830181a0f4db7030fb11ccb7d8748eff52dd22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.8 MB (120773928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c49cc8d84a3397f07fd531be3a78af6f0b948026c70ae98d3df181978564164`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cbbfe9c78c82698902d2f699f3a866996d040be1686dd10f629e37d89ea33ee`  
		Last Modified: Thu, 15 Jun 2023 05:28:31 GMT  
		Size: 16.3 MB (16250874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6241ab295fb796705bb1de344f9cde5653dbc4191daed43a1cf47fe1805182b`  
		Last Modified: Thu, 15 Jun 2023 05:28:30 GMT  
		Size: 17.5 MB (17450703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5a58cac5e4b64757ca20adc724c0a74b8cb675a38ff930ce7e07687c173a35`  
		Last Modified: Tue, 04 Jul 2023 01:33:16 GMT  
		Size: 18.0 MB (17980092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c2e62070458ff3dde948865619b6beac1ae337205bb5cfc19f1088c3f70d10`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68467f5fca993e316d538ed225728a96098a02dd11f48e513b6d03a08e7841d7`  
		Last Modified: Tue, 04 Jul 2023 01:33:13 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2892b4d2a8dc07735031687013ddabdd8809fc7c2d94d0d154c51f5018d3e822`  
		Last Modified: Tue, 04 Jul 2023 01:33:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076afaf4d64adc51c53657a07c2275f547f6ac4b610ac533f1b20932a319ecc8`  
		Last Modified: Tue, 04 Jul 2023 01:33:30 GMT  
		Size: 7.1 MB (7080776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d195469b6eac7a68b54cfde34f782f0debb46cb1b726372dec84595c5016b`  
		Last Modified: Tue, 04 Jul 2023 01:33:28 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88abf93ae78701dcac50d1abf4034a70b85d32fa2929f8308141bc2068baec1`  
		Last Modified: Tue, 04 Jul 2023 01:33:36 GMT  
		Size: 51.7 MB (51657486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be8d48a01490c395c9041bd08b53515d9073519d03aae84b70e7676bbd46eb6`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8998c0beee29347a27bde1f6527f68fe0b6288ec28d3342917201cd3bb1b0130`  
		Last Modified: Tue, 04 Jul 2023 01:33:29 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb37bb0381f31821739ffcc42cffd870a6aa14895be165928d5ad49f72fcbe77`  
		Last Modified: Tue, 04 Jul 2023 01:34:13 GMT  
		Size: 4.9 MB (4934745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4d8f9537914221ed9a2c8979b6d5895bbde7ae6df58c5f24fe2bce3fa71a1958
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.1 MB (112122687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:554c8b0d3a3dc5cd4365799c2ff56abe07a40f1d542463f55f149075c4b0da21`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:04:13 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:04:12 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:04:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:04:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:04:12 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:04:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:04:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:04:12 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51d2d067e69a1f5a948d2d1133441f75a192e5bcc4154ca7be51943ff4a24d5`  
		Last Modified: Wed, 14 Jun 2023 22:42:12 GMT  
		Size: 15.3 MB (15325099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54896eea313c91a3310409b75e7f19bf9549e622830a9bb2ccf641133d3443b2`  
		Last Modified: Wed, 14 Jun 2023 22:42:10 GMT  
		Size: 15.8 MB (15758022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8a94781991d571db2828d582b586a42f112b48a5360b945c4ac9f9361714bd`  
		Last Modified: Tue, 04 Jul 2023 00:41:53 GMT  
		Size: 16.3 MB (16312955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dff06bfb8947cafc3522167543d585c8634cf8b9d13f3980b48b71412679b8f`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5908dea7a9ed1d51b3eb2f29dbb1dfb076aeb9a08ca25b17fa646a4518967ca0`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996d55d19a70400bb873ae31f26a5f6850daffd93617eba14d2734e9679b207`  
		Last Modified: Tue, 04 Jul 2023 00:41:51 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b145cfaa7d24d1c7cbd5e7182ae589b3936c16923f90301ce4a1346f5fbabf0`  
		Last Modified: Tue, 04 Jul 2023 00:42:06 GMT  
		Size: 7.3 MB (7291371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82916a858ce89e51c27d4fe316f410e0f12c57c04861c7458aab93e205811d7b`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7365d07ed554f358029ded05eece566d7101d0afb5f418cd751b10affe5685b2`  
		Last Modified: Tue, 04 Jul 2023 00:42:10 GMT  
		Size: 47.1 MB (47053358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f235eaa9f5ebce0468c5ec2ccd96647fe6f796322b5e673c52c49d1f025d96`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37625190857ba27b7fce0deb611dad6ad888ee4b06db5626c83d2fe991483ae1`  
		Last Modified: Tue, 04 Jul 2023 00:42:05 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92bfbd724bb6b24fe4ead1511532394e222311c398f8e02125247eeed7759cf5`  
		Last Modified: Tue, 04 Jul 2023 00:42:48 GMT  
		Size: 5.0 MB (5021100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-windowsservercore`

```console
$ docker pull docker@sha256:487c6f6d2b2d9632e6c0eb53e84c7c7de46b13b705f863ed58fb27a2392817e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `docker:23.0.6-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:e16a9f4d6529304ae75e5e87b9676cf9de5698456bedc4791f0cf7a09420a56d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480280953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8419ea824aa11c888a44bb0ea52f5d804c08f13ff9828f5d8f125ffa44eb0c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:37:22 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:37:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:37:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:37:51 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:37:52 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:37:53 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:38:20 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:16:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:56 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e4d934aedb3408d39924086e00ca7aaad6ba9093494927ec3193aafd92a20f`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d47816062ca7fccecb96be7bf6468c4f36ffddd3115cf4d9bf244c0379bf7c`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520b4152b36536d9d6e0fbb761f4d738b989c5b9bc20fdcb54002f3531479b5`  
		Last Modified: Sat, 24 Jun 2023 03:42:18 GMT  
		Size: 17.3 MB (17325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29907b163c6b32e00b8763615b85445316f0e6cb7cd8c84e9e27ef2d3f409a1e`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99329c21e6a062ffac537c99b986885a8362333c37717e126cb5d88df72bfca3`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ff267e35546ccc351184e91eb2272e461f812168c1c315fbc2ff57b7408600`  
		Last Modified: Sat, 24 Jun 2023 03:42:13 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6b99421718086797da2255cb6dc64b1c37da7f21897b880a0e613168d72ce5`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 17.9 MB (17867625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020919e393d62b234026651fe526978a97e7497d89f3729492f3845ccffa0ba1`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea00cd1e900add94d978485461ef3689853aa4df28a37aa9f323b472a6331d0`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9856084393b0037c77765698dc88b22c99e6245a2f4491290959963bb9f6cacc`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13781f9f6fb0ab46635807dd978bb80fe0a32078b7942c0cc76b7aae45492698`  
		Last Modified: Tue, 04 Jul 2023 01:18:44 GMT  
		Size: 18.5 MB (18450181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.6-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:6e0b433184a45352544aaf4fd7d47bd7948d6113df04508d58bd94723ff122de
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704687111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6e5dc354031de16fdb42eef9f33197a8cf2a865cfc2f2cc7444159eeb0dc7b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:39:11 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:39:12 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:39:46 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:39:47 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:39:48 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:40:21 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:17:07 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:17:37 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabd176de44496cc60e08f954b7d47c99eb8d47e8a4338216815756e4e9659db`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b649bbc9bc70f0249f614bd545fd46c7cae1690a92cc79ea5befcd92cdcbdaa`  
		Last Modified: Sat, 24 Jun 2023 03:42:33 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f0093a3b9ea484ba6ea7db9214d3bc0d379d6ecdd7ee3a7fdecb30b09cde0`  
		Last Modified: Sat, 24 Jun 2023 03:42:36 GMT  
		Size: 17.3 MB (17317987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d15fecfe4327fa2649e3f89e72313f0422c9437822bd74b524549b42db8b71d`  
		Last Modified: Sat, 24 Jun 2023 03:42:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e5df5c643dd2fedeee943bc8960602ba9ad5380bfca064d0a5172a881cf6ee`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a32c51db291cc48fecb9640f7f516872275591d2c22cc3a8936a86ad45dc7e3`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b397682ddc1d0a0b22c92691691e7a787b2b7ac52eee263f47d7447edc8e336`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 17.9 MB (17857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415e61d7b47f78b19cafe15f8ec23830bbfd3cc09ba32b574c8b3709f9d9c73c`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250a626d9b7c309298042f6e5caa22099a134d01adf912982d92f40673f21ac5`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5e1fbabe536045bfb6179fb5a5f0a06799b9c4708f70d00df7b03848ea0ffe`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1205d9c3f51c766ca715b96f2836a9a0a9178124ea20c0f037f7d384e959a66a`  
		Last Modified: Tue, 04 Jul 2023 01:18:58 GMT  
		Size: 18.5 MB (18456783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-windowsservercore-1809`

```console
$ docker pull docker@sha256:5a44a5290d7055f171d743debcc74ef98264ec41bb37a1bbb5cce44cd0f90364
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `docker:23.0.6-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:6e0b433184a45352544aaf4fd7d47bd7948d6113df04508d58bd94723ff122de
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704687111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6e5dc354031de16fdb42eef9f33197a8cf2a865cfc2f2cc7444159eeb0dc7b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:39:11 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:39:12 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:39:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:39:46 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:39:47 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:39:48 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:40:21 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:17:06 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:17:07 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:17:37 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dabd176de44496cc60e08f954b7d47c99eb8d47e8a4338216815756e4e9659db`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b649bbc9bc70f0249f614bd545fd46c7cae1690a92cc79ea5befcd92cdcbdaa`  
		Last Modified: Sat, 24 Jun 2023 03:42:33 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f0093a3b9ea484ba6ea7db9214d3bc0d379d6ecdd7ee3a7fdecb30b09cde0`  
		Last Modified: Sat, 24 Jun 2023 03:42:36 GMT  
		Size: 17.3 MB (17317987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d15fecfe4327fa2649e3f89e72313f0422c9437822bd74b524549b42db8b71d`  
		Last Modified: Sat, 24 Jun 2023 03:42:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e5df5c643dd2fedeee943bc8960602ba9ad5380bfca064d0a5172a881cf6ee`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a32c51db291cc48fecb9640f7f516872275591d2c22cc3a8936a86ad45dc7e3`  
		Last Modified: Sat, 24 Jun 2023 03:42:31 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b397682ddc1d0a0b22c92691691e7a787b2b7ac52eee263f47d7447edc8e336`  
		Last Modified: Sat, 24 Jun 2023 03:42:34 GMT  
		Size: 17.9 MB (17857148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415e61d7b47f78b19cafe15f8ec23830bbfd3cc09ba32b574c8b3709f9d9c73c`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250a626d9b7c309298042f6e5caa22099a134d01adf912982d92f40673f21ac5`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5e1fbabe536045bfb6179fb5a5f0a06799b9c4708f70d00df7b03848ea0ffe`  
		Last Modified: Tue, 04 Jul 2023 01:18:54 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1205d9c3f51c766ca715b96f2836a9a0a9178124ea20c0f037f7d384e959a66a`  
		Last Modified: Tue, 04 Jul 2023 01:18:58 GMT  
		Size: 18.5 MB (18456783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.6-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:9eebb50b9d3133014ca7138f450cdbe0d43901e15c71d0895a8b09751fcc22a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `docker:23.0.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:e16a9f4d6529304ae75e5e87b9676cf9de5698456bedc4791f0cf7a09420a56d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480280953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8419ea824aa11c888a44bb0ea52f5d804c08f13ff9828f5d8f125ffa44eb0c1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:37:22 GMT
ENV DOCKER_VERSION=23.0.6
# Sat, 24 Jun 2023 03:37:23 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.6.zip
# Sat, 24 Jun 2023 03:37:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:37:51 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:37:52 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:37:53 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:38:20 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:16:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:16:29 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:56 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e4d934aedb3408d39924086e00ca7aaad6ba9093494927ec3193aafd92a20f`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d47816062ca7fccecb96be7bf6468c4f36ffddd3115cf4d9bf244c0379bf7c`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0520b4152b36536d9d6e0fbb761f4d738b989c5b9bc20fdcb54002f3531479b5`  
		Last Modified: Sat, 24 Jun 2023 03:42:18 GMT  
		Size: 17.3 MB (17325743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29907b163c6b32e00b8763615b85445316f0e6cb7cd8c84e9e27ef2d3f409a1e`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99329c21e6a062ffac537c99b986885a8362333c37717e126cb5d88df72bfca3`  
		Last Modified: Sat, 24 Jun 2023 03:42:14 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ff267e35546ccc351184e91eb2272e461f812168c1c315fbc2ff57b7408600`  
		Last Modified: Sat, 24 Jun 2023 03:42:13 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be6b99421718086797da2255cb6dc64b1c37da7f21897b880a0e613168d72ce5`  
		Last Modified: Sat, 24 Jun 2023 03:42:16 GMT  
		Size: 17.9 MB (17867625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020919e393d62b234026651fe526978a97e7497d89f3729492f3845ccffa0ba1`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea00cd1e900add94d978485461ef3689853aa4df28a37aa9f323b472a6331d0`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9856084393b0037c77765698dc88b22c99e6245a2f4491290959963bb9f6cacc`  
		Last Modified: Tue, 04 Jul 2023 01:18:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13781f9f6fb0ab46635807dd978bb80fe0a32078b7942c0cc76b7aae45492698`  
		Last Modified: Tue, 04 Jul 2023 01:18:44 GMT  
		Size: 18.5 MB (18450181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24`

```console
$ docker pull docker@sha256:1d148deae16a6bb4c89224c636e1fd1799a4d5925f545861ce0d7bea3a527b5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24` - linux; amd64

```console
$ docker pull docker@sha256:d981b86555d31fb68b974505d0815223c027362a5802ad3ac394a0dabb0da658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118462458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5829c74e85fa07da97fd9037040924753901cd98940f67c2f226929786e9cd4b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5b01775c0863b42341d3df01481ff9ce1c712ade7f91f07c81cfed29bd042cc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109606522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae260d1409cdf7db300be0af648736f65e73c8145b04b4e904a75fcdde550313`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-cli`

```console
$ docker pull docker@sha256:7d93367e8dfc948b404112c84b1d73ecfaec5bc6ceca84ff9cf357bbd7b602e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24-cli` - linux; amd64

```console
$ docker pull docker@sha256:ea42d460ccff0758263eef66c8c1b409e996d54a2d121a2e1de3a8c6496794e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57221041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee66614da79015ee8107d72aba1b458d00cc1f4bfa720f609068c669efef0f55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:33b53c1858e9e6e91f84ad976efe9c27857eea849a9eb27184dece4d5916f0b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52849269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408670017333ebfd1dc30efbf3239bafa6b4d47ba3026f2c93fcc86accdd1a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-dind`

```console
$ docker pull docker@sha256:1d148deae16a6bb4c89224c636e1fd1799a4d5925f545861ce0d7bea3a527b5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24-dind` - linux; amd64

```console
$ docker pull docker@sha256:d981b86555d31fb68b974505d0815223c027362a5802ad3ac394a0dabb0da658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118462458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5829c74e85fa07da97fd9037040924753901cd98940f67c2f226929786e9cd4b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5b01775c0863b42341d3df01481ff9ce1c712ade7f91f07c81cfed29bd042cc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109606522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae260d1409cdf7db300be0af648736f65e73c8145b04b4e904a75fcdde550313`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-dind-rootless`

```console
$ docker pull docker@sha256:aef709e3162c6bc5d4b1c2f98096f54118be78291f2b01319927fb9aa4023863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:0e2aca3dc5e93360d18598e68fb58d7ca0f1733145f757e8f4de2920a2b86bad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140474708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309a0725f91644cb6d2cdccd50090e71ab9fff316c1cf28e84711d0bf8991f72`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Fri, 26 May 2023 11:04:23 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Fri, 26 May 2023 11:04:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 26 May 2023 11:04:23 GMT
USER rootless
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf16789a58c55457cee5b5dea3ac9ace1c4f15499986c26f2e13655c1b768dcd`  
		Last Modified: Tue, 04 Jul 2023 01:32:42 GMT  
		Size: 1.4 MB (1362406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbaa5522bc864948a64d63e75eac1b189c8e9a008ead5d970742f574c05c1e6c`  
		Last Modified: Tue, 04 Jul 2023 01:32:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf27a63fa4923d77203dda9ab8a72b4157fc19ae8922a02daa7bc25e9b9a4cb`  
		Last Modified: Tue, 04 Jul 2023 01:32:41 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282d809d9de1aeb57fb044c9300ba957a61ad3f1cfa0611d216a33a08f91cdf3`  
		Last Modified: Tue, 04 Jul 2023 01:32:44 GMT  
		Size: 20.6 MB (20648105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065b646c6e3ad529c817eceb5086bf765f719bb748cd49a5ca96182de3a11e51`  
		Last Modified: Tue, 04 Jul 2023 01:32:41 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:371d5cab8af7045313eb35e128caf9f6b37e2eefcb6592ccf388c8e63a36b721
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133468784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d60b9329aad0fb988800150f788731cbcba7523b0ca0b966400de69edc359711`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Fri, 26 May 2023 11:04:23 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Fri, 26 May 2023 11:04:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 26 May 2023 11:04:23 GMT
USER rootless
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f714784001e9d8c14948baac4835ded976982aac8a222a9b2a2791f59cd58d5`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 1.4 MB (1413240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66eabe53b410390d19d597c4ab31ee16cd0f77b5efa4e85e6d93fc1c3aeebfa`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65ef0e8cf7c2b897cd9fd8758cd812be95d2ae0f90bd4767c30b891e552e0ef`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c421e62f4bf588f68492e056bcd6c83f0a2752dc121219df0291109930a0d1e0`  
		Last Modified: Tue, 04 Jul 2023 00:41:24 GMT  
		Size: 22.4 MB (22447282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dced6027db50499673892f95086ef051e029d2a09bcb4054ec070467aa7c326f`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-git`

```console
$ docker pull docker@sha256:8a87af6545738a273b485a0dc4bff66735cf41cc35a23929027639edc49bb05b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24-git` - linux; amd64

```console
$ docker pull docker@sha256:c8ab7e6f31fffb628596df7f6d35c11a8be02ab1014dab3ee30a04d5c584389d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123397230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de733045dd40cde5dd291a537d3c3d3de017e80272edbd47826aff35c1472fe`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ef31e2ceed61978d174eb9f9cfa695a77d1017bec926abcf1faa8051505df3`  
		Last Modified: Tue, 04 Jul 2023 01:33:00 GMT  
		Size: 4.9 MB (4934772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:ddf472489fd7fc53ea4017e019fcb48b950f08bf1df50074e07401a5c446baa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114627613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:245bf306be8309dc02e78795a8df592aef3b174749650b2e835886a19923aa4b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e1282f386508ce93c06c9ec0d98b6d7e2bc6d2fcc51436d8132ac495359cf8`  
		Last Modified: Tue, 04 Jul 2023 00:41:38 GMT  
		Size: 5.0 MB (5021091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-windowsservercore`

```console
$ docker pull docker@sha256:b53edc69b4bfc7bda7ae78de45d5cef538690b0beb5dbc325485763cbf0b9589
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `docker:24-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:289b3bcbad32da3373061c8465cd16a6909eac54d333de0593d6707f58cefaf5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480392435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e048d92ef9dc0429997b83171a6c0e361b0a987366a8da4d5f7292260fc0cb79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:33:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:33:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:34:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:34:05 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:34:06 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:34:07 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:34:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:08 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:15:36 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422c57cfa4958bc0481159cf6f3ea51c62e434b415bd37af5122a927dad44e5`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038159acbdccb213594b93376d485aeeb899ddecb260c15c35876de1a826205`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de76d8841c57bd71ac348e6e5adafd8c4bb7b220dba2990cfb45212e8c02ec51`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 17.4 MB (17435791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601d2c848cc34db3244fd32712379ae9207438e92e8b1bfc93158f40c450b05f`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2546289e6eaf1c79435f5ebc3913d3400b9e48f9865fbac9a4f64a9631e16c`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7be502d4e9bbbfde8c8e153a1b773402566c1780fe74fc0ebd74481ab156a59`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a421c1544ba646557911d25deeb82872547032eda17bffad452d2d66dbe4714`  
		Last Modified: Sat, 24 Jun 2023 03:41:34 GMT  
		Size: 17.9 MB (17867701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39d4002a5465e2a54b5562a0a7b6a187bfaa7700be739499df976f3bc44d0ca`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef31be35c2ca19b058f5d6fea8c49089984e462a7994f4b3b84e66c9021d4124`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71959fbe60409fc46fb15bdaee5d9ce0320956c47afdd91fc1e2f83fc0e2c84`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9be1b06df89d2d6712ac575cdfddf225e926515586db03c65f6391c11f10bc`  
		Last Modified: Tue, 04 Jul 2023 01:18:08 GMT  
		Size: 18.5 MB (18450913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:f310a3854e7bf80794dcd9ff1c8cc30806fd9645b5a5717472b2fed1c2fc5537
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704797453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb5d4fa3d80518f588ad3eee4f7f6ee350dd0d2d76f23e98bf9bfa681733e74`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:35:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:35:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:36:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:36:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:36:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:36:10 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:36:41 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:44 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:18 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed839336f22dd57d3537286fd2cb28bb3fc0572198a3b9bd727227ee4cbdf055`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce643c4303a7b93be26b0dd0216711bedc40974b948aa175e501ebfd967e8da`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc026cb3268fba4d3f45b15b22d85c45b0833d7e6f03faf3f1adb1f7750eb889`  
		Last Modified: Sat, 24 Jun 2023 03:41:57 GMT  
		Size: 17.4 MB (17427965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ada76c0fbca30898687db44782375adfd8511d9f5fe79eb1df4524e36cb3b`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a336a464a58681af94fdcfb3fbc461c2ac77b4bd2d6ec0c339fbae654521420`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f6fe82d1e4f989c122320481c6c3473632cffcc634f225106e7c73585db1c7`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6f83ed64356628e46ae865b628bc2568b3e8679ec35b1c6211d4c49ee99d80`  
		Last Modified: Sat, 24 Jun 2023 03:41:55 GMT  
		Size: 17.9 MB (17857203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575bb31d4e1e844481bc4365c5a09edf18ca961693140e5fd407ab5a31943de7`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a439f4a0f428f900ced959aa5f68c22dac2269bff9bdd57b58fbc8f7d369589`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc63a64ccb561d80e3f36ce2e08139e02746ab4884c778ca92c4b867f445f6`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcee50f9938bfef5140021817f8dac5f7f2a23e6a07a960d54ac08bce33ee`  
		Last Modified: Tue, 04 Jul 2023 01:18:26 GMT  
		Size: 18.5 MB (18457426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-windowsservercore-1809`

```console
$ docker pull docker@sha256:0f5015bb466628fdfd18594e4de5b65e09631323ee555e80be32ae5dc8c138d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `docker:24-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:f310a3854e7bf80794dcd9ff1c8cc30806fd9645b5a5717472b2fed1c2fc5537
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704797453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb5d4fa3d80518f588ad3eee4f7f6ee350dd0d2d76f23e98bf9bfa681733e74`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:35:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:35:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:36:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:36:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:36:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:36:10 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:36:41 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:44 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:18 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed839336f22dd57d3537286fd2cb28bb3fc0572198a3b9bd727227ee4cbdf055`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce643c4303a7b93be26b0dd0216711bedc40974b948aa175e501ebfd967e8da`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc026cb3268fba4d3f45b15b22d85c45b0833d7e6f03faf3f1adb1f7750eb889`  
		Last Modified: Sat, 24 Jun 2023 03:41:57 GMT  
		Size: 17.4 MB (17427965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ada76c0fbca30898687db44782375adfd8511d9f5fe79eb1df4524e36cb3b`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a336a464a58681af94fdcfb3fbc461c2ac77b4bd2d6ec0c339fbae654521420`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f6fe82d1e4f989c122320481c6c3473632cffcc634f225106e7c73585db1c7`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6f83ed64356628e46ae865b628bc2568b3e8679ec35b1c6211d4c49ee99d80`  
		Last Modified: Sat, 24 Jun 2023 03:41:55 GMT  
		Size: 17.9 MB (17857203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575bb31d4e1e844481bc4365c5a09edf18ca961693140e5fd407ab5a31943de7`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a439f4a0f428f900ced959aa5f68c22dac2269bff9bdd57b58fbc8f7d369589`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc63a64ccb561d80e3f36ce2e08139e02746ab4884c778ca92c4b867f445f6`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcee50f9938bfef5140021817f8dac5f7f2a23e6a07a960d54ac08bce33ee`  
		Last Modified: Tue, 04 Jul 2023 01:18:26 GMT  
		Size: 18.5 MB (18457426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:d5627f339264d7d83b50ecf1e417b431507253f53a915f0dc398c6b2166baece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `docker:24-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:289b3bcbad32da3373061c8465cd16a6909eac54d333de0593d6707f58cefaf5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480392435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e048d92ef9dc0429997b83171a6c0e361b0a987366a8da4d5f7292260fc0cb79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:33:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:33:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:34:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:34:05 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:34:06 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:34:07 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:34:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:08 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:15:36 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422c57cfa4958bc0481159cf6f3ea51c62e434b415bd37af5122a927dad44e5`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038159acbdccb213594b93376d485aeeb899ddecb260c15c35876de1a826205`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de76d8841c57bd71ac348e6e5adafd8c4bb7b220dba2990cfb45212e8c02ec51`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 17.4 MB (17435791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601d2c848cc34db3244fd32712379ae9207438e92e8b1bfc93158f40c450b05f`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2546289e6eaf1c79435f5ebc3913d3400b9e48f9865fbac9a4f64a9631e16c`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7be502d4e9bbbfde8c8e153a1b773402566c1780fe74fc0ebd74481ab156a59`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a421c1544ba646557911d25deeb82872547032eda17bffad452d2d66dbe4714`  
		Last Modified: Sat, 24 Jun 2023 03:41:34 GMT  
		Size: 17.9 MB (17867701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39d4002a5465e2a54b5562a0a7b6a187bfaa7700be739499df976f3bc44d0ca`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef31be35c2ca19b058f5d6fea8c49089984e462a7994f4b3b84e66c9021d4124`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71959fbe60409fc46fb15bdaee5d9ce0320956c47afdd91fc1e2f83fc0e2c84`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9be1b06df89d2d6712ac575cdfddf225e926515586db03c65f6391c11f10bc`  
		Last Modified: Tue, 04 Jul 2023 01:18:08 GMT  
		Size: 18.5 MB (18450913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0`

```console
$ docker pull docker@sha256:1d148deae16a6bb4c89224c636e1fd1799a4d5925f545861ce0d7bea3a527b5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24.0` - linux; amd64

```console
$ docker pull docker@sha256:d981b86555d31fb68b974505d0815223c027362a5802ad3ac394a0dabb0da658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118462458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5829c74e85fa07da97fd9037040924753901cd98940f67c2f226929786e9cd4b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5b01775c0863b42341d3df01481ff9ce1c712ade7f91f07c81cfed29bd042cc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109606522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae260d1409cdf7db300be0af648736f65e73c8145b04b4e904a75fcdde550313`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-cli`

```console
$ docker pull docker@sha256:7d93367e8dfc948b404112c84b1d73ecfaec5bc6ceca84ff9cf357bbd7b602e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24.0-cli` - linux; amd64

```console
$ docker pull docker@sha256:ea42d460ccff0758263eef66c8c1b409e996d54a2d121a2e1de3a8c6496794e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57221041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee66614da79015ee8107d72aba1b458d00cc1f4bfa720f609068c669efef0f55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:33b53c1858e9e6e91f84ad976efe9c27857eea849a9eb27184dece4d5916f0b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52849269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408670017333ebfd1dc30efbf3239bafa6b4d47ba3026f2c93fcc86accdd1a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-dind`

```console
$ docker pull docker@sha256:1d148deae16a6bb4c89224c636e1fd1799a4d5925f545861ce0d7bea3a527b5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24.0-dind` - linux; amd64

```console
$ docker pull docker@sha256:d981b86555d31fb68b974505d0815223c027362a5802ad3ac394a0dabb0da658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118462458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5829c74e85fa07da97fd9037040924753901cd98940f67c2f226929786e9cd4b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5b01775c0863b42341d3df01481ff9ce1c712ade7f91f07c81cfed29bd042cc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109606522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae260d1409cdf7db300be0af648736f65e73c8145b04b4e904a75fcdde550313`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-dind-rootless`

```console
$ docker pull docker@sha256:aef709e3162c6bc5d4b1c2f98096f54118be78291f2b01319927fb9aa4023863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24.0-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:0e2aca3dc5e93360d18598e68fb58d7ca0f1733145f757e8f4de2920a2b86bad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140474708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309a0725f91644cb6d2cdccd50090e71ab9fff316c1cf28e84711d0bf8991f72`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Fri, 26 May 2023 11:04:23 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Fri, 26 May 2023 11:04:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 26 May 2023 11:04:23 GMT
USER rootless
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf16789a58c55457cee5b5dea3ac9ace1c4f15499986c26f2e13655c1b768dcd`  
		Last Modified: Tue, 04 Jul 2023 01:32:42 GMT  
		Size: 1.4 MB (1362406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbaa5522bc864948a64d63e75eac1b189c8e9a008ead5d970742f574c05c1e6c`  
		Last Modified: Tue, 04 Jul 2023 01:32:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf27a63fa4923d77203dda9ab8a72b4157fc19ae8922a02daa7bc25e9b9a4cb`  
		Last Modified: Tue, 04 Jul 2023 01:32:41 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282d809d9de1aeb57fb044c9300ba957a61ad3f1cfa0611d216a33a08f91cdf3`  
		Last Modified: Tue, 04 Jul 2023 01:32:44 GMT  
		Size: 20.6 MB (20648105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065b646c6e3ad529c817eceb5086bf765f719bb748cd49a5ca96182de3a11e51`  
		Last Modified: Tue, 04 Jul 2023 01:32:41 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:371d5cab8af7045313eb35e128caf9f6b37e2eefcb6592ccf388c8e63a36b721
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133468784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d60b9329aad0fb988800150f788731cbcba7523b0ca0b966400de69edc359711`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Fri, 26 May 2023 11:04:23 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Fri, 26 May 2023 11:04:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 26 May 2023 11:04:23 GMT
USER rootless
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f714784001e9d8c14948baac4835ded976982aac8a222a9b2a2791f59cd58d5`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 1.4 MB (1413240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66eabe53b410390d19d597c4ab31ee16cd0f77b5efa4e85e6d93fc1c3aeebfa`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65ef0e8cf7c2b897cd9fd8758cd812be95d2ae0f90bd4767c30b891e552e0ef`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c421e62f4bf588f68492e056bcd6c83f0a2752dc121219df0291109930a0d1e0`  
		Last Modified: Tue, 04 Jul 2023 00:41:24 GMT  
		Size: 22.4 MB (22447282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dced6027db50499673892f95086ef051e029d2a09bcb4054ec070467aa7c326f`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-git`

```console
$ docker pull docker@sha256:8a87af6545738a273b485a0dc4bff66735cf41cc35a23929027639edc49bb05b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:24.0-git` - linux; amd64

```console
$ docker pull docker@sha256:c8ab7e6f31fffb628596df7f6d35c11a8be02ab1014dab3ee30a04d5c584389d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123397230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de733045dd40cde5dd291a537d3c3d3de017e80272edbd47826aff35c1472fe`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ef31e2ceed61978d174eb9f9cfa695a77d1017bec926abcf1faa8051505df3`  
		Last Modified: Tue, 04 Jul 2023 01:33:00 GMT  
		Size: 4.9 MB (4934772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:ddf472489fd7fc53ea4017e019fcb48b950f08bf1df50074e07401a5c446baa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114627613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:245bf306be8309dc02e78795a8df592aef3b174749650b2e835886a19923aa4b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e1282f386508ce93c06c9ec0d98b6d7e2bc6d2fcc51436d8132ac495359cf8`  
		Last Modified: Tue, 04 Jul 2023 00:41:38 GMT  
		Size: 5.0 MB (5021091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-windowsservercore`

```console
$ docker pull docker@sha256:b53edc69b4bfc7bda7ae78de45d5cef538690b0beb5dbc325485763cbf0b9589
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `docker:24.0-windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:289b3bcbad32da3373061c8465cd16a6909eac54d333de0593d6707f58cefaf5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480392435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e048d92ef9dc0429997b83171a6c0e361b0a987366a8da4d5f7292260fc0cb79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:33:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:33:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:34:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:34:05 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:34:06 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:34:07 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:34:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:08 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:15:36 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422c57cfa4958bc0481159cf6f3ea51c62e434b415bd37af5122a927dad44e5`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038159acbdccb213594b93376d485aeeb899ddecb260c15c35876de1a826205`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de76d8841c57bd71ac348e6e5adafd8c4bb7b220dba2990cfb45212e8c02ec51`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 17.4 MB (17435791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601d2c848cc34db3244fd32712379ae9207438e92e8b1bfc93158f40c450b05f`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2546289e6eaf1c79435f5ebc3913d3400b9e48f9865fbac9a4f64a9631e16c`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7be502d4e9bbbfde8c8e153a1b773402566c1780fe74fc0ebd74481ab156a59`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a421c1544ba646557911d25deeb82872547032eda17bffad452d2d66dbe4714`  
		Last Modified: Sat, 24 Jun 2023 03:41:34 GMT  
		Size: 17.9 MB (17867701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39d4002a5465e2a54b5562a0a7b6a187bfaa7700be739499df976f3bc44d0ca`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef31be35c2ca19b058f5d6fea8c49089984e462a7994f4b3b84e66c9021d4124`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71959fbe60409fc46fb15bdaee5d9ce0320956c47afdd91fc1e2f83fc0e2c84`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9be1b06df89d2d6712ac575cdfddf225e926515586db03c65f6391c11f10bc`  
		Last Modified: Tue, 04 Jul 2023 01:18:08 GMT  
		Size: 18.5 MB (18450913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24.0-windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:f310a3854e7bf80794dcd9ff1c8cc30806fd9645b5a5717472b2fed1c2fc5537
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704797453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb5d4fa3d80518f588ad3eee4f7f6ee350dd0d2d76f23e98bf9bfa681733e74`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:35:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:35:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:36:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:36:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:36:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:36:10 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:36:41 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:44 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:18 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed839336f22dd57d3537286fd2cb28bb3fc0572198a3b9bd727227ee4cbdf055`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce643c4303a7b93be26b0dd0216711bedc40974b948aa175e501ebfd967e8da`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc026cb3268fba4d3f45b15b22d85c45b0833d7e6f03faf3f1adb1f7750eb889`  
		Last Modified: Sat, 24 Jun 2023 03:41:57 GMT  
		Size: 17.4 MB (17427965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ada76c0fbca30898687db44782375adfd8511d9f5fe79eb1df4524e36cb3b`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a336a464a58681af94fdcfb3fbc461c2ac77b4bd2d6ec0c339fbae654521420`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f6fe82d1e4f989c122320481c6c3473632cffcc634f225106e7c73585db1c7`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6f83ed64356628e46ae865b628bc2568b3e8679ec35b1c6211d4c49ee99d80`  
		Last Modified: Sat, 24 Jun 2023 03:41:55 GMT  
		Size: 17.9 MB (17857203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575bb31d4e1e844481bc4365c5a09edf18ca961693140e5fd407ab5a31943de7`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a439f4a0f428f900ced959aa5f68c22dac2269bff9bdd57b58fbc8f7d369589`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc63a64ccb561d80e3f36ce2e08139e02746ab4884c778ca92c4b867f445f6`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcee50f9938bfef5140021817f8dac5f7f2a23e6a07a960d54ac08bce33ee`  
		Last Modified: Tue, 04 Jul 2023 01:18:26 GMT  
		Size: 18.5 MB (18457426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-windowsservercore-1809`

```console
$ docker pull docker@sha256:0f5015bb466628fdfd18594e4de5b65e09631323ee555e80be32ae5dc8c138d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `docker:24.0-windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:f310a3854e7bf80794dcd9ff1c8cc30806fd9645b5a5717472b2fed1c2fc5537
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704797453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb5d4fa3d80518f588ad3eee4f7f6ee350dd0d2d76f23e98bf9bfa681733e74`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:35:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:35:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:36:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:36:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:36:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:36:10 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:36:41 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:44 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:18 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed839336f22dd57d3537286fd2cb28bb3fc0572198a3b9bd727227ee4cbdf055`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce643c4303a7b93be26b0dd0216711bedc40974b948aa175e501ebfd967e8da`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc026cb3268fba4d3f45b15b22d85c45b0833d7e6f03faf3f1adb1f7750eb889`  
		Last Modified: Sat, 24 Jun 2023 03:41:57 GMT  
		Size: 17.4 MB (17427965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ada76c0fbca30898687db44782375adfd8511d9f5fe79eb1df4524e36cb3b`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a336a464a58681af94fdcfb3fbc461c2ac77b4bd2d6ec0c339fbae654521420`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f6fe82d1e4f989c122320481c6c3473632cffcc634f225106e7c73585db1c7`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6f83ed64356628e46ae865b628bc2568b3e8679ec35b1c6211d4c49ee99d80`  
		Last Modified: Sat, 24 Jun 2023 03:41:55 GMT  
		Size: 17.9 MB (17857203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575bb31d4e1e844481bc4365c5a09edf18ca961693140e5fd407ab5a31943de7`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a439f4a0f428f900ced959aa5f68c22dac2269bff9bdd57b58fbc8f7d369589`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc63a64ccb561d80e3f36ce2e08139e02746ab4884c778ca92c4b867f445f6`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcee50f9938bfef5140021817f8dac5f7f2a23e6a07a960d54ac08bce33ee`  
		Last Modified: Tue, 04 Jul 2023 01:18:26 GMT  
		Size: 18.5 MB (18457426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:d5627f339264d7d83b50ecf1e417b431507253f53a915f0dc398c6b2166baece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `docker:24.0-windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:289b3bcbad32da3373061c8465cd16a6909eac54d333de0593d6707f58cefaf5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480392435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e048d92ef9dc0429997b83171a6c0e361b0a987366a8da4d5f7292260fc0cb79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:33:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:33:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:34:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:34:05 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:34:06 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:34:07 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:34:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:08 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:15:36 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422c57cfa4958bc0481159cf6f3ea51c62e434b415bd37af5122a927dad44e5`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038159acbdccb213594b93376d485aeeb899ddecb260c15c35876de1a826205`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de76d8841c57bd71ac348e6e5adafd8c4bb7b220dba2990cfb45212e8c02ec51`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 17.4 MB (17435791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601d2c848cc34db3244fd32712379ae9207438e92e8b1bfc93158f40c450b05f`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2546289e6eaf1c79435f5ebc3913d3400b9e48f9865fbac9a4f64a9631e16c`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7be502d4e9bbbfde8c8e153a1b773402566c1780fe74fc0ebd74481ab156a59`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a421c1544ba646557911d25deeb82872547032eda17bffad452d2d66dbe4714`  
		Last Modified: Sat, 24 Jun 2023 03:41:34 GMT  
		Size: 17.9 MB (17867701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39d4002a5465e2a54b5562a0a7b6a187bfaa7700be739499df976f3bc44d0ca`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef31be35c2ca19b058f5d6fea8c49089984e462a7994f4b3b84e66c9021d4124`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71959fbe60409fc46fb15bdaee5d9ce0320956c47afdd91fc1e2f83fc0e2c84`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9be1b06df89d2d6712ac575cdfddf225e926515586db03c65f6391c11f10bc`  
		Last Modified: Tue, 04 Jul 2023 01:18:08 GMT  
		Size: 18.5 MB (18450913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:24.0.3`

**does not exist** (yet?)

## `docker:24.0.3-alpine3.18`

**does not exist** (yet?)

## `docker:24.0.3-cli`

**does not exist** (yet?)

## `docker:24.0.3-cli-alpine3.18`

**does not exist** (yet?)

## `docker:24.0.3-dind`

**does not exist** (yet?)

## `docker:24.0.3-dind-alpine3.18`

**does not exist** (yet?)

## `docker:24.0.3-dind-rootless`

**does not exist** (yet?)

## `docker:24.0.3-git`

**does not exist** (yet?)

## `docker:24.0.3-windowsservercore`

**does not exist** (yet?)

## `docker:24.0.3-windowsservercore-1809`

**does not exist** (yet?)

## `docker:24.0.3-windowsservercore-ltsc2022`

**does not exist** (yet?)

## `docker:cli`

```console
$ docker pull docker@sha256:7d93367e8dfc948b404112c84b1d73ecfaec5bc6ceca84ff9cf357bbd7b602e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:cli` - linux; amd64

```console
$ docker pull docker@sha256:ea42d460ccff0758263eef66c8c1b409e996d54a2d121a2e1de3a8c6496794e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57221041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee66614da79015ee8107d72aba1b458d00cc1f4bfa720f609068c669efef0f55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:33b53c1858e9e6e91f84ad976efe9c27857eea849a9eb27184dece4d5916f0b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52849269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408670017333ebfd1dc30efbf3239bafa6b4d47ba3026f2c93fcc86accdd1a33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:1d148deae16a6bb4c89224c636e1fd1799a4d5925f545861ce0d7bea3a527b5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:d981b86555d31fb68b974505d0815223c027362a5802ad3ac394a0dabb0da658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118462458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5829c74e85fa07da97fd9037040924753901cd98940f67c2f226929786e9cd4b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5b01775c0863b42341d3df01481ff9ce1c712ade7f91f07c81cfed29bd042cc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109606522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae260d1409cdf7db300be0af648736f65e73c8145b04b4e904a75fcdde550313`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:aef709e3162c6bc5d4b1c2f98096f54118be78291f2b01319927fb9aa4023863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:0e2aca3dc5e93360d18598e68fb58d7ca0f1733145f757e8f4de2920a2b86bad
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140474708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:309a0725f91644cb6d2cdccd50090e71ab9fff316c1cf28e84711d0bf8991f72`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Fri, 26 May 2023 11:04:23 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Fri, 26 May 2023 11:04:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 26 May 2023 11:04:23 GMT
USER rootless
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf16789a58c55457cee5b5dea3ac9ace1c4f15499986c26f2e13655c1b768dcd`  
		Last Modified: Tue, 04 Jul 2023 01:32:42 GMT  
		Size: 1.4 MB (1362406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbaa5522bc864948a64d63e75eac1b189c8e9a008ead5d970742f574c05c1e6c`  
		Last Modified: Tue, 04 Jul 2023 01:32:41 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf27a63fa4923d77203dda9ab8a72b4157fc19ae8922a02daa7bc25e9b9a4cb`  
		Last Modified: Tue, 04 Jul 2023 01:32:41 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282d809d9de1aeb57fb044c9300ba957a61ad3f1cfa0611d216a33a08f91cdf3`  
		Last Modified: Tue, 04 Jul 2023 01:32:44 GMT  
		Size: 20.6 MB (20648105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:065b646c6e3ad529c817eceb5086bf765f719bb748cd49a5ca96182de3a11e51`  
		Last Modified: Tue, 04 Jul 2023 01:32:41 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:371d5cab8af7045313eb35e128caf9f6b37e2eefcb6592ccf388c8e63a36b721
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.5 MB (133468784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d60b9329aad0fb988800150f788731cbcba7523b0ca0b966400de69edc359711`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Fri, 26 May 2023 11:04:23 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Fri, 26 May 2023 11:04:23 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Fri, 26 May 2023 11:04:23 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 26 May 2023 11:04:23 GMT
USER rootless
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f714784001e9d8c14948baac4835ded976982aac8a222a9b2a2791f59cd58d5`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 1.4 MB (1413240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66eabe53b410390d19d597c4ab31ee16cd0f77b5efa4e85e6d93fc1c3aeebfa`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65ef0e8cf7c2b897cd9fd8758cd812be95d2ae0f90bd4767c30b891e552e0ef`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c421e62f4bf588f68492e056bcd6c83f0a2752dc121219df0291109930a0d1e0`  
		Last Modified: Tue, 04 Jul 2023 00:41:24 GMT  
		Size: 22.4 MB (22447282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dced6027db50499673892f95086ef051e029d2a09bcb4054ec070467aa7c326f`  
		Last Modified: Tue, 04 Jul 2023 00:41:21 GMT  
		Size: 232.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:8a87af6545738a273b485a0dc4bff66735cf41cc35a23929027639edc49bb05b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:c8ab7e6f31fffb628596df7f6d35c11a8be02ab1014dab3ee30a04d5c584389d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123397230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3de733045dd40cde5dd291a537d3c3d3de017e80272edbd47826aff35c1472fe`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ef31e2ceed61978d174eb9f9cfa695a77d1017bec926abcf1faa8051505df3`  
		Last Modified: Tue, 04 Jul 2023 01:33:00 GMT  
		Size: 4.9 MB (4934772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:ddf472489fd7fc53ea4017e019fcb48b950f08bf1df50074e07401a5c446baa6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114627613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:245bf306be8309dc02e78795a8df592aef3b174749650b2e835886a19923aa4b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e1282f386508ce93c06c9ec0d98b6d7e2bc6d2fcc51436d8132ac495359cf8`  
		Last Modified: Tue, 04 Jul 2023 00:41:38 GMT  
		Size: 5.0 MB (5021091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:1d148deae16a6bb4c89224c636e1fd1799a4d5925f545861ce0d7bea3a527b5d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:d981b86555d31fb68b974505d0815223c027362a5802ad3ac394a0dabb0da658
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.5 MB (118462458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5829c74e85fa07da97fd9037040924753901cd98940f67c2f226929786e9cd4b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366db03861711486fedda5cd6f1359c0261a1734594df3a61eafc2e920d92488`  
		Last Modified: Thu, 15 Jun 2023 05:27:07 GMT  
		Size: 16.4 MB (16376159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e922f84bca8da20b7db33748ee6660acc3629598bc8e5f5e7bc158c08339a426`  
		Last Modified: Thu, 15 Jun 2023 05:27:06 GMT  
		Size: 17.5 MB (17450708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3902146b3c46c6168444617531cabde93ac2800250169780e9153cf2c41a72`  
		Last Modified: Tue, 04 Jul 2023 01:31:54 GMT  
		Size: 18.0 MB (17980096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c407b77f4b2987302e5778118d91c624c1f02f653adb0c9e8fbbb4c8561b40`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f473f68c87d22432d3bb28b534950ca78ce73f4ad06c2721deceba0f3bada4`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99903b5ac087c63365fa406168088ef45ebca142b9ce332b3562798e058eb2a0`  
		Last Modified: Tue, 04 Jul 2023 01:31:51 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f3adbfe76ad4c497c7d39bfdfc931a5a16925a5df1e58ad32ef4e3cac01b032`  
		Last Modified: Tue, 04 Jul 2023 01:32:09 GMT  
		Size: 7.1 MB (7080772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0c77d852f955b8535ce43427aa17d43b1e2eeefd43f330c4be26afc425bd99`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba42c39435b7f9701729259cc6267250c887d64f2668dd70f97a48caa6c9cdb`  
		Last Modified: Tue, 04 Jul 2023 01:32:15 GMT  
		Size: 54.2 MB (54155477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ceb275b87685d6266bd75f8ed9064daecf849613b483cc0c118b65c94f4bea`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c79f2b8e75d82359462fd731751c953b220f312858e701b064bf0d8d14d246`  
		Last Modified: Tue, 04 Jul 2023 01:32:08 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5b01775c0863b42341d3df01481ff9ce1c712ade7f91f07c81cfed29bd042cc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109606522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae260d1409cdf7db300be0af648736f65e73c8145b04b4e904a75fcdde550313`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_VERSION=24.0.2
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-amd64'; 			sha256='ec2c9da22c3b733ad96d6a6897750153d884f1b2b86f2864ee5f743ce931055d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v6'; 			sha256='a925462288a55b709a42431fe39bb0e67f033961f02a4754897c4a388355feea'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm-v7'; 			sha256='e3f18a0d10346d8e53aff743fccfc0b95e45dc0235c3b0b72b49d3452c72b9e0'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-arm64'; 			sha256='e50f34f8feb7004407f826a375090bec6191891c473347b41b05cf5864bc5240'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-ppc64le'; 			sha256='de8670ab6b2c34feb32289d04af07014bb4517de879d1fdb6e31a00da28f1df4'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-riscv64'; 			sha256='a07ad5791d6e60094e38147ef5f5eac406b2692aa380eae5ac866bde91bcdc89'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.linux-s390x'; 			sha256='fc1a57b9fb69f7736908bbea94013eb17b5ae03cd5ed99b0bd61e223f9b6e4a7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Thu, 29 Jun 2023 23:05:40 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Jun 2023 23:05:40 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 29 Jun 2023 23:05:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Jun 2023 23:05:40 GMT
CMD ["sh"]
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 30 May 2023 23:05:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 30 May 2023 23:05:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 30 May 2023 23:05:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 30 May 2023 23:05:39 GMT
VOLUME [/var/lib/docker]
# Tue, 30 May 2023 23:05:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 30 May 2023 23:05:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 30 May 2023 23:05:39 GMT
CMD []
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9586bf63fa36870e788c8a018102294740f7423584b67cd9109415feef2bfd5e`  
		Last Modified: Wed, 14 Jun 2023 22:40:53 GMT  
		Size: 15.4 MB (15422673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1478b55d813a1aa989a4c3214a2e2dc0570eec3865fceae167d1ee66a440f4`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 15.8 MB (15758023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fdc50f005e049694ace3914d5f1f6136e60a11bc5fb52e3674636187dfce13`  
		Last Modified: Tue, 04 Jul 2023 00:40:34 GMT  
		Size: 16.3 MB (16312961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18eaf9e0867e77c4aae4ae3ee7f8498ee6910b33df6cc7d7aabb052254ccf0e`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288c6f8cca98a591de3bef3f72fa6e72fa05dc48bb7c151357d269f105e282c0`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003c443699d93502858aade5b1103c74cb7f7b79f755eafde9b1707109ceebc`  
		Last Modified: Tue, 04 Jul 2023 00:40:32 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1122c74b8be96849feb2df27205900943e9489cbbbc1514aee6341f89ebabe58`  
		Last Modified: Tue, 04 Jul 2023 00:40:49 GMT  
		Size: 7.3 MB (7291367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0511e4472f995553892e3e9eae1730dc479f27d73911845e35b8a648960a6c`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a8d1362fe35fbba16eb34c7b62a9f554d6d09db79e1560094c8a1b0e9586c`  
		Last Modified: Tue, 04 Jul 2023 00:40:53 GMT  
		Size: 49.5 MB (49460720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26e466edb290083b7bad6147362cf043f9ea4c75d3880f27f6efe5c1d593202`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f5cadd9777ec0b50d9325a74a31b97784cf9fd06e98da3436edda7c2bc4003`  
		Last Modified: Tue, 04 Jul 2023 00:40:48 GMT  
		Size: 2.8 KB (2795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:b53edc69b4bfc7bda7ae78de45d5cef538690b0beb5dbc325485763cbf0b9589
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1787; amd64
	-	windows version 10.0.17763.4499; amd64

### `docker:windowsservercore` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:289b3bcbad32da3373061c8465cd16a6909eac54d333de0593d6707f58cefaf5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480392435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e048d92ef9dc0429997b83171a6c0e361b0a987366a8da4d5f7292260fc0cb79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:33:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:33:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:34:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:34:05 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:34:06 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:34:07 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:34:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:08 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:15:36 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422c57cfa4958bc0481159cf6f3ea51c62e434b415bd37af5122a927dad44e5`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038159acbdccb213594b93376d485aeeb899ddecb260c15c35876de1a826205`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de76d8841c57bd71ac348e6e5adafd8c4bb7b220dba2990cfb45212e8c02ec51`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 17.4 MB (17435791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601d2c848cc34db3244fd32712379ae9207438e92e8b1bfc93158f40c450b05f`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2546289e6eaf1c79435f5ebc3913d3400b9e48f9865fbac9a4f64a9631e16c`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7be502d4e9bbbfde8c8e153a1b773402566c1780fe74fc0ebd74481ab156a59`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a421c1544ba646557911d25deeb82872547032eda17bffad452d2d66dbe4714`  
		Last Modified: Sat, 24 Jun 2023 03:41:34 GMT  
		Size: 17.9 MB (17867701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39d4002a5465e2a54b5562a0a7b6a187bfaa7700be739499df976f3bc44d0ca`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef31be35c2ca19b058f5d6fea8c49089984e462a7994f4b3b84e66c9021d4124`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71959fbe60409fc46fb15bdaee5d9ce0320956c47afdd91fc1e2f83fc0e2c84`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9be1b06df89d2d6712ac575cdfddf225e926515586db03c65f6391c11f10bc`  
		Last Modified: Tue, 04 Jul 2023 01:18:08 GMT  
		Size: 18.5 MB (18450913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:f310a3854e7bf80794dcd9ff1c8cc30806fd9645b5a5717472b2fed1c2fc5537
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704797453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb5d4fa3d80518f588ad3eee4f7f6ee350dd0d2d76f23e98bf9bfa681733e74`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:35:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:35:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:36:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:36:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:36:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:36:10 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:36:41 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:44 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:18 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed839336f22dd57d3537286fd2cb28bb3fc0572198a3b9bd727227ee4cbdf055`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce643c4303a7b93be26b0dd0216711bedc40974b948aa175e501ebfd967e8da`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc026cb3268fba4d3f45b15b22d85c45b0833d7e6f03faf3f1adb1f7750eb889`  
		Last Modified: Sat, 24 Jun 2023 03:41:57 GMT  
		Size: 17.4 MB (17427965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ada76c0fbca30898687db44782375adfd8511d9f5fe79eb1df4524e36cb3b`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a336a464a58681af94fdcfb3fbc461c2ac77b4bd2d6ec0c339fbae654521420`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f6fe82d1e4f989c122320481c6c3473632cffcc634f225106e7c73585db1c7`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6f83ed64356628e46ae865b628bc2568b3e8679ec35b1c6211d4c49ee99d80`  
		Last Modified: Sat, 24 Jun 2023 03:41:55 GMT  
		Size: 17.9 MB (17857203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575bb31d4e1e844481bc4365c5a09edf18ca961693140e5fd407ab5a31943de7`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a439f4a0f428f900ced959aa5f68c22dac2269bff9bdd57b58fbc8f7d369589`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc63a64ccb561d80e3f36ce2e08139e02746ab4884c778ca92c4b867f445f6`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcee50f9938bfef5140021817f8dac5f7f2a23e6a07a960d54ac08bce33ee`  
		Last Modified: Tue, 04 Jul 2023 01:18:26 GMT  
		Size: 18.5 MB (18457426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:0f5015bb466628fdfd18594e4de5b65e09631323ee555e80be32ae5dc8c138d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4499; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.4499; amd64

```console
$ docker pull docker@sha256:f310a3854e7bf80794dcd9ff1c8cc30806fd9645b5a5717472b2fed1c2fc5537
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1704797453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb5d4fa3d80518f588ad3eee4f7f6ee350dd0d2d76f23e98bf9bfa681733e74`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:47:17 GMT
RUN Apply image 10.0.17763.4499
# Sat, 24 Jun 2023 00:40:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:35:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:35:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:35:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:36:07 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:36:08 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:36:09 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:36:10 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:36:41 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:44 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:45 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:16:18 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b1471cc22404d036d95728a9c37c1e3f025a1f0a331072c8613e38cf8f7ff1ed`  
		Last Modified: Fri, 23 Jun 2023 02:36:08 GMT  
		Size: 1.7 GB (1650736778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58717a727cd3a756d7c1180dfb74e95d49735ed12628bd25d2058bc90fa96991`  
		Last Modified: Sat, 24 Jun 2023 01:20:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb210483c7a5877c9d4e754a46a0085ff94bc31d9e32e64c37e1ed4d6e30162e`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 306.0 KB (305975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed839336f22dd57d3537286fd2cb28bb3fc0572198a3b9bd727227ee4cbdf055`  
		Last Modified: Sat, 24 Jun 2023 03:41:56 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce643c4303a7b93be26b0dd0216711bedc40974b948aa175e501ebfd967e8da`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc026cb3268fba4d3f45b15b22d85c45b0833d7e6f03faf3f1adb1f7750eb889`  
		Last Modified: Sat, 24 Jun 2023 03:41:57 GMT  
		Size: 17.4 MB (17427965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ada76c0fbca30898687db44782375adfd8511d9f5fe79eb1df4524e36cb3b`  
		Last Modified: Sat, 24 Jun 2023 03:41:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a336a464a58681af94fdcfb3fbc461c2ac77b4bd2d6ec0c339fbae654521420`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f6fe82d1e4f989c122320481c6c3473632cffcc634f225106e7c73585db1c7`  
		Last Modified: Sat, 24 Jun 2023 03:41:52 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6f83ed64356628e46ae865b628bc2568b3e8679ec35b1c6211d4c49ee99d80`  
		Last Modified: Sat, 24 Jun 2023 03:41:55 GMT  
		Size: 17.9 MB (17857203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:575bb31d4e1e844481bc4365c5a09edf18ca961693140e5fd407ab5a31943de7`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a439f4a0f428f900ced959aa5f68c22dac2269bff9bdd57b58fbc8f7d369589`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc63a64ccb561d80e3f36ce2e08139e02746ab4884c778ca92c4b867f445f6`  
		Last Modified: Tue, 04 Jul 2023 01:18:22 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5bcee50f9938bfef5140021817f8dac5f7f2a23e6a07a960d54ac08bce33ee`  
		Last Modified: Tue, 04 Jul 2023 01:18:26 GMT  
		Size: 18.5 MB (18457426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:d5627f339264d7d83b50ecf1e417b431507253f53a915f0dc398c6b2166baece
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull docker@sha256:289b3bcbad32da3373061c8465cd16a6909eac54d333de0593d6707f58cefaf5
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.5 GB (1480392435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e048d92ef9dc0429997b83171a6c0e361b0a987366a8da4d5f7292260fc0cb79`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Wed, 21 Jun 2023 08:51:34 GMT
RUN Apply image 10.0.20348.1787
# Sat, 24 Jun 2023 00:38:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Sat, 24 Jun 2023 03:33:33 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 24 Jun 2023 03:33:34 GMT
ENV DOCKER_VERSION=24.0.2
# Sat, 24 Jun 2023 03:33:35 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-24.0.2.zip
# Sat, 24 Jun 2023 03:34:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
# Sat, 24 Jun 2023 03:34:05 GMT
ENV DOCKER_BUILDX_VERSION=0.11.0
# Sat, 24 Jun 2023 03:34:06 GMT
ENV DOCKER_BUILDX_URL=https://github.com/docker/buildx/releases/download/v0.11.0/buildx-v0.11.0.windows-amd64.exe
# Sat, 24 Jun 2023 03:34:07 GMT
ENV DOCKER_BUILDX_SHA256=e314569943a591a097fa9119bf786556a4eb5c710e8ddefa57e95cd95aa7cc7f
# Sat, 24 Jun 2023 03:34:34 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-buildx.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_BUILDX_URL); 	Invoke-WebRequest -Uri $env:DOCKER_BUILDX_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_BUILDX_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_BUILDX_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker buildx version") ...'; 	docker buildx version; 		Write-Host 'Complete.';
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Tue, 04 Jul 2023 01:15:07 GMT
ENV DOCKER_COMPOSE_URL=https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-windows-x86_64.exe
# Tue, 04 Jul 2023 01:15:08 GMT
ENV DOCKER_COMPOSE_SHA256=e77e4764e939782d27570fc17a6029b63fe922ebce6800128dfe1c047a9395ed
# Tue, 04 Jul 2023 01:15:36 GMT
RUN $dir = ('{0}\docker\cli-plugins' -f $env:ProgramFiles); 	Write-Host ('Creating {0} ...' -f $dir); 	New-Item -ItemType Directory $dir -Force; 		$plugin = ('{0}\docker-compose.exe' -f $dir); 	Write-Host ('Downloading {0} ...' -f $env:DOCKER_COMPOSE_URL); 	Invoke-WebRequest -Uri $env:DOCKER_COMPOSE_URL -OutFile $plugin; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:DOCKER_COMPOSE_SHA256); 	if ((Get-FileHash $plugin -Algorithm sha256).Hash -ne $env:DOCKER_COMPOSE_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Verifying install ("docker compose version") ...'; 	docker compose version; 		$link = ('{0}\docker\docker-compose.exe' -f $env:ProgramFiles); 	Write-Host ('Linking {0} to {1} ...' -f $plugin, $link); 	New-Item -ItemType SymbolicLink -Path $link -Target $plugin; 		Write-Host 'Verifying install ("docker-compose --version") ...'; 	docker-compose --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:0ce49598e7371c2c318cfa408f639c917d1f43843fb9e0a3316db1ba7fbb14db`  
		Last Modified: Fri, 23 Jun 2023 03:10:46 GMT  
		Size: 1.4 GB (1426298723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27db350c833f7fe0378bc977cd819c1ffe4133ff02ff69f1531f8ddc552c2366`  
		Last Modified: Sat, 24 Jun 2023 01:15:58 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c818796445a77806e10e6c159d076d6b0f5105edd8e7f27848042efb890970dd`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 326.7 KB (326673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9422c57cfa4958bc0481159cf6f3ea51c62e434b415bd37af5122a927dad44e5`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3038159acbdccb213594b93376d485aeeb899ddecb260c15c35876de1a826205`  
		Last Modified: Sat, 24 Jun 2023 03:41:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de76d8841c57bd71ac348e6e5adafd8c4bb7b220dba2990cfb45212e8c02ec51`  
		Last Modified: Sat, 24 Jun 2023 03:41:36 GMT  
		Size: 17.4 MB (17435791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601d2c848cc34db3244fd32712379ae9207438e92e8b1bfc93158f40c450b05f`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2546289e6eaf1c79435f5ebc3913d3400b9e48f9865fbac9a4f64a9631e16c`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7be502d4e9bbbfde8c8e153a1b773402566c1780fe74fc0ebd74481ab156a59`  
		Last Modified: Sat, 24 Jun 2023 03:41:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a421c1544ba646557911d25deeb82872547032eda17bffad452d2d66dbe4714`  
		Last Modified: Sat, 24 Jun 2023 03:41:34 GMT  
		Size: 17.9 MB (17867701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39d4002a5465e2a54b5562a0a7b6a187bfaa7700be739499df976f3bc44d0ca`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef31be35c2ca19b058f5d6fea8c49089984e462a7994f4b3b84e66c9021d4124`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a71959fbe60409fc46fb15bdaee5d9ce0320956c47afdd91fc1e2f83fc0e2c84`  
		Last Modified: Tue, 04 Jul 2023 01:18:04 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9be1b06df89d2d6712ac575cdfddf225e926515586db03c65f6391c11f10bc`  
		Last Modified: Tue, 04 Jul 2023 01:18:08 GMT  
		Size: 18.5 MB (18450913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
