## `docker:dind-rootless`

```console
$ docker pull docker@sha256:3a7be9893b4df0db62aaa708fd1f45ce480daa30abde47358f3d1cc8918ae9a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:9ae1650b7165ef666096ec5305d82f51740659a2b91e6a23661c7bec5f5929f6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121818968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b41566b7e62df73439bdd825aed0a72c8c55ec04a4cf50276c73aa01568f878`
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
# Tue, 07 Jun 2022 18:23:40 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:23:46 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:23:46 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:23:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Tue, 07 Jun 2022 18:23:48 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.0
# Tue, 07 Jun 2022 18:23:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-x86_64'; 			sha256='4eb9084cd9e33d906bd1ea11b5bc2e77a43f8ffbe7228bcf7c829a7687f5c4bb'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv6'; 			sha256='6f447869c2286d583d5497e8a1c50b7251dc9f0763c45b064a4b898a53ebce4c'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-armv7'; 			sha256='cf566ae18f89498bb20ac71d949b82b97bec3e9f972e009141c4f2faf440257a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-aarch64'; 			sha256='f2bc74dddaa58add7b428b5a764ccd4f048b366f3eb5c80a77ff06fcdc00b3ce'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-ppc64le'; 			sha256='0e6163ccbddf4faea428a78c46c214c6bba0ab3fef57e3cad364e9ca520fa176'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.0/docker-compose-linux-s390x'; 			sha256='df667634751a575ab29bc4f125b69dfa09d1924daf26bbc0f46e6b09ee1e6699'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 07 Jun 2022 18:23:51 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 07 Jun 2022 18:23:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:23:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 07 Jun 2022 18:23:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 07 Jun 2022 18:23:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 07 Jun 2022 18:23:52 GMT
CMD ["sh"]
# Tue, 07 Jun 2022 18:24:02 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Tue, 07 Jun 2022 18:24:03 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Tue, 07 Jun 2022 18:24:03 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Tue, 07 Jun 2022 18:24:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Tue, 07 Jun 2022 18:24:04 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Tue, 07 Jun 2022 18:24:04 GMT
VOLUME [/var/lib/docker]
# Tue, 07 Jun 2022 18:24:04 GMT
EXPOSE 2375 2376
# Tue, 07 Jun 2022 18:24:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 07 Jun 2022 18:24:05 GMT
CMD []
# Thu, 16 Jun 2022 21:19:53 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Thu, 16 Jun 2022 21:19:54 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 16 Jun 2022 21:19:54 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 16 Jun 2022 21:19:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 16 Jun 2022 21:19:56 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 16 Jun 2022 21:19:57 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 16 Jun 2022 21:19:57 GMT
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
	-	`sha256:4a01eeb4b9660234932fe1a5ed6ee12b88476503688d1af44ef2cf5589db59c5`  
		Last Modified: Tue, 07 Jun 2022 18:25:11 GMT  
		Size: 65.5 MB (65511093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f16477544224c056335320872aa8dd6c2a404df9982484e1f62603e0f1f8e2a`  
		Last Modified: Tue, 07 Jun 2022 18:25:01 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e917105572c19bab12a64c5f1079e8d7b0a3e10899bd0398d1f136d41a4af191`  
		Last Modified: Tue, 07 Jun 2022 18:25:00 GMT  
		Size: 9.5 MB (9456585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b709778230e46fbd5042dc9165462ac00b69b08da200fd164c4b55ee90d71ed6`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94076fc9c77a2ec8cd8737d8ee69c11882eaa16be0e46ea97b42763d6de07213`  
		Last Modified: Tue, 07 Jun 2022 18:24:59 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0650593e055d90b3f09ecf2e61114a35929437150d1f25d6e9aea5e4d4ef57`  
		Last Modified: Tue, 07 Jun 2022 18:24:58 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8739efbf33852756a9d17dd471ab7ab9d9a1f183df6185763c4f54d55f3e5ef`  
		Last Modified: Tue, 07 Jun 2022 18:25:31 GMT  
		Size: 6.9 MB (6862542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1528486149a1ec660cc13a105d322cbe384bf2fd0bb5b32436043928d35701e8`  
		Last Modified: Tue, 07 Jun 2022 18:25:30 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fce28207d4c0f42d2a8352f195f1551714dfa68bcc768565b63a0e030a46813`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 959.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6543c9821cdb12ce3c3b95bed6148272f6ee648fcaf31c1b5b6d7aa67c459`  
		Last Modified: Tue, 07 Jun 2022 18:25:29 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f97da07775d74fef00f68ceea759559c493ec540282e0c150a0b5f40d0387a`  
		Last Modified: Thu, 16 Jun 2022 21:20:59 GMT  
		Size: 1.4 MB (1358426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6c6d18f209cec707e5dd938e5a7e9c38319191dddfc2527395ebf4922f2fdc`  
		Last Modified: Thu, 16 Jun 2022 21:20:59 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3ff5744b0a3e60672e2e8c4765b835bb5fb3d4add1cf0897f47ff7b25903fc`  
		Last Modified: Thu, 16 Jun 2022 21:20:59 GMT  
		Size: 1.4 KB (1353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c32f3663fe9c2e79e0971970c5964f09a39a83809b59aeb2601f238054c17b3`  
		Last Modified: Thu, 16 Jun 2022 21:21:02 GMT  
		Size: 19.3 MB (19346878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9084b7cd3b336717c47c00412e9106b9335b8bfaf7ccab245d0fbc4c4af5eb`  
		Last Modified: Thu, 16 Jun 2022 21:20:59 GMT  
		Size: 216.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:79728767115a191b17a69d129a65be1a067d5828bbf90d43e5833b92e2fe41b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.7 MB (115679783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23551a0cecc123712f378299710ae922fa0cb237e78e630aad050070f84ad943`
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
# Tue, 07 Jun 2022 18:44:31 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 07 Jun 2022 18:44:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Tue, 07 Jun 2022 18:44:36 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Tue, 07 Jun 2022 18:44:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Mon, 27 Jun 2022 19:40:28 GMT
ENV DOCKER_COMPOSE_VERSION=2.6.1
# Mon, 27 Jun 2022 19:40:30 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.6.1/docker-compose-linux-x86_64'; 			sha256='ed79398562f3a80a5d8c068fde14b0b12101e80b494aabb2b3533eaa10599e0f'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.6.1/docker-compose-linux-armv6'; 			sha256='2b5efc48e8359047cc280712f52e97be23fcb571b47b1e67ba6f56e971ac30f5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.6.1/docker-compose-linux-armv7'; 			sha256='727f67b78d6b1fbfed5de4d66869a691551f7341ad71504476d8a902e37588bb'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.6.1/docker-compose-linux-aarch64'; 			sha256='2890aade218c145827521efb247b5765ac10ac5c46f21dddb2220c03c98d7f83'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.6.1/docker-compose-linux-ppc64le'; 			sha256='93560efd323f39fe86244b80cbe1ffeb2c16b169c72a3ae25535def98c04e744'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.6.1/docker-compose-linux-s390x'; 			sha256='2a56c35df12d7a7ce9a9ae83426df36a612b0035ee36053912594d6f5a6ff356'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Mon, 27 Jun 2022 19:40:32 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Mon, 27 Jun 2022 19:40:33 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Mon, 27 Jun 2022 19:40:33 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 27 Jun 2022 19:40:34 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Mon, 27 Jun 2022 19:40:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 27 Jun 2022 19:40:36 GMT
CMD ["sh"]
# Mon, 27 Jun 2022 19:40:45 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Mon, 27 Jun 2022 19:40:46 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Mon, 27 Jun 2022 19:40:47 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Mon, 27 Jun 2022 19:40:48 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Mon, 27 Jun 2022 19:40:50 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Mon, 27 Jun 2022 19:40:50 GMT
VOLUME [/var/lib/docker]
# Mon, 27 Jun 2022 19:40:51 GMT
EXPOSE 2375 2376
# Mon, 27 Jun 2022 19:40:52 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 27 Jun 2022 19:40:53 GMT
CMD []
# Mon, 27 Jun 2022 19:41:01 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Mon, 27 Jun 2022 19:41:01 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Mon, 27 Jun 2022 19:41:02 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Mon, 27 Jun 2022 19:41:04 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Mon, 27 Jun 2022 19:41:05 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Mon, 27 Jun 2022 19:41:06 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 27 Jun 2022 19:41:07 GMT
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
	-	`sha256:7208c9164699a390332f26552a4e3372cbba8153d21dd8c579d78b4820727447`  
		Last Modified: Tue, 07 Jun 2022 18:46:58 GMT  
		Size: 60.0 MB (60022171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fd660eb6acfde977fdcc2e06e1f8b820b994c605f8d7c2a43c8043fee47a59`  
		Last Modified: Tue, 07 Jun 2022 18:46:49 GMT  
		Size: 13.1 MB (13097908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f160187a62e1b649c0d32c9af1c12aaf377e1a55a966ddbcce7ab48eff550cf`  
		Last Modified: Mon, 27 Jun 2022 19:43:44 GMT  
		Size: 8.6 MB (8578076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb4f2231cc40657d523a7139d6058b16f8aa0ae3cd70eb599be2335399d6812`  
		Last Modified: Mon, 27 Jun 2022 19:43:42 GMT  
		Size: 553.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b57f8edcb1810114c6447d0de3ac17bb8f2fd04a1e4ce01bbf97b9ff89ec5f5`  
		Last Modified: Mon, 27 Jun 2022 19:43:42 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32406cfcb79f2d4b1a7d7e63e3ef70119cdca171feea62f1c874636771f0650a`  
		Last Modified: Mon, 27 Jun 2022 19:43:42 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c82eb82389bdb9c7d276b1643f13d3c5caae406cf7465fdc96939f266e6f12`  
		Last Modified: Mon, 27 Jun 2022 19:44:06 GMT  
		Size: 6.7 MB (6734644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bbc1c8669d112dd5ccbe24eae85fcf64a7e05164f1f15bda3f7af0bcbffbb6`  
		Last Modified: Mon, 27 Jun 2022 19:44:05 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12b2450c676909ee9dae0cd4c9dde25caa5de2d4e5522a64aa5baf279120806`  
		Last Modified: Mon, 27 Jun 2022 19:44:05 GMT  
		Size: 963.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17ce1449b637b669cb1dff1718ae17b979ff4efa77ec1fc72be0194468c9540`  
		Last Modified: Mon, 27 Jun 2022 19:44:04 GMT  
		Size: 2.8 KB (2754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73afe9c1ea8a9add0560096dfa62e68214d911a898f87a2e607375f2fe5683eb`  
		Last Modified: Mon, 27 Jun 2022 19:44:28 GMT  
		Size: 1.4 MB (1370343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ba1c6a8841b95b395c49b28169677c6307a3101e227708a700de94e9c8d0b2`  
		Last Modified: Mon, 27 Jun 2022 19:44:28 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64830e281baf40fb6bf58458f881f01f312bda27135405c9b5546de5cabf49d`  
		Last Modified: Mon, 27 Jun 2022 19:44:28 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28141130595ce38345733636d0d91f525fa08777adf2284bfce0a9c5236dab2d`  
		Last Modified: Mon, 27 Jun 2022 19:44:31 GMT  
		Size: 21.2 MB (21177072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fab70f37b78c4047be0923ffdada8d53cc2e47aa319d07b593475cc92dd034`  
		Last Modified: Mon, 27 Jun 2022 19:44:28 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
