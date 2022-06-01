## `docker:dind-rootless`

```console
$ docker pull docker@sha256:a1275c4ac7e3309525ab3b961726583c79905779d6e38bb8afed3c30bc71e0ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:f418a4e0bf428815526d38fa66fc8d62ad36dd16a31d4f64327e9958b8ee9910
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121681823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6613f3a68740c06c23b312bf39d1cf9dc7034b813b5db8f9087fc3da83c7eb2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:21:47 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:21:48 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:21:48 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:21:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:21:53 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:21:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 01 Jun 2022 00:22:24 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Wed, 01 Jun 2022 00:22:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Jun 2022 00:22:26 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Jun 2022 00:22:26 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Jun 2022 00:22:26 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Jun 2022 00:22:27 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Jun 2022 00:22:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Jun 2022 00:22:27 GMT
CMD ["sh"]
# Wed, 01 Jun 2022 00:22:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Jun 2022 00:22:33 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Jun 2022 00:22:33 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Jun 2022 00:22:34 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Jun 2022 00:22:34 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Jun 2022 00:22:34 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Jun 2022 00:22:34 GMT
EXPOSE 2375 2376
# Wed, 01 Jun 2022 00:22:34 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Jun 2022 00:22:34 GMT
CMD []
# Wed, 01 Jun 2022 00:22:38 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Jun 2022 00:22:39 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Jun 2022 00:22:39 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Jun 2022 00:22:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Jun 2022 00:22:43 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Jun 2022 00:22:43 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Jun 2022 00:22:43 GMT
USER rootless
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d991df732aca5558e3374cd6554967a937cd594176f8e0fb592322528caf411f`  
		Last Modified: Fri, 27 May 2022 00:22:47 GMT  
		Size: 2.0 MB (2021620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d05af1c4101377236dcaf5b686eb6313f88a6ccf0cb4b1ad9383337eaaabd1`  
		Last Modified: Fri, 27 May 2022 00:22:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb5a3015bf80b070d4bce71ac156c87dcd4ad72ab2502fa2013d4c1e0fead92`  
		Last Modified: Fri, 27 May 2022 00:22:56 GMT  
		Size: 65.5 MB (65503686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb264a375f3f406fba9d11740f35f04686da753ae8292563677e4584f454446`  
		Last Modified: Fri, 27 May 2022 00:22:46 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceaead5f332c961f1a12e63bee3c9ad8992b90eb7433e9dd722b05a365c97fd6`  
		Last Modified: Wed, 01 Jun 2022 00:23:13 GMT  
		Size: 9.5 MB (9456584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38229eb29bf0a3c2cfddceafb8eb69af0fded38837740dd201d06d7ab77e1a9`  
		Last Modified: Wed, 01 Jun 2022 00:23:11 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae67dbc815da6f56499eb143026bc1ea44f9b6e01288560069dca1b655564d3`  
		Last Modified: Wed, 01 Jun 2022 00:23:11 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea3cfd40cf98cf6cfe1b5b4646fa28de1b56fbee4903e495218b1f4e0a62fbb`  
		Last Modified: Wed, 01 Jun 2022 00:23:11 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d79ffddb300967e6099c1a5b6bab408fd186386aa08cd474b87aacd24b9e6b1`  
		Last Modified: Wed, 01 Jun 2022 00:23:32 GMT  
		Size: 6.9 MB (6862546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ee2d5f7ab4a3db3eafba60e0dbef709bb65c7179fb6afc49b172e18c216ca8`  
		Last Modified: Wed, 01 Jun 2022 00:23:30 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6565e4039a05e334f335c508a00cc5be88e8925d7c72fa5407ca9ab924c47932`  
		Last Modified: Wed, 01 Jun 2022 00:23:31 GMT  
		Size: 958.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6409072794b6ecd30798be1e79545fb14ba8b7b2b0b56dbfde1ad209ce13f32`  
		Last Modified: Wed, 01 Jun 2022 00:23:30 GMT  
		Size: 2.7 KB (2749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654ddf7ce51c14d55e27ea9fcae01c2f1b8c0e7c04a8d9e06139de2cf76524d3`  
		Last Modified: Wed, 01 Jun 2022 00:23:51 GMT  
		Size: 1.2 MB (1232598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6d173ccabe858786eb8d132243d739ed42f30c273622fcdbae57c97320ba0b`  
		Last Modified: Wed, 01 Jun 2022 00:23:50 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf07dc73f5b81ce1aa3ba3f989cac47935f63b9aacd1582ebb99e491d6847a5`  
		Last Modified: Wed, 01 Jun 2022 00:23:50 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf0c40e74d23c1393751285d56bd4523e1ee440ee6879579f15b2847b883164`  
		Last Modified: Wed, 01 Jun 2022 00:23:54 GMT  
		Size: 19.3 MB (19342959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b4502d8e1a25b0bfe0d783d33569a0fc11a48c1823001fe7e278ba0b2e7aa2`  
		Last Modified: Wed, 01 Jun 2022 00:23:51 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5011050b9ab48d906a64ff8810f790db915e6e109be30f165ba64752bc0c2b5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.6 MB (115627475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71f002e164dbdf6a2f0c6410fb3ba219a30a7ea0268412c2f4a9e6cc78a5d5f`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:42:03 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Fri, 27 May 2022 00:42:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:42:05 GMT
ENV DOCKER_VERSION=20.10.16
# Fri, 27 May 2022 00:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.16.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.16.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Fri, 27 May 2022 00:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Fri, 27 May 2022 00:42:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 01 Jun 2022 00:58:05 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Wed, 01 Jun 2022 00:58:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 01 Jun 2022 00:58:10 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 01 Jun 2022 00:58:11 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 01 Jun 2022 00:58:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 01 Jun 2022 00:58:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 01 Jun 2022 00:58:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Jun 2022 00:58:14 GMT
CMD ["sh"]
# Wed, 01 Jun 2022 00:58:25 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 01 Jun 2022 00:58:25 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 01 Jun 2022 00:58:26 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 01 Jun 2022 00:58:27 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 01 Jun 2022 00:58:29 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 01 Jun 2022 00:58:29 GMT
VOLUME [/var/lib/docker]
# Wed, 01 Jun 2022 00:58:30 GMT
EXPOSE 2375 2376
# Wed, 01 Jun 2022 00:58:31 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 01 Jun 2022 00:58:32 GMT
CMD []
# Wed, 01 Jun 2022 00:58:40 GMT
RUN apk add --no-cache iproute2
# Wed, 01 Jun 2022 00:58:41 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 01 Jun 2022 00:58:42 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 01 Jun 2022 00:58:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.16.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.16.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 01 Jun 2022 00:58:46 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 01 Jun 2022 00:58:47 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 01 Jun 2022 00:58:48 GMT
USER rootless
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3e5a9e15a60519e35e8b9a753200b3a5fd5d702eb7ce3db15a5cc6dfea4c7d`  
		Last Modified: Fri, 27 May 2022 00:44:06 GMT  
		Size: 2.0 MB (1996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2296f0760e1d9178f62ef54c685f9eeea21ee68455df53b6823bf3da5784f5df`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e849ad00357eb1e6cf62ee3ac11c3ec8a62fdadc0a1b8b017e6803664b057dce`  
		Last Modified: Fri, 27 May 2022 00:44:14 GMT  
		Size: 60.0 MB (60009152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b449558387c3b597b0d43943c6910ae3acd2f931fbb1cfecc2009974571fe19`  
		Last Modified: Fri, 27 May 2022 00:44:05 GMT  
		Size: 13.1 MB (13097915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6d9de3485725ef5cc3be38ab53d3a95a5e6fb80aac6ab609bd7e86ae82eeee`  
		Last Modified: Wed, 01 Jun 2022 00:59:39 GMT  
		Size: 8.7 MB (8663391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5788c9847ffc95d732910353bef21029e5d7265961532fb1009ab18d8b114`  
		Last Modified: Wed, 01 Jun 2022 00:59:37 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff3e8866c6fb5ba70a7cbfa82858852de6b756185baf6f819512c8c278f25f5`  
		Last Modified: Wed, 01 Jun 2022 00:59:37 GMT  
		Size: 1.0 KB (1024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87178099d43fb291060f6b9579f854ec88a24ed97552fa45b3397ef388e9a113`  
		Last Modified: Wed, 01 Jun 2022 00:59:37 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27c00ea3711f30e8b86a3f5978705c3500943ee3384e9dff017ed57b13f7b2a`  
		Last Modified: Wed, 01 Jun 2022 01:00:01 GMT  
		Size: 6.7 MB (6734655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ff8fa9fb1c5a911efe53340be0c1cb9efe8f1be27deb392662c52c3b43e3c5`  
		Last Modified: Wed, 01 Jun 2022 01:00:00 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8b00528dde1506b845418aef5241fa19b9ffff704886ba1119989257dbc162`  
		Last Modified: Wed, 01 Jun 2022 01:00:00 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b2c0c0fa48ff98b6efcee52fddcc07d65231d20cc3a6cf51013b448d24b8e2`  
		Last Modified: Wed, 01 Jun 2022 01:00:00 GMT  
		Size: 2.8 KB (2751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1735a3f96f8a602b69c3c869c4b6c7bdcadd091e6d58a528be6e170a131586`  
		Last Modified: Wed, 01 Jun 2022 01:00:25 GMT  
		Size: 1.2 MB (1246074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c42a31b40431d1a2754ca8874a254eb79daeb61e94b60a7c4d4f967bf9881f`  
		Last Modified: Wed, 01 Jun 2022 01:00:25 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18405e3e40a5c2b63568b41579c979920d5597fef62f661a9fe96cf6d8d3e66`  
		Last Modified: Wed, 01 Jun 2022 01:00:25 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efcc751ed0b230cd7c1ecb6a4b37eb8d2a0aeafab51cde8bb011c83d79d9dfef`  
		Last Modified: Wed, 01 Jun 2022 01:00:29 GMT  
		Size: 21.2 MB (21176731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65403038fea74331e5001d11b4f93a3114e52f298ddf10cbbc6e22a409940d4e`  
		Last Modified: Wed, 01 Jun 2022 01:00:25 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
