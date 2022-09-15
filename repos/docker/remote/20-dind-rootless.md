## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:01b4ef9770b7794253e4756e01b11cda368e8b9c9d83d9160682272e2765a4be
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:67cf7188f0bc314901204bf4275d1f6170f9adef12291cd49520cc4b612d12e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124349979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddca4304da199e4e6705790b5167c9c251aff4fb69cd26e2c28bccf3110b0ac2`
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
# Mon, 12 Sep 2022 22:23:13 GMT
ENV DOCKER_VERSION=20.10.18
# Mon, 12 Sep 2022 22:23:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.18.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.18.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.18.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.18.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Mon, 12 Sep 2022 22:23:18 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Mon, 12 Sep 2022 22:23:20 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Mon, 12 Sep 2022 22:23:20 GMT
ENV DOCKER_COMPOSE_VERSION=2.10.2
# Mon, 12 Sep 2022 22:23:22 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.10.2/docker-compose-linux-x86_64'; 			sha256='41e9657c8abd7d656c3a40df1ae9c1171930313707a3abd5420ec8852b59eeb7'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.10.2/docker-compose-linux-armv6'; 			sha256='56fe4280d29c8714ef63e3e8de039522b519a1cdcfb577c1c02c7c00f581e326'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.10.2/docker-compose-linux-armv7'; 			sha256='709aa427507a3a064d822977d2b1d68a0bd78a114c714970033b5e6731f9879b'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.10.2/docker-compose-linux-aarch64'; 			sha256='dcac4e71c52264a795d0271b36cd6b2ea0ac266931618fab2e9e9a803ed16a4a'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.10.2/docker-compose-linux-ppc64le'; 			sha256='5c1b7a13f39aa24d3369954f692aee776d9621a3cad4ddd513aa26918debd202'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.10.2/docker-compose-linux-riscv64'; 			sha256='4bf02048f307cf1e8b432c18aee33022be50562d52afbab09d28e90cbff9e900'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.10.2/docker-compose-linux-s390x'; 			sha256='a29c82751b14f2693933ddbfc00c464fc3d78143f534024244e915880ed15760'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 12 Sep 2022 22:23:22 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 12 Sep 2022 22:23:22 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 12 Sep 2022 22:23:22 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 12 Sep 2022 22:23:23 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 12 Sep 2022 22:23:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Sep 2022 22:23:23 GMT
CMD ["sh"]
# Mon, 12 Sep 2022 22:23:29 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 12 Sep 2022 22:23:30 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 12 Sep 2022 22:23:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.18.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.18.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.18.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.18.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Mon, 12 Sep 2022 22:23:34 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 12 Sep 2022 22:23:35 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 12 Sep 2022 22:23:35 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 12 Sep 2022 22:23:35 GMT
VOLUME [/var/lib/docker]
# Mon, 12 Sep 2022 22:23:35 GMT
EXPOSE 2375 2376
# Mon, 12 Sep 2022 22:23:35 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 12 Sep 2022 22:23:36 GMT
CMD []
# Mon, 12 Sep 2022 22:23:40 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Mon, 12 Sep 2022 22:23:40 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 12 Sep 2022 22:23:41 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 12 Sep 2022 22:23:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.18.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.18.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 12 Sep 2022 22:23:43 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 12 Sep 2022 22:23:43 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 12 Sep 2022 22:23:43 GMT
USER rootless
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
	-	`sha256:58acb0837d57c9a561da28ca175336526bb5c2c50e44d323b25c40ae3127b7a9`  
		Last Modified: Mon, 12 Sep 2022 22:24:39 GMT  
		Size: 14.0 MB (13980885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12036fa7433001098dd8357378492e871675cc0d622afe6de6921568ff66bcad`  
		Last Modified: Mon, 12 Sep 2022 22:24:37 GMT  
		Size: 15.2 MB (15204102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a12f2a2423fc678a4153324cfe1ae5773d1fe9702c0bda8b0ebe4f81802090`  
		Last Modified: Mon, 12 Sep 2022 22:24:36 GMT  
		Size: 9.4 MB (9350806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9246aed32f2173a5d40f3c18d60f553637e0d868aca6d2f652b9122696a30a01`  
		Last Modified: Mon, 12 Sep 2022 22:24:35 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76a4d17082749de9c979801085e898704bd5947167e0826aa7e75c411b88e60`  
		Last Modified: Mon, 12 Sep 2022 22:24:35 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2710e0b2459ed701eed97036246487e72d583b99d0a871cfcaf925975d498c22`  
		Last Modified: Mon, 12 Sep 2022 22:24:35 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df54679093f26cff95fb44948143ba698a06baca012e2b4abd407d34919ddccf`  
		Last Modified: Mon, 12 Sep 2022 22:25:11 GMT  
		Size: 6.9 MB (6863650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be51451c3ad6b7b0e2d0484bef26284198304091ccc6676b81629fd9fe3bb8a6`  
		Last Modified: Mon, 12 Sep 2022 22:25:10 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29952b28962b208aa3258eaedc8b886b5f0b42e378a31ff9cb39e898651920c`  
		Last Modified: Mon, 12 Sep 2022 22:25:23 GMT  
		Size: 52.8 MB (52831039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4672346d8a18ce88fbec6bc6b1bfab8c77bab0c3bb69d804c465367a2f67f94`  
		Last Modified: Mon, 12 Sep 2022 22:25:10 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9decb9d5aeff67848584e755af4ec304a4b2867e4ebfb05bdf43f4c23af6ed43`  
		Last Modified: Mon, 12 Sep 2022 22:25:10 GMT  
		Size: 2.7 KB (2749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e67991c2f97095e106ff8af925eb6c7614fab168c1ffa6ac4c15d42f49e2656`  
		Last Modified: Mon, 12 Sep 2022 22:25:43 GMT  
		Size: 1.4 MB (1358652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bc297aad54d055be40851ceb9f954f7b0e7b851181409824921c604b10d12f`  
		Last Modified: Mon, 12 Sep 2022 22:25:43 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05c24cb72e5b8f70290d1684db4bed41c684449b3f6d72d49c79832eccd020f3`  
		Last Modified: Mon, 12 Sep 2022 22:25:43 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdee0706285f1967b3d5da38ea95c6af5730937cb326a0a14571b1712f54c76`  
		Last Modified: Mon, 12 Sep 2022 22:25:46 GMT  
		Size: 19.9 MB (19910121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be08a83042d6865e1388285553d7232c3db80d289175f9b165e34cf2b0d41e5`  
		Last Modified: Mon, 12 Sep 2022 22:25:43 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b3b942381fd0dbda4e2385da030d9dcb098c53f613d41189f2a7cba52eb6158a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122616461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d20c1775171f31dbb333093e7c82951720f7b2b90f7099817d95c292601fc969`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:24:48 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 09 Aug 2022 18:24:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Sep 2022 22:45:01 GMT
ENV DOCKER_VERSION=20.10.18
# Mon, 12 Sep 2022 22:45:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.18.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.18.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.18.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.18.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Mon, 12 Sep 2022 22:45:06 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Mon, 12 Sep 2022 22:45:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Thu, 15 Sep 2022 17:40:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.11.0
# Thu, 15 Sep 2022 17:40:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.11.0/docker-compose-linux-x86_64'; 			sha256='e15e0d04bb2ae3885a375a575f27ebd79679f01df2dcb1257bd2c5afe1966122'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.11.0/docker-compose-linux-armv6'; 			sha256='25b8aca3e61654be4324080ccb758f47a165c6028b57d2c4b4a0bae967274a4e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.11.0/docker-compose-linux-armv7'; 			sha256='d13b829fc9637bbf291cd4c90ddc19da7d9c69e4788399641e01657f93208c9e'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.11.0/docker-compose-linux-aarch64'; 			sha256='26088a6f1afbb58c78b2d7a7eaa0ec36df59f9f45729843ca1031ec75472b6bc'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.11.0/docker-compose-linux-ppc64le'; 			sha256='44334a3632c9a34a519860c1edc2f251addbcace694ec38f04a5d825358d9fd9'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.11.0/docker-compose-linux-riscv64'; 			sha256='dd6cf7a96fec0abd69be360f525e21ae85b97b18e45dd393feee1678457fc1b9'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.11.0/docker-compose-linux-s390x'; 			sha256='fc350527128f6ed0fb71baed1df0f905217c1ac90565be5b57c2a3d784de0e14'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Thu, 15 Sep 2022 17:40:43 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 15 Sep 2022 17:40:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 15 Sep 2022 17:40:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 15 Sep 2022 17:40:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 15 Sep 2022 17:40:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 15 Sep 2022 17:40:47 GMT
CMD ["sh"]
# Thu, 15 Sep 2022 17:40:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 15 Sep 2022 17:40:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 15 Sep 2022 17:41:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.18.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.18.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.18.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.18.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Thu, 15 Sep 2022 17:41:05 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Thu, 15 Sep 2022 17:41:06 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 15 Sep 2022 17:41:08 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 15 Sep 2022 17:41:08 GMT
VOLUME [/var/lib/docker]
# Thu, 15 Sep 2022 17:41:09 GMT
EXPOSE 2375 2376
# Thu, 15 Sep 2022 17:41:10 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 15 Sep 2022 17:41:11 GMT
CMD []
# Thu, 15 Sep 2022 17:41:19 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Thu, 15 Sep 2022 17:41:20 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 15 Sep 2022 17:41:21 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 15 Sep 2022 17:41:24 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.18.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.18.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 15 Sep 2022 17:41:25 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 15 Sep 2022 17:41:26 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 15 Sep 2022 17:41:27 GMT
USER rootless
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abd6445c68b28c4fea9c5ead64de6d84bfbcf44d2ea150df466f2efe4ca7ac8`  
		Last Modified: Tue, 09 Aug 2022 18:28:29 GMT  
		Size: 2.0 MB (2010519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6c1cdde4920e39b02e2eaa9a348dd527a363263a4901b3efdf13020d24a917`  
		Last Modified: Tue, 09 Aug 2022 18:28:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7917cc27eb40c8e61940776d61814b9a1f4e5423ba6889a65a41043147327747`  
		Last Modified: Mon, 12 Sep 2022 22:47:44 GMT  
		Size: 12.7 MB (12735456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2fb837c2a97665eab0aab456d16f5b592aa67f3dcfd8f83377aa8b294c0ef4`  
		Last Modified: Mon, 12 Sep 2022 22:47:42 GMT  
		Size: 13.8 MB (13764591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2486db73c6ed3a5f55b8aa7106c177c306d879eeb5ffbe1098ac067208d172c9`  
		Last Modified: Thu, 15 Sep 2022 17:44:36 GMT  
		Size: 12.9 MB (12924798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8154f64baeb189d07a54db4dc2a8f0d71a63ac0a91df30108c53e053bb462d`  
		Last Modified: Thu, 15 Sep 2022 17:44:34 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fa92f19f9d3a1de172e78fdf9375e304277fbbb2a8403ed88ad985cdc42966`  
		Last Modified: Thu, 15 Sep 2022 17:44:34 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7efe5d1ee3220ce766a16687956ecc2fd8b15440ae2208ae9b0b88a4d465b77`  
		Last Modified: Thu, 15 Sep 2022 17:44:34 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bcb5e7a93586618658797c63652cd89ccee7c830e7ba5ac1869f13bd8aa302`  
		Last Modified: Thu, 15 Sep 2022 17:45:13 GMT  
		Size: 6.7 MB (6736613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b059c18cbaafb2803e32fd9f2b385251022ec8165012f748e92efb77f354c2eb`  
		Last Modified: Thu, 15 Sep 2022 17:45:12 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db74ddccb79791c2ad289617368af97382e7993ab984eccc4138d84aa01956f5`  
		Last Modified: Thu, 15 Sep 2022 17:45:19 GMT  
		Size: 48.5 MB (48480345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e830cada4803c8bbadf7f343ba6d4931aa0ea9a2401c69bae1b4e468e99411`  
		Last Modified: Thu, 15 Sep 2022 17:45:12 GMT  
		Size: 964.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fea78637a8a6747baa4f8d0378a716ea0e8d5513ced35e9ba9f44810670f15`  
		Last Modified: Thu, 15 Sep 2022 17:45:12 GMT  
		Size: 2.8 KB (2753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e667b6683fa9a33107e3b86c6a221ee192b39cc00bad31af55bff19d69fadb17`  
		Last Modified: Thu, 15 Sep 2022 17:45:41 GMT  
		Size: 1.4 MB (1370604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa5f8d50b5bc2592b49d9969253f214318fdfbc5dfe5b090d90552077f6d51a`  
		Last Modified: Thu, 15 Sep 2022 17:45:41 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d2c627c2e186e9df76f1c8ae4f60a7cb392787e612013b95999c0cb1c56d7f`  
		Last Modified: Thu, 15 Sep 2022 17:45:41 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e230850574fca1faa1955ea40be1316d45ac8e445f1195b2832dde83e1792f`  
		Last Modified: Thu, 15 Sep 2022 17:45:44 GMT  
		Size: 21.9 MB (21877385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8c3633c6abc411ab286d0f2ebc96dcb3b2307a45b0c09d80e1e1220dfa7eaa`  
		Last Modified: Thu, 15 Sep 2022 17:45:41 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
