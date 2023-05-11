## `docker:rc`

```console
$ docker pull docker@sha256:77dcdadf84be5dc26c142ae16c73e66ad3c3d6357fe0be62ba70d2d79ecc32d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc` - linux; amd64

```console
$ docker pull docker@sha256:c09bc1b4d6881dc35cce5458c212e7f030d380777d15e74d726269d19a86e57a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.2 MB (115228645 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05731c3e085b465917f34745bf7960c503c2dd0fdd9d0cb724e8e55269974bb3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Thu, 11 May 2023 21:35:47 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 11 May 2023 21:35:47 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 11 May 2023 21:35:47 GMT
ENV DOCKER_VERSION=24.0.0-rc.3
# Thu, 11 May 2023 21:35:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-24.0.0-rc.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-24.0.0-rc.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-24.0.0-rc.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-24.0.0-rc.3.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 11 May 2023 21:35:47 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Thu, 11 May 2023 21:35:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-amd64'; 			sha256='dbe68cdc537d0150fc83e3f30974cd0ca11c179dafbf27f32d6f063be26e869b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm-v6'; 			sha256='d50aa01a22a53e5a0eae9918274c9931b813b5336c0e30061a6b1904efb0c5eb'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm-v7'; 			sha256='aabc8cef5b9221ecbcb0af9846004a30591540be8668504d70814efe870448c8'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm64'; 			sha256='e8f666134cf4aa83ec2b1b6afef0c83b1ea1387984d7a40ae6657b7da4d82d91'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-ppc64le'; 			sha256='d107178f36e6c83286f3f9316e2f66b18f08306570cef209cb5840c880bd91ae'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-riscv64'; 			sha256='393db8518aeb442d0ca5f3ccf4800622dfc5eb8993c29bbfccb023cbfde6cdbc'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-s390x'; 			sha256='16ce9071c14293640e9bcd547ff01578c65cfc68fc6c154091abd81daaf10929'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 11 May 2023 21:35:47 GMT
ENV DOCKER_COMPOSE_VERSION=2.17.3
# Thu, 11 May 2023 21:35:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-x86_64'; 			sha256='6abb771a438b8ef82b0ff0ef0e2e404032699104c3c40c59cd174b56214876c3'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-armv6'; 			sha256='e8c20e7e02faa623839ccb2af725ae0b343eafaf836b2386579e35c598d7468a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-armv7'; 			sha256='72c26a8ab6a519bd9c645a314d6ed33ed694efeda3f787123806990124446fe8'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-aarch64'; 			sha256='07bdced6f502ab24b481f46aa6b205f97e2256e5cb11279648ac9c088220a38d'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-ppc64le'; 			sha256='06075ea6594e42fd62360c029ed2b7cf294e8a50428cc3c8f0e022a68f672660'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-riscv64'; 			sha256='51c3e1b631be5845aecc9a66d4d0525c94dfec4d20a4ccf535a7f960f780e9f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-s390x'; 			sha256='666a07a5605e985ac96608a315cdae8151e72196733147dd81b61dd42c0777fe'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 11 May 2023 21:35:47 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 11 May 2023 21:35:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 11 May 2023 21:35:47 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 11 May 2023 21:35:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 11 May 2023 21:35:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 May 2023 21:35:47 GMT
CMD ["sh"]
# Thu, 11 May 2023 21:35:47 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Thu, 11 May 2023 21:35:47 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Thu, 11 May 2023 21:35:47 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-24.0.0-rc.3.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-24.0.0-rc.3.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-24.0.0-rc.3.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-24.0.0-rc.3.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Thu, 11 May 2023 21:35:47 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Thu, 11 May 2023 21:35:47 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Thu, 11 May 2023 21:35:47 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 11 May 2023 21:35:47 GMT
VOLUME [/var/lib/docker]
# Thu, 11 May 2023 21:35:47 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Thu, 11 May 2023 21:35:47 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 11 May 2023 21:35:47 GMT
CMD []
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb60e7f5d22cf3e06856538fbb2c518c629c1bbe07d62a60d16e3c7fefa06f4`  
		Last Modified: Thu, 11 May 2023 19:23:43 GMT  
		Size: 2.0 MB (2014357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74671f55a8da50720028684fd32ee90f4fdeb79ffcadf0e7213a90cd50ef5c3`  
		Last Modified: Thu, 11 May 2023 19:23:42 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65af7e03560184764a57e59e0c0c5ea9a03686fbdb5586344c639072b053b5fd`  
		Last Modified: Thu, 11 May 2023 22:52:08 GMT  
		Size: 16.4 MB (16375807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3bba302375616e402dc9800f2eaa3c7d76ab0d78cba1513b0ecf3d20da1f91`  
		Last Modified: Thu, 11 May 2023 22:52:07 GMT  
		Size: 16.0 MB (16001757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4c67bb9d6ac071c06712ad2509b1527e53f7b9e55068d81fcf2b7c6ebcb5dd`  
		Last Modified: Thu, 11 May 2023 22:52:07 GMT  
		Size: 16.4 MB (16384819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c36aa896517c53efac586e77366bbf7d97c9088297b44307b76c7c216b6ad2c`  
		Last Modified: Thu, 11 May 2023 22:52:05 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b2bf4c064336eeb94d04bb932144c5e3962a605141f2314bd94fa5812efc77`  
		Last Modified: Thu, 11 May 2023 22:52:05 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6355be813038e6066569c526b88f435c4aff4a906fd35d083ddc6ff89fc65c`  
		Last Modified: Thu, 11 May 2023 22:52:05 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adc62c23e75a2f326a5d653c96abf39fefc9337abca021d5c4c4c2938e03f0f`  
		Last Modified: Thu, 11 May 2023 22:52:22 GMT  
		Size: 7.0 MB (7025255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fb9c3716d4b94bed4bc5d439ef574e9b3d00ff976a689ed156a7c91374b12e`  
		Last Modified: Thu, 11 May 2023 22:52:21 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff2dfdf91d420286c73dadfa6b0173af37367a9e94432da3ab2b87194b45cb4`  
		Last Modified: Thu, 11 May 2023 22:52:29 GMT  
		Size: 54.0 MB (54022156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6b14bc3bad8c55212942c45d61a97196a376d30c32e4a6efa59a5b2b05f9d9`  
		Last Modified: Thu, 11 May 2023 22:52:21 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c87a0fe84391fde7c65384c10c73de0c980f266c1ab40c3b77829aef258664c`  
		Last Modified: Thu, 11 May 2023 22:52:21 GMT  
		Size: 2.8 KB (2813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b926df4fa3e66c2857005454b6bb15019f0235464e3727b354656eb0c67b74ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106636700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26b6959450cbf67180f0b5524ff8d934c5a53c091af56dca90354a078e4dfe6`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 10:04:23 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 10 May 2023 10:04:23 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 10 May 2023 10:04:23 GMT
ENV DOCKER_VERSION=24.0.0-rc.2
# Wed, 10 May 2023 10:04:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-24.0.0-rc.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-24.0.0-rc.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-24.0.0-rc.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-24.0.0-rc.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 10 May 2023 10:04:23 GMT
ENV DOCKER_BUILDX_VERSION=0.10.4
# Wed, 10 May 2023 10:04:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-amd64'; 			sha256='dbe68cdc537d0150fc83e3f30974cd0ca11c179dafbf27f32d6f063be26e869b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm-v6'; 			sha256='d50aa01a22a53e5a0eae9918274c9931b813b5336c0e30061a6b1904efb0c5eb'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm-v7'; 			sha256='aabc8cef5b9221ecbcb0af9846004a30591540be8668504d70814efe870448c8'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-arm64'; 			sha256='e8f666134cf4aa83ec2b1b6afef0c83b1ea1387984d7a40ae6657b7da4d82d91'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-ppc64le'; 			sha256='d107178f36e6c83286f3f9316e2f66b18f08306570cef209cb5840c880bd91ae'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-riscv64'; 			sha256='393db8518aeb442d0ca5f3ccf4800622dfc5eb8993c29bbfccb023cbfde6cdbc'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.4/buildx-v0.10.4.linux-s390x'; 			sha256='16ce9071c14293640e9bcd547ff01578c65cfc68fc6c154091abd81daaf10929'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 10 May 2023 10:04:23 GMT
ENV DOCKER_COMPOSE_VERSION=2.17.3
# Wed, 10 May 2023 10:04:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-x86_64'; 			sha256='6abb771a438b8ef82b0ff0ef0e2e404032699104c3c40c59cd174b56214876c3'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-armv6'; 			sha256='e8c20e7e02faa623839ccb2af725ae0b343eafaf836b2386579e35c598d7468a'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-armv7'; 			sha256='72c26a8ab6a519bd9c645a314d6ed33ed694efeda3f787123806990124446fe8'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-aarch64'; 			sha256='07bdced6f502ab24b481f46aa6b205f97e2256e5cb11279648ac9c088220a38d'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-ppc64le'; 			sha256='06075ea6594e42fd62360c029ed2b7cf294e8a50428cc3c8f0e022a68f672660'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-riscv64'; 			sha256='51c3e1b631be5845aecc9a66d4d0525c94dfec4d20a4ccf535a7f960f780e9f2'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.17.3/docker-compose-linux-s390x'; 			sha256='666a07a5605e985ac96608a315cdae8151e72196733147dd81b61dd42c0777fe'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 10 May 2023 10:04:23 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 10 May 2023 10:04:23 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 10 May 2023 10:04:23 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 10 May 2023 10:04:23 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 10 May 2023 10:04:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 May 2023 10:04:23 GMT
CMD ["sh"]
# Wed, 10 May 2023 10:04:23 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Wed, 10 May 2023 10:04:23 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Wed, 10 May 2023 10:04:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-24.0.0-rc.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-24.0.0-rc.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-24.0.0-rc.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-24.0.0-rc.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Wed, 10 May 2023 10:04:23 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Wed, 10 May 2023 10:04:23 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Wed, 10 May 2023 10:04:23 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 10 May 2023 10:04:23 GMT
VOLUME [/var/lib/docker]
# Wed, 10 May 2023 10:04:23 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Wed, 10 May 2023 10:04:23 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 10 May 2023 10:04:23 GMT
CMD []
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf127bdc9f4f627525a187a7bf41c41f4706220fb1fe5b5c7d6cbc52114a9224`  
		Last Modified: Thu, 11 May 2023 19:42:22 GMT  
		Size: 2.0 MB (2024535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b4810136f4ceecd47a02cbf6a0c55b8d9de3b014cf917ac2bf8ee632787ba0`  
		Last Modified: Thu, 11 May 2023 19:42:22 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9cdbf6cf96d2756d10df0899b75ea6b148021551a074cd6138027ce349a5139`  
		Last Modified: Thu, 11 May 2023 19:42:23 GMT  
		Size: 15.4 MB (15422879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e29323b159a006ed99648e56e398c3321c2a83c1a8a46cc2bc927c8fe02d07`  
		Last Modified: Thu, 11 May 2023 19:42:22 GMT  
		Size: 14.4 MB (14441505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6242cd869bed05c8ede6acec5c525d1a9e816d8e5e4c752ae15560e663c1f8d4`  
		Last Modified: Thu, 11 May 2023 19:42:22 GMT  
		Size: 14.8 MB (14835065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b497d2057847cec6353a82bffcca690e14e6ec77b42e185d2ea9d4b896de8dc6`  
		Last Modified: Thu, 11 May 2023 19:42:20 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49abd705ac1906348247d33e88a6be7df25eb8c1445e238131a18f1846adfdf0`  
		Last Modified: Thu, 11 May 2023 19:42:20 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ee4fc48068e89a4049e7fb0ca131c3a7687228b5acb2a3543e61e6270ef908`  
		Last Modified: Thu, 11 May 2023 19:42:20 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b52b8cb964b1d1f9be3e2e5eaee8b338043ec0550f05e25a2cdaa5bb4866de`  
		Last Modified: Thu, 11 May 2023 19:42:36 GMT  
		Size: 7.2 MB (7245063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed405abfb4f90c841d8d67a68996ec7593d7131c02e542c91ce6250dd3395b6b`  
		Last Modified: Thu, 11 May 2023 19:42:35 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2bae630a24dd5254abdd272679bf99eea40e293dd8cd84d5caf21f6276062e`  
		Last Modified: Thu, 11 May 2023 19:42:40 GMT  
		Size: 49.3 MB (49317795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668f70e8314bc17b4d5532f06d5f9a4bfaa61a919683572ba4620dfd39224ac0`  
		Last Modified: Thu, 11 May 2023 19:42:35 GMT  
		Size: 1.1 KB (1051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25a0e6b7c31228c3411ddec1986b580d081f0ef168ba518f2a5295d90783988`  
		Last Modified: Thu, 11 May 2023 19:42:35 GMT  
		Size: 2.8 KB (2815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
