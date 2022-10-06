## `docker:rc-dind`

```console
$ docker pull docker@sha256:aaafd957a5220aaba7d083e2518c24f7226677f7f64300c8f40b89efe91a60d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-dind` - linux; amd64

```console
$ docker pull docker@sha256:396634ae2e7d699cf59dc3622fc6d2fc7e87e1a36e9a5b6ac8021e18c30ef71a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.3 MB (103289631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d37d3c3cc1bcaa8f1bc28271b3433daf95c6140ac5e01a2b2d99aaf91e167177`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:48 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 09 Aug 2022 18:20:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:20:49 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Tue, 09 Aug 2022 18:20:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 19 Aug 2022 00:19:27 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Fri, 19 Aug 2022 00:19:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 28 Sep 2022 01:52:10 GMT
ENV DOCKER_COMPOSE_VERSION=2.11.2
# Wed, 28 Sep 2022 01:52:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-x86_64'; 			sha256='1178848502b0771b96895febeb4b1736acd5019c4ed71a8efbabf6915185fe8a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-armv6'; 			sha256='3e863e83a2701b26e168118f30456c3bd2ec37886182fc3373a8fe460e714761'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-armv7'; 			sha256='c133c194f36b3a6dcd552c4e32652f6ef7c22af258a6f14b414bf751aad3d2fd'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-aarch64'; 			sha256='eb65ae4a4dd4de7dc767935c2bc49e3641d265df1273ea8f577cadb6bd9b4ebf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-ppc64le'; 			sha256='24f65d215a198e33f3f1646ebabd6cae00eb6d2d3442b86c97d8198331350785'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-riscv64'; 			sha256='14a3de648bfa75a33ee8ded1cc8d501cff10c9d1565aab3dd641cf7283e9b51a'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-s390x'; 			sha256='08e8612dc7aa2d983c6c07c54e483cbc1ec089cfe9d7f790643dd8dbd30ee4f5'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 28 Sep 2022 01:52:12 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 28 Sep 2022 01:52:12 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 28 Sep 2022 01:52:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 28 Sep 2022 01:52:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 28 Sep 2022 01:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 28 Sep 2022 01:52:13 GMT
CMD ["sh"]
# Wed, 28 Sep 2022 01:52:18 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 28 Sep 2022 01:52:19 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 28 Sep 2022 01:52:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 28 Sep 2022 01:52:23 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 28 Sep 2022 01:52:24 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 28 Sep 2022 01:52:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 28 Sep 2022 01:52:24 GMT
VOLUME [/var/lib/docker]
# Wed, 28 Sep 2022 01:52:25 GMT
EXPOSE 2375 2376
# Wed, 28 Sep 2022 01:52:25 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 28 Sep 2022 01:52:25 GMT
CMD []
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb510456a427665c9755e7417ad432e68b6e95a1a9a6665f72f0adc6f9ec59d`  
		Last Modified: Tue, 09 Aug 2022 18:22:44 GMT  
		Size: 2.0 MB (2036045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4627ba0696d0614a94c97a4b5c212e055112e2a8f0831f342f3b138955035153`  
		Last Modified: Tue, 09 Aug 2022 18:22:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d957832b8a49136f6d95f00340a0c764c8cd051be7514885f8fca6a80053215`  
		Last Modified: Tue, 09 Aug 2022 18:22:45 GMT  
		Size: 8.7 MB (8706435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd48969715b862016850752e05193de3fe3dbc355a5f277cece7c52d69f4793`  
		Last Modified: Fri, 19 Aug 2022 00:21:18 GMT  
		Size: 15.2 MB (15204103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3e5154383742170e19c0b58c4b6d9bb22313cd9c8174090f80b1f8968c5637`  
		Last Modified: Wed, 28 Sep 2022 01:53:52 GMT  
		Size: 14.3 MB (14327697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ca82975f27cee51d1a45cfdd80db796d3b8c20c4cb4c91fd85b1218693b329`  
		Last Modified: Wed, 28 Sep 2022 01:53:49 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ff3965bebb5701dc62cb21abfa147948499e8fca849dca67a40dacbeb24ea7`  
		Last Modified: Wed, 28 Sep 2022 01:53:49 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c1826808d6140b93dc8fa61a51957b153bd065c1e097212118e6a3d6231a91`  
		Last Modified: Wed, 28 Sep 2022 01:53:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109b8897c7d9b8166694a8cdfc4902fedbc4fde25badab92e8ed624ace6dbb60`  
		Last Modified: Wed, 28 Sep 2022 01:54:07 GMT  
		Size: 6.9 MB (6863660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b852a3e4d7eeda94204803b326d9ca6618116ced5a92cc0c7c41ecb9759de3ce`  
		Last Modified: Wed, 28 Sep 2022 01:54:06 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3731a6d302a955fab973de7e713da19b29632702e4dfeb6a2885980bc9379b`  
		Last Modified: Wed, 28 Sep 2022 01:54:14 GMT  
		Size: 53.3 MB (53338719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93409b40b65e2b738927377ede6adedb8f2a3f68674293ac032f1416504ad9`  
		Last Modified: Wed, 28 Sep 2022 01:54:06 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0a4ae4975f7d0f4b17eca03da4b0e472a25dade7f8246d7959cecde2b13e2d`  
		Last Modified: Wed, 28 Sep 2022 01:54:06 GMT  
		Size: 2.8 KB (2754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:eee4e411634afb6ac861f9a3fff00d11f4e445be701e3a6c9208f8f0249d13de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.2 MB (95174363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58da6416bdef075107a1d833371340e3c456938ad0b9e9770086f02b5defce08`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:57:19 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 06 Oct 2022 19:57:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:57:21 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Thu, 06 Oct 2022 19:57:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Thu, 06 Oct 2022 19:57:27 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Thu, 06 Oct 2022 19:57:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Thu, 06 Oct 2022 19:57:31 GMT
ENV DOCKER_COMPOSE_VERSION=2.11.2
# Thu, 06 Oct 2022 19:57:35 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-x86_64'; 			sha256='1178848502b0771b96895febeb4b1736acd5019c4ed71a8efbabf6915185fe8a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-armv6'; 			sha256='3e863e83a2701b26e168118f30456c3bd2ec37886182fc3373a8fe460e714761'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-armv7'; 			sha256='c133c194f36b3a6dcd552c4e32652f6ef7c22af258a6f14b414bf751aad3d2fd'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-aarch64'; 			sha256='eb65ae4a4dd4de7dc767935c2bc49e3641d265df1273ea8f577cadb6bd9b4ebf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-ppc64le'; 			sha256='24f65d215a198e33f3f1646ebabd6cae00eb6d2d3442b86c97d8198331350785'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-riscv64'; 			sha256='14a3de648bfa75a33ee8ded1cc8d501cff10c9d1565aab3dd641cf7283e9b51a'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-s390x'; 			sha256='08e8612dc7aa2d983c6c07c54e483cbc1ec089cfe9d7f790643dd8dbd30ee4f5'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Thu, 06 Oct 2022 19:57:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 06 Oct 2022 19:57:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 06 Oct 2022 19:57:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 06 Oct 2022 19:57:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 06 Oct 2022 19:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:57:40 GMT
CMD ["sh"]
# Thu, 06 Oct 2022 19:57:49 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 06 Oct 2022 19:57:49 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 06 Oct 2022 19:57:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Thu, 06 Oct 2022 19:57:54 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 06 Oct 2022 19:57:55 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 06 Oct 2022 19:57:57 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 06 Oct 2022 19:57:57 GMT
VOLUME [/var/lib/docker]
# Thu, 06 Oct 2022 19:57:58 GMT
EXPOSE 2375 2376
# Thu, 06 Oct 2022 19:57:59 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 06 Oct 2022 19:58:00 GMT
CMD []
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21cba7d4ed21dc7eb0647c8bf12c0d6eac2550dc72a53a6c2b5137b34244372`  
		Last Modified: Thu, 06 Oct 2022 20:00:58 GMT  
		Size: 2.0 MB (2010535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dea5e927109f9fe9d7738e508aabd501392a9436d4abab847d6d2954293055`  
		Last Modified: Thu, 06 Oct 2022 20:00:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2839662109c3662f36d20d4f9e06dda4da895298bd450b424415319f4261f84b`  
		Last Modified: Thu, 06 Oct 2022 20:00:59 GMT  
		Size: 8.0 MB (8048674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9684c7523557099cadb09af30feb21c5970402c4ca96feae5c8f72f46bd3760`  
		Last Modified: Thu, 06 Oct 2022 20:00:57 GMT  
		Size: 13.8 MB (13764592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d20c4ade12ffae7ed6630a09f7f4c94dbc100f1dcf791b5f907f55b17cf7b18`  
		Last Modified: Thu, 06 Oct 2022 20:00:57 GMT  
		Size: 12.9 MB (12922235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6b727d69e856e487fb3e51787c22e3df0cf1b1fef6f13815db1a6b64316c2b`  
		Last Modified: Thu, 06 Oct 2022 20:00:55 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11923e04324f2f23c1f0349823a0be5e693965db2bba963d2549f7d73c4e8002`  
		Last Modified: Thu, 06 Oct 2022 20:00:56 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bc2ebea890470749369dffb0865d3032bcf4f0e478ef6fb19cdc8b26188077`  
		Last Modified: Thu, 06 Oct 2022 20:00:55 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c5400d3e50a60045ae6d277707abdce87ae984bbb91ad2fb0c6fa51db7643`  
		Last Modified: Thu, 06 Oct 2022 20:01:17 GMT  
		Size: 6.7 MB (6736641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1b092fbec2df80c26a2df47548175db675def6261186b2ee05958405249689`  
		Last Modified: Thu, 06 Oct 2022 20:01:16 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a546230ea2a71a8709773c797033bc1dc9c96ecc54925782cadaa918648755`  
		Last Modified: Thu, 06 Oct 2022 20:01:24 GMT  
		Size: 49.0 MB (48977179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fee6859af2160a531a7f70ae48e9c20965f7384dab98708a404b4270b07231`  
		Last Modified: Thu, 06 Oct 2022 20:01:16 GMT  
		Size: 961.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635b77e933681744594c031349788f23a0c67f5a7831439ef7ca2704956708e6`  
		Last Modified: Thu, 06 Oct 2022 20:01:16 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
