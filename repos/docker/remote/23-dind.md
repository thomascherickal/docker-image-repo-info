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
