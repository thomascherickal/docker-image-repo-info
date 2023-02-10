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
-	[`docker:23.0.1`](#docker2301)
-	[`docker:23.0.1-alpine3.17`](#docker2301-alpine317)
-	[`docker:23.0.1-cli`](#docker2301-cli)
-	[`docker:23.0.1-cli-alpine3.17`](#docker2301-cli-alpine317)
-	[`docker:23.0.1-dind`](#docker2301-dind)
-	[`docker:23.0.1-dind-alpine3.17`](#docker2301-dind-alpine317)
-	[`docker:23.0.1-dind-rootless`](#docker2301-dind-rootless)
-	[`docker:23.0.1-git`](#docker2301-git)
-	[`docker:23.0.1-windowsservercore`](#docker2301-windowsservercore)
-	[`docker:23.0.1-windowsservercore-1809`](#docker2301-windowsservercore-1809)
-	[`docker:23.0.1-windowsservercore-ltsc2022`](#docker2301-windowsservercore-ltsc2022)
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
$ docker pull docker@sha256:cd9b4d47651788ed1f32bc131ef22f42b9222c0b0750352073ceceda114763b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20` - linux; amd64

```console
$ docker pull docker@sha256:bc8f9f4b0cc421f0c70bdc05a02862eb60332b3b3709edfc92a187c32bb8b2e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50758855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88c236d65f5ade44463973beaa59550d57b1005025301fa3f580577822e74ea`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:96af89bbac131bbf583aed882a3cdf93aa8f93b3ab086642e3e3b0bcc542b5d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46295813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557fb0f2a956299c610fac400a0b42c683fd9483b32a6eb856eb2609b2c04f6`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-cli`

```console
$ docker pull docker@sha256:cd9b4d47651788ed1f32bc131ef22f42b9222c0b0750352073ceceda114763b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-cli` - linux; amd64

```console
$ docker pull docker@sha256:bc8f9f4b0cc421f0c70bdc05a02862eb60332b3b3709edfc92a187c32bb8b2e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50758855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88c236d65f5ade44463973beaa59550d57b1005025301fa3f580577822e74ea`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:96af89bbac131bbf583aed882a3cdf93aa8f93b3ab086642e3e3b0bcc542b5d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46295813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557fb0f2a956299c610fac400a0b42c683fd9483b32a6eb856eb2609b2c04f6`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind`

```console
$ docker pull docker@sha256:901c6805c0f1da51ca0ce879bb6566e26f8d8f9ebfb545a6f0a2b4e52c22ab69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind` - linux; amd64

```console
$ docker pull docker@sha256:6159865b08ae8ff72347679562e9d1b6a4d2c7d01cbba14a07bcbd2c28e1b17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110618607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f1e4455f1560756473210f66a697ff667365dcd7e0cc8c892bc02c2bff6179`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:20:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:20:17 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:20:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:32 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:32 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:32 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:33 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:33 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a3786230fec8b2e8ea1d6552b03a9681baca465150bef02e02b5afee3d78ba`  
		Last Modified: Wed, 08 Feb 2023 23:23:07 GMT  
		Size: 6.8 MB (6837950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133e82c7a9eacfbce784e854848d1cf3783e2e9e7aeb7ccf00dccb3afed319a6`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1726821a9b880be1a65b9252ec76a1c1a6d862be6c2d24d370946b578ada6`  
		Last Modified: Wed, 08 Feb 2023 23:23:13 GMT  
		Size: 53.0 MB (53016614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65af730be0a8c810ef5456e304c21b22b0332c41746bfb8a6b9313b1e9e7fa46`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8620ede1f7013bcc1d4ffe2f8f5931d564b59efea015d121ec0c43fcd28736d5`  
		Last Modified: Fri, 10 Feb 2023 18:24:57 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:983cb0a95194cf49e6b1c11ffc02571754ff7f3213ae1e016e543987a11e5c8b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101972537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0351ed2e1de673fbd6fb5746511f27dfc9002cd1132bf338d192035cf58409bb`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:40:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:40:04 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:40:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:18 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:18 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:18 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:18 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:18 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e874c6fdbe7145e5147cf03134043b5c7b1dc1387fb173c17c4856ba27f344ea`  
		Last Modified: Wed, 08 Feb 2023 23:42:46 GMT  
		Size: 7.0 MB (6991132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ef4db2270128049db3c0bd9eab51724f7a624b3a6903ff3bc6ff5b55732cd0`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e662ab7ef4842b45920649d0ef5c7faeaa2a0cd51ec9d6fd7d99fe8f0cd67c82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 48.7 MB (48680403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e39c54ad4cd3332ae45fc32facbe6289cbd09c69dc47945ee52b60271dc2`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f7f377b9529e3248c464543228e2bb5a9026712dc25cef21d1f19654be56a3`  
		Last Modified: Fri, 10 Feb 2023 01:42:43 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:b8feb031ef5ead5f164e005dcefc768ef33ab0ab6313db1ba51a05927d88a01e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ab1410405ead532055c5f5ad787da7d9f24c3e9b596fd9173fc3b58c671a5219
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131905514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e35590a3624a5952f1690004750072e6672520cd5e2db37a5633a143a5f4ebc`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:20:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:20:17 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:20:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:32 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:32 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:32 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:33 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:33 GMT
CMD []
# Fri, 10 Feb 2023 18:22:36 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 18:22:37 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 18:22:37 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 18:22:40 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 18:22:40 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 18:22:40 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a3786230fec8b2e8ea1d6552b03a9681baca465150bef02e02b5afee3d78ba`  
		Last Modified: Wed, 08 Feb 2023 23:23:07 GMT  
		Size: 6.8 MB (6837950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133e82c7a9eacfbce784e854848d1cf3783e2e9e7aeb7ccf00dccb3afed319a6`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1726821a9b880be1a65b9252ec76a1c1a6d862be6c2d24d370946b578ada6`  
		Last Modified: Wed, 08 Feb 2023 23:23:13 GMT  
		Size: 53.0 MB (53016614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65af730be0a8c810ef5456e304c21b22b0332c41746bfb8a6b9313b1e9e7fa46`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8620ede1f7013bcc1d4ffe2f8f5931d564b59efea015d121ec0c43fcd28736d5`  
		Last Modified: Fri, 10 Feb 2023 18:24:57 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2d7dbc0c5e0eb5cf38cbbe764923e1231d97670a81bda66697a8cce36c0a2e`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 1.4 MB (1375665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4f5adf0c18a5f46528e401f035e36d0fadf41871df28bc7343286f37b8c0d0`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c17c0886bcfa70b12ef21bc065a55367bd1324ef247987df6d0e4bffdd5ee2`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06b42082b56e18be55827349ac3363fb803fe4e1ad8c60f845d648c1083e0ca`  
		Last Modified: Fri, 10 Feb 2023 18:25:15 GMT  
		Size: 19.9 MB (19909525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feeffbb4b636ab6ccda9e566b256782c4c2dd4b94be98ab72802b8393330652`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c2db0c76de7f007539eac3fcc471b817fafc8ef1bfa32ad01f6a989fe6e7f985
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125257696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af933fec0f6c7f7a96cc947525e0c052c2009722276f1dfd470ad5b4fbe8b5`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:40:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:40:04 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:40:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:18 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:18 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:18 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:18 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:18 GMT
CMD []
# Fri, 10 Feb 2023 01:40:21 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 01:40:22 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 01:40:22 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 01:40:25 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 01:40:25 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 01:40:25 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e874c6fdbe7145e5147cf03134043b5c7b1dc1387fb173c17c4856ba27f344ea`  
		Last Modified: Wed, 08 Feb 2023 23:42:46 GMT  
		Size: 7.0 MB (6991132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ef4db2270128049db3c0bd9eab51724f7a624b3a6903ff3bc6ff5b55732cd0`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e662ab7ef4842b45920649d0ef5c7faeaa2a0cd51ec9d6fd7d99fe8f0cd67c82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 48.7 MB (48680403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e39c54ad4cd3332ae45fc32facbe6289cbd09c69dc47945ee52b60271dc2`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f7f377b9529e3248c464543228e2bb5a9026712dc25cef21d1f19654be56a3`  
		Last Modified: Fri, 10 Feb 2023 01:42:43 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10dcb13ac0c9efe482c70acb11888a8cab595cb59f34b9fb5238e4286284793`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 1.4 MB (1401566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a284f26ce91d88efa6100549509d51544cbd8821790a6acacd2ad53e552e11`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d877913246c4f79cd42bea937d784bcdeb12e67973b3449735dbec206fda0b`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b734d91a07346c0013d8cb49d142b18f046aa4b3e6d0d83b3bdaf79f958688c`  
		Last Modified: Fri, 10 Feb 2023 01:42:59 GMT  
		Size: 21.9 MB (21881869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6404a64e6d572bba08511eb866e1a2984b29a1718bf23ba6c22de1a5ee41ce`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20-git`

```console
$ docker pull docker@sha256:11331c07da7c6b1923dd27755216c35f09267ac56fe84d6427ff2f9065a62809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-git` - linux; amd64

```console
$ docker pull docker@sha256:0524de3fd9c569649b9cd43e492188690a2ddefa417cfbd2502e9d1a30353b76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54902464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da536a967eb861bcba207a0eb975e9ad6bb8fd0e07be098add1ea147c32603bb`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:20:31 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506a620b017c02b66a7738e053875a5de7d97db7a8d4e3c7ef8508da5cff8c02`  
		Last Modified: Wed, 08 Feb 2023 23:23:44 GMT  
		Size: 4.1 MB (4143609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5a8b12fc51a874a2cba1c845a661f3d3d1f358a3376b1121ae8f38e6925c5c0f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50481733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c984436456e1790c2b69715d275ffa8c39842d8920260c25ae9ef3404fbdd965`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:40:16 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168107c95ac1a091e3c254b2e3dce1e86a5f365256e5eaf2837b03fe7d536b7c`  
		Last Modified: Wed, 08 Feb 2023 23:43:21 GMT  
		Size: 4.2 MB (4185920 bytes)  
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
$ docker pull docker@sha256:cd9b4d47651788ed1f32bc131ef22f42b9222c0b0750352073ceceda114763b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10` - linux; amd64

```console
$ docker pull docker@sha256:bc8f9f4b0cc421f0c70bdc05a02862eb60332b3b3709edfc92a187c32bb8b2e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50758855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88c236d65f5ade44463973beaa59550d57b1005025301fa3f580577822e74ea`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:96af89bbac131bbf583aed882a3cdf93aa8f93b3ab086642e3e3b0bcc542b5d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46295813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557fb0f2a956299c610fac400a0b42c683fd9483b32a6eb856eb2609b2c04f6`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-cli`

```console
$ docker pull docker@sha256:cd9b4d47651788ed1f32bc131ef22f42b9222c0b0750352073ceceda114763b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-cli` - linux; amd64

```console
$ docker pull docker@sha256:bc8f9f4b0cc421f0c70bdc05a02862eb60332b3b3709edfc92a187c32bb8b2e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50758855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88c236d65f5ade44463973beaa59550d57b1005025301fa3f580577822e74ea`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:96af89bbac131bbf583aed882a3cdf93aa8f93b3ab086642e3e3b0bcc542b5d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46295813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557fb0f2a956299c610fac400a0b42c683fd9483b32a6eb856eb2609b2c04f6`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind`

```console
$ docker pull docker@sha256:901c6805c0f1da51ca0ce879bb6566e26f8d8f9ebfb545a6f0a2b4e52c22ab69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind` - linux; amd64

```console
$ docker pull docker@sha256:6159865b08ae8ff72347679562e9d1b6a4d2c7d01cbba14a07bcbd2c28e1b17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110618607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f1e4455f1560756473210f66a697ff667365dcd7e0cc8c892bc02c2bff6179`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:20:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:20:17 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:20:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:32 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:32 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:32 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:33 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:33 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a3786230fec8b2e8ea1d6552b03a9681baca465150bef02e02b5afee3d78ba`  
		Last Modified: Wed, 08 Feb 2023 23:23:07 GMT  
		Size: 6.8 MB (6837950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133e82c7a9eacfbce784e854848d1cf3783e2e9e7aeb7ccf00dccb3afed319a6`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1726821a9b880be1a65b9252ec76a1c1a6d862be6c2d24d370946b578ada6`  
		Last Modified: Wed, 08 Feb 2023 23:23:13 GMT  
		Size: 53.0 MB (53016614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65af730be0a8c810ef5456e304c21b22b0332c41746bfb8a6b9313b1e9e7fa46`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8620ede1f7013bcc1d4ffe2f8f5931d564b59efea015d121ec0c43fcd28736d5`  
		Last Modified: Fri, 10 Feb 2023 18:24:57 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:983cb0a95194cf49e6b1c11ffc02571754ff7f3213ae1e016e543987a11e5c8b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101972537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0351ed2e1de673fbd6fb5746511f27dfc9002cd1132bf338d192035cf58409bb`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:40:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:40:04 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:40:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:18 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:18 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:18 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:18 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:18 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e874c6fdbe7145e5147cf03134043b5c7b1dc1387fb173c17c4856ba27f344ea`  
		Last Modified: Wed, 08 Feb 2023 23:42:46 GMT  
		Size: 7.0 MB (6991132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ef4db2270128049db3c0bd9eab51724f7a624b3a6903ff3bc6ff5b55732cd0`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e662ab7ef4842b45920649d0ef5c7faeaa2a0cd51ec9d6fd7d99fe8f0cd67c82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 48.7 MB (48680403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e39c54ad4cd3332ae45fc32facbe6289cbd09c69dc47945ee52b60271dc2`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f7f377b9529e3248c464543228e2bb5a9026712dc25cef21d1f19654be56a3`  
		Last Modified: Fri, 10 Feb 2023 01:42:43 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-dind-rootless`

```console
$ docker pull docker@sha256:b8feb031ef5ead5f164e005dcefc768ef33ab0ab6313db1ba51a05927d88a01e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ab1410405ead532055c5f5ad787da7d9f24c3e9b596fd9173fc3b58c671a5219
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131905514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e35590a3624a5952f1690004750072e6672520cd5e2db37a5633a143a5f4ebc`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:20:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:20:17 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:20:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:32 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:32 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:32 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:33 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:33 GMT
CMD []
# Fri, 10 Feb 2023 18:22:36 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 18:22:37 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 18:22:37 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 18:22:40 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 18:22:40 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 18:22:40 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a3786230fec8b2e8ea1d6552b03a9681baca465150bef02e02b5afee3d78ba`  
		Last Modified: Wed, 08 Feb 2023 23:23:07 GMT  
		Size: 6.8 MB (6837950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133e82c7a9eacfbce784e854848d1cf3783e2e9e7aeb7ccf00dccb3afed319a6`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1726821a9b880be1a65b9252ec76a1c1a6d862be6c2d24d370946b578ada6`  
		Last Modified: Wed, 08 Feb 2023 23:23:13 GMT  
		Size: 53.0 MB (53016614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65af730be0a8c810ef5456e304c21b22b0332c41746bfb8a6b9313b1e9e7fa46`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8620ede1f7013bcc1d4ffe2f8f5931d564b59efea015d121ec0c43fcd28736d5`  
		Last Modified: Fri, 10 Feb 2023 18:24:57 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2d7dbc0c5e0eb5cf38cbbe764923e1231d97670a81bda66697a8cce36c0a2e`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 1.4 MB (1375665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4f5adf0c18a5f46528e401f035e36d0fadf41871df28bc7343286f37b8c0d0`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c17c0886bcfa70b12ef21bc065a55367bd1324ef247987df6d0e4bffdd5ee2`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06b42082b56e18be55827349ac3363fb803fe4e1ad8c60f845d648c1083e0ca`  
		Last Modified: Fri, 10 Feb 2023 18:25:15 GMT  
		Size: 19.9 MB (19909525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feeffbb4b636ab6ccda9e566b256782c4c2dd4b94be98ab72802b8393330652`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c2db0c76de7f007539eac3fcc471b817fafc8ef1bfa32ad01f6a989fe6e7f985
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125257696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af933fec0f6c7f7a96cc947525e0c052c2009722276f1dfd470ad5b4fbe8b5`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:40:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:40:04 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:40:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:18 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:18 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:18 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:18 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:18 GMT
CMD []
# Fri, 10 Feb 2023 01:40:21 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 01:40:22 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 01:40:22 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 01:40:25 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 01:40:25 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 01:40:25 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e874c6fdbe7145e5147cf03134043b5c7b1dc1387fb173c17c4856ba27f344ea`  
		Last Modified: Wed, 08 Feb 2023 23:42:46 GMT  
		Size: 7.0 MB (6991132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ef4db2270128049db3c0bd9eab51724f7a624b3a6903ff3bc6ff5b55732cd0`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e662ab7ef4842b45920649d0ef5c7faeaa2a0cd51ec9d6fd7d99fe8f0cd67c82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 48.7 MB (48680403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e39c54ad4cd3332ae45fc32facbe6289cbd09c69dc47945ee52b60271dc2`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f7f377b9529e3248c464543228e2bb5a9026712dc25cef21d1f19654be56a3`  
		Last Modified: Fri, 10 Feb 2023 01:42:43 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10dcb13ac0c9efe482c70acb11888a8cab595cb59f34b9fb5238e4286284793`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 1.4 MB (1401566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a284f26ce91d88efa6100549509d51544cbd8821790a6acacd2ad53e552e11`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d877913246c4f79cd42bea937d784bcdeb12e67973b3449735dbec206fda0b`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b734d91a07346c0013d8cb49d142b18f046aa4b3e6d0d83b3bdaf79f958688c`  
		Last Modified: Fri, 10 Feb 2023 01:42:59 GMT  
		Size: 21.9 MB (21881869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6404a64e6d572bba08511eb866e1a2984b29a1718bf23ba6c22de1a5ee41ce`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10-git`

```console
$ docker pull docker@sha256:11331c07da7c6b1923dd27755216c35f09267ac56fe84d6427ff2f9065a62809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10-git` - linux; amd64

```console
$ docker pull docker@sha256:0524de3fd9c569649b9cd43e492188690a2ddefa417cfbd2502e9d1a30353b76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54902464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da536a967eb861bcba207a0eb975e9ad6bb8fd0e07be098add1ea147c32603bb`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:20:31 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506a620b017c02b66a7738e053875a5de7d97db7a8d4e3c7ef8508da5cff8c02`  
		Last Modified: Wed, 08 Feb 2023 23:23:44 GMT  
		Size: 4.1 MB (4143609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5a8b12fc51a874a2cba1c845a661f3d3d1f358a3376b1121ae8f38e6925c5c0f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50481733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c984436456e1790c2b69715d275ffa8c39842d8920260c25ae9ef3404fbdd965`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:40:16 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168107c95ac1a091e3c254b2e3dce1e86a5f365256e5eaf2837b03fe7d536b7c`  
		Last Modified: Wed, 08 Feb 2023 23:43:21 GMT  
		Size: 4.2 MB (4185920 bytes)  
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
$ docker pull docker@sha256:cd9b4d47651788ed1f32bc131ef22f42b9222c0b0750352073ceceda114763b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23` - linux; amd64

```console
$ docker pull docker@sha256:bc8f9f4b0cc421f0c70bdc05a02862eb60332b3b3709edfc92a187c32bb8b2e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50758855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88c236d65f5ade44463973beaa59550d57b1005025301fa3f580577822e74ea`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:96af89bbac131bbf583aed882a3cdf93aa8f93b3ab086642e3e3b0bcc542b5d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46295813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557fb0f2a956299c610fac400a0b42c683fd9483b32a6eb856eb2609b2c04f6`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-alpine3.17`

```console
$ docker pull docker@sha256:cd9b4d47651788ed1f32bc131ef22f42b9222c0b0750352073ceceda114763b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-alpine3.17` - linux; amd64

```console
$ docker pull docker@sha256:bc8f9f4b0cc421f0c70bdc05a02862eb60332b3b3709edfc92a187c32bb8b2e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50758855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88c236d65f5ade44463973beaa59550d57b1005025301fa3f580577822e74ea`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:96af89bbac131bbf583aed882a3cdf93aa8f93b3ab086642e3e3b0bcc542b5d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46295813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557fb0f2a956299c610fac400a0b42c683fd9483b32a6eb856eb2609b2c04f6`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-cli`

```console
$ docker pull docker@sha256:cd9b4d47651788ed1f32bc131ef22f42b9222c0b0750352073ceceda114763b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-cli` - linux; amd64

```console
$ docker pull docker@sha256:bc8f9f4b0cc421f0c70bdc05a02862eb60332b3b3709edfc92a187c32bb8b2e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50758855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88c236d65f5ade44463973beaa59550d57b1005025301fa3f580577822e74ea`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:96af89bbac131bbf583aed882a3cdf93aa8f93b3ab086642e3e3b0bcc542b5d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46295813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557fb0f2a956299c610fac400a0b42c683fd9483b32a6eb856eb2609b2c04f6`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-cli-alpine3.17`

```console
$ docker pull docker@sha256:cd9b4d47651788ed1f32bc131ef22f42b9222c0b0750352073ceceda114763b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-cli-alpine3.17` - linux; amd64

```console
$ docker pull docker@sha256:bc8f9f4b0cc421f0c70bdc05a02862eb60332b3b3709edfc92a187c32bb8b2e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50758855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f88c236d65f5ade44463973beaa59550d57b1005025301fa3f580577822e74ea`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-cli-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:96af89bbac131bbf583aed882a3cdf93aa8f93b3ab086642e3e3b0bcc542b5d6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46295813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5557fb0f2a956299c610fac400a0b42c683fd9483b32a6eb856eb2609b2c04f6`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-dind`

```console
$ docker pull docker@sha256:901c6805c0f1da51ca0ce879bb6566e26f8d8f9ebfb545a6f0a2b4e52c22ab69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-dind` - linux; amd64

```console
$ docker pull docker@sha256:6159865b08ae8ff72347679562e9d1b6a4d2c7d01cbba14a07bcbd2c28e1b17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110618607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f1e4455f1560756473210f66a697ff667365dcd7e0cc8c892bc02c2bff6179`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:20:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:20:17 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:20:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:32 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:32 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:32 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:33 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:33 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a3786230fec8b2e8ea1d6552b03a9681baca465150bef02e02b5afee3d78ba`  
		Last Modified: Wed, 08 Feb 2023 23:23:07 GMT  
		Size: 6.8 MB (6837950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133e82c7a9eacfbce784e854848d1cf3783e2e9e7aeb7ccf00dccb3afed319a6`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1726821a9b880be1a65b9252ec76a1c1a6d862be6c2d24d370946b578ada6`  
		Last Modified: Wed, 08 Feb 2023 23:23:13 GMT  
		Size: 53.0 MB (53016614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65af730be0a8c810ef5456e304c21b22b0332c41746bfb8a6b9313b1e9e7fa46`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8620ede1f7013bcc1d4ffe2f8f5931d564b59efea015d121ec0c43fcd28736d5`  
		Last Modified: Fri, 10 Feb 2023 18:24:57 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:983cb0a95194cf49e6b1c11ffc02571754ff7f3213ae1e016e543987a11e5c8b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101972537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0351ed2e1de673fbd6fb5746511f27dfc9002cd1132bf338d192035cf58409bb`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:40:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:40:04 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:40:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:18 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:18 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:18 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:18 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:18 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e874c6fdbe7145e5147cf03134043b5c7b1dc1387fb173c17c4856ba27f344ea`  
		Last Modified: Wed, 08 Feb 2023 23:42:46 GMT  
		Size: 7.0 MB (6991132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ef4db2270128049db3c0bd9eab51724f7a624b3a6903ff3bc6ff5b55732cd0`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e662ab7ef4842b45920649d0ef5c7faeaa2a0cd51ec9d6fd7d99fe8f0cd67c82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 48.7 MB (48680403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e39c54ad4cd3332ae45fc32facbe6289cbd09c69dc47945ee52b60271dc2`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f7f377b9529e3248c464543228e2bb5a9026712dc25cef21d1f19654be56a3`  
		Last Modified: Fri, 10 Feb 2023 01:42:43 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-dind-alpine3.17`

```console
$ docker pull docker@sha256:901c6805c0f1da51ca0ce879bb6566e26f8d8f9ebfb545a6f0a2b4e52c22ab69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-dind-alpine3.17` - linux; amd64

```console
$ docker pull docker@sha256:6159865b08ae8ff72347679562e9d1b6a4d2c7d01cbba14a07bcbd2c28e1b17a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110618607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5f1e4455f1560756473210f66a697ff667365dcd7e0cc8c892bc02c2bff6179`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:20:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:20:17 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:20:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:32 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:32 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:32 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:33 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:33 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a3786230fec8b2e8ea1d6552b03a9681baca465150bef02e02b5afee3d78ba`  
		Last Modified: Wed, 08 Feb 2023 23:23:07 GMT  
		Size: 6.8 MB (6837950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133e82c7a9eacfbce784e854848d1cf3783e2e9e7aeb7ccf00dccb3afed319a6`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1726821a9b880be1a65b9252ec76a1c1a6d862be6c2d24d370946b578ada6`  
		Last Modified: Wed, 08 Feb 2023 23:23:13 GMT  
		Size: 53.0 MB (53016614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65af730be0a8c810ef5456e304c21b22b0332c41746bfb8a6b9313b1e9e7fa46`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8620ede1f7013bcc1d4ffe2f8f5931d564b59efea015d121ec0c43fcd28736d5`  
		Last Modified: Fri, 10 Feb 2023 18:24:57 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-dind-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:983cb0a95194cf49e6b1c11ffc02571754ff7f3213ae1e016e543987a11e5c8b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.0 MB (101972537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0351ed2e1de673fbd6fb5746511f27dfc9002cd1132bf338d192035cf58409bb`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:40:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:40:04 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:40:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:18 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:18 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:18 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:18 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:18 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e874c6fdbe7145e5147cf03134043b5c7b1dc1387fb173c17c4856ba27f344ea`  
		Last Modified: Wed, 08 Feb 2023 23:42:46 GMT  
		Size: 7.0 MB (6991132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ef4db2270128049db3c0bd9eab51724f7a624b3a6903ff3bc6ff5b55732cd0`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e662ab7ef4842b45920649d0ef5c7faeaa2a0cd51ec9d6fd7d99fe8f0cd67c82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 48.7 MB (48680403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e39c54ad4cd3332ae45fc32facbe6289cbd09c69dc47945ee52b60271dc2`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f7f377b9529e3248c464543228e2bb5a9026712dc25cef21d1f19654be56a3`  
		Last Modified: Fri, 10 Feb 2023 01:42:43 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-dind-rootless`

```console
$ docker pull docker@sha256:b8feb031ef5ead5f164e005dcefc768ef33ab0ab6313db1ba51a05927d88a01e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:ab1410405ead532055c5f5ad787da7d9f24c3e9b596fd9173fc3b58c671a5219
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131905514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e35590a3624a5952f1690004750072e6672520cd5e2db37a5633a143a5f4ebc`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:20:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:20:17 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:20:17 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:20:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:32 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:32 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:32 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:33 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:33 GMT
CMD []
# Fri, 10 Feb 2023 18:22:36 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 18:22:37 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 18:22:37 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 18:22:40 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 18:22:40 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 18:22:40 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08a3786230fec8b2e8ea1d6552b03a9681baca465150bef02e02b5afee3d78ba`  
		Last Modified: Wed, 08 Feb 2023 23:23:07 GMT  
		Size: 6.8 MB (6837950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:133e82c7a9eacfbce784e854848d1cf3783e2e9e7aeb7ccf00dccb3afed319a6`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed1726821a9b880be1a65b9252ec76a1c1a6d862be6c2d24d370946b578ada6`  
		Last Modified: Wed, 08 Feb 2023 23:23:13 GMT  
		Size: 53.0 MB (53016614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65af730be0a8c810ef5456e304c21b22b0332c41746bfb8a6b9313b1e9e7fa46`  
		Last Modified: Wed, 08 Feb 2023 23:23:05 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8620ede1f7013bcc1d4ffe2f8f5931d564b59efea015d121ec0c43fcd28736d5`  
		Last Modified: Fri, 10 Feb 2023 18:24:57 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2d7dbc0c5e0eb5cf38cbbe764923e1231d97670a81bda66697a8cce36c0a2e`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 1.4 MB (1375665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4f5adf0c18a5f46528e401f035e36d0fadf41871df28bc7343286f37b8c0d0`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c17c0886bcfa70b12ef21bc065a55367bd1324ef247987df6d0e4bffdd5ee2`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06b42082b56e18be55827349ac3363fb803fe4e1ad8c60f845d648c1083e0ca`  
		Last Modified: Fri, 10 Feb 2023 18:25:15 GMT  
		Size: 19.9 MB (19909525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7feeffbb4b636ab6ccda9e566b256782c4c2dd4b94be98ab72802b8393330652`  
		Last Modified: Fri, 10 Feb 2023 18:25:12 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:c2db0c76de7f007539eac3fcc471b817fafc8ef1bfa32ad01f6a989fe6e7f985
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125257696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97af933fec0f6c7f7a96cc947525e0c052c2009722276f1dfd470ad5b4fbe8b5`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 08 Feb 2023 23:39:58 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 08 Feb 2023 23:40:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.23.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.23.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 08 Feb 2023 23:40:04 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 08 Feb 2023 23:40:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:18 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:18 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:18 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:18 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:18 GMT
CMD []
# Fri, 10 Feb 2023 01:40:21 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 01:40:22 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 01:40:22 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.23.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.23.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 01:40:25 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 01:40:25 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 01:40:25 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e874c6fdbe7145e5147cf03134043b5c7b1dc1387fb173c17c4856ba27f344ea`  
		Last Modified: Wed, 08 Feb 2023 23:42:46 GMT  
		Size: 7.0 MB (6991132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ef4db2270128049db3c0bd9eab51724f7a624b3a6903ff3bc6ff5b55732cd0`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e662ab7ef4842b45920649d0ef5c7faeaa2a0cd51ec9d6fd7d99fe8f0cd67c82`  
		Last Modified: Wed, 08 Feb 2023 23:42:51 GMT  
		Size: 48.7 MB (48680403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c373e39c54ad4cd3332ae45fc32facbe6289cbd09c69dc47945ee52b60271dc2`  
		Last Modified: Wed, 08 Feb 2023 23:42:45 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f7f377b9529e3248c464543228e2bb5a9026712dc25cef21d1f19654be56a3`  
		Last Modified: Fri, 10 Feb 2023 01:42:43 GMT  
		Size: 2.8 KB (2822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10dcb13ac0c9efe482c70acb11888a8cab595cb59f34b9fb5238e4286284793`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 1.4 MB (1401566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a284f26ce91d88efa6100549509d51544cbd8821790a6acacd2ad53e552e11`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d877913246c4f79cd42bea937d784bcdeb12e67973b3449735dbec206fda0b`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b734d91a07346c0013d8cb49d142b18f046aa4b3e6d0d83b3bdaf79f958688c`  
		Last Modified: Fri, 10 Feb 2023 01:42:59 GMT  
		Size: 21.9 MB (21881869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6404a64e6d572bba08511eb866e1a2984b29a1718bf23ba6c22de1a5ee41ce`  
		Last Modified: Fri, 10 Feb 2023 01:42:56 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:20.10.23-git`

```console
$ docker pull docker@sha256:11331c07da7c6b1923dd27755216c35f09267ac56fe84d6427ff2f9065a62809
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20.10.23-git` - linux; amd64

```console
$ docker pull docker@sha256:0524de3fd9c569649b9cd43e492188690a2ddefa417cfbd2502e9d1a30353b76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54902464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da536a967eb861bcba207a0eb975e9ad6bb8fd0e07be098add1ea147c32603bb`
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
# Wed, 08 Feb 2023 23:20:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:20:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:20:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:20:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:20:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:20:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:20:06 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:20:31 GMT
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
	-	`sha256:7b9ed87865f8145889c4fab3fa44219774b3dfda74e20b6e64dbc59d5923b48d`  
		Last Modified: Wed, 08 Feb 2023 23:22:43 GMT  
		Size: 15.3 MB (15343478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ed807a82d49a03f5063d3c53840779019bdd9cf41a442a9d061fc72683fcd0`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcac7dbfc98a0aa7cc41e9d0e680afe943b96bfc67996b05dcb8b92399ffc611`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d33d751839bdb615f5b7fd26c9ef95073bea42400802b189ff381d9c4856dc56`  
		Last Modified: Wed, 08 Feb 2023 23:22:40 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506a620b017c02b66a7738e053875a5de7d97db7a8d4e3c7ef8508da5cff8c02`  
		Last Modified: Wed, 08 Feb 2023 23:23:44 GMT  
		Size: 4.1 MB (4143609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20.10.23-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5a8b12fc51a874a2cba1c845a661f3d3d1f358a3376b1121ae8f38e6925c5c0f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50481733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c984436456e1790c2b69715d275ffa8c39842d8920260c25ae9ef3404fbdd965`
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
# Wed, 08 Feb 2023 23:39:50 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Wed, 08 Feb 2023 23:39:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 08 Feb 2023 23:39:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 08 Feb 2023 23:39:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 08 Feb 2023 23:39:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 08 Feb 2023 23:39:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Feb 2023 23:39:53 GMT
CMD ["sh"]
# Wed, 08 Feb 2023 23:40:16 GMT
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
	-	`sha256:76b2fb7c70c42dffe1c41289728077950743f07bb10d9107058e4cfa8a0cfb4a`  
		Last Modified: Wed, 08 Feb 2023 23:42:23 GMT  
		Size: 13.8 MB (13819095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63041de0294bc860a85a7a9577813388f3cff5ecb1b376d782e55dce825b0592`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0fd4f4c26ae3605b531f7115d8916041d91d80a5fbe1d503ea5026a4148a5`  
		Last Modified: Wed, 08 Feb 2023 23:42:22 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da035c8ad8640c859131ebc8ba3cb220e6faa97aa9d93e8a908efd365212a30d`  
		Last Modified: Wed, 08 Feb 2023 23:42:21 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168107c95ac1a091e3c254b2e3dce1e86a5f365256e5eaf2837b03fe7d536b7c`  
		Last Modified: Wed, 08 Feb 2023 23:43:21 GMT  
		Size: 4.2 MB (4185920 bytes)  
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

```console
$ docker pull docker@sha256:82f534bca79c1b9222851511ed1e85e29d73185ecb820fc7fa24d6bc23f158de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23` - linux; amd64

```console
$ docker pull docker@sha256:ac49b6d30def1445ef481ea0b40112d1ec81bacfb6ebf38678fbb1f485bd55cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111355086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b62af8d4fe6ad7923e26671b2f334fc0ab6b1f2f3f4ebaeef413969b8b76b2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f1b7854dd6e08e6399d76d6407c940ff5256e3d908b67b6a3f2bc67339f0446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102767745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8605baee59c3b6761d42902458231f8ff356810384858298e4cf9ac36475aa`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-cli`

```console
$ docker pull docker@sha256:6ea6ac10351a3f4670424cff8f43272bbc7e221a5692fc6ff1c46b3b717a09eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-cli` - linux; amd64

```console
$ docker pull docker@sha256:c880a3345030d52528b9086f906e6afaf71d5a49be9be121c6213eec91ac3582
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52995991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edf3255c7bac424d71f8e03f71e1a483d3087253906fc07137df8a94bbfb7f35`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4512423530157859811ce109f20c1ee0ce566651bd42fc7c1a896112be6857da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48848520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f1cf9973f493622927611f9c0b59d1a3131b1076ec17ca4896396eeaa00ba`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-dind`

```console
$ docker pull docker@sha256:82f534bca79c1b9222851511ed1e85e29d73185ecb820fc7fa24d6bc23f158de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-dind` - linux; amd64

```console
$ docker pull docker@sha256:ac49b6d30def1445ef481ea0b40112d1ec81bacfb6ebf38678fbb1f485bd55cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111355086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b62af8d4fe6ad7923e26671b2f334fc0ab6b1f2f3f4ebaeef413969b8b76b2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f1b7854dd6e08e6399d76d6407c940ff5256e3d908b67b6a3f2bc67339f0446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102767745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8605baee59c3b6761d42902458231f8ff356810384858298e4cf9ac36475aa`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-dind-rootless`

```console
$ docker pull docker@sha256:92cd2395cb20fec3682222f7af3ad69820c591f44a17e5e1e467fb7a547e060d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:956dcaef873746161a8b4df7ec7758692c81c3dbc44ac6b54283c33d0063d3a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133058390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19fd1ca0a7ee0431a44864140759e7f6b766f38d183dbda33c479b50199e25ea`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
CMD []
# Fri, 10 Feb 2023 18:22:20 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 18:22:20 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 18:22:21 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 18:22:23 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 18:22:24 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 18:22:24 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4a59800b3ff4ea8eef490aa8a8c857489cf86620c9e0520380d6d7f600165e`  
		Last Modified: Fri, 10 Feb 2023 18:24:22 GMT  
		Size: 1.4 MB (1375660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3913a018ce9ccaa6090f5fd22ae38ef94633a82270ed97d9262c4a5acb48ecf`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b668142e8f5abb9532cd382b84634282aed7b6d6c0dc03984c2321d0377d72f0`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea07488668e5eaa6cecf986076943932f4b838bdf7a81ee65bd868d8ef6ff05e`  
		Last Modified: Fri, 10 Feb 2023 18:24:25 GMT  
		Size: 20.3 MB (20325931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb0bb87ed7f9974ff16b062385127b1216f2dff67b20c3a831dcc047c04b5`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:681fd333bfe151c44afc36dadc90d6c7a57739eec704f067a9e31c9ac64b4b04
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126403269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154cee901c71bc181226a8859dfdd45c7a8c964fdb6aa244f8456ca91887575e`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
CMD []
# Fri, 10 Feb 2023 01:40:07 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 01:40:08 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 01:40:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 01:40:11 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 01:40:11 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 01:40:11 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3dc53d7d003c42e619e0f0d987282b443cbd3c27f2ea7adb66fdd00ce482dc`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 1.4 MB (1401559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6a946dbd7e8b65ea508bf6da9de31a6ba5685341a96fea0f596e526e561943`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae187c227f61f574c537060340536d98e81b5a2dbf3fe54dab0ac8958276afd`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781222ed4e59469046da1c4cce7fd70bb7547e5bf0039492c2f75eca75f0ed4c`  
		Last Modified: Fri, 10 Feb 2023 01:42:10 GMT  
		Size: 22.2 MB (22232243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810d859f0d275a30b178e088500caf03121e6d1cf6754976db572876133b124`  
		Last Modified: Fri, 10 Feb 2023 01:42:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-git`

```console
$ docker pull docker@sha256:008585ccb370d47bea570dcd9ed670befbd150c4498cd732724394ccc8b8fa70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23-git` - linux; amd64

```console
$ docker pull docker@sha256:41ed4d04a08469987631a4804370804913ac1c83e6d17a402490173f2f332074
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57139588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db43d1ae0dd659407f03338f3d49c72351f6a856fb5882346dd3bad5bd5041a2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:28 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3e04e933edd5be5e2423369fe61779b1ae2d7897d85031e72446095455f440`  
		Last Modified: Fri, 10 Feb 2023 18:24:41 GMT  
		Size: 4.1 MB (4143597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:85675576039d66bcc9c28de94404d7f3d7496cf13d4246a4c6acf622ed23ee9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53034428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e3e9fb67a75da1d4c083d1d1f74515e47143a9aa60eaa4fb9b238420b3d539`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:40:15 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c226941ea6751d6d947043e88e38ab6035098a001e27328b23d3c278f04c592`  
		Last Modified: Fri, 10 Feb 2023 01:42:25 GMT  
		Size: 4.2 MB (4185908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore`

```console
$ docker pull docker@sha256:6e424a985f0ac4690156b9f335d6345ff6225d0e72d209e17393d4a3cc220c0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `docker:23-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:32ebebed775320910f69ccfd06a3399051911bb12e2629321d15e2f92decf69f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1404240045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837fbe50c93ae962bd5d7df3d8d457cf279cf5c09ec1697153177fe9a3d9b4ba`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:15:53 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:15:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:16:32 GMT
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
	-	`sha256:ceb91a25fd6b227bd2ce1f4f3f0e001e0b4bda5a7f4c104a2f9030837a0217de`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb879bb8ff0dde7aead336ae453cdff5540f8c7f9747a306f758343afefad9f0`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9953dfbd0c49a493b80699b68fb1ba1355d08e2c63b827ef4725a88510898a`  
		Last Modified: Fri, 10 Feb 2023 02:18:16 GMT  
		Size: 17.6 MB (17594490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:ae74f76c3a2177ae1a1ff3ba98fa20d04bf94ad29fc92fb0523dd3efc9818469
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1725697339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5047252e3253ba4fb0d6024419bb9a071aa688f530872917de7e2c10822f8ef1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:16:40 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:16:41 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:17:27 GMT
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
	-	`sha256:16844f8b21e8556c61a8be9f8a035e77965fb2d1a9118446a04ab963453e2818`  
		Last Modified: Fri, 10 Feb 2023 02:18:29 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be212fb1d316bd604c933ad3541fbd93e77d53e596b3502449e519771d577f31`  
		Last Modified: Fri, 10 Feb 2023 02:18:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29150ca563004d89b203a1d45636f9664ff10c98390c8fc3755a45610971a1ea`  
		Last Modified: Fri, 10 Feb 2023 02:18:32 GMT  
		Size: 17.4 MB (17383752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore-1809`

```console
$ docker pull docker@sha256:242c2c7e2cc10720d8b7c21b3ffb73fae24e4b517723abb796d623343a318edd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `docker:23-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:ae74f76c3a2177ae1a1ff3ba98fa20d04bf94ad29fc92fb0523dd3efc9818469
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1725697339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5047252e3253ba4fb0d6024419bb9a071aa688f530872917de7e2c10822f8ef1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:16:40 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:16:41 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:17:27 GMT
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
	-	`sha256:16844f8b21e8556c61a8be9f8a035e77965fb2d1a9118446a04ab963453e2818`  
		Last Modified: Fri, 10 Feb 2023 02:18:29 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be212fb1d316bd604c933ad3541fbd93e77d53e596b3502449e519771d577f31`  
		Last Modified: Fri, 10 Feb 2023 02:18:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29150ca563004d89b203a1d45636f9664ff10c98390c8fc3755a45610971a1ea`  
		Last Modified: Fri, 10 Feb 2023 02:18:32 GMT  
		Size: 17.4 MB (17383752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:3fc74477620758a206afd0639937786867600a94cc05961e56377047c494a0a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `docker:23-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:32ebebed775320910f69ccfd06a3399051911bb12e2629321d15e2f92decf69f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1404240045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837fbe50c93ae962bd5d7df3d8d457cf279cf5c09ec1697153177fe9a3d9b4ba`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:15:53 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:15:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:16:32 GMT
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
	-	`sha256:ceb91a25fd6b227bd2ce1f4f3f0e001e0b4bda5a7f4c104a2f9030837a0217de`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb879bb8ff0dde7aead336ae453cdff5540f8c7f9747a306f758343afefad9f0`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9953dfbd0c49a493b80699b68fb1ba1355d08e2c63b827ef4725a88510898a`  
		Last Modified: Fri, 10 Feb 2023 02:18:16 GMT  
		Size: 17.6 MB (17594490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0`

```console
$ docker pull docker@sha256:82f534bca79c1b9222851511ed1e85e29d73185ecb820fc7fa24d6bc23f158de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0` - linux; amd64

```console
$ docker pull docker@sha256:ac49b6d30def1445ef481ea0b40112d1ec81bacfb6ebf38678fbb1f485bd55cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111355086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b62af8d4fe6ad7923e26671b2f334fc0ab6b1f2f3f4ebaeef413969b8b76b2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f1b7854dd6e08e6399d76d6407c940ff5256e3d908b67b6a3f2bc67339f0446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102767745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8605baee59c3b6761d42902458231f8ff356810384858298e4cf9ac36475aa`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-cli`

```console
$ docker pull docker@sha256:6ea6ac10351a3f4670424cff8f43272bbc7e221a5692fc6ff1c46b3b717a09eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-cli` - linux; amd64

```console
$ docker pull docker@sha256:c880a3345030d52528b9086f906e6afaf71d5a49be9be121c6213eec91ac3582
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52995991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edf3255c7bac424d71f8e03f71e1a483d3087253906fc07137df8a94bbfb7f35`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4512423530157859811ce109f20c1ee0ce566651bd42fc7c1a896112be6857da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48848520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f1cf9973f493622927611f9c0b59d1a3131b1076ec17ca4896396eeaa00ba`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-dind`

```console
$ docker pull docker@sha256:82f534bca79c1b9222851511ed1e85e29d73185ecb820fc7fa24d6bc23f158de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-dind` - linux; amd64

```console
$ docker pull docker@sha256:ac49b6d30def1445ef481ea0b40112d1ec81bacfb6ebf38678fbb1f485bd55cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111355086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b62af8d4fe6ad7923e26671b2f334fc0ab6b1f2f3f4ebaeef413969b8b76b2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f1b7854dd6e08e6399d76d6407c940ff5256e3d908b67b6a3f2bc67339f0446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102767745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8605baee59c3b6761d42902458231f8ff356810384858298e4cf9ac36475aa`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-dind-rootless`

```console
$ docker pull docker@sha256:92cd2395cb20fec3682222f7af3ad69820c591f44a17e5e1e467fb7a547e060d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:956dcaef873746161a8b4df7ec7758692c81c3dbc44ac6b54283c33d0063d3a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133058390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19fd1ca0a7ee0431a44864140759e7f6b766f38d183dbda33c479b50199e25ea`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
CMD []
# Fri, 10 Feb 2023 18:22:20 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 18:22:20 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 18:22:21 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 18:22:23 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 18:22:24 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 18:22:24 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4a59800b3ff4ea8eef490aa8a8c857489cf86620c9e0520380d6d7f600165e`  
		Last Modified: Fri, 10 Feb 2023 18:24:22 GMT  
		Size: 1.4 MB (1375660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3913a018ce9ccaa6090f5fd22ae38ef94633a82270ed97d9262c4a5acb48ecf`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b668142e8f5abb9532cd382b84634282aed7b6d6c0dc03984c2321d0377d72f0`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea07488668e5eaa6cecf986076943932f4b838bdf7a81ee65bd868d8ef6ff05e`  
		Last Modified: Fri, 10 Feb 2023 18:24:25 GMT  
		Size: 20.3 MB (20325931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb0bb87ed7f9974ff16b062385127b1216f2dff67b20c3a831dcc047c04b5`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:681fd333bfe151c44afc36dadc90d6c7a57739eec704f067a9e31c9ac64b4b04
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126403269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154cee901c71bc181226a8859dfdd45c7a8c964fdb6aa244f8456ca91887575e`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
CMD []
# Fri, 10 Feb 2023 01:40:07 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 01:40:08 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 01:40:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 01:40:11 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 01:40:11 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 01:40:11 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3dc53d7d003c42e619e0f0d987282b443cbd3c27f2ea7adb66fdd00ce482dc`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 1.4 MB (1401559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6a946dbd7e8b65ea508bf6da9de31a6ba5685341a96fea0f596e526e561943`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae187c227f61f574c537060340536d98e81b5a2dbf3fe54dab0ac8958276afd`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781222ed4e59469046da1c4cce7fd70bb7547e5bf0039492c2f75eca75f0ed4c`  
		Last Modified: Fri, 10 Feb 2023 01:42:10 GMT  
		Size: 22.2 MB (22232243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810d859f0d275a30b178e088500caf03121e6d1cf6754976db572876133b124`  
		Last Modified: Fri, 10 Feb 2023 01:42:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-git`

```console
$ docker pull docker@sha256:008585ccb370d47bea570dcd9ed670befbd150c4498cd732724394ccc8b8fa70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0-git` - linux; amd64

```console
$ docker pull docker@sha256:41ed4d04a08469987631a4804370804913ac1c83e6d17a402490173f2f332074
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57139588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db43d1ae0dd659407f03338f3d49c72351f6a856fb5882346dd3bad5bd5041a2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:28 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3e04e933edd5be5e2423369fe61779b1ae2d7897d85031e72446095455f440`  
		Last Modified: Fri, 10 Feb 2023 18:24:41 GMT  
		Size: 4.1 MB (4143597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:85675576039d66bcc9c28de94404d7f3d7496cf13d4246a4c6acf622ed23ee9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53034428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e3e9fb67a75da1d4c083d1d1f74515e47143a9aa60eaa4fb9b238420b3d539`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:40:15 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c226941ea6751d6d947043e88e38ab6035098a001e27328b23d3c278f04c592`  
		Last Modified: Fri, 10 Feb 2023 01:42:25 GMT  
		Size: 4.2 MB (4185908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore`

```console
$ docker pull docker@sha256:6e424a985f0ac4690156b9f335d6345ff6225d0e72d209e17393d4a3cc220c0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `docker:23.0-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:32ebebed775320910f69ccfd06a3399051911bb12e2629321d15e2f92decf69f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1404240045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837fbe50c93ae962bd5d7df3d8d457cf279cf5c09ec1697153177fe9a3d9b4ba`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:15:53 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:15:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:16:32 GMT
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
	-	`sha256:ceb91a25fd6b227bd2ce1f4f3f0e001e0b4bda5a7f4c104a2f9030837a0217de`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb879bb8ff0dde7aead336ae453cdff5540f8c7f9747a306f758343afefad9f0`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9953dfbd0c49a493b80699b68fb1ba1355d08e2c63b827ef4725a88510898a`  
		Last Modified: Fri, 10 Feb 2023 02:18:16 GMT  
		Size: 17.6 MB (17594490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:ae74f76c3a2177ae1a1ff3ba98fa20d04bf94ad29fc92fb0523dd3efc9818469
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1725697339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5047252e3253ba4fb0d6024419bb9a071aa688f530872917de7e2c10822f8ef1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:16:40 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:16:41 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:17:27 GMT
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
	-	`sha256:16844f8b21e8556c61a8be9f8a035e77965fb2d1a9118446a04ab963453e2818`  
		Last Modified: Fri, 10 Feb 2023 02:18:29 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be212fb1d316bd604c933ad3541fbd93e77d53e596b3502449e519771d577f31`  
		Last Modified: Fri, 10 Feb 2023 02:18:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29150ca563004d89b203a1d45636f9664ff10c98390c8fc3755a45610971a1ea`  
		Last Modified: Fri, 10 Feb 2023 02:18:32 GMT  
		Size: 17.4 MB (17383752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore-1809`

```console
$ docker pull docker@sha256:242c2c7e2cc10720d8b7c21b3ffb73fae24e4b517723abb796d623343a318edd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `docker:23.0-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:ae74f76c3a2177ae1a1ff3ba98fa20d04bf94ad29fc92fb0523dd3efc9818469
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1725697339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5047252e3253ba4fb0d6024419bb9a071aa688f530872917de7e2c10822f8ef1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:16:40 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:16:41 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:17:27 GMT
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
	-	`sha256:16844f8b21e8556c61a8be9f8a035e77965fb2d1a9118446a04ab963453e2818`  
		Last Modified: Fri, 10 Feb 2023 02:18:29 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be212fb1d316bd604c933ad3541fbd93e77d53e596b3502449e519771d577f31`  
		Last Modified: Fri, 10 Feb 2023 02:18:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29150ca563004d89b203a1d45636f9664ff10c98390c8fc3755a45610971a1ea`  
		Last Modified: Fri, 10 Feb 2023 02:18:32 GMT  
		Size: 17.4 MB (17383752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:3fc74477620758a206afd0639937786867600a94cc05961e56377047c494a0a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `docker:23.0-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:32ebebed775320910f69ccfd06a3399051911bb12e2629321d15e2f92decf69f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1404240045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837fbe50c93ae962bd5d7df3d8d457cf279cf5c09ec1697153177fe9a3d9b4ba`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:15:53 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:15:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:16:32 GMT
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
	-	`sha256:ceb91a25fd6b227bd2ce1f4f3f0e001e0b4bda5a7f4c104a2f9030837a0217de`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb879bb8ff0dde7aead336ae453cdff5540f8c7f9747a306f758343afefad9f0`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9953dfbd0c49a493b80699b68fb1ba1355d08e2c63b827ef4725a88510898a`  
		Last Modified: Fri, 10 Feb 2023 02:18:16 GMT  
		Size: 17.6 MB (17594490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1`

```console
$ docker pull docker@sha256:82f534bca79c1b9222851511ed1e85e29d73185ecb820fc7fa24d6bc23f158de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.1` - linux; amd64

```console
$ docker pull docker@sha256:ac49b6d30def1445ef481ea0b40112d1ec81bacfb6ebf38678fbb1f485bd55cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111355086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b62af8d4fe6ad7923e26671b2f334fc0ab6b1f2f3f4ebaeef413969b8b76b2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.1` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f1b7854dd6e08e6399d76d6407c940ff5256e3d908b67b6a3f2bc67339f0446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102767745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8605baee59c3b6761d42902458231f8ff356810384858298e4cf9ac36475aa`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1-alpine3.17`

```console
$ docker pull docker@sha256:82f534bca79c1b9222851511ed1e85e29d73185ecb820fc7fa24d6bc23f158de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.1-alpine3.17` - linux; amd64

```console
$ docker pull docker@sha256:ac49b6d30def1445ef481ea0b40112d1ec81bacfb6ebf38678fbb1f485bd55cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111355086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b62af8d4fe6ad7923e26671b2f334fc0ab6b1f2f3f4ebaeef413969b8b76b2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.1-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f1b7854dd6e08e6399d76d6407c940ff5256e3d908b67b6a3f2bc67339f0446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102767745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8605baee59c3b6761d42902458231f8ff356810384858298e4cf9ac36475aa`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1-cli`

```console
$ docker pull docker@sha256:6ea6ac10351a3f4670424cff8f43272bbc7e221a5692fc6ff1c46b3b717a09eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.1-cli` - linux; amd64

```console
$ docker pull docker@sha256:c880a3345030d52528b9086f906e6afaf71d5a49be9be121c6213eec91ac3582
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52995991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edf3255c7bac424d71f8e03f71e1a483d3087253906fc07137df8a94bbfb7f35`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.1-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4512423530157859811ce109f20c1ee0ce566651bd42fc7c1a896112be6857da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48848520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f1cf9973f493622927611f9c0b59d1a3131b1076ec17ca4896396eeaa00ba`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1-cli-alpine3.17`

```console
$ docker pull docker@sha256:6ea6ac10351a3f4670424cff8f43272bbc7e221a5692fc6ff1c46b3b717a09eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.1-cli-alpine3.17` - linux; amd64

```console
$ docker pull docker@sha256:c880a3345030d52528b9086f906e6afaf71d5a49be9be121c6213eec91ac3582
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52995991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edf3255c7bac424d71f8e03f71e1a483d3087253906fc07137df8a94bbfb7f35`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.1-cli-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4512423530157859811ce109f20c1ee0ce566651bd42fc7c1a896112be6857da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48848520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f1cf9973f493622927611f9c0b59d1a3131b1076ec17ca4896396eeaa00ba`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1-dind`

```console
$ docker pull docker@sha256:82f534bca79c1b9222851511ed1e85e29d73185ecb820fc7fa24d6bc23f158de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.1-dind` - linux; amd64

```console
$ docker pull docker@sha256:ac49b6d30def1445ef481ea0b40112d1ec81bacfb6ebf38678fbb1f485bd55cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111355086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b62af8d4fe6ad7923e26671b2f334fc0ab6b1f2f3f4ebaeef413969b8b76b2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.1-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f1b7854dd6e08e6399d76d6407c940ff5256e3d908b67b6a3f2bc67339f0446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102767745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8605baee59c3b6761d42902458231f8ff356810384858298e4cf9ac36475aa`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1-dind-alpine3.17`

```console
$ docker pull docker@sha256:82f534bca79c1b9222851511ed1e85e29d73185ecb820fc7fa24d6bc23f158de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.1-dind-alpine3.17` - linux; amd64

```console
$ docker pull docker@sha256:ac49b6d30def1445ef481ea0b40112d1ec81bacfb6ebf38678fbb1f485bd55cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111355086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b62af8d4fe6ad7923e26671b2f334fc0ab6b1f2f3f4ebaeef413969b8b76b2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.1-dind-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f1b7854dd6e08e6399d76d6407c940ff5256e3d908b67b6a3f2bc67339f0446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102767745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8605baee59c3b6761d42902458231f8ff356810384858298e4cf9ac36475aa`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1-dind-rootless`

```console
$ docker pull docker@sha256:92cd2395cb20fec3682222f7af3ad69820c591f44a17e5e1e467fb7a547e060d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.1-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:956dcaef873746161a8b4df7ec7758692c81c3dbc44ac6b54283c33d0063d3a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133058390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19fd1ca0a7ee0431a44864140759e7f6b766f38d183dbda33c479b50199e25ea`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
CMD []
# Fri, 10 Feb 2023 18:22:20 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 18:22:20 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 18:22:21 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 18:22:23 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 18:22:24 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 18:22:24 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4a59800b3ff4ea8eef490aa8a8c857489cf86620c9e0520380d6d7f600165e`  
		Last Modified: Fri, 10 Feb 2023 18:24:22 GMT  
		Size: 1.4 MB (1375660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3913a018ce9ccaa6090f5fd22ae38ef94633a82270ed97d9262c4a5acb48ecf`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b668142e8f5abb9532cd382b84634282aed7b6d6c0dc03984c2321d0377d72f0`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea07488668e5eaa6cecf986076943932f4b838bdf7a81ee65bd868d8ef6ff05e`  
		Last Modified: Fri, 10 Feb 2023 18:24:25 GMT  
		Size: 20.3 MB (20325931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb0bb87ed7f9974ff16b062385127b1216f2dff67b20c3a831dcc047c04b5`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.1-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:681fd333bfe151c44afc36dadc90d6c7a57739eec704f067a9e31c9ac64b4b04
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126403269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154cee901c71bc181226a8859dfdd45c7a8c964fdb6aa244f8456ca91887575e`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
CMD []
# Fri, 10 Feb 2023 01:40:07 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 01:40:08 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 01:40:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 01:40:11 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 01:40:11 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 01:40:11 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3dc53d7d003c42e619e0f0d987282b443cbd3c27f2ea7adb66fdd00ce482dc`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 1.4 MB (1401559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6a946dbd7e8b65ea508bf6da9de31a6ba5685341a96fea0f596e526e561943`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae187c227f61f574c537060340536d98e81b5a2dbf3fe54dab0ac8958276afd`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781222ed4e59469046da1c4cce7fd70bb7547e5bf0039492c2f75eca75f0ed4c`  
		Last Modified: Fri, 10 Feb 2023 01:42:10 GMT  
		Size: 22.2 MB (22232243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810d859f0d275a30b178e088500caf03121e6d1cf6754976db572876133b124`  
		Last Modified: Fri, 10 Feb 2023 01:42:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1-git`

```console
$ docker pull docker@sha256:008585ccb370d47bea570dcd9ed670befbd150c4498cd732724394ccc8b8fa70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:23.0.1-git` - linux; amd64

```console
$ docker pull docker@sha256:41ed4d04a08469987631a4804370804913ac1c83e6d17a402490173f2f332074
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57139588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db43d1ae0dd659407f03338f3d49c72351f6a856fb5882346dd3bad5bd5041a2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:28 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3e04e933edd5be5e2423369fe61779b1ae2d7897d85031e72446095455f440`  
		Last Modified: Fri, 10 Feb 2023 18:24:41 GMT  
		Size: 4.1 MB (4143597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.1-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:85675576039d66bcc9c28de94404d7f3d7496cf13d4246a4c6acf622ed23ee9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53034428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e3e9fb67a75da1d4c083d1d1f74515e47143a9aa60eaa4fb9b238420b3d539`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:40:15 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c226941ea6751d6d947043e88e38ab6035098a001e27328b23d3c278f04c592`  
		Last Modified: Fri, 10 Feb 2023 01:42:25 GMT  
		Size: 4.2 MB (4185908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1-windowsservercore`

```console
$ docker pull docker@sha256:6e424a985f0ac4690156b9f335d6345ff6225d0e72d209e17393d4a3cc220c0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `docker:23.0.1-windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:32ebebed775320910f69ccfd06a3399051911bb12e2629321d15e2f92decf69f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1404240045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837fbe50c93ae962bd5d7df3d8d457cf279cf5c09ec1697153177fe9a3d9b4ba`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:15:53 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:15:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:16:32 GMT
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
	-	`sha256:ceb91a25fd6b227bd2ce1f4f3f0e001e0b4bda5a7f4c104a2f9030837a0217de`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb879bb8ff0dde7aead336ae453cdff5540f8c7f9747a306f758343afefad9f0`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9953dfbd0c49a493b80699b68fb1ba1355d08e2c63b827ef4725a88510898a`  
		Last Modified: Fri, 10 Feb 2023 02:18:16 GMT  
		Size: 17.6 MB (17594490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:23.0.1-windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:ae74f76c3a2177ae1a1ff3ba98fa20d04bf94ad29fc92fb0523dd3efc9818469
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1725697339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5047252e3253ba4fb0d6024419bb9a071aa688f530872917de7e2c10822f8ef1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:16:40 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:16:41 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:17:27 GMT
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
	-	`sha256:16844f8b21e8556c61a8be9f8a035e77965fb2d1a9118446a04ab963453e2818`  
		Last Modified: Fri, 10 Feb 2023 02:18:29 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be212fb1d316bd604c933ad3541fbd93e77d53e596b3502449e519771d577f31`  
		Last Modified: Fri, 10 Feb 2023 02:18:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29150ca563004d89b203a1d45636f9664ff10c98390c8fc3755a45610971a1ea`  
		Last Modified: Fri, 10 Feb 2023 02:18:32 GMT  
		Size: 17.4 MB (17383752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1-windowsservercore-1809`

```console
$ docker pull docker@sha256:242c2c7e2cc10720d8b7c21b3ffb73fae24e4b517723abb796d623343a318edd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `docker:23.0.1-windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:ae74f76c3a2177ae1a1ff3ba98fa20d04bf94ad29fc92fb0523dd3efc9818469
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1725697339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5047252e3253ba4fb0d6024419bb9a071aa688f530872917de7e2c10822f8ef1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:16:40 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:16:41 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:17:27 GMT
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
	-	`sha256:16844f8b21e8556c61a8be9f8a035e77965fb2d1a9118446a04ab963453e2818`  
		Last Modified: Fri, 10 Feb 2023 02:18:29 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be212fb1d316bd604c933ad3541fbd93e77d53e596b3502449e519771d577f31`  
		Last Modified: Fri, 10 Feb 2023 02:18:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29150ca563004d89b203a1d45636f9664ff10c98390c8fc3755a45610971a1ea`  
		Last Modified: Fri, 10 Feb 2023 02:18:32 GMT  
		Size: 17.4 MB (17383752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:23.0.1-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:3fc74477620758a206afd0639937786867600a94cc05961e56377047c494a0a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `docker:23.0.1-windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:32ebebed775320910f69ccfd06a3399051911bb12e2629321d15e2f92decf69f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1404240045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837fbe50c93ae962bd5d7df3d8d457cf279cf5c09ec1697153177fe9a3d9b4ba`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:15:53 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:15:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:16:32 GMT
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
	-	`sha256:ceb91a25fd6b227bd2ce1f4f3f0e001e0b4bda5a7f4c104a2f9030837a0217de`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb879bb8ff0dde7aead336ae453cdff5540f8c7f9747a306f758343afefad9f0`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9953dfbd0c49a493b80699b68fb1ba1355d08e2c63b827ef4725a88510898a`  
		Last Modified: Fri, 10 Feb 2023 02:18:16 GMT  
		Size: 17.6 MB (17594490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:cli`

```console
$ docker pull docker@sha256:6ea6ac10351a3f4670424cff8f43272bbc7e221a5692fc6ff1c46b3b717a09eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:cli` - linux; amd64

```console
$ docker pull docker@sha256:c880a3345030d52528b9086f906e6afaf71d5a49be9be121c6213eec91ac3582
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52995991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edf3255c7bac424d71f8e03f71e1a483d3087253906fc07137df8a94bbfb7f35`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4512423530157859811ce109f20c1ee0ce566651bd42fc7c1a896112be6857da
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48848520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9f1cf9973f493622927611f9c0b59d1a3131b1076ec17ca4896396eeaa00ba`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind`

```console
$ docker pull docker@sha256:82f534bca79c1b9222851511ed1e85e29d73185ecb820fc7fa24d6bc23f158de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:ac49b6d30def1445ef481ea0b40112d1ec81bacfb6ebf38678fbb1f485bd55cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111355086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b62af8d4fe6ad7923e26671b2f334fc0ab6b1f2f3f4ebaeef413969b8b76b2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f1b7854dd6e08e6399d76d6407c940ff5256e3d908b67b6a3f2bc67339f0446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102767745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8605baee59c3b6761d42902458231f8ff356810384858298e4cf9ac36475aa`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:dind-rootless`

```console
$ docker pull docker@sha256:92cd2395cb20fec3682222f7af3ad69820c591f44a17e5e1e467fb7a547e060d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:956dcaef873746161a8b4df7ec7758692c81c3dbc44ac6b54283c33d0063d3a7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133058390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19fd1ca0a7ee0431a44864140759e7f6b766f38d183dbda33c479b50199e25ea`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
CMD []
# Fri, 10 Feb 2023 18:22:20 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 18:22:20 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 18:22:21 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 18:22:23 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 18:22:24 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 18:22:24 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb4a59800b3ff4ea8eef490aa8a8c857489cf86620c9e0520380d6d7f600165e`  
		Last Modified: Fri, 10 Feb 2023 18:24:22 GMT  
		Size: 1.4 MB (1375660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3913a018ce9ccaa6090f5fd22ae38ef94633a82270ed97d9262c4a5acb48ecf`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b668142e8f5abb9532cd382b84634282aed7b6d6c0dc03984c2321d0377d72f0`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea07488668e5eaa6cecf986076943932f4b838bdf7a81ee65bd868d8ef6ff05e`  
		Last Modified: Fri, 10 Feb 2023 18:24:25 GMT  
		Size: 20.3 MB (20325931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb0bb87ed7f9974ff16b062385127b1216f2dff67b20c3a831dcc047c04b5`  
		Last Modified: Fri, 10 Feb 2023 18:24:21 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:681fd333bfe151c44afc36dadc90d6c7a57739eec704f067a9e31c9ac64b4b04
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126403269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154cee901c71bc181226a8859dfdd45c7a8c964fdb6aa244f8456ca91887575e`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
CMD []
# Fri, 10 Feb 2023 01:40:07 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 10 Feb 2023 01:40:08 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 10 Feb 2023 01:40:08 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:10 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 10 Feb 2023 01:40:11 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 10 Feb 2023 01:40:11 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 10 Feb 2023 01:40:11 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3dc53d7d003c42e619e0f0d987282b443cbd3c27f2ea7adb66fdd00ce482dc`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 1.4 MB (1401559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6a946dbd7e8b65ea508bf6da9de31a6ba5685341a96fea0f596e526e561943`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae187c227f61f574c537060340536d98e81b5a2dbf3fe54dab0ac8958276afd`  
		Last Modified: Fri, 10 Feb 2023 01:42:07 GMT  
		Size: 1.4 KB (1351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781222ed4e59469046da1c4cce7fd70bb7547e5bf0039492c2f75eca75f0ed4c`  
		Last Modified: Fri, 10 Feb 2023 01:42:10 GMT  
		Size: 22.2 MB (22232243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810d859f0d275a30b178e088500caf03121e6d1cf6754976db572876133b124`  
		Last Modified: Fri, 10 Feb 2023 01:42:06 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:git`

```console
$ docker pull docker@sha256:008585ccb370d47bea570dcd9ed670befbd150c4498cd732724394ccc8b8fa70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:git` - linux; amd64

```console
$ docker pull docker@sha256:41ed4d04a08469987631a4804370804913ac1c83e6d17a402490173f2f332074
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57139588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db43d1ae0dd659407f03338f3d49c72351f6a856fb5882346dd3bad5bd5041a2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:28 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3e04e933edd5be5e2423369fe61779b1ae2d7897d85031e72446095455f440`  
		Last Modified: Fri, 10 Feb 2023 18:24:41 GMT  
		Size: 4.1 MB (4143597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:85675576039d66bcc9c28de94404d7f3d7496cf13d4246a4c6acf622ed23ee9a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53034428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e3e9fb67a75da1d4c083d1d1f74515e47143a9aa60eaa4fb9b238420b3d539`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:40:15 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c226941ea6751d6d947043e88e38ab6035098a001e27328b23d3c278f04c592`  
		Last Modified: Fri, 10 Feb 2023 01:42:25 GMT  
		Size: 4.2 MB (4185908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:latest`

```console
$ docker pull docker@sha256:82f534bca79c1b9222851511ed1e85e29d73185ecb820fc7fa24d6bc23f158de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:latest` - linux; amd64

```console
$ docker pull docker@sha256:ac49b6d30def1445ef481ea0b40112d1ec81bacfb6ebf38678fbb1f485bd55cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111355086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05b62af8d4fe6ad7923e26671b2f334fc0ab6b1f2f3f4ebaeef413969b8b76b2`
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
# Fri, 10 Feb 2023 18:21:55 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 18:21:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 18:21:59 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 18:22:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 18:22:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 18:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 18:22:03 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 18:22:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 18:22:04 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 18:22:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:04 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 18:22:09 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 18:22:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 18:22:14 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 18:22:15 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 18:22:15 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 18:22:15 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 18:22:15 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 18:22:15 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 18:22:15 GMT
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
	-	`sha256:48995ffb01582225606132fc91ceee1ff26e13be903122771dcdf91e4742bd36`  
		Last Modified: Fri, 10 Feb 2023 18:23:27 GMT  
		Size: 16.2 MB (16220358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d42eb817ad7198dcfcf13f1c85422866041788c1e4c318c0d72fef9c26bc5fd`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 16.0 MB (15995568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd610afdf8cc6a92d5c232d31d2a02a5df1f6baecc857f89523de0d53c3ddf`  
		Last Modified: Fri, 10 Feb 2023 18:23:26 GMT  
		Size: 15.3 MB (15343454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de137ab3bd8985a82eef1e368f94b9a99acdec1319d3b9263762986d20cba10`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b052fd3a6a7a1bd05d9f2a24178b34dd726b62ba34217df92ba2130371ee8ae`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf0639b0a2f8ef651b84d667edf0c86dbf2912a559915d09f1899dcea6d9e61`  
		Last Modified: Fri, 10 Feb 2023 18:23:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6e8ad4c5d8f2c4939c74e70a0915bd498b6c698a3c0b134236e6eadba650cb`  
		Last Modified: Fri, 10 Feb 2023 18:23:44 GMT  
		Size: 6.8 MB (6837930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d8cda089bb000a2ace87012e7c03b9245e7a18b39863fef97c9e0bb5ef4f82`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e376f981b567b77b771d185294e807d3d5e35e55a0d32023411cfbc1f1a9c7`  
		Last Modified: Fri, 10 Feb 2023 18:23:51 GMT  
		Size: 51.5 MB (51515981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895584c72f30eaeb02cda956f3db2f4b635db9cdd3dedc9c639c4b171d27c362`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538e470b25e69cec162ddb35d3fbf435d64e7009e0882daec0e821b3a4189bc`  
		Last Modified: Fri, 10 Feb 2023 18:23:43 GMT  
		Size: 2.8 KB (2820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:latest` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:4f1b7854dd6e08e6399d76d6407c940ff5256e3d908b67b6a3f2bc67339f0446
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.8 MB (102767745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a8605baee59c3b6761d42902458231f8ff356810384858298e4cf9ac36475aa`
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
# Fri, 10 Feb 2023 01:39:35 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 01:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 10 Feb 2023 01:39:38 GMT
ENV DOCKER_BUILDX_VERSION=0.10.2
# Fri, 10 Feb 2023 01:39:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-amd64'; 			sha256='ee5a5e3ebf5e5c73ac840993720bd1e72c4beb3b4ee9e85e2d6b4364cac87d89'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v6'; 			sha256='4d7c2e9eaed303306b40e0505577f4c7088c99f048a5870dd133cb7ad2336bd6'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm-v7'; 			sha256='d74936a4e4e9266aeca66e6a545ed99d83753b4901e0f5210e7646c987591974'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-arm64'; 			sha256='5f6c706833221cd2cae267ac8612c1809f9d7e8f3fe87707ae86cb695c560cd9'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-ppc64le'; 			sha256='fe55ae43e009b4523523575f500257d7dafeb0aa637392b1853676b8a7a55b7b'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-riscv64'; 			sha256='b57cd352329baebca4cc8102806927de3f5402fff16f6f6e4a2e48080434472b'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.2/buildx-v0.10.2.linux-s390x'; 			sha256='9a3be43a3a6902617a8224b41177a840e1a638597a27d7b7c2d558adb8be3a24'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 10 Feb 2023 01:39:43 GMT
ENV DOCKER_COMPOSE_VERSION=2.16.0
# Fri, 10 Feb 2023 01:39:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-x86_64'; 			sha256='54ab01967b05e392e6bf13afbc654146890b9fa40501b40aca83a2db18f10427'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv6'; 			sha256='59caa4c31a6515a81b44446d978891c5e1d0f460b9b11e38dea27e1bffdb4cd6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-armv7'; 			sha256='558a083683bd597f5e167178dbdbe57824eecf2132bfb497a58f5d39c5e49e8a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-aarch64'; 			sha256='edaf196a0b9ebe749aa1a42a6ce4550d2c6c2620762aa98c36088a9b96fd22ef'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-ppc64le'; 			sha256='aac719dc81ef117bdcca96d7e43ecd605ebcdc1df77c0b09b9d5faf15ccf952e'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-riscv64'; 			sha256='8c485ee45cf6be4d483179e925ffeb3b046280d1be045cdfc999c0a011ddfcd1'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.16.0/docker-compose-linux-s390x'; 			sha256='fbaff480bd7901c31ead046652c3f5a3c1236766ce9f52fadfa935a18dd463b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 10 Feb 2023 01:39:49 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:39:49 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 10 Feb 2023 01:39:50 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 10 Feb 2023 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 01:39:50 GMT
CMD ["sh"]
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 10 Feb 2023 01:39:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 10 Feb 2023 01:40:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 10 Feb 2023 01:40:01 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 10 Feb 2023 01:40:02 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 10 Feb 2023 01:40:02 GMT
COPY file:adb1d28efd9d119c42d2a02a001281e9671f528b2fae1d982de1c5d1af55b3f9 in /usr/local/bin/ 
# Fri, 10 Feb 2023 01:40:02 GMT
VOLUME [/var/lib/docker]
# Fri, 10 Feb 2023 01:40:02 GMT
EXPOSE 2375 2376
# Fri, 10 Feb 2023 01:40:02 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 10 Feb 2023 01:40:02 GMT
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
	-	`sha256:31e20f77607956971fdf7ef1ded793b84f8351ca45a7a287c4b9192c25fa1e38`  
		Last Modified: Fri, 10 Feb 2023 01:41:15 GMT  
		Size: 15.3 MB (15294696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2738270eae3d3d093948b4e1a3e7031c0ae667b0f84a7146071c04310d88869`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 14.4 MB (14436885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee74c4162f548e616505a66f20473b1f5f4ab3211f31148bfe1a695bd19a7fe`  
		Last Modified: Fri, 10 Feb 2023 01:41:14 GMT  
		Size: 13.8 MB (13819070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcb4de8c76d91633c08bc1a8f36eb54ee85bac6ab5bcf96f651d474e66d6f31`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59318d785d25f608efe457813c31cadc504478aab73c610c40cf183746942d28`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a948a67cc80192bb185648a1e7e22c9b720cb853dbab2445e24ce2c20f7c5f8`  
		Last Modified: Fri, 10 Feb 2023 01:41:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310764d07b78d041ab166ff9e103139ddf4fd19919ebc962461a508660189ab8`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 7.0 MB (6991147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff0d50921fb68732ec9e9233df2b526eea85848ad4167975d3e98be531b8486`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f73f8ede4ec7a2ada324753196f2b2cf591d736bec72b0d20733f2f77a17bd`  
		Last Modified: Fri, 10 Feb 2023 01:41:36 GMT  
		Size: 46.9 MB (46922896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07a2595dfd138a24e75d3d42e922166f1627f0691d50e6edc46ad3e38da0205`  
		Last Modified: Fri, 10 Feb 2023 01:41:31 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84de123a5489f602aa48c8eef3d1219355de45c8ee535c7644e1fec0c2168bb`  
		Last Modified: Fri, 10 Feb 2023 01:41:30 GMT  
		Size: 2.8 KB (2819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore`

```console
$ docker pull docker@sha256:6e424a985f0ac4690156b9f335d6345ff6225d0e72d209e17393d4a3cc220c0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `docker:windowsservercore` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:32ebebed775320910f69ccfd06a3399051911bb12e2629321d15e2f92decf69f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1404240045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837fbe50c93ae962bd5d7df3d8d457cf279cf5c09ec1697153177fe9a3d9b4ba`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:15:53 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:15:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:16:32 GMT
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
	-	`sha256:ceb91a25fd6b227bd2ce1f4f3f0e001e0b4bda5a7f4c104a2f9030837a0217de`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb879bb8ff0dde7aead336ae453cdff5540f8c7f9747a306f758343afefad9f0`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9953dfbd0c49a493b80699b68fb1ba1355d08e2c63b827ef4725a88510898a`  
		Last Modified: Fri, 10 Feb 2023 02:18:16 GMT  
		Size: 17.6 MB (17594490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:windowsservercore` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:ae74f76c3a2177ae1a1ff3ba98fa20d04bf94ad29fc92fb0523dd3efc9818469
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1725697339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5047252e3253ba4fb0d6024419bb9a071aa688f530872917de7e2c10822f8ef1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:16:40 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:16:41 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:17:27 GMT
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
	-	`sha256:16844f8b21e8556c61a8be9f8a035e77965fb2d1a9118446a04ab963453e2818`  
		Last Modified: Fri, 10 Feb 2023 02:18:29 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be212fb1d316bd604c933ad3541fbd93e77d53e596b3502449e519771d577f31`  
		Last Modified: Fri, 10 Feb 2023 02:18:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29150ca563004d89b203a1d45636f9664ff10c98390c8fc3755a45610971a1ea`  
		Last Modified: Fri, 10 Feb 2023 02:18:32 GMT  
		Size: 17.4 MB (17383752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:242c2c7e2cc10720d8b7c21b3ffb73fae24e4b517723abb796d623343a318edd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3887; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.3887; amd64

```console
$ docker pull docker@sha256:ae74f76c3a2177ae1a1ff3ba98fa20d04bf94ad29fc92fb0523dd3efc9818469
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1725697339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5047252e3253ba4fb0d6024419bb9a071aa688f530872917de7e2c10822f8ef1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 01:43:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:39:36 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:16:40 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:16:41 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:17:27 GMT
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
	-	`sha256:16844f8b21e8556c61a8be9f8a035e77965fb2d1a9118446a04ab963453e2818`  
		Last Modified: Fri, 10 Feb 2023 02:18:29 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be212fb1d316bd604c933ad3541fbd93e77d53e596b3502449e519771d577f31`  
		Last Modified: Fri, 10 Feb 2023 02:18:30 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29150ca563004d89b203a1d45636f9664ff10c98390c8fc3755a45610971a1ea`  
		Last Modified: Fri, 10 Feb 2023 02:18:32 GMT  
		Size: 17.4 MB (17383752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:3fc74477620758a206afd0639937786867600a94cc05961e56377047c494a0a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1487; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.1487; amd64

```console
$ docker pull docker@sha256:32ebebed775320910f69ccfd06a3399051911bb12e2629321d15e2f92decf69f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1404240045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:837fbe50c93ae962bd5d7df3d8d457cf279cf5c09ec1697153177fe9a3d9b4ba`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 01:40:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 12 Jan 2023 05:38:30 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Fri, 10 Feb 2023 02:15:53 GMT
ENV DOCKER_VERSION=23.0.1
# Fri, 10 Feb 2023 02:15:54 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-23.0.1.zip
# Fri, 10 Feb 2023 02:16:32 GMT
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
	-	`sha256:ceb91a25fd6b227bd2ce1f4f3f0e001e0b4bda5a7f4c104a2f9030837a0217de`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb879bb8ff0dde7aead336ae453cdff5540f8c7f9747a306f758343afefad9f0`  
		Last Modified: Fri, 10 Feb 2023 02:18:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9953dfbd0c49a493b80699b68fb1ba1355d08e2c63b827ef4725a88510898a`  
		Last Modified: Fri, 10 Feb 2023 02:18:16 GMT  
		Size: 17.6 MB (17594490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
