## `docker:dind-rootless`

```console
$ docker pull docker@sha256:aa45a0004d874e539af63bfad8db9ee7f00e847dae83be333a59cbed442751c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:b05edbab49df0c916810ee6ff4aab6bab3dc9518b4a8e1b960af37143c7320d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121065216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92f1b93e523ccc3bb545467872a43f2a1bbc5a8a20a515cc7a9d0b643a52093a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:02:42 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 11:02:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 01:19:25 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 01:30:40 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 01:30:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 01:30:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 01:30:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 01:30:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 01:30:45 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:45 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 01:30:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 01:30:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 01:30:46 GMT
CMD ["sh"]
# Wed, 11 May 2022 01:30:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 01:30:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 01:30:52 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 01:30:53 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 01:30:53 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 01:30:53 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 01:30:53 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 01:30:53 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 01:30:53 GMT
CMD []
# Wed, 11 May 2022 01:30:58 GMT
RUN apk add --no-cache iproute2
# Wed, 11 May 2022 01:30:58 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 May 2022 01:30:59 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 May 2022 01:31:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 11 May 2022 01:31:01 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 11 May 2022 01:31:01 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 11 May 2022 01:31:01 GMT
USER rootless
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e3bd692ff4ff4d32e553972ecdb6781dd2c64e1b8ce0ea011f36caf237816`  
		Last Modified: Tue, 05 Apr 2022 11:03:50 GMT  
		Size: 2.0 MB (1969568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36df9e333c707e825d69eb4d7bff03bb32304316c692a4a4a6cdf2860b94ccd9`  
		Last Modified: Tue, 05 Apr 2022 11:03:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde439603efe4d8aa07f865a0f0c54a9f1f8067f28c2a8c09f21c21633626a7f`  
		Last Modified: Fri, 06 May 2022 01:20:23 GMT  
		Size: 65.5 MB (65461079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2220c12dac3441d27b5387a49fccc6b7f5af7ddc9aff8ed33606d0d7edfd8eaa`  
		Last Modified: Wed, 11 May 2022 01:31:30 GMT  
		Size: 14.5 MB (14454323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc445e1e497c3b13a52a6d0a3d80ca2647800e00269b8a565d6bda861a29ace7`  
		Last Modified: Wed, 11 May 2022 01:31:29 GMT  
		Size: 9.1 MB (9114015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd7ed9cb253bc64e75aca8594cea35b4855c0dc0019b0deafc2129cb1654839`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3b84550078ef54a0f19b21faabcfbab4b0bee902667e27e99677b7823f5e7b`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2706e8f26ae6d1aeac1334e6877023ee32ac62243384effb1448afd5b2c8d`  
		Last Modified: Wed, 11 May 2022 01:31:28 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1d61b2da2cecaa5e21adefa8917ed7b2cb9dcf5b98a76806fc9a0f90957161`  
		Last Modified: Wed, 11 May 2022 01:31:49 GMT  
		Size: 6.7 MB (6737213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e2bb1776af038787fb0139867e401b56118a1570400eded6f5f8f62a178d50`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95cd43b09a63fd9c74d4e411be4c31cad9d8f04219b28b6d4c5b62fecae7f7a`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f07cfe16f952028090e2c8fb742533364042619bc8dafa2cf4a0410770a352`  
		Last Modified: Wed, 11 May 2022 01:31:48 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3274bbdde54bb4a48874b2ce035e92a09cb808e71aa62674d2b45feb1b8c335`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 1.2 MB (1161979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d1ddc5adfd1cb7677ff044ff73cb26aadc1c8bfd561d4d01bd5a277ea695bf`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4637389793458adbb0a60e604cf1a24c364b4ebfba0bf0dcb518c42d1bda9768`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f7d295b80db32082883f9fe59863d70d879876e123ec3d35965b8a5a0d8b99`  
		Last Modified: Wed, 11 May 2022 01:32:13 GMT  
		Size: 19.3 MB (19343874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb529ec47f8280e1c14cafe4c44f90ee830858c572841b0a981ab78b6e2550d3`  
		Last Modified: Wed, 11 May 2022 01:32:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:86bdf6636db6a8b06847ac84644c7d50300c2955b2b200ce3aa55f3074ebecd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.1 MB (115065045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3e6f1e988d89dd418bf82197674b0e012f1aece1514f899a6397dd8a544668e`
-	Entrypoint: `["dockerd-entrypoint.sh"]`
-	Default Command: `[]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 08:57:00 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 05 Apr 2022 08:57:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 06 May 2022 00:39:33 GMT
ENV DOCKER_VERSION=20.10.15
# Fri, 06 May 2022 00:39:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.15.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.15.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O docker.tgz "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 	; 	rm docker.tgz; 		dockerd --version; 	docker --version
# Wed, 11 May 2022 00:42:54 GMT
ENV DOCKER_BUILDX_VERSION=0.8.2
# Wed, 11 May 2022 00:42:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-amd64'; 			sha256='c64de4f3c30f7a73ff9db637660c7aa0f00234368105b0a09fa8e24eebe910c3'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v6'; 			sha256='d0e5d19cd67ea7a351e3bfe1de96f3d583a5b80f1bbadd61f7adcd61b147e5f5'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm-v7'; 			sha256='b5bb1e28e9413a75b2600955c486870aafd234f69953601eecc3664bd3af7463'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-arm64'; 			sha256='304d3d9822c75f98ad9cf57f0c234bcf326bbb96d791d551728cadd72a7a377f'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-ppc64le'; 			sha256='32b317d86c700d920468f162f93ae2282777da556ee49b4329f6c72ee2b11b85'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-riscv64'; 			sha256='76d5fcf92ffa31b3e470d8ec1ab11f7b6997729e5c94d543fec765ad79ad0630'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.8.2/buildx-v0.8.2.linux-s390x'; 			sha256='ec4bb6f271f38dca5a377a70be24ee2108a85f6e6ba511ad3b805c4f1602a0d2'; 			;; 		*) echo >&2 "warning: unsupported buildx architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	docker buildx version
# Wed, 11 May 2022 00:42:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.5.0
# Wed, 11 May 2022 00:43:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-x86_64'; 			sha256='6296d17268c77a7159f57f04ed26dd2989f909c58cca4d44d1865f28bd27dd67'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv6'; 			sha256='92b423e2c4d0ca0a979d7b6a4fb13707612f8fa19b900bc6cd1c2cf83f2780c5'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-armv7'; 			sha256='d728dcbe5e20103e9b025efdbb6bfbca9ea9866851e669f7775fe3ebb7ab945c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-aarch64'; 			sha256='7efc61cc85fe712f14f04a6886d1481c96fe958be265f67482583b4b713b6a22'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-ppc64le'; 			sha256='e40af00a5f3ef87d31372f949134411b574042b8c055b2e5da12b92192405cb6'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-linux-s390x'; 			sha256='c36e48910f095d07d582b69363fb3f902bb6fab9e2bd3d5ed82a67d1b2279a39'; 			;; 		*) echo >&2 "warning: unsupported compose architecture ($apkArch); skipping"; exit 0 ;; 	esac; 	plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	wget -O "$plugin" "$url"; 	echo "$sha256 *$plugin" | sha256sum -c -; 	chmod +x "$plugin"; 	ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 11 May 2022 00:43:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 11 May 2022 00:43:05 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 11 May 2022 00:43:06 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 11 May 2022 00:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 11 May 2022 00:43:08 GMT
CMD ["sh"]
# Wed, 11 May 2022 00:43:19 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 11 May 2022 00:43:20 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:21 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 11 May 2022 00:43:22 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 11 May 2022 00:43:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 11 May 2022 00:43:24 GMT
VOLUME [/var/lib/docker]
# Wed, 11 May 2022 00:43:25 GMT
EXPOSE 2375 2376
# Wed, 11 May 2022 00:43:26 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 11 May 2022 00:43:27 GMT
CMD []
# Wed, 11 May 2022 00:43:36 GMT
RUN apk add --no-cache iproute2
# Wed, 11 May 2022 00:43:36 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 11 May 2022 00:43:37 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 11 May 2022 00:43:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.15.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.15.tgz'; 			;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O rootless.tgz "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 11 May 2022 00:43:41 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 11 May 2022 00:43:42 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 11 May 2022 00:43:43 GMT
USER rootless
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b8a1a2bc336776643f1641eb7c6c2c8fbe180e51541b40d7abec0ceb17668b`  
		Last Modified: Tue, 05 Apr 2022 08:58:34 GMT  
		Size: 1.9 MB (1938913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa25d67de920b612e26aef152b86d46e8cd4eb0e7e991d33f616108107c752e3`  
		Last Modified: Tue, 05 Apr 2022 08:58:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bace62412be99e37e41c6209417615e6e417cb0bdb8a0e509110a3b9b5af5b`  
		Last Modified: Fri, 06 May 2022 00:41:14 GMT  
		Size: 60.0 MB (59973422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8b8a1b3f8ca4629fce0550d02a91d6faf92e020a1cfa050c4e73fbeecffd0f`  
		Last Modified: Wed, 11 May 2022 00:44:37 GMT  
		Size: 13.1 MB (13097921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd73b57441486d29bba8adc690d019a81a58d55afb2144a0a0ee9f04c48b58b`  
		Last Modified: Wed, 11 May 2022 00:44:36 GMT  
		Size: 8.4 MB (8353176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1491e487ee15eff8d1484795137ca77e8c33cef424c8009f58efb98b55e498c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7428344a1d209df26c6007938ae720ca5314b7194aad26da9450b76c2fdfb3c`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf19d592fc22ab6b365349a62e52010658ab6d152e903ad319f7b2ac588820b7`  
		Last Modified: Wed, 11 May 2022 00:44:35 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7787c7635a670bb2a73df457b35cc7189fcb71df87fcebab6a587c6868c1eba9`  
		Last Modified: Wed, 11 May 2022 00:44:59 GMT  
		Size: 6.6 MB (6620287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929242070a07212fa6187a6481abb7f4f2537de4ca5834dc672eb54aabe985e`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce59cda5df84ca4590a12f295c6e1bdae8b5ab886613f7cb21c8f9981f2ba2a`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 957.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fe15f5668d48ec3ac87bcfd1153c4f44d21b5932a5b0431b126f12ad38dbd7`  
		Last Modified: Wed, 11 May 2022 00:44:58 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b3985e0ad4d291eea7cf874cc318605bcf5da8770d51f4b65555611d8ec1cd`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 1.2 MB (1177961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7d124f6c1ceea4201be7da76786410ebeebbc1ca0754d98f312a30c3d9421f`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1273b4a7d40bb74302f237cb53eb0bcc54444ca383e15e5d33b3d060b5f98dd1`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2a3f703dc20a84ab20a7a95730da6579aac72a8c58bc0d24929d8617dc634c`  
		Last Modified: Wed, 11 May 2022 00:45:25 GMT  
		Size: 21.2 MB (21178440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66854ad6b8b792204d375a5f73dd9da3f91f4ef4bca9cce17479a18a62843ce8`  
		Last Modified: Wed, 11 May 2022 00:45:22 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
