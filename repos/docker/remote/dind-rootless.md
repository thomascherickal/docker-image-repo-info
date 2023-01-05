## `docker:dind-rootless`

```console
$ docker pull docker@sha256:46652bce87b7520f470e7c4a918c155e0235e858c9532f7dca47a69237b2de7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:bb58cd1dff9ed4079bba37a786e8dad0b02e810d4bd3a7f0850299eda71e0b72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.2 MB (130248795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5de1fa8087a4f8816d7d4d78231b98ffb2a69de764aa9d5ed2a6167826e27d8`
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
# Fri, 16 Dec 2022 23:19:56 GMT
ENV DOCKER_VERSION=20.10.22
# Fri, 16 Dec 2022 23:19:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.22.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.22.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.22.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.22.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 16 Dec 2022 23:19:59 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Fri, 16 Dec 2022 23:20:02 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Thu, 05 Jan 2023 21:21:49 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.0
# Thu, 05 Jan 2023 21:21:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-x86_64'; 			sha256='ba481d45be2b137a2a185abd05f61d6d7766dbedfa038f16e4705760767a206e'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-armv6'; 			sha256='0f46aea568f35decc22e1db6af76decaf1c36b9bb374610bc08c3b3618170f8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-armv7'; 			sha256='343b552c61d74446fc8e8ce7695f878cb2ad49f7fae98deb7fb76a37f24c251e'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-aarch64'; 			sha256='634e397090ca0e857a898d853ab08d7e2f226328b305026c143c68d6ce0686de'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-ppc64le'; 			sha256='236831ebb63ad30fe716bf22946c91e21b1277bff2785a8538e616168a0d93f1'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-riscv64'; 			sha256='365d9bf34ae7a2ad0dc028d13363c8c427db1300b1335834a4e06b7e4fa412af'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-s390x'; 			sha256='8072776b50f34d135f90c8118da60749435b2474afee3df96bbd9c95755f7a2f'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Thu, 05 Jan 2023 21:21:52 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 05 Jan 2023 21:21:52 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 05 Jan 2023 21:21:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 05 Jan 2023 21:21:53 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 05 Jan 2023 21:21:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Jan 2023 21:21:53 GMT
CMD ["sh"]
# Thu, 05 Jan 2023 21:21:58 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 05 Jan 2023 21:21:59 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 05 Jan 2023 21:22:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.22.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.22.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.22.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.22.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Thu, 05 Jan 2023 21:22:04 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Thu, 05 Jan 2023 21:22:04 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 05 Jan 2023 21:22:05 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 05 Jan 2023 21:22:05 GMT
VOLUME [/var/lib/docker]
# Thu, 05 Jan 2023 21:22:05 GMT
EXPOSE 2375 2376
# Thu, 05 Jan 2023 21:22:05 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 05 Jan 2023 21:22:05 GMT
CMD []
# Thu, 05 Jan 2023 21:22:09 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Thu, 05 Jan 2023 21:22:09 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 05 Jan 2023 21:22:10 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 05 Jan 2023 21:22:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.22.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.22.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 05 Jan 2023 21:22:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 05 Jan 2023 21:22:12 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 05 Jan 2023 21:22:13 GMT
USER rootless
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
	-	`sha256:08b41ddca615c02560ac2876c1f1a4f4f0c2fe3f8b091488146e1098c5a3eda4`  
		Last Modified: Fri, 16 Dec 2022 23:22:29 GMT  
		Size: 14.0 MB (13982924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de76f94013e41735f015f26d3c3df1af256e1fd761926325deaf30759c53494`  
		Last Modified: Fri, 16 Dec 2022 23:22:28 GMT  
		Size: 15.2 MB (15204113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e300e409a8eec7162a8676943a73b3d129627668357ef158f85947a66122251`  
		Last Modified: Thu, 05 Jan 2023 21:24:20 GMT  
		Size: 14.5 MB (14477427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7564aa83a2f2bd29071dfacfbb67290825ccdc246baf8c4e5483d419668070f`  
		Last Modified: Thu, 05 Jan 2023 21:24:17 GMT  
		Size: 551.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b771ef457284440567ed829304474bf81f2806a564c77b9398f1d6ee475101b`  
		Last Modified: Thu, 05 Jan 2023 21:24:18 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323fe0eabec356c8896653ec7f8ba3a99ad59f4683be47e2edd4d6cada58ca80`  
		Last Modified: Thu, 05 Jan 2023 21:24:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a9b1f00d8c71f36fbbc05d53145a6461b01f22d58bcdad2da2861ae8e657cc`  
		Last Modified: Thu, 05 Jan 2023 21:24:48 GMT  
		Size: 6.8 MB (6837950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cbb2c68dd211a3732940e6f91584a976dbd20befd6a5a1afb225294d9ba0c0`  
		Last Modified: Thu, 05 Jan 2023 21:24:47 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f9fa2e7fe7226a68bd8e0a9e69c083048dab820c2b0b6c61a4aa8d87c91b31`  
		Last Modified: Thu, 05 Jan 2023 21:24:55 GMT  
		Size: 53.0 MB (53017992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6240f6f8ff419159a31faea2c13d2526e74dec0db8090d6728f9ca67d1e201a2`  
		Last Modified: Thu, 05 Jan 2023 21:24:47 GMT  
		Size: 1.0 KB (1047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d439a12187dfebb34b9e65fe913b74899ceac59d4eff3f637d338a8a45fda0`  
		Last Modified: Thu, 05 Jan 2023 21:24:47 GMT  
		Size: 2.8 KB (2751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0cc2551629b74304692008bcd2fa71cf35e6673f3eb7f59270ff7b09622df3`  
		Last Modified: Thu, 05 Jan 2023 21:25:14 GMT  
		Size: 1.4 MB (1375674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43dfe46e513a3e115932e8f2124ea736c5232a1a6d015a0c3387a74fb143b253`  
		Last Modified: Thu, 05 Jan 2023 21:25:14 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a79397b7219d902438a6ecafeee6116590091866a1807f62c86483d40495c7`  
		Last Modified: Thu, 05 Jan 2023 21:25:14 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c4eec84e29c0b7368500506f51957cb533a6b180d13a6d6cd0ba5adf7c8374`  
		Last Modified: Thu, 05 Jan 2023 21:25:17 GMT  
		Size: 19.9 MB (19909191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49f5c83afef4bcda498b3682c8c838a62acfdb303b23a00b09156385b09ffa6`  
		Last Modified: Thu, 05 Jan 2023 21:25:14 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:63de3466afaf9468933b58f7ac58de9b627baa039df94fe59b1ea6316e3ecd4e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123839446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3aa8344b214010d89ba836807a8abef143f96ad2469860b8fd941cb42c513673`
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
# Sat, 17 Dec 2022 00:10:28 GMT
ENV DOCKER_VERSION=20.10.22
# Sat, 17 Dec 2022 00:10:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.22.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.22.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.22.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.22.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Sat, 17 Dec 2022 00:10:31 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Sat, 17 Dec 2022 00:10:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Thu, 05 Jan 2023 21:41:34 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.0
# Thu, 05 Jan 2023 21:41:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-x86_64'; 			sha256='ba481d45be2b137a2a185abd05f61d6d7766dbedfa038f16e4705760767a206e'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-armv6'; 			sha256='0f46aea568f35decc22e1db6af76decaf1c36b9bb374610bc08c3b3618170f8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-armv7'; 			sha256='343b552c61d74446fc8e8ce7695f878cb2ad49f7fae98deb7fb76a37f24c251e'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-aarch64'; 			sha256='634e397090ca0e857a898d853ab08d7e2f226328b305026c143c68d6ce0686de'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-ppc64le'; 			sha256='236831ebb63ad30fe716bf22946c91e21b1277bff2785a8538e616168a0d93f1'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-riscv64'; 			sha256='365d9bf34ae7a2ad0dc028d13363c8c427db1300b1335834a4e06b7e4fa412af'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.0/docker-compose-linux-s390x'; 			sha256='8072776b50f34d135f90c8118da60749435b2474afee3df96bbd9c95755f7a2f'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Thu, 05 Jan 2023 21:41:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 05 Jan 2023 21:41:36 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 05 Jan 2023 21:41:36 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 05 Jan 2023 21:41:36 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 05 Jan 2023 21:41:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 05 Jan 2023 21:41:37 GMT
CMD ["sh"]
# Thu, 05 Jan 2023 21:41:42 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Thu, 05 Jan 2023 21:41:42 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Thu, 05 Jan 2023 21:41:45 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.22.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.22.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.22.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.22.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Thu, 05 Jan 2023 21:41:46 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Thu, 05 Jan 2023 21:41:46 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Thu, 05 Jan 2023 21:41:46 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Thu, 05 Jan 2023 21:41:46 GMT
VOLUME [/var/lib/docker]
# Thu, 05 Jan 2023 21:41:46 GMT
EXPOSE 2375 2376
# Thu, 05 Jan 2023 21:41:46 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 05 Jan 2023 21:41:47 GMT
CMD []
# Thu, 05 Jan 2023 21:41:50 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Thu, 05 Jan 2023 21:41:50 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Thu, 05 Jan 2023 21:41:51 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Thu, 05 Jan 2023 21:41:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.22.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.22.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Thu, 05 Jan 2023 21:41:53 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Thu, 05 Jan 2023 21:41:53 GMT
VOLUME [/home/rootless/.local/share/docker]
# Thu, 05 Jan 2023 21:41:53 GMT
USER rootless
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
	-	`sha256:f9db874a82a64c48213d6d1ce2e45eb51359f913358fa4d785dd4a6d5219631c`  
		Last Modified: Sat, 17 Dec 2022 00:12:52 GMT  
		Size: 12.7 MB (12743372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16bcbc5124e189b1ab3f0affe49da5b5b8037788919a0816840b1270409f1a3c`  
		Last Modified: Sat, 17 Dec 2022 00:12:50 GMT  
		Size: 13.8 MB (13764588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b918a7e8bbe3d99fb2a974018d28246fb12375e855467b9f5c25b56631536a79`  
		Last Modified: Thu, 05 Jan 2023 21:43:54 GMT  
		Size: 13.1 MB (13069210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c823f32ed1b1e25192b03856736e19a71b0dfe848fd2865f64fba1e8668cf7f`  
		Last Modified: Thu, 05 Jan 2023 21:43:52 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023d601a201fdffb12d133e91992f6e1095b1c18215882bc21927ddd4ed2ff76`  
		Last Modified: Thu, 05 Jan 2023 21:43:52 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6e8232b2cb8b64e1fa903903eb5795acf7aa646ff0a107c3f3b276270f2136`  
		Last Modified: Thu, 05 Jan 2023 21:43:52 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87714f2821eb4b99ecad57cb6b67361446be03d58e115474820bf8573826d35f`  
		Last Modified: Thu, 05 Jan 2023 21:44:20 GMT  
		Size: 7.0 MB (6991066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725d5d0746f4e4c75ede69744e1d3648e369e13cd637c33abdaecd12db160148`  
		Last Modified: Thu, 05 Jan 2023 21:44:19 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa698fc20d4c72cdeb55fcad3a229ccf954678bddd85c62620b4427a6d1094b`  
		Last Modified: Thu, 05 Jan 2023 21:44:25 GMT  
		Size: 48.7 MB (48676605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46845023bbe2d30adaabd8ceee9f61cd49f9f045459f9ce9abfafb8a0f87ad41`  
		Last Modified: Thu, 05 Jan 2023 21:44:19 GMT  
		Size: 1.0 KB (1048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99bed76d1a5a851784d578f3f2c6c66409843f87ba1edd987099d86d0fdf9105`  
		Last Modified: Thu, 05 Jan 2023 21:44:19 GMT  
		Size: 2.8 KB (2755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba9b96b8403f9d366267b199576f2f7ff218951e140da6b3da8040f4227f29c`  
		Last Modified: Thu, 05 Jan 2023 21:44:42 GMT  
		Size: 1.4 MB (1401550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b44ec2e494bc5d6b333778ddfc5e637bbf5d5029555a32ef941441e9bc4803`  
		Last Modified: Thu, 05 Jan 2023 21:44:41 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aee6f96509c8c2f6263feecbd17678265a7c472564f8b950758a0838e28c2d8`  
		Last Modified: Thu, 05 Jan 2023 21:44:41 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5f72fd057b8c0d55cd3b33fd0c8507e20f53934450fb31051d752eda6376b0`  
		Last Modified: Thu, 05 Jan 2023 21:44:44 GMT  
		Size: 21.9 MB (21888448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acedf715b8db067abaca4113e583aef7ac84869916b2e6d76c9a398ee255db0`  
		Last Modified: Thu, 05 Jan 2023 21:44:41 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
