## `docker:dind`

```console
$ docker pull docker@sha256:5da8f946c2b2b9e37b6554680ef3cac95875cb4f5bf66001c80a5e0cc726ddac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:a2dba2c0260200fe08074edd2e951287a0d3b3137726cf0eab044599e73d7b41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108056338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c82a93f89b8dca89e129732754f5fe2e948379bd4d28f117036589ab6d039941`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:19:24 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 06 Oct 2022 20:19:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:20:03 GMT
ENV DOCKER_VERSION=20.10.18
# Thu, 06 Oct 2022 20:20:08 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.18.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.18.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.18.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.18.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Thu, 06 Oct 2022 20:20:08 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Thu, 06 Oct 2022 20:20:09 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Thu, 06 Oct 2022 20:20:10 GMT
ENV DOCKER_COMPOSE_VERSION=2.11.2
# Thu, 06 Oct 2022 20:20:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-x86_64'; 			sha256='1178848502b0771b96895febeb4b1736acd5019c4ed71a8efbabf6915185fe8a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-armv6'; 			sha256='3e863e83a2701b26e168118f30456c3bd2ec37886182fc3373a8fe460e714761'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-armv7'; 			sha256='c133c194f36b3a6dcd552c4e32652f6ef7c22af258a6f14b414bf751aad3d2fd'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-aarch64'; 			sha256='eb65ae4a4dd4de7dc767935c2bc49e3641d265df1273ea8f577cadb6bd9b4ebf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-ppc64le'; 			sha256='24f65d215a198e33f3f1646ebabd6cae00eb6d2d3442b86c97d8198331350785'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-riscv64'; 			sha256='14a3de648bfa75a33ee8ded1cc8d501cff10c9d1565aab3dd641cf7283e9b51a'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-s390x'; 			sha256='08e8612dc7aa2d983c6c07c54e483cbc1ec089cfe9d7f790643dd8dbd30ee4f5'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Thu, 06 Oct 2022 20:20:11 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 06 Oct 2022 20:20:12 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:20:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 06 Oct 2022 20:20:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 06 Oct 2022 20:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:20:12 GMT
CMD ["sh"]
# Thu, 06 Oct 2022 20:20:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 06 Oct 2022 20:20:19 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 06 Oct 2022 20:20:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.18.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.18.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.18.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.18.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Thu, 06 Oct 2022 20:20:25 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 06 Oct 2022 20:20:26 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 06 Oct 2022 20:20:26 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 06 Oct 2022 20:20:26 GMT
VOLUME [/var/lib/docker]
# Thu, 06 Oct 2022 20:20:26 GMT
EXPOSE 2375 2376
# Thu, 06 Oct 2022 20:20:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 06 Oct 2022 20:20:26 GMT
CMD []
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0dd730a5c3e0f2ca69ebcd573f312df80344d4349d3cdfc40bdc75c406b44d`  
		Last Modified: Thu, 06 Oct 2022 20:21:25 GMT  
		Size: 2.0 MB (2036059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b90f8029a368ccb8e58eae4ebf51ea850e9116df1d92a8e8687a6902c01e69f`  
		Last Modified: Thu, 06 Oct 2022 20:21:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2204c289e68225254a6419362b0472241d48e145ac9cbaf4f62cfa3c1c9e218`  
		Last Modified: Thu, 06 Oct 2022 20:22:54 GMT  
		Size: 14.0 MB (13980868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75dcb107a3780a2440d552e1f7d699ae5f71f6936397f3d97e3fce096a824e3`  
		Last Modified: Thu, 06 Oct 2022 20:22:52 GMT  
		Size: 15.2 MB (15204101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a173a06c3138721d3c98974e00f4d246c35c4a29818dbb2d121b7d312e909c2`  
		Last Modified: Thu, 06 Oct 2022 20:22:52 GMT  
		Size: 14.3 MB (14327709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f3a1cb7a3f3bd9d05a42eb88a3a04e300470da7e5ee1ba4b2c9fb1e1f9c1a0`  
		Last Modified: Thu, 06 Oct 2022 20:22:50 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d2f4b1d0b5372da42d4a04c0247f7c9686d22edf44f10e3dfdfec44375a72f`  
		Last Modified: Thu, 06 Oct 2022 20:22:50 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2ccc3f55757cd87a0379d2c77c9348e2427a63f69c63af54feb1110ebeee4c`  
		Last Modified: Thu, 06 Oct 2022 20:22:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd921a442ce67dac01524a9c5d9ec49c619aeb750624a85a35690d243c74895`  
		Last Modified: Thu, 06 Oct 2022 20:23:25 GMT  
		Size: 6.9 MB (6863610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae98848a64da82e60e05a5cbeea04266a2284b9da3470b5d96dcf2d7274aeb1`  
		Last Modified: Thu, 06 Oct 2022 20:23:25 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e57da9404b5085b883436ab5107bb0ecaa2509b4d03b1b88361d124b38de865`  
		Last Modified: Thu, 06 Oct 2022 20:23:32 GMT  
		Size: 52.8 MB (52831038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5dbc91b680280e93f5e67c9c67802a42195978fdbe4474e6b5a68d23bb833`  
		Last Modified: Thu, 06 Oct 2022 20:23:24 GMT  
		Size: 960.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7770816ba3ff49781e383ec4315761a04c75f65dc9084a184e1e1e65e3ed466d`  
		Last Modified: Thu, 06 Oct 2022 20:23:24 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:2576c3d253c592221ada86777e1cf9ed8686bc3ce00655113bb2a559b2e2f6e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99364238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77dabccc5ea5c54ce235b3e4fc679368ba587500b0f8d42949f55ec66177e201`
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
# Thu, 06 Oct 2022 19:58:30 GMT
ENV DOCKER_VERSION=20.10.18
# Thu, 06 Oct 2022 19:58:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.18.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.18.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.18.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.18.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Thu, 06 Oct 2022 19:58:34 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Thu, 06 Oct 2022 19:58:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Thu, 06 Oct 2022 19:58:37 GMT
ENV DOCKER_COMPOSE_VERSION=2.11.2
# Thu, 06 Oct 2022 19:58:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-x86_64'; 			sha256='1178848502b0771b96895febeb4b1736acd5019c4ed71a8efbabf6915185fe8a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-armv6'; 			sha256='3e863e83a2701b26e168118f30456c3bd2ec37886182fc3373a8fe460e714761'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-armv7'; 			sha256='c133c194f36b3a6dcd552c4e32652f6ef7c22af258a6f14b414bf751aad3d2fd'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-aarch64'; 			sha256='eb65ae4a4dd4de7dc767935c2bc49e3641d265df1273ea8f577cadb6bd9b4ebf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-ppc64le'; 			sha256='24f65d215a198e33f3f1646ebabd6cae00eb6d2d3442b86c97d8198331350785'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-riscv64'; 			sha256='14a3de648bfa75a33ee8ded1cc8d501cff10c9d1565aab3dd641cf7283e9b51a'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.11.2/docker-compose-linux-s390x'; 			sha256='08e8612dc7aa2d983c6c07c54e483cbc1ec089cfe9d7f790643dd8dbd30ee4f5'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Thu, 06 Oct 2022 19:58:41 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 06 Oct 2022 19:58:42 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 06 Oct 2022 19:58:42 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 06 Oct 2022 19:58:43 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 06 Oct 2022 19:58:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:58:45 GMT
CMD ["sh"]
# Thu, 06 Oct 2022 19:58:56 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 06 Oct 2022 19:58:57 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 06 Oct 2022 19:59:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.18.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.18.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.18.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.18.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Thu, 06 Oct 2022 19:59:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 06 Oct 2022 19:59:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 06 Oct 2022 19:59:06 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 06 Oct 2022 19:59:06 GMT
VOLUME [/var/lib/docker]
# Thu, 06 Oct 2022 19:59:07 GMT
EXPOSE 2375 2376
# Thu, 06 Oct 2022 19:59:08 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 06 Oct 2022 19:59:09 GMT
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
	-	`sha256:9d2c8901bb3fdcd729a8086b88b484be4e0ae8b413091e28c3a52840a6810464`  
		Last Modified: Thu, 06 Oct 2022 20:02:35 GMT  
		Size: 12.7 MB (12735468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617bdaf04ff9e4e23b0d0ce0ee6f8a588a263dbf8ee9bb6f3522a04fbf897671`  
		Last Modified: Thu, 06 Oct 2022 20:02:33 GMT  
		Size: 13.8 MB (13764585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905797b402e18c92f478183c71ffd378fa1a3ea8e0fac2f8589ccce2ce06d2e5`  
		Last Modified: Thu, 06 Oct 2022 20:02:33 GMT  
		Size: 12.9 MB (12922224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4200b31db3e1660c3da83c18cbd9b6b5756355c0d89adcce2fac34ab37e5f423`  
		Last Modified: Thu, 06 Oct 2022 20:02:31 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f100482841ca2a3ae10e6580c062b44f3a63ef116e3d2e832969d5cdca5868b`  
		Last Modified: Thu, 06 Oct 2022 20:02:31 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a7cc51cc60fff0902402a5b867b277e987f5f9b2aaa96386cad00b5bc17240`  
		Last Modified: Thu, 06 Oct 2022 20:02:31 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22fd0a03f4a0fa806b5d0db2701727a9f81459705c00f53db79a89d29e71453`  
		Last Modified: Thu, 06 Oct 2022 20:03:14 GMT  
		Size: 6.7 MB (6736574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf811c799871b7593556ceaa7b1a61bf0d1a88903fa6b0bba45ed9e9d0411c0`  
		Last Modified: Thu, 06 Oct 2022 20:03:12 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd27ffbd3cee52f259a4c0e5da6afd43ed6f1f6e5b0633a521e222d2107423`  
		Last Modified: Thu, 06 Oct 2022 20:03:20 GMT  
		Size: 48.5 MB (48480343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d85902f7e6e85c846141c69b093301d4c22dee4de6144644d4cad71bd82a89d6`  
		Last Modified: Thu, 06 Oct 2022 20:03:12 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2591cfe124f16f13acae5cfcee32b477a1243d3a874cf0dba586c9f4b994b6b`  
		Last Modified: Thu, 06 Oct 2022 20:03:13 GMT  
		Size: 2.7 KB (2749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
