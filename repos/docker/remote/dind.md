## `docker:dind`

```console
$ docker pull docker@sha256:27e12d4d743ff939ca7e21e9e171b11bab576bfc621dfe714ceaec7ea7356b4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:d80086e7e267e52a167ed722023bae982b9998cdc79e8cec355d3f8c836c220c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.3 MB (109251760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57525a72eb8985901c576fb15be3d135e97310678edcf9c44159c0005045f9be`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Tue, 29 Nov 2022 01:27:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 29 Nov 2022 01:27:02 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Tue, 29 Nov 2022 01:27:39 GMT
ENV DOCKER_VERSION=20.10.21
# Tue, 29 Nov 2022 01:27:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.21.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.21.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.21.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.21.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Tue, 29 Nov 2022 01:27:43 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Tue, 29 Nov 2022 01:27:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Tue, 29 Nov 2022 01:27:46 GMT
ENV DOCKER_COMPOSE_VERSION=2.13.0
# Tue, 29 Nov 2022 01:27:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-x86_64'; 			sha256='943ff254867e1c23cd6414d7255790daddc7ab69013dd79ba5c172410cbafb14'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-armv6'; 			sha256='c188afabb4565145beaf3ccd025d04428f7ba543616fb7042190d267ffb3df77'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-armv7'; 			sha256='7f985bf4b61f70b17a3c7da2d4cedb7e8fb13bc7c67d5e6e2fd23dd28212d61a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-aarch64'; 			sha256='4a920b7d5fe5011dd466fa87ea3b47ee5f224b5770337188daee359ec606eb20'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-ppc64le'; 			sha256='2aaa046eb055d2b0ccbdeac2c22f2bf927adb4c328b912a458686bf0861322d1'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-riscv64'; 			sha256='f8690e1c715a1bd87316cdd4e1ba1c0144f02eaa9f037075a471d926af133306'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-s390x'; 			sha256='e48830b80893ac41d8f7198f6660f23c24c4a7cde3b95593e534ff7bb3ee0a03'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 29 Nov 2022 01:27:48 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 29 Nov 2022 01:27:48 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 29 Nov 2022 01:27:48 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 29 Nov 2022 01:27:49 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 29 Nov 2022 01:27:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Nov 2022 01:27:49 GMT
CMD ["sh"]
# Tue, 29 Nov 2022 01:27:55 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 29 Nov 2022 01:27:56 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 29 Nov 2022 01:28:00 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.21.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.21.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.21.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.21.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Tue, 29 Nov 2022 01:28:00 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Tue, 29 Nov 2022 01:28:01 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 29 Nov 2022 01:28:01 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 29 Nov 2022 01:28:01 GMT
VOLUME [/var/lib/docker]
# Tue, 29 Nov 2022 01:28:01 GMT
EXPOSE 2375 2376
# Tue, 29 Nov 2022 01:28:01 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 29 Nov 2022 01:28:01 GMT
CMD []
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93eea1d5d8e5eb7f3c01c44eb6652605d4b5ad66cf819d1e3b6053733f2f13cf`  
		Last Modified: Tue, 29 Nov 2022 01:28:59 GMT  
		Size: 2.1 MB (2064254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6984615ae18456cfe3414608e241ff765a9b48524ec0d8f2820d1067f08fa892`  
		Last Modified: Tue, 29 Nov 2022 01:30:17 GMT  
		Size: 14.0 MB (13983067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e603bb994164c1620cee092b6fc73ee016c526c92af58f26b3900e68f913a1b`  
		Last Modified: Tue, 29 Nov 2022 01:30:16 GMT  
		Size: 15.2 MB (15204113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8102f44846c19c561ef1195b487c4c622d7a173e7bfc9c754185368f06136d10`  
		Last Modified: Tue, 29 Nov 2022 01:30:16 GMT  
		Size: 14.8 MB (14772086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65281e1e3f66b64785398e019ecd16fab9c7e9c28c317a904ece18885fad5291`  
		Last Modified: Tue, 29 Nov 2022 01:30:13 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36e18e3aa06c1e5d5a5810d2a99c4ba4d8d0174c0842d14d8c8368da236e1ad`  
		Last Modified: Tue, 29 Nov 2022 01:30:13 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ec3bdf275562da8d95a87fa3cc11bbdd4581e89afdd4af6c38184380700219`  
		Last Modified: Tue, 29 Nov 2022 01:30:13 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa6390823627c0cdd34ca6ed3cb7bdd314cacf82b7c8c26030ab325478b3200`  
		Last Modified: Tue, 29 Nov 2022 01:30:44 GMT  
		Size: 6.8 MB (6837145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a77c182fc80c0753eb69ff089c3455e7dc273ba676448b3a3f8051071aadf0f`  
		Last Modified: Tue, 29 Nov 2022 01:30:43 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03ef4bfca0181218305111e22199da2d8cfbc624b9ad399ef766fa214b1f1e3`  
		Last Modified: Tue, 29 Nov 2022 01:30:51 GMT  
		Size: 53.0 MB (53013557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5469d2ac32564b11d0ba870fb28a262fd1778b9e3dd7388e98cdefedfb6c069`  
		Last Modified: Tue, 29 Nov 2022 01:30:43 GMT  
		Size: 1.0 KB (1045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8ff3731cfae99aa04159664f0874759b0a3a60a4d029d5c2156e023237bb818`  
		Last Modified: Tue, 29 Nov 2022 01:30:43 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:d5455f6e461c1e23da9884e7dff16999d783f640c8030ed61646e4b90ba46f37
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.5 MB (100529654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70722f4941fe6b807694fc2cc40101286b5c40df34bad1c1ffc49810d854728`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Tue, 29 Nov 2022 01:42:08 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 29 Nov 2022 01:42:08 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Tue, 29 Nov 2022 01:42:55 GMT
ENV DOCKER_VERSION=20.10.21
# Tue, 29 Nov 2022 01:42:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.21.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.21.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.21.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.21.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Tue, 29 Nov 2022 01:42:59 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Tue, 29 Nov 2022 01:43:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Mon, 05 Dec 2022 20:40:02 GMT
ENV DOCKER_COMPOSE_VERSION=2.14.0
# Mon, 05 Dec 2022 20:40:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.14.0/docker-compose-linux-x86_64'; 			sha256='fdf634ab2b01aca33372bef2bf866699ef2e1f2dab19972e37967b1fc2a11402'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.14.0/docker-compose-linux-armv6'; 			sha256='63e0826ddebc1ae776f38ab872b41f68b48fca246cdf67c709e07eef543cdf88'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.14.0/docker-compose-linux-armv7'; 			sha256='c1664c4dcefc2a56a4f16f4dbd76e531f237bfbf713b90d3acea50df42a1aada'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.14.0/docker-compose-linux-aarch64'; 			sha256='0265f45b30f4f0e1d53c1968c590181f64c546129d967460de382c6de38af191'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.14.0/docker-compose-linux-ppc64le'; 			sha256='dbee58426af567787e5c1d14e925cca0d0a958edc55203c4b29c10dda8e27355'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.14.0/docker-compose-linux-riscv64'; 			sha256='d447a75ff4d900b19d40e0c69811b335518f8a5fbc6377e0aff25a3b999a8c49'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.14.0/docker-compose-linux-s390x'; 			sha256='2c5bbb6513d7377919bd4189f25d8bf5d8706a5345f10609d8c49d5cf4d8ab88'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 05 Dec 2022 20:40:05 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 05 Dec 2022 20:40:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 05 Dec 2022 20:40:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 05 Dec 2022 20:40:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 05 Dec 2022 20:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 05 Dec 2022 20:40:05 GMT
CMD ["sh"]
# Mon, 05 Dec 2022 20:40:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 05 Dec 2022 20:40:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 05 Dec 2022 20:40:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.21.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.21.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.21.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.21.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Mon, 05 Dec 2022 20:40:16 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Mon, 05 Dec 2022 20:40:17 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 05 Dec 2022 20:40:17 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 05 Dec 2022 20:40:17 GMT
VOLUME [/var/lib/docker]
# Mon, 05 Dec 2022 20:40:17 GMT
EXPOSE 2375 2376
# Mon, 05 Dec 2022 20:40:17 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 05 Dec 2022 20:40:17 GMT
CMD []
```

-	Layers:
	-	`sha256:261da4162673b93e5c0e7700a3718d40bcc086dbf24b1ec9b54bca0b82300626`  
		Last Modified: Tue, 22 Nov 2022 22:39:45 GMT  
		Size: 3.3 MB (3259190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb5dec0c1f562bd55dc773ccc0c77fbfd42b92083262478523c19bcc0f397af`  
		Last Modified: Tue, 29 Nov 2022 01:44:14 GMT  
		Size: 2.0 MB (2036851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90e06f207318e77d0df221e7f354882895dee491dd233e5d36728caa3e56f7a`  
		Last Modified: Tue, 29 Nov 2022 01:45:27 GMT  
		Size: 12.7 MB (12739256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f45adca886768ef514f318c52a8be2bfb2cf2c3b77a4f79080aee488d34bf51`  
		Last Modified: Tue, 29 Nov 2022 01:45:25 GMT  
		Size: 13.8 MB (13764593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d61cddf01ddc68098c5b2fd19d61bce2f5f132c7ac7b93c397f0a86aedd9b15`  
		Last Modified: Mon, 05 Dec 2022 20:42:24 GMT  
		Size: 13.1 MB (13066783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24c9ba3ddce3e9bfe6e84522bbfe59583e4ef7d4fb98391ac49dc00696d3f7d`  
		Last Modified: Mon, 05 Dec 2022 20:42:23 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7deb8a233dd4d65d382b8e84672684f3ab2d31aaef29c104f249ae1bda12f0`  
		Last Modified: Mon, 05 Dec 2022 20:42:23 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1447d85b5ea17ee9732a6be6f2982b71a22de35ff9d893f25b4003f6e38bed89`  
		Last Modified: Mon, 05 Dec 2022 20:42:23 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95f9bf7750a9a771df39fd36d53bf0473b57d5be66c7796fc39225770f0c582`  
		Last Modified: Mon, 05 Dec 2022 20:42:51 GMT  
		Size: 7.0 MB (6990975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011d6af44e2923a3e72b89583ad896d9d3f4f19524fe5c63f2308749b8e7ca39`  
		Last Modified: Mon, 05 Dec 2022 20:42:50 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0c127cb2a153731f96a42c91471c1ca75ae0e84d6caca9b5f94e53dcc569d6`  
		Last Modified: Mon, 05 Dec 2022 20:42:55 GMT  
		Size: 48.7 MB (48665163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4351d2f5d80024f27d4db14ed0b15ce9a5a8d3ed66030c22e573a62adb67a44`  
		Last Modified: Mon, 05 Dec 2022 20:42:50 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee28717f9f0601644002e8c274b7b083f196528d1360ae76fbe92e65f03366f`  
		Last Modified: Mon, 05 Dec 2022 20:42:50 GMT  
		Size: 2.8 KB (2751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
