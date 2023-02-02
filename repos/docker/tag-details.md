<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `docker`

-	[`docker:20`](#docker20)
-	[`docker:20-cli`](#docker20-cli)
-	[`docker:20-dind`](#docker20-dind)
-	[`docker:20-dind-rootless`](#docker20-dind-rootless)
-	[`docker:20-git`](#docker20-git)
-	[`docker:20-windowsservercore`](#docker20-windowsservercore)
-	[`docker:20-windowsservercore-1809`](#docker20-windowsservercore-1809)
-	[`docker:20-windowsservercore-ltsc2022`](#docker20-windowsservercore-ltsc2022)
-	[`docker:20.10`](#docker2010)
-	[`docker:20.10-cli`](#docker2010-cli)
-	[`docker:20.10-dind`](#docker2010-dind)
-	[`docker:20.10-dind-rootless`](#docker2010-dind-rootless)
-	[`docker:20.10-git`](#docker2010-git)
-	[`docker:20.10-windowsservercore`](#docker2010-windowsservercore)
-	[`docker:20.10-windowsservercore-1809`](#docker2010-windowsservercore-1809)
-	[`docker:20.10-windowsservercore-ltsc2022`](#docker2010-windowsservercore-ltsc2022)
-	[`docker:20.10.23`](#docker201023)
-	[`docker:20.10.23-alpine3.17`](#docker201023-alpine317)
-	[`docker:20.10.23-cli`](#docker201023-cli)
-	[`docker:20.10.23-cli-alpine3.17`](#docker201023-cli-alpine317)
-	[`docker:20.10.23-dind`](#docker201023-dind)
-	[`docker:20.10.23-dind-alpine3.17`](#docker201023-dind-alpine317)
-	[`docker:20.10.23-dind-rootless`](#docker201023-dind-rootless)
-	[`docker:20.10.23-git`](#docker201023-git)
-	[`docker:20.10.23-windowsservercore`](#docker201023-windowsservercore)
-	[`docker:20.10.23-windowsservercore-1809`](#docker201023-windowsservercore-1809)
-	[`docker:20.10.23-windowsservercore-ltsc2022`](#docker201023-windowsservercore-ltsc2022)
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
-	[`docker:23.0.0`](#docker2300)
-	[`docker:23.0.0-alpine3.17`](#docker2300-alpine317)
-	[`docker:23.0.0-cli`](#docker2300-cli)
-	[`docker:23.0.0-cli-alpine3.17`](#docker2300-cli-alpine317)
-	[`docker:23.0.0-dind`](#docker2300-dind)
-	[`docker:23.0.0-dind-alpine3.17`](#docker2300-dind-alpine317)
-	[`docker:23.0.0-dind-rootless`](#docker2300-dind-rootless)
-	[`docker:23.0.0-git`](#docker2300-git)
-	[`docker:23.0.0-windowsservercore`](#docker2300-windowsservercore)
-	[`docker:23.0.0-windowsservercore-1809`](#docker2300-windowsservercore-1809)
-	[`docker:23.0.0-windowsservercore-ltsc2022`](#docker2300-windowsservercore-ltsc2022)
-	[`docker:cli`](#dockercli)
-	[`docker:dind`](#dockerdind)
-	[`docker:dind-rootless`](#dockerdind-rootless)
-	[`docker:git`](#dockergit)
-	[`docker:latest`](#dockerlatest)
-	[`docker:windowsservercore`](#dockerwindowsservercore)
-	[`docker:windowsservercore-1809`](#dockerwindowsservercore-1809)
-	[`docker:windowsservercore-ltsc2022`](#dockerwindowsservercore-ltsc2022)

## `docker:20`

```console
$ docker pull docker@sha256:2245cd9cd5bc068987a1d3fd9eede6faf8231b396bba968234fffbeb01b09648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:c53db7693d089e1f9cd5267253e3885b394d48df2722f85e21232e101d7c30b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49906275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c69eddee82bdf5a05bc7fd67029f1471fad9f176c63a06806c1558b7f170f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c7065a8b516c423d6a0a5a4b66f46b080409ed4444eba2246d6c19e314e8200
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45557146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392797d878b40e7452088c60471c605f48b473dc41bfbfbe696a0ab41f324600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-cli`

```console
$ docker pull docker@sha256:2245cd9cd5bc068987a1d3fd9eede6faf8231b396bba968234fffbeb01b09648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-cli` - linux; amd64

```console
$ docker pull docker@sha256:c53db7693d089e1f9cd5267253e3885b394d48df2722f85e21232e101d7c30b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49906275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c69eddee82bdf5a05bc7fd67029f1471fad9f176c63a06806c1558b7f170f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c7065a8b516c423d6a0a5a4b66f46b080409ed4444eba2246d6c19e314e8200
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45557146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392797d878b40e7452088c60471c605f48b473dc41bfbfbe696a0ab41f324600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:c8bb6fa5388b56304dd770c4bc0478de81ce18540173b1a589178c0d31bfce90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:591f6c54b0c604fdd8ef81162511227d605168028959c46d483ac889a390f04c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109765844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ea606aec782052e886db5032f90c3f6cd23a8af9163f4696fd72e3204eea30`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:20 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 04:05:21 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 04:05:25 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 04:05:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 04:05:26 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:26 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 04:05:26 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 04:05:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:26 GMT
CMD []
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657a65d7b144ff4eeb487ecf89686a5eca2b180080560c7cf17c678428b7f08`  
		Last Modified: Wed, 01 Feb 2023 04:07:59 GMT  
		Size: 6.8 MB (6837845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ea906fa6ed48c4b804df209f79243fbd8b108339badba8a884fec2cf130f04`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b1215a55bdb1f902ac71ea22a2cadd14aee077bc384bc3ccc16741f5fc76f9`  
		Last Modified: Wed, 01 Feb 2023 04:08:06 GMT  
		Size: 53.0 MB (53016613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d574b1479f9a6ac9108c936ed4477803c0c87d3349f002446be9ca2327aff14`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6660a3266d0004cbe28ac50821dc4043d1d25b5988c35a6d9df4ba9b3458ba7e`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:37660314f84150240ebe7ebc5371db0c7093cbef7dd6776294a8471145d0205c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101233760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39dc6bda9a9d0e65c84bb3057c4e9e4cf51ce7e779c1af9dae82b2595a57f214`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 00:37:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 00:37:05 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 00:37:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 00:37:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:37:06 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 00:37:06 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 00:37:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 00:37:06 GMT
CMD []
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc945062d021c449734196bd8eefb1772e1013ea72a8256ea8be071ed207f07`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 7.0 MB (6991074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491a782827a868eaf31c591bc6379c49819d2c2400942f83e0adf741d5a2634e`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae70598918314a90ebb6a27b541bda3041b47324f97d6bd1ef78efd3f34816`  
		Last Modified: Wed, 01 Feb 2023 00:39:43 GMT  
		Size: 48.7 MB (48680432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d33670412195614483d416742482303f48a3adca4e461ed545458768cc341`  
		Last Modified: Wed, 01 Feb 2023 00:39:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e209a5c7ae3588bc38f565bd4526b4abf1bd4f9bd01b52b23e68c4446c3fa7`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:14bb6eb5660af1af2a33a95f7707297f3d1e8a61c3c01c07dbe77857153fbdc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:eb14c1f101aa62eba00cf2d60d2178399f9ad95914b3909743428ef2982b1e48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131052772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e15f614d183abc83f854cc82c6c7574f6468cdce6de600ed013c5f7bf8bc3069`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:20 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 04:05:21 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 04:05:25 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 04:05:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 04:05:26 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:26 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 04:05:26 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 04:05:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:26 GMT
CMD []
# Wed, 01 Feb 2023 04:05:30 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Wed, 01 Feb 2023 04:05:31 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Feb 2023 04:05:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Feb 2023 04:05:34 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Feb 2023 04:05:34 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Feb 2023 04:05:35 GMT
USER rootless
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657a65d7b144ff4eeb487ecf89686a5eca2b180080560c7cf17c678428b7f08`  
		Last Modified: Wed, 01 Feb 2023 04:07:59 GMT  
		Size: 6.8 MB (6837845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ea906fa6ed48c4b804df209f79243fbd8b108339badba8a884fec2cf130f04`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b1215a55bdb1f902ac71ea22a2cadd14aee077bc384bc3ccc16741f5fc76f9`  
		Last Modified: Wed, 01 Feb 2023 04:08:06 GMT  
		Size: 53.0 MB (53016613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d574b1479f9a6ac9108c936ed4477803c0c87d3349f002446be9ca2327aff14`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6660a3266d0004cbe28ac50821dc4043d1d25b5988c35a6d9df4ba9b3458ba7e`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb764ad342644ff732b54b161e93ec3873477da2bf6346b1f1020d5ef810e563`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 1.4 MB (1375668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02a1aa44838b715c59cfa1b0dbcfd8ea07aa7e33df033855199029ea94d8cdf`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204c78b7022762a1c0760c2e99d4b25625148975da4789d8d1c05dd1a758d947`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8597899ad7865929af69069ce025eedae7e8986018b708b883ec907d5b41e6db`  
		Last Modified: Wed, 01 Feb 2023 04:08:25 GMT  
		Size: 19.9 MB (19909541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d1c4aa6615e34de84a9a9573c5a2365263508cc2a265c9c697fa86ce11e456`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:49a9e42cfdd96a87ecb3bf321adf45e42d5800e802c2fc626d01cb35aaeb8bf8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124518920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4299632a5f96d92add93fdb64a65a20109b26c4354be75accc2c91059cbca4e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 00:37:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 00:37:05 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 00:37:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 00:37:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:37:06 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 00:37:06 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 00:37:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 00:37:06 GMT
CMD []
# Wed, 01 Feb 2023 00:37:09 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Wed, 01 Feb 2023 00:37:10 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Feb 2023 00:37:10 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Feb 2023 00:37:13 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Feb 2023 00:37:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Feb 2023 00:37:13 GMT
USER rootless
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc945062d021c449734196bd8eefb1772e1013ea72a8256ea8be071ed207f07`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 7.0 MB (6991074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491a782827a868eaf31c591bc6379c49819d2c2400942f83e0adf741d5a2634e`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae70598918314a90ebb6a27b541bda3041b47324f97d6bd1ef78efd3f34816`  
		Last Modified: Wed, 01 Feb 2023 00:39:43 GMT  
		Size: 48.7 MB (48680432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d33670412195614483d416742482303f48a3adca4e461ed545458768cc341`  
		Last Modified: Wed, 01 Feb 2023 00:39:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e209a5c7ae3588bc38f565bd4526b4abf1bd4f9bd01b52b23e68c4446c3fa7`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4d24358327dbc4574d13e07b7315b8fd0310226e93ad616c55dc38bb65377`  
		Last Modified: Wed, 01 Feb 2023 00:40:00 GMT  
		Size: 1.4 MB (1401569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa1f40b8ca0e6e2932e14514ffa6fc66385c5fbd93434c212a424d7c458207f`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78b90d7aa4a2d70a466b0a85c7a0e0abb708eb1a7222edb44a64d55cd28de3a`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef22e21656c05d745b8fc51f001d17e33390307b2ece9b51e505c5f3008fc93`  
		Last Modified: Wed, 01 Feb 2023 00:40:02 GMT  
		Size: 21.9 MB (21881872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62753962eb9b54f1ac313ab364f9d70c2a1198fed033defe74d6c373d30263c8`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:52eee6f3f485167cebbcf0b96bac6d21e88914ac78033a0d777ecf5af043cd2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:dc6a34c36bf375f46c7cf5842245db5cd1688b7247e5bd3bd31ab709c7829ef0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (54049886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efaab8d96745854bae6d0065e573f8acbece37e9bbea45f88d30afb33cfbf5c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:39 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b4013945f6b4a47db6082ee8b532b481fb874c69ba2987426b8f4b97ae4f4d`  
		Last Modified: Wed, 01 Feb 2023 04:08:40 GMT  
		Size: 4.1 MB (4143611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e345a2dec0c8c958aa7d6ec56aa93d6228cb3d9fc252687e2194ec026b9661f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49743064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87183771c4819d3c6d0f993edd4bc2923cbe12b6c24d6cb076fd9b51525d2f08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:18 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9306ce797b04d3a543ef0453f92c3133e32b16a17b9f30fe2e833284d0971843`  
		Last Modified: Wed, 01 Feb 2023 00:40:19 GMT  
		Size: 4.2 MB (4185918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:ab14bee152695abf535de1a7793c8ce196b946d107651eee3d8b72f9086a5115
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `docker:20-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:70a5dbaf037e96c1033085997dcb07fa2e1596ebbbee0833a20b0337163f9d6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1442613350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c27520dbe24ddc045216c37cc47aa58e765aa000a386bc55372e2063b3bed4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:17:25 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:17:26 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9fbb5bb66b4765df4292381a96e1cfc78d67a08a48a930d66d57438abacd1`  
		Last Modified: Thu, 12 Jan 2023 05:42:25 GMT  
		Size: 612.2 KB (612183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f7f7f53251ba2d0181e199d1bd37876042b23e037cf0cd6a8678056c7a98a6`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4544079819db2e2462b9038aae6831b0fd0c36c80dbe76a11a5ffbdad78e7664`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b86944ef48015c16735dee2382dbeabc6fd568d801115b072f686fc0526631`  
		Last Modified: Sat, 21 Jan 2023 01:20:09 GMT  
		Size: 56.0 MB (55967846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:5639bb93318b23396e1f042343cce52f2281a3ffd5ba174ca19b76b3b3c69a3c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1764075185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ad0f3cc6a58f272290a178406070162ea53046d3d87f8b10b030df2c90a70a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:18:11 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:18:13 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1203a660d1e7b9cba56b0f2b04e0f4d443536c90572741405636436ed42c43`  
		Last Modified: Thu, 12 Jan 2023 05:42:38 GMT  
		Size: 365.4 KB (365388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc933231f525632f226b4c16194bf32a3adf3e01067661c25cd3ab6086490b`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a46a5a5f1ab4b72084c67f039869f7ad88b4872681007659ecefbf38bf6af20`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d463f4d2ea1bed72ce82bd6b4a98f88513b4799d253684f46b220c0495b358c1`  
		Last Modified: Sat, 21 Jan 2023 01:20:34 GMT  
		Size: 55.8 MB (55761582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:b14c305e443d06050ef5660c5973adb221a0b1f9e0fd09ad42d4561f977283bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:5639bb93318b23396e1f042343cce52f2281a3ffd5ba174ca19b76b3b3c69a3c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1764075185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ad0f3cc6a58f272290a178406070162ea53046d3d87f8b10b030df2c90a70a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:18:11 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:18:13 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1203a660d1e7b9cba56b0f2b04e0f4d443536c90572741405636436ed42c43`  
		Last Modified: Thu, 12 Jan 2023 05:42:38 GMT  
		Size: 365.4 KB (365388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc933231f525632f226b4c16194bf32a3adf3e01067661c25cd3ab6086490b`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a46a5a5f1ab4b72084c67f039869f7ad88b4872681007659ecefbf38bf6af20`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d463f4d2ea1bed72ce82bd6b4a98f88513b4799d253684f46b220c0495b358c1`  
		Last Modified: Sat, 21 Jan 2023 01:20:34 GMT  
		Size: 55.8 MB (55761582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:ea15275a18f3012592e67e8051872a11e2b2945203b191c1da0d5771fb77d3ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `docker:20-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:70a5dbaf037e96c1033085997dcb07fa2e1596ebbbee0833a20b0337163f9d6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1442613350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c27520dbe24ddc045216c37cc47aa58e765aa000a386bc55372e2063b3bed4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:17:25 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:17:26 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9fbb5bb66b4765df4292381a96e1cfc78d67a08a48a930d66d57438abacd1`  
		Last Modified: Thu, 12 Jan 2023 05:42:25 GMT  
		Size: 612.2 KB (612183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f7f7f53251ba2d0181e199d1bd37876042b23e037cf0cd6a8678056c7a98a6`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4544079819db2e2462b9038aae6831b0fd0c36c80dbe76a11a5ffbdad78e7664`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b86944ef48015c16735dee2382dbeabc6fd568d801115b072f686fc0526631`  
		Last Modified: Sat, 21 Jan 2023 01:20:09 GMT  
		Size: 56.0 MB (55967846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10`

```console
$ docker pull docker@sha256:2245cd9cd5bc068987a1d3fd9eede6faf8231b396bba968234fffbeb01b09648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:c53db7693d089e1f9cd5267253e3885b394d48df2722f85e21232e101d7c30b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49906275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c69eddee82bdf5a05bc7fd67029f1471fad9f176c63a06806c1558b7f170f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c7065a8b516c423d6a0a5a4b66f46b080409ed4444eba2246d6c19e314e8200
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45557146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392797d878b40e7452088c60471c605f48b473dc41bfbfbe696a0ab41f324600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-cli`

```console
$ docker pull docker@sha256:2245cd9cd5bc068987a1d3fd9eede6faf8231b396bba968234fffbeb01b09648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-cli` - linux; amd64

```console
$ docker pull docker@sha256:c53db7693d089e1f9cd5267253e3885b394d48df2722f85e21232e101d7c30b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49906275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c69eddee82bdf5a05bc7fd67029f1471fad9f176c63a06806c1558b7f170f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c7065a8b516c423d6a0a5a4b66f46b080409ed4444eba2246d6c19e314e8200
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45557146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392797d878b40e7452088c60471c605f48b473dc41bfbfbe696a0ab41f324600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:c8bb6fa5388b56304dd770c4bc0478de81ce18540173b1a589178c0d31bfce90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:591f6c54b0c604fdd8ef81162511227d605168028959c46d483ac889a390f04c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109765844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ea606aec782052e886db5032f90c3f6cd23a8af9163f4696fd72e3204eea30`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:20 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 04:05:21 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 04:05:25 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 04:05:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 04:05:26 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:26 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 04:05:26 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 04:05:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:26 GMT
CMD []
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657a65d7b144ff4eeb487ecf89686a5eca2b180080560c7cf17c678428b7f08`  
		Last Modified: Wed, 01 Feb 2023 04:07:59 GMT  
		Size: 6.8 MB (6837845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ea906fa6ed48c4b804df209f79243fbd8b108339badba8a884fec2cf130f04`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b1215a55bdb1f902ac71ea22a2cadd14aee077bc384bc3ccc16741f5fc76f9`  
		Last Modified: Wed, 01 Feb 2023 04:08:06 GMT  
		Size: 53.0 MB (53016613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d574b1479f9a6ac9108c936ed4477803c0c87d3349f002446be9ca2327aff14`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6660a3266d0004cbe28ac50821dc4043d1d25b5988c35a6d9df4ba9b3458ba7e`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:37660314f84150240ebe7ebc5371db0c7093cbef7dd6776294a8471145d0205c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101233760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39dc6bda9a9d0e65c84bb3057c4e9e4cf51ce7e779c1af9dae82b2595a57f214`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 00:37:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 00:37:05 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 00:37:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 00:37:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:37:06 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 00:37:06 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 00:37:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 00:37:06 GMT
CMD []
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc945062d021c449734196bd8eefb1772e1013ea72a8256ea8be071ed207f07`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 7.0 MB (6991074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491a782827a868eaf31c591bc6379c49819d2c2400942f83e0adf741d5a2634e`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae70598918314a90ebb6a27b541bda3041b47324f97d6bd1ef78efd3f34816`  
		Last Modified: Wed, 01 Feb 2023 00:39:43 GMT  
		Size: 48.7 MB (48680432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d33670412195614483d416742482303f48a3adca4e461ed545458768cc341`  
		Last Modified: Wed, 01 Feb 2023 00:39:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e209a5c7ae3588bc38f565bd4526b4abf1bd4f9bd01b52b23e68c4446c3fa7`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:14bb6eb5660af1af2a33a95f7707297f3d1e8a61c3c01c07dbe77857153fbdc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:eb14c1f101aa62eba00cf2d60d2178399f9ad95914b3909743428ef2982b1e48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131052772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e15f614d183abc83f854cc82c6c7574f6468cdce6de600ed013c5f7bf8bc3069`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:20 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 04:05:21 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 04:05:25 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 04:05:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 04:05:26 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:26 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 04:05:26 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 04:05:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:26 GMT
CMD []
# Wed, 01 Feb 2023 04:05:30 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Wed, 01 Feb 2023 04:05:31 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Feb 2023 04:05:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Feb 2023 04:05:34 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Feb 2023 04:05:34 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Feb 2023 04:05:35 GMT
USER rootless
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657a65d7b144ff4eeb487ecf89686a5eca2b180080560c7cf17c678428b7f08`  
		Last Modified: Wed, 01 Feb 2023 04:07:59 GMT  
		Size: 6.8 MB (6837845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ea906fa6ed48c4b804df209f79243fbd8b108339badba8a884fec2cf130f04`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b1215a55bdb1f902ac71ea22a2cadd14aee077bc384bc3ccc16741f5fc76f9`  
		Last Modified: Wed, 01 Feb 2023 04:08:06 GMT  
		Size: 53.0 MB (53016613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d574b1479f9a6ac9108c936ed4477803c0c87d3349f002446be9ca2327aff14`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6660a3266d0004cbe28ac50821dc4043d1d25b5988c35a6d9df4ba9b3458ba7e`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb764ad342644ff732b54b161e93ec3873477da2bf6346b1f1020d5ef810e563`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 1.4 MB (1375668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02a1aa44838b715c59cfa1b0dbcfd8ea07aa7e33df033855199029ea94d8cdf`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204c78b7022762a1c0760c2e99d4b25625148975da4789d8d1c05dd1a758d947`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8597899ad7865929af69069ce025eedae7e8986018b708b883ec907d5b41e6db`  
		Last Modified: Wed, 01 Feb 2023 04:08:25 GMT  
		Size: 19.9 MB (19909541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d1c4aa6615e34de84a9a9573c5a2365263508cc2a265c9c697fa86ce11e456`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:49a9e42cfdd96a87ecb3bf321adf45e42d5800e802c2fc626d01cb35aaeb8bf8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124518920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4299632a5f96d92add93fdb64a65a20109b26c4354be75accc2c91059cbca4e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 00:37:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 00:37:05 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 00:37:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 00:37:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:37:06 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 00:37:06 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 00:37:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 00:37:06 GMT
CMD []
# Wed, 01 Feb 2023 00:37:09 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Wed, 01 Feb 2023 00:37:10 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Feb 2023 00:37:10 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Feb 2023 00:37:13 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Feb 2023 00:37:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Feb 2023 00:37:13 GMT
USER rootless
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc945062d021c449734196bd8eefb1772e1013ea72a8256ea8be071ed207f07`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 7.0 MB (6991074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491a782827a868eaf31c591bc6379c49819d2c2400942f83e0adf741d5a2634e`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae70598918314a90ebb6a27b541bda3041b47324f97d6bd1ef78efd3f34816`  
		Last Modified: Wed, 01 Feb 2023 00:39:43 GMT  
		Size: 48.7 MB (48680432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d33670412195614483d416742482303f48a3adca4e461ed545458768cc341`  
		Last Modified: Wed, 01 Feb 2023 00:39:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e209a5c7ae3588bc38f565bd4526b4abf1bd4f9bd01b52b23e68c4446c3fa7`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4d24358327dbc4574d13e07b7315b8fd0310226e93ad616c55dc38bb65377`  
		Last Modified: Wed, 01 Feb 2023 00:40:00 GMT  
		Size: 1.4 MB (1401569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa1f40b8ca0e6e2932e14514ffa6fc66385c5fbd93434c212a424d7c458207f`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78b90d7aa4a2d70a466b0a85c7a0e0abb708eb1a7222edb44a64d55cd28de3a`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef22e21656c05d745b8fc51f001d17e33390307b2ece9b51e505c5f3008fc93`  
		Last Modified: Wed, 01 Feb 2023 00:40:02 GMT  
		Size: 21.9 MB (21881872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62753962eb9b54f1ac313ab364f9d70c2a1198fed033defe74d6c373d30263c8`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:52eee6f3f485167cebbcf0b96bac6d21e88914ac78033a0d777ecf5af043cd2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:dc6a34c36bf375f46c7cf5842245db5cd1688b7247e5bd3bd31ab709c7829ef0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (54049886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efaab8d96745854bae6d0065e573f8acbece37e9bbea45f88d30afb33cfbf5c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:39 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b4013945f6b4a47db6082ee8b532b481fb874c69ba2987426b8f4b97ae4f4d`  
		Last Modified: Wed, 01 Feb 2023 04:08:40 GMT  
		Size: 4.1 MB (4143611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e345a2dec0c8c958aa7d6ec56aa93d6228cb3d9fc252687e2194ec026b9661f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49743064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87183771c4819d3c6d0f993edd4bc2923cbe12b6c24d6cb076fd9b51525d2f08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:18 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9306ce797b04d3a543ef0453f92c3133e32b16a17b9f30fe2e833284d0971843`  
		Last Modified: Wed, 01 Feb 2023 00:40:19 GMT  
		Size: 4.2 MB (4185918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore`

```console
$ docker pull docker@sha256:ab14bee152695abf535de1a7793c8ce196b946d107651eee3d8b72f9086a5115
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `docker:20.10-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:70a5dbaf037e96c1033085997dcb07fa2e1596ebbbee0833a20b0337163f9d6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1442613350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c27520dbe24ddc045216c37cc47aa58e765aa000a386bc55372e2063b3bed4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:17:25 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:17:26 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9fbb5bb66b4765df4292381a96e1cfc78d67a08a48a930d66d57438abacd1`  
		Last Modified: Thu, 12 Jan 2023 05:42:25 GMT  
		Size: 612.2 KB (612183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f7f7f53251ba2d0181e199d1bd37876042b23e037cf0cd6a8678056c7a98a6`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4544079819db2e2462b9038aae6831b0fd0c36c80dbe76a11a5ffbdad78e7664`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b86944ef48015c16735dee2382dbeabc6fd568d801115b072f686fc0526631`  
		Last Modified: Sat, 21 Jan 2023 01:20:09 GMT  
		Size: 56.0 MB (55967846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:5639bb93318b23396e1f042343cce52f2281a3ffd5ba174ca19b76b3b3c69a3c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1764075185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ad0f3cc6a58f272290a178406070162ea53046d3d87f8b10b030df2c90a70a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:18:11 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:18:13 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1203a660d1e7b9cba56b0f2b04e0f4d443536c90572741405636436ed42c43`  
		Last Modified: Thu, 12 Jan 2023 05:42:38 GMT  
		Size: 365.4 KB (365388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc933231f525632f226b4c16194bf32a3adf3e01067661c25cd3ab6086490b`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a46a5a5f1ab4b72084c67f039869f7ad88b4872681007659ecefbf38bf6af20`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d463f4d2ea1bed72ce82bd6b4a98f88513b4799d253684f46b220c0495b358c1`  
		Last Modified: Sat, 21 Jan 2023 01:20:34 GMT  
		Size: 55.8 MB (55761582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-1809`

```console
$ docker pull docker@sha256:b14c305e443d06050ef5660c5973adb221a0b1f9e0fd09ad42d4561f977283bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `docker:20.10-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:5639bb93318b23396e1f042343cce52f2281a3ffd5ba174ca19b76b3b3c69a3c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1764075185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ad0f3cc6a58f272290a178406070162ea53046d3d87f8b10b030df2c90a70a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:18:11 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:18:13 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1203a660d1e7b9cba56b0f2b04e0f4d443536c90572741405636436ed42c43`  
		Last Modified: Thu, 12 Jan 2023 05:42:38 GMT  
		Size: 365.4 KB (365388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc933231f525632f226b4c16194bf32a3adf3e01067661c25cd3ab6086490b`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a46a5a5f1ab4b72084c67f039869f7ad88b4872681007659ecefbf38bf6af20`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d463f4d2ea1bed72ce82bd6b4a98f88513b4799d253684f46b220c0495b358c1`  
		Last Modified: Sat, 21 Jan 2023 01:20:34 GMT  
		Size: 55.8 MB (55761582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:ea15275a18f3012592e67e8051872a11e2b2945203b191c1da0d5771fb77d3ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `docker:20.10-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:70a5dbaf037e96c1033085997dcb07fa2e1596ebbbee0833a20b0337163f9d6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1442613350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c27520dbe24ddc045216c37cc47aa58e765aa000a386bc55372e2063b3bed4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:17:25 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:17:26 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9fbb5bb66b4765df4292381a96e1cfc78d67a08a48a930d66d57438abacd1`  
		Last Modified: Thu, 12 Jan 2023 05:42:25 GMT  
		Size: 612.2 KB (612183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f7f7f53251ba2d0181e199d1bd37876042b23e037cf0cd6a8678056c7a98a6`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4544079819db2e2462b9038aae6831b0fd0c36c80dbe76a11a5ffbdad78e7664`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b86944ef48015c16735dee2382dbeabc6fd568d801115b072f686fc0526631`  
		Last Modified: Sat, 21 Jan 2023 01:20:09 GMT  
		Size: 56.0 MB (55967846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23`

```console
$ docker pull docker@sha256:2245cd9cd5bc068987a1d3fd9eede6faf8231b396bba968234fffbeb01b09648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23` - linux; amd64

```console
$ docker pull docker@sha256:c53db7693d089e1f9cd5267253e3885b394d48df2722f85e21232e101d7c30b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49906275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c69eddee82bdf5a05bc7fd67029f1471fad9f176c63a06806c1558b7f170f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c7065a8b516c423d6a0a5a4b66f46b080409ed4444eba2246d6c19e314e8200
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45557146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392797d878b40e7452088c60471c605f48b473dc41bfbfbe696a0ab41f324600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-alpine3.17`

```console
$ docker pull docker@sha256:2245cd9cd5bc068987a1d3fd9eede6faf8231b396bba968234fffbeb01b09648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-alpine3.17` - linux; amd64

```console
$ docker pull docker@sha256:c53db7693d089e1f9cd5267253e3885b394d48df2722f85e21232e101d7c30b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49906275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c69eddee82bdf5a05bc7fd67029f1471fad9f176c63a06806c1558b7f170f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c7065a8b516c423d6a0a5a4b66f46b080409ed4444eba2246d6c19e314e8200
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45557146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392797d878b40e7452088c60471c605f48b473dc41bfbfbe696a0ab41f324600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-cli`

```console
$ docker pull docker@sha256:2245cd9cd5bc068987a1d3fd9eede6faf8231b396bba968234fffbeb01b09648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-cli` - linux; amd64

```console
$ docker pull docker@sha256:c53db7693d089e1f9cd5267253e3885b394d48df2722f85e21232e101d7c30b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49906275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c69eddee82bdf5a05bc7fd67029f1471fad9f176c63a06806c1558b7f170f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c7065a8b516c423d6a0a5a4b66f46b080409ed4444eba2246d6c19e314e8200
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45557146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392797d878b40e7452088c60471c605f48b473dc41bfbfbe696a0ab41f324600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-cli-alpine3.17`

```console
$ docker pull docker@sha256:2245cd9cd5bc068987a1d3fd9eede6faf8231b396bba968234fffbeb01b09648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-cli-alpine3.17` - linux; amd64

```console
$ docker pull docker@sha256:c53db7693d089e1f9cd5267253e3885b394d48df2722f85e21232e101d7c30b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49906275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c69eddee82bdf5a05bc7fd67029f1471fad9f176c63a06806c1558b7f170f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-cli-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c7065a8b516c423d6a0a5a4b66f46b080409ed4444eba2246d6c19e314e8200
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45557146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392797d878b40e7452088c60471c605f48b473dc41bfbfbe696a0ab41f324600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-dind`

```console
$ docker pull docker@sha256:c8bb6fa5388b56304dd770c4bc0478de81ce18540173b1a589178c0d31bfce90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-dind` - linux; amd64

```console
$ docker pull docker@sha256:591f6c54b0c604fdd8ef81162511227d605168028959c46d483ac889a390f04c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109765844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ea606aec782052e886db5032f90c3f6cd23a8af9163f4696fd72e3204eea30`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:20 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 04:05:21 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 04:05:25 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 04:05:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 04:05:26 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:26 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 04:05:26 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 04:05:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:26 GMT
CMD []
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657a65d7b144ff4eeb487ecf89686a5eca2b180080560c7cf17c678428b7f08`  
		Last Modified: Wed, 01 Feb 2023 04:07:59 GMT  
		Size: 6.8 MB (6837845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ea906fa6ed48c4b804df209f79243fbd8b108339badba8a884fec2cf130f04`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b1215a55bdb1f902ac71ea22a2cadd14aee077bc384bc3ccc16741f5fc76f9`  
		Last Modified: Wed, 01 Feb 2023 04:08:06 GMT  
		Size: 53.0 MB (53016613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d574b1479f9a6ac9108c936ed4477803c0c87d3349f002446be9ca2327aff14`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6660a3266d0004cbe28ac50821dc4043d1d25b5988c35a6d9df4ba9b3458ba7e`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:37660314f84150240ebe7ebc5371db0c7093cbef7dd6776294a8471145d0205c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101233760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39dc6bda9a9d0e65c84bb3057c4e9e4cf51ce7e779c1af9dae82b2595a57f214`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 00:37:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 00:37:05 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 00:37:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 00:37:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:37:06 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 00:37:06 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 00:37:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 00:37:06 GMT
CMD []
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc945062d021c449734196bd8eefb1772e1013ea72a8256ea8be071ed207f07`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 7.0 MB (6991074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491a782827a868eaf31c591bc6379c49819d2c2400942f83e0adf741d5a2634e`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae70598918314a90ebb6a27b541bda3041b47324f97d6bd1ef78efd3f34816`  
		Last Modified: Wed, 01 Feb 2023 00:39:43 GMT  
		Size: 48.7 MB (48680432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d33670412195614483d416742482303f48a3adca4e461ed545458768cc341`  
		Last Modified: Wed, 01 Feb 2023 00:39:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e209a5c7ae3588bc38f565bd4526b4abf1bd4f9bd01b52b23e68c4446c3fa7`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-dind-alpine3.17`

```console
$ docker pull docker@sha256:c8bb6fa5388b56304dd770c4bc0478de81ce18540173b1a589178c0d31bfce90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-dind-alpine3.17` - linux; amd64

```console
$ docker pull docker@sha256:591f6c54b0c604fdd8ef81162511227d605168028959c46d483ac889a390f04c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109765844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ea606aec782052e886db5032f90c3f6cd23a8af9163f4696fd72e3204eea30`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:20 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 04:05:21 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 04:05:25 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 04:05:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 04:05:26 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:26 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 04:05:26 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 04:05:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:26 GMT
CMD []
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657a65d7b144ff4eeb487ecf89686a5eca2b180080560c7cf17c678428b7f08`  
		Last Modified: Wed, 01 Feb 2023 04:07:59 GMT  
		Size: 6.8 MB (6837845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ea906fa6ed48c4b804df209f79243fbd8b108339badba8a884fec2cf130f04`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b1215a55bdb1f902ac71ea22a2cadd14aee077bc384bc3ccc16741f5fc76f9`  
		Last Modified: Wed, 01 Feb 2023 04:08:06 GMT  
		Size: 53.0 MB (53016613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d574b1479f9a6ac9108c936ed4477803c0c87d3349f002446be9ca2327aff14`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6660a3266d0004cbe28ac50821dc4043d1d25b5988c35a6d9df4ba9b3458ba7e`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-dind-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:37660314f84150240ebe7ebc5371db0c7093cbef7dd6776294a8471145d0205c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101233760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39dc6bda9a9d0e65c84bb3057c4e9e4cf51ce7e779c1af9dae82b2595a57f214`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 00:37:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 00:37:05 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 00:37:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 00:37:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:37:06 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 00:37:06 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 00:37:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 00:37:06 GMT
CMD []
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc945062d021c449734196bd8eefb1772e1013ea72a8256ea8be071ed207f07`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 7.0 MB (6991074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491a782827a868eaf31c591bc6379c49819d2c2400942f83e0adf741d5a2634e`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae70598918314a90ebb6a27b541bda3041b47324f97d6bd1ef78efd3f34816`  
		Last Modified: Wed, 01 Feb 2023 00:39:43 GMT  
		Size: 48.7 MB (48680432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d33670412195614483d416742482303f48a3adca4e461ed545458768cc341`  
		Last Modified: Wed, 01 Feb 2023 00:39:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e209a5c7ae3588bc38f565bd4526b4abf1bd4f9bd01b52b23e68c4446c3fa7`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-dind-rootless`

```console
$ docker pull docker@sha256:14bb6eb5660af1af2a33a95f7707297f3d1e8a61c3c01c07dbe77857153fbdc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:eb14c1f101aa62eba00cf2d60d2178399f9ad95914b3909743428ef2982b1e48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131052772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e15f614d183abc83f854cc82c6c7574f6468cdce6de600ed013c5f7bf8bc3069`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:20 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 04:05:21 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 04:05:25 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 04:05:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 04:05:26 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:26 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 04:05:26 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 04:05:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:26 GMT
CMD []
# Wed, 01 Feb 2023 04:05:30 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Wed, 01 Feb 2023 04:05:31 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Feb 2023 04:05:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Feb 2023 04:05:34 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Feb 2023 04:05:34 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Feb 2023 04:05:35 GMT
USER rootless
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657a65d7b144ff4eeb487ecf89686a5eca2b180080560c7cf17c678428b7f08`  
		Last Modified: Wed, 01 Feb 2023 04:07:59 GMT  
		Size: 6.8 MB (6837845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ea906fa6ed48c4b804df209f79243fbd8b108339badba8a884fec2cf130f04`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b1215a55bdb1f902ac71ea22a2cadd14aee077bc384bc3ccc16741f5fc76f9`  
		Last Modified: Wed, 01 Feb 2023 04:08:06 GMT  
		Size: 53.0 MB (53016613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d574b1479f9a6ac9108c936ed4477803c0c87d3349f002446be9ca2327aff14`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6660a3266d0004cbe28ac50821dc4043d1d25b5988c35a6d9df4ba9b3458ba7e`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb764ad342644ff732b54b161e93ec3873477da2bf6346b1f1020d5ef810e563`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 1.4 MB (1375668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02a1aa44838b715c59cfa1b0dbcfd8ea07aa7e33df033855199029ea94d8cdf`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204c78b7022762a1c0760c2e99d4b25625148975da4789d8d1c05dd1a758d947`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8597899ad7865929af69069ce025eedae7e8986018b708b883ec907d5b41e6db`  
		Last Modified: Wed, 01 Feb 2023 04:08:25 GMT  
		Size: 19.9 MB (19909541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d1c4aa6615e34de84a9a9573c5a2365263508cc2a265c9c697fa86ce11e456`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:49a9e42cfdd96a87ecb3bf321adf45e42d5800e802c2fc626d01cb35aaeb8bf8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124518920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4299632a5f96d92add93fdb64a65a20109b26c4354be75accc2c91059cbca4e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 00:37:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 00:37:05 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 00:37:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 00:37:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:37:06 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 00:37:06 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 00:37:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 00:37:06 GMT
CMD []
# Wed, 01 Feb 2023 00:37:09 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Wed, 01 Feb 2023 00:37:10 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Feb 2023 00:37:10 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Feb 2023 00:37:13 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Feb 2023 00:37:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Feb 2023 00:37:13 GMT
USER rootless
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc945062d021c449734196bd8eefb1772e1013ea72a8256ea8be071ed207f07`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 7.0 MB (6991074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491a782827a868eaf31c591bc6379c49819d2c2400942f83e0adf741d5a2634e`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae70598918314a90ebb6a27b541bda3041b47324f97d6bd1ef78efd3f34816`  
		Last Modified: Wed, 01 Feb 2023 00:39:43 GMT  
		Size: 48.7 MB (48680432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d33670412195614483d416742482303f48a3adca4e461ed545458768cc341`  
		Last Modified: Wed, 01 Feb 2023 00:39:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e209a5c7ae3588bc38f565bd4526b4abf1bd4f9bd01b52b23e68c4446c3fa7`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4d24358327dbc4574d13e07b7315b8fd0310226e93ad616c55dc38bb65377`  
		Last Modified: Wed, 01 Feb 2023 00:40:00 GMT  
		Size: 1.4 MB (1401569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa1f40b8ca0e6e2932e14514ffa6fc66385c5fbd93434c212a424d7c458207f`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78b90d7aa4a2d70a466b0a85c7a0e0abb708eb1a7222edb44a64d55cd28de3a`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef22e21656c05d745b8fc51f001d17e33390307b2ece9b51e505c5f3008fc93`  
		Last Modified: Wed, 01 Feb 2023 00:40:02 GMT  
		Size: 21.9 MB (21881872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62753962eb9b54f1ac313ab364f9d70c2a1198fed033defe74d6c373d30263c8`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-git`

```console
$ docker pull docker@sha256:52eee6f3f485167cebbcf0b96bac6d21e88914ac78033a0d777ecf5af043cd2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-git` - linux; amd64

```console
$ docker pull docker@sha256:dc6a34c36bf375f46c7cf5842245db5cd1688b7247e5bd3bd31ab709c7829ef0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (54049886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efaab8d96745854bae6d0065e573f8acbece37e9bbea45f88d30afb33cfbf5c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:39 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b4013945f6b4a47db6082ee8b532b481fb874c69ba2987426b8f4b97ae4f4d`  
		Last Modified: Wed, 01 Feb 2023 04:08:40 GMT  
		Size: 4.1 MB (4143611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e345a2dec0c8c958aa7d6ec56aa93d6228cb3d9fc252687e2194ec026b9661f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49743064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87183771c4819d3c6d0f993edd4bc2923cbe12b6c24d6cb076fd9b51525d2f08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:18 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9306ce797b04d3a543ef0453f92c3133e32b16a17b9f30fe2e833284d0971843`  
		Last Modified: Wed, 01 Feb 2023 00:40:19 GMT  
		Size: 4.2 MB (4185918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-windowsservercore`

```console
$ docker pull docker@sha256:ab14bee152695abf535de1a7793c8ce196b946d107651eee3d8b72f9086a5115
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `docker:20.10.23-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:70a5dbaf037e96c1033085997dcb07fa2e1596ebbbee0833a20b0337163f9d6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1442613350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c27520dbe24ddc045216c37cc47aa58e765aa000a386bc55372e2063b3bed4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:17:25 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:17:26 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9fbb5bb66b4765df4292381a96e1cfc78d67a08a48a930d66d57438abacd1`  
		Last Modified: Thu, 12 Jan 2023 05:42:25 GMT  
		Size: 612.2 KB (612183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f7f7f53251ba2d0181e199d1bd37876042b23e037cf0cd6a8678056c7a98a6`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4544079819db2e2462b9038aae6831b0fd0c36c80dbe76a11a5ffbdad78e7664`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b86944ef48015c16735dee2382dbeabc6fd568d801115b072f686fc0526631`  
		Last Modified: Sat, 21 Jan 2023 01:20:09 GMT  
		Size: 56.0 MB (55967846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:5639bb93318b23396e1f042343cce52f2281a3ffd5ba174ca19b76b3b3c69a3c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1764075185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ad0f3cc6a58f272290a178406070162ea53046d3d87f8b10b030df2c90a70a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:18:11 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:18:13 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1203a660d1e7b9cba56b0f2b04e0f4d443536c90572741405636436ed42c43`  
		Last Modified: Thu, 12 Jan 2023 05:42:38 GMT  
		Size: 365.4 KB (365388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc933231f525632f226b4c16194bf32a3adf3e01067661c25cd3ab6086490b`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a46a5a5f1ab4b72084c67f039869f7ad88b4872681007659ecefbf38bf6af20`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d463f4d2ea1bed72ce82bd6b4a98f88513b4799d253684f46b220c0495b358c1`  
		Last Modified: Sat, 21 Jan 2023 01:20:34 GMT  
		Size: 55.8 MB (55761582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-windowsservercore-1809`

```console
$ docker pull docker@sha256:b14c305e443d06050ef5660c5973adb221a0b1f9e0fd09ad42d4561f977283bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `docker:20.10.23-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:5639bb93318b23396e1f042343cce52f2281a3ffd5ba174ca19b76b3b3c69a3c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1764075185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ad0f3cc6a58f272290a178406070162ea53046d3d87f8b10b030df2c90a70a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:18:11 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:18:13 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1203a660d1e7b9cba56b0f2b04e0f4d443536c90572741405636436ed42c43`  
		Last Modified: Thu, 12 Jan 2023 05:42:38 GMT  
		Size: 365.4 KB (365388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc933231f525632f226b4c16194bf32a3adf3e01067661c25cd3ab6086490b`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a46a5a5f1ab4b72084c67f039869f7ad88b4872681007659ecefbf38bf6af20`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d463f4d2ea1bed72ce82bd6b4a98f88513b4799d253684f46b220c0495b358c1`  
		Last Modified: Sat, 21 Jan 2023 01:20:34 GMT  
		Size: 55.8 MB (55761582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:ea15275a18f3012592e67e8051872a11e2b2945203b191c1da0d5771fb77d3ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `docker:20.10.23-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:70a5dbaf037e96c1033085997dcb07fa2e1596ebbbee0833a20b0337163f9d6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1442613350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c27520dbe24ddc045216c37cc47aa58e765aa000a386bc55372e2063b3bed4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:17:25 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:17:26 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9fbb5bb66b4765df4292381a96e1cfc78d67a08a48a930d66d57438abacd1`  
		Last Modified: Thu, 12 Jan 2023 05:42:25 GMT  
		Size: 612.2 KB (612183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f7f7f53251ba2d0181e199d1bd37876042b23e037cf0cd6a8678056c7a98a6`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4544079819db2e2462b9038aae6831b0fd0c36c80dbe76a11a5ffbdad78e7664`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b86944ef48015c16735dee2382dbeabc6fd568d801115b072f686fc0526631`  
		Last Modified: Sat, 21 Jan 2023 01:20:09 GMT  
		Size: 56.0 MB (55967846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23`

**does not exist** (yet?)

## `docker:23-cli`

**does not exist** (yet?)

## `docker:23-dind`

**does not exist** (yet?)

## `docker:23-dind-rootless`

**does not exist** (yet?)

## `docker:23-git`

**does not exist** (yet?)

## `docker:23-windowsservercore`

**does not exist** (yet?)

## `docker:23-windowsservercore-1809`

**does not exist** (yet?)

## `docker:23-windowsservercore-ltsc2022`

**does not exist** (yet?)

## `docker:23.0`

**does not exist** (yet?)

## `docker:23.0-cli`

**does not exist** (yet?)

## `docker:23.0-dind`

**does not exist** (yet?)

## `docker:23.0-dind-rootless`

**does not exist** (yet?)

## `docker:23.0-git`

**does not exist** (yet?)

## `docker:23.0-windowsservercore`

**does not exist** (yet?)

## `docker:23.0-windowsservercore-1809`

**does not exist** (yet?)

## `docker:23.0-windowsservercore-ltsc2022`

**does not exist** (yet?)

## `docker:23.0.0`

**does not exist** (yet?)

## `docker:23.0.0-alpine3.17`

**does not exist** (yet?)

## `docker:23.0.0-cli`

**does not exist** (yet?)

## `docker:23.0.0-cli-alpine3.17`

**does not exist** (yet?)

## `docker:23.0.0-dind`

**does not exist** (yet?)

## `docker:23.0.0-dind-alpine3.17`

**does not exist** (yet?)

## `docker:23.0.0-dind-rootless`

**does not exist** (yet?)

## `docker:23.0.0-git`

**does not exist** (yet?)

## `docker:23.0.0-windowsservercore`

**does not exist** (yet?)

## `docker:23.0.0-windowsservercore-1809`

**does not exist** (yet?)

## `docker:23.0.0-windowsservercore-ltsc2022`

**does not exist** (yet?)

## `docker:cli`

```console
$ docker pull docker@sha256:2245cd9cd5bc068987a1d3fd9eede6faf8231b396bba968234fffbeb01b09648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:cli` - linux; amd64

```console
$ docker pull docker@sha256:c53db7693d089e1f9cd5267253e3885b394d48df2722f85e21232e101d7c30b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49906275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c69eddee82bdf5a05bc7fd67029f1471fad9f176c63a06806c1558b7f170f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c7065a8b516c423d6a0a5a4b66f46b080409ed4444eba2246d6c19e314e8200
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45557146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392797d878b40e7452088c60471c605f48b473dc41bfbfbe696a0ab41f324600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:c8bb6fa5388b56304dd770c4bc0478de81ce18540173b1a589178c0d31bfce90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:591f6c54b0c604fdd8ef81162511227d605168028959c46d483ac889a390f04c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109765844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ea606aec782052e886db5032f90c3f6cd23a8af9163f4696fd72e3204eea30`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:20 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 04:05:21 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 04:05:25 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 04:05:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 04:05:26 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:26 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 04:05:26 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 04:05:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:26 GMT
CMD []
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657a65d7b144ff4eeb487ecf89686a5eca2b180080560c7cf17c678428b7f08`  
		Last Modified: Wed, 01 Feb 2023 04:07:59 GMT  
		Size: 6.8 MB (6837845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ea906fa6ed48c4b804df209f79243fbd8b108339badba8a884fec2cf130f04`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b1215a55bdb1f902ac71ea22a2cadd14aee077bc384bc3ccc16741f5fc76f9`  
		Last Modified: Wed, 01 Feb 2023 04:08:06 GMT  
		Size: 53.0 MB (53016613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d574b1479f9a6ac9108c936ed4477803c0c87d3349f002446be9ca2327aff14`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6660a3266d0004cbe28ac50821dc4043d1d25b5988c35a6d9df4ba9b3458ba7e`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:37660314f84150240ebe7ebc5371db0c7093cbef7dd6776294a8471145d0205c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101233760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39dc6bda9a9d0e65c84bb3057c4e9e4cf51ce7e779c1af9dae82b2595a57f214`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 00:37:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 00:37:05 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 00:37:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 00:37:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:37:06 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 00:37:06 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 00:37:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 00:37:06 GMT
CMD []
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc945062d021c449734196bd8eefb1772e1013ea72a8256ea8be071ed207f07`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 7.0 MB (6991074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491a782827a868eaf31c591bc6379c49819d2c2400942f83e0adf741d5a2634e`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae70598918314a90ebb6a27b541bda3041b47324f97d6bd1ef78efd3f34816`  
		Last Modified: Wed, 01 Feb 2023 00:39:43 GMT  
		Size: 48.7 MB (48680432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d33670412195614483d416742482303f48a3adca4e461ed545458768cc341`  
		Last Modified: Wed, 01 Feb 2023 00:39:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e209a5c7ae3588bc38f565bd4526b4abf1bd4f9bd01b52b23e68c4446c3fa7`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:14bb6eb5660af1af2a33a95f7707297f3d1e8a61c3c01c07dbe77857153fbdc5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:eb14c1f101aa62eba00cf2d60d2178399f9ad95914b3909743428ef2982b1e48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.1 MB (131052772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e15f614d183abc83f854cc82c6c7574f6468cdce6de600ed013c5f7bf8bc3069`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:20 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 04:05:21 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 04:05:25 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 04:05:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 04:05:26 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:26 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 04:05:26 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 04:05:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:26 GMT
CMD []
# Wed, 01 Feb 2023 04:05:30 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Wed, 01 Feb 2023 04:05:31 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Feb 2023 04:05:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Feb 2023 04:05:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Feb 2023 04:05:34 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Feb 2023 04:05:34 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Feb 2023 04:05:35 GMT
USER rootless
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657a65d7b144ff4eeb487ecf89686a5eca2b180080560c7cf17c678428b7f08`  
		Last Modified: Wed, 01 Feb 2023 04:07:59 GMT  
		Size: 6.8 MB (6837845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ea906fa6ed48c4b804df209f79243fbd8b108339badba8a884fec2cf130f04`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b1215a55bdb1f902ac71ea22a2cadd14aee077bc384bc3ccc16741f5fc76f9`  
		Last Modified: Wed, 01 Feb 2023 04:08:06 GMT  
		Size: 53.0 MB (53016613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d574b1479f9a6ac9108c936ed4477803c0c87d3349f002446be9ca2327aff14`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6660a3266d0004cbe28ac50821dc4043d1d25b5988c35a6d9df4ba9b3458ba7e`  
		Last Modified: Wed, 01 Feb 2023 04:07:58 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb764ad342644ff732b54b161e93ec3873477da2bf6346b1f1020d5ef810e563`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 1.4 MB (1375668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02a1aa44838b715c59cfa1b0dbcfd8ea07aa7e33df033855199029ea94d8cdf`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204c78b7022762a1c0760c2e99d4b25625148975da4789d8d1c05dd1a758d947`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8597899ad7865929af69069ce025eedae7e8986018b708b883ec907d5b41e6db`  
		Last Modified: Wed, 01 Feb 2023 04:08:25 GMT  
		Size: 19.9 MB (19909541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10d1c4aa6615e34de84a9a9573c5a2365263508cc2a265c9c697fa86ce11e456`  
		Last Modified: Wed, 01 Feb 2023 04:08:22 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:49a9e42cfdd96a87ecb3bf321adf45e42d5800e802c2fc626d01cb35aaeb8bf8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124518920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4299632a5f96d92add93fdb64a65a20109b26c4354be75accc2c91059cbca4e3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:01 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Feb 2023 00:37:02 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 01 Feb 2023 00:37:05 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 01 Feb 2023 00:37:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Feb 2023 00:37:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:37:06 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Feb 2023 00:37:06 GMT
EXPOSE 2375 2376
# Wed, 01 Feb 2023 00:37:06 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Feb 2023 00:37:06 GMT
CMD []
# Wed, 01 Feb 2023 00:37:09 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Wed, 01 Feb 2023 00:37:10 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Feb 2023 00:37:10 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Feb 2023 00:37:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Feb 2023 00:37:13 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Feb 2023 00:37:13 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Feb 2023 00:37:13 GMT
USER rootless
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc945062d021c449734196bd8eefb1772e1013ea72a8256ea8be071ed207f07`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 7.0 MB (6991074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491a782827a868eaf31c591bc6379c49819d2c2400942f83e0adf741d5a2634e`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eae70598918314a90ebb6a27b541bda3041b47324f97d6bd1ef78efd3f34816`  
		Last Modified: Wed, 01 Feb 2023 00:39:43 GMT  
		Size: 48.7 MB (48680432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d33670412195614483d416742482303f48a3adca4e461ed545458768cc341`  
		Last Modified: Wed, 01 Feb 2023 00:39:37 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e209a5c7ae3588bc38f565bd4526b4abf1bd4f9bd01b52b23e68c4446c3fa7`  
		Last Modified: Wed, 01 Feb 2023 00:39:38 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b4d24358327dbc4574d13e07b7315b8fd0310226e93ad616c55dc38bb65377`  
		Last Modified: Wed, 01 Feb 2023 00:40:00 GMT  
		Size: 1.4 MB (1401569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa1f40b8ca0e6e2932e14514ffa6fc66385c5fbd93434c212a424d7c458207f`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e78b90d7aa4a2d70a466b0a85c7a0e0abb708eb1a7222edb44a64d55cd28de3a`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef22e21656c05d745b8fc51f001d17e33390307b2ece9b51e505c5f3008fc93`  
		Last Modified: Wed, 01 Feb 2023 00:40:02 GMT  
		Size: 21.9 MB (21881872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62753962eb9b54f1ac313ab364f9d70c2a1198fed033defe74d6c373d30263c8`  
		Last Modified: Wed, 01 Feb 2023 00:39:59 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:52eee6f3f485167cebbcf0b96bac6d21e88914ac78033a0d777ecf5af043cd2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:dc6a34c36bf375f46c7cf5842245db5cd1688b7247e5bd3bd31ab709c7829ef0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.0 MB (54049886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efaab8d96745854bae6d0065e573f8acbece37e9bbea45f88d30afb33cfbf5c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 04:05:39 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b4013945f6b4a47db6082ee8b532b481fb874c69ba2987426b8f4b97ae4f4d`  
		Last Modified: Wed, 01 Feb 2023 04:08:40 GMT  
		Size: 4.1 MB (4143611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4e345a2dec0c8c958aa7d6ec56aa93d6228cb3d9fc252687e2194ec026b9661f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49743064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87183771c4819d3c6d0f993edd4bc2923cbe12b6c24d6cb076fd9b51525d2f08`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
# Wed, 01 Feb 2023 00:37:18 GMT
RUN apk add --no-cache git
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9306ce797b04d3a543ef0453f92c3133e32b16a17b9f30fe2e833284d0971843`  
		Last Modified: Wed, 01 Feb 2023 00:40:19 GMT  
		Size: 4.2 MB (4185918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:2245cd9cd5bc068987a1d3fd9eede6faf8231b396bba968234fffbeb01b09648
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:c53db7693d089e1f9cd5267253e3885b394d48df2722f85e21232e101d7c30b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49906275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c69eddee82bdf5a05bc7fd67029f1471fad9f176c63a06806c1558b7f170f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:20 GMT
ADD file:e4d600fc4c9c293efe360be7b30ee96579925d1b4634c94332e2ec73f7d8eca1 in / 
# Mon, 09 Jan 2023 17:05:20 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 21:12:54 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 21:12:54 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:20:06 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:20:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 04:05:08 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 04:05:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 04:05:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 04:05:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 04:05:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 04:05:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 04:05:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 04:05:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 04:05:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8921db27df2831fa6eaa85321205a2470c669b855f3ec95d5a3c2b46de0442c9`  
		Last Modified: Mon, 09 Jan 2023 17:05:45 GMT  
		Size: 3.4 MB (3370628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea237885379427b44e97fa21c0d47eaa42f826dfd0833a69279002a7ce8f50d9`  
		Last Modified: Mon, 09 Jan 2023 21:14:56 GMT  
		Size: 2.1 MB (2064267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201afc762d4387d79af22a29b3c10cf0087308df49bed7f8a49a23c9cf96923`  
		Last Modified: Sat, 21 Jan 2023 00:22:43 GMT  
		Size: 14.0 MB (13983181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4707a9d4defb46fd9dad26448912783413147c03d7bc7b5a85ba7a0ceb383d`  
		Last Modified: Wed, 01 Feb 2023 04:07:33 GMT  
		Size: 16.0 MB (15995576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ac56fd67deb1ec97dae7271bbc343cc8c1478c2812c04bea87a7c8c4207bb8`  
		Last Modified: Wed, 01 Feb 2023 04:07:32 GMT  
		Size: 14.5 MB (14490905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3c8b6cc3abd66e9054115636ba4c42c8b4d984c4fe03973e9af7bc12e9aa34`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36cb8af9e7460cb01101901bd6db8ab0fcaacc4c48589433a638f6da77d17a`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bae7a7836e3103d21acc33f2e7dc2402707e1f5cbb70cc404a208d0d8bc611`  
		Last Modified: Wed, 01 Feb 2023 04:07:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:1c7065a8b516c423d6a0a5a4b66f46b080409ed4444eba2246d6c19e314e8200
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45557146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:392797d878b40e7452088c60471c605f48b473dc41bfbfbe696a0ab41f324600`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:29:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Mon, 09 Jan 2023 17:29:01 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Sat, 21 Jan 2023 00:39:56 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Wed, 01 Feb 2023 00:36:52 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Wed, 01 Feb 2023 00:36:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 01 Feb 2023 00:36:54 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Wed, 01 Feb 2023 00:36:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Feb 2023 00:36:56 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Feb 2023 00:36:56 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Feb 2023 00:36:57 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Feb 2023 00:36:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Feb 2023 00:36:57 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7e78d5cc3f021297e04408059511c5dff9e32e8d9410a4f7815ccdd7d509eb`  
		Last Modified: Mon, 09 Jan 2023 17:30:59 GMT  
		Size: 2.0 MB (2036908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0603170b2f7902394d21011bcf24dd4eb1201cdc6fb46df092f67652550a21b1`  
		Last Modified: Sat, 21 Jan 2023 00:42:26 GMT  
		Size: 12.7 MB (12741960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4e4802eb5ead6a0c80a50faf9009fc083100646a29fabb9d3784ff6ba3d043`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 14.4 MB (14436884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dce7cfe8d3ec1849134fdffde8eae1da5a2cec44503e99d57fbcdecab9a85f35`  
		Last Modified: Wed, 01 Feb 2023 00:39:12 GMT  
		Size: 13.1 MB (13080437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b36a6e12ba38fc36bfbe98eb5c71446ba7308c112353b4dd9260798ec099993`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c12b4b732633988e9310058350b671d68e28de5b47972205d68603764238ffa`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886acde54de0c805c32cbb9ccaf9f27ca19b57882de5fb945a5aa16cc05178f2`  
		Last Modified: Wed, 01 Feb 2023 00:39:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:ab14bee152695abf535de1a7793c8ce196b946d107651eee3d8b72f9086a5115
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `docker:windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:70a5dbaf037e96c1033085997dcb07fa2e1596ebbbee0833a20b0337163f9d6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1442613350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c27520dbe24ddc045216c37cc47aa58e765aa000a386bc55372e2063b3bed4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:17:25 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:17:26 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9fbb5bb66b4765df4292381a96e1cfc78d67a08a48a930d66d57438abacd1`  
		Last Modified: Thu, 12 Jan 2023 05:42:25 GMT  
		Size: 612.2 KB (612183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f7f7f53251ba2d0181e199d1bd37876042b23e037cf0cd6a8678056c7a98a6`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4544079819db2e2462b9038aae6831b0fd0c36c80dbe76a11a5ffbdad78e7664`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b86944ef48015c16735dee2382dbeabc6fd568d801115b072f686fc0526631`  
		Last Modified: Sat, 21 Jan 2023 01:20:09 GMT  
		Size: 56.0 MB (55967846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:5639bb93318b23396e1f042343cce52f2281a3ffd5ba174ca19b76b3b3c69a3c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1764075185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ad0f3cc6a58f272290a178406070162ea53046d3d87f8b10b030df2c90a70a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:18:11 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:18:13 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1203a660d1e7b9cba56b0f2b04e0f4d443536c90572741405636436ed42c43`  
		Last Modified: Thu, 12 Jan 2023 05:42:38 GMT  
		Size: 365.4 KB (365388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc933231f525632f226b4c16194bf32a3adf3e01067661c25cd3ab6086490b`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a46a5a5f1ab4b72084c67f039869f7ad88b4872681007659ecefbf38bf6af20`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d463f4d2ea1bed72ce82bd6b4a98f88513b4799d253684f46b220c0495b358c1`  
		Last Modified: Sat, 21 Jan 2023 01:20:34 GMT  
		Size: 55.8 MB (55761582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:b14c305e443d06050ef5660c5973adb221a0b1f9e0fd09ad42d4561f977283bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:5639bb93318b23396e1f042343cce52f2281a3ffd5ba174ca19b76b3b3c69a3c
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1764075185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ad0f3cc6a58f272290a178406070162ea53046d3d87f8b10b030df2c90a70a`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:18:11 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:18:13 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691d210e0841eeceff800f3b441be6db4bc689728f1bb771ce88f839d06f57d0`  
		Last Modified: Thu, 12 Jan 2023 02:34:04 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1203a660d1e7b9cba56b0f2b04e0f4d443536c90572741405636436ed42c43`  
		Last Modified: Thu, 12 Jan 2023 05:42:38 GMT  
		Size: 365.4 KB (365388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9cc933231f525632f226b4c16194bf32a3adf3e01067661c25cd3ab6086490b`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a46a5a5f1ab4b72084c67f039869f7ad88b4872681007659ecefbf38bf6af20`  
		Last Modified: Sat, 21 Jan 2023 01:20:22 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d463f4d2ea1bed72ce82bd6b4a98f88513b4799d253684f46b220c0495b358c1`  
		Last Modified: Sat, 21 Jan 2023 01:20:34 GMT  
		Size: 55.8 MB (55761582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:ea15275a18f3012592e67e8051872a11e2b2945203b191c1da0d5771fb77d3ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:70a5dbaf037e96c1033085997dcb07fa2e1596ebbbee0833a20b0337163f9d6b
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1442613350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c27520dbe24ddc045216c37cc47aa58e765aa000a386bc55372e2063b3bed4`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 21 Jan 2023 01:17:25 GMT
ENV DOCKER_VERSION=20.10.23
# Sat, 21 Jan 2023 01:17:26 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.23.zip
# Sat, 21 Jan 2023 01:18:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa41f3a43cc9e40e953b9cfe1530c27eed49cf79cdae96e9dfc39b04a1b75ecf`  
		Last Modified: Thu, 12 Jan 2023 02:29:45 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf9fbb5bb66b4765df4292381a96e1cfc78d67a08a48a930d66d57438abacd1`  
		Last Modified: Thu, 12 Jan 2023 05:42:25 GMT  
		Size: 612.2 KB (612183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f7f7f53251ba2d0181e199d1bd37876042b23e037cf0cd6a8678056c7a98a6`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4544079819db2e2462b9038aae6831b0fd0c36c80dbe76a11a5ffbdad78e7664`  
		Last Modified: Sat, 21 Jan 2023 01:19:58 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b86944ef48015c16735dee2382dbeabc6fd568d801115b072f686fc0526631`  
		Last Modified: Sat, 21 Jan 2023 01:20:09 GMT  
		Size: 56.0 MB (55967846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
