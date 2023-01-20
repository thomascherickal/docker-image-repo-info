## `docker:rc-dind-rootless`

```console
$ docker pull docker@sha256:b52442a232a0ed8604954bfc9365d43dff03d0edf17b0e45024eae438ab4df21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:b887c14d9f6f34d0a740093cf8ac7623f6ea5f7a8d868e0b1a2ed85429d767a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.1 MB (132123820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ae4ff0bb57e90d6b218f43f79564021ec3cb71d0a6da882d4a0a90118095fd8`
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
# Fri, 20 Jan 2023 01:19:25 GMT
ENV DOCKER_VERSION=23.0.0-rc.2
# Fri, 20 Jan 2023 01:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-23.0.0-rc.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-23.0.0-rc.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-23.0.0-rc.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-23.0.0-rc.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 20 Jan 2023 01:19:31 GMT
ENV DOCKER_BUILDX_VERSION=0.10.0
# Fri, 20 Jan 2023 01:19:33 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-amd64'; 			sha256='f76047e43cd2526a870b9cf385effc7c9642c1a17d144559c43545525415867d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v6'; 			sha256='dc037b64e14388cbf5441d3b23a3f1ccd9a56a47007555ce681d89b70d411d31'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v7'; 			sha256='19b82ba259d83cc75b12bddb1cdc0712dd276f8763d0a65ded2048193973260b'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm64'; 			sha256='abf375431775d46139312591aa9471cdf6909d8a4e8392b73940ca136c34eb4d'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-ppc64le'; 			sha256='9850f6ad445d1014a156c33ac7f9074fffd3358db304ef5b4e4509355a4d9fb9'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-riscv64'; 			sha256='07529564e5b2f1f6e33fbf947700f9118a727dde2d8486c3e2115bc4fb42d86a'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-s390x'; 			sha256='871b4a746765334a1a0b56700525d5ef7f83adcafbb193734e238c8ac102eccc'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 20 Jan 2023 01:19:34 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Fri, 20 Jan 2023 01:19:36 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 20 Jan 2023 01:19:36 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 20 Jan 2023 01:19:37 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 20 Jan 2023 01:19:37 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 20 Jan 2023 01:19:37 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 20 Jan 2023 01:19:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Jan 2023 01:19:37 GMT
CMD ["sh"]
# Fri, 20 Jan 2023 01:19:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 20 Jan 2023 01:19:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 20 Jan 2023 01:19:49 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-23.0.0-rc.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-23.0.0-rc.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-23.0.0-rc.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-23.0.0-rc.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 20 Jan 2023 01:19:50 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 20 Jan 2023 01:19:51 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 20 Jan 2023 01:19:51 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 20 Jan 2023 01:19:51 GMT
VOLUME [/var/lib/docker]
# Fri, 20 Jan 2023 01:19:51 GMT
EXPOSE 2375 2376
# Fri, 20 Jan 2023 01:19:51 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 20 Jan 2023 01:19:51 GMT
CMD []
# Fri, 20 Jan 2023 01:19:55 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 20 Jan 2023 01:19:55 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 20 Jan 2023 01:19:56 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 20 Jan 2023 01:19:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-23.0.0-rc.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-23.0.0-rc.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 20 Jan 2023 01:19:59 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 20 Jan 2023 01:19:59 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 20 Jan 2023 01:19:59 GMT
USER rootless
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
	-	`sha256:b5645e17e8e772f0f5e8fb51320c291e57e60777930f33fb5ec288a7aafafebf`  
		Last Modified: Fri, 20 Jan 2023 01:21:23 GMT  
		Size: 16.2 MB (16210492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786cbea4ef3a6d7445da857bb0179da13092d722ad3bc1d1cfc9fba5643c3c84`  
		Last Modified: Fri, 20 Jan 2023 01:21:22 GMT  
		Size: 16.0 MB (15988681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f87cdbce7976e9b98233450652b68ef8593367ab2aeebc6f8dc3647c9b4a3f3`  
		Last Modified: Fri, 20 Jan 2023 01:21:22 GMT  
		Size: 14.5 MB (14490924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec84e687e49dbe093639faf81ca33b8662f366d37e9b103602202fe7abcf3f2c`  
		Last Modified: Fri, 20 Jan 2023 01:21:19 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b270ffbe8b5bc2423e115882f87b26ef4c75aba7e80668927aead08227029e`  
		Last Modified: Fri, 20 Jan 2023 01:21:19 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803439012a9eb382b563b9f840079fe0b9d292fd874edab986b7cbde6671dfb8`  
		Last Modified: Fri, 20 Jan 2023 01:21:19 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da045d0684000d39cc20ec578970de4734217424220956c046cf9d68fdfc11c`  
		Last Modified: Fri, 20 Jan 2023 01:21:37 GMT  
		Size: 6.8 MB (6837905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d20fbd029417362ecc240151600f3d744e50df5c4d0d58e5f1aaf7eec3aff`  
		Last Modified: Fri, 20 Jan 2023 01:21:36 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b33441ca16c44936aa1d083086734b282a89d0e47d20333492ed1afe1219327`  
		Last Modified: Fri, 20 Jan 2023 01:21:44 GMT  
		Size: 51.5 MB (51450816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:042a83f8c9b9d08d9f21b2554d6467fdbf7c8e11c7704509a573252aff128dcf`  
		Last Modified: Fri, 20 Jan 2023 01:21:37 GMT  
		Size: 1.0 KB (1042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c715357050307b220838ffa6be0e70abbe18334698cbc27f1bcb3b4e3d6d3c9`  
		Last Modified: Fri, 20 Jan 2023 01:21:36 GMT  
		Size: 2.7 KB (2746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ab814aaaea59cd0ffa76260e6db7676a992e5b336478ad7068d8d0618b88cb`  
		Last Modified: Fri, 20 Jan 2023 01:22:10 GMT  
		Size: 1.4 MB (1375656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950deb02e8361d436bb231a5720a812814e8e4717a983b1dbc75712767449c64`  
		Last Modified: Fri, 20 Jan 2023 01:22:10 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26a34e64f95b662b2acd4187ff424fc163703f0aecf1a05b5f552ee69afa8f4`  
		Last Modified: Fri, 20 Jan 2023 01:22:10 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdd8556af975d8f2b34916d692bdff0cd5b98762889d3b5f05e53dbc92e5b1c`  
		Last Modified: Fri, 20 Jan 2023 01:22:13 GMT  
		Size: 20.3 MB (20325909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89386c7c3b1ad4bcb99275f0511f3288224184484186c9c035b45ca1bb49447b`  
		Last Modified: Fri, 20 Jan 2023 01:22:10 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:46227b37b944e4faacef8f2e0b89258d2178047322bcb425551c14e59766c2eb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125624634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24eb0b89028f158d2a1cc222522d269e6db4ccb77220d9f6837a31e0a9e9689c`
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
# Fri, 20 Jan 2023 00:39:23 GMT
ENV DOCKER_VERSION=23.0.0-rc.2
# Fri, 20 Jan 2023 00:39:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-23.0.0-rc.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-23.0.0-rc.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-23.0.0-rc.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-23.0.0-rc.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 20 Jan 2023 00:39:27 GMT
ENV DOCKER_BUILDX_VERSION=0.10.0
# Fri, 20 Jan 2023 00:39:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-amd64'; 			sha256='f76047e43cd2526a870b9cf385effc7c9642c1a17d144559c43545525415867d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v6'; 			sha256='dc037b64e14388cbf5441d3b23a3f1ccd9a56a47007555ce681d89b70d411d31'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v7'; 			sha256='19b82ba259d83cc75b12bddb1cdc0712dd276f8763d0a65ded2048193973260b'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm64'; 			sha256='abf375431775d46139312591aa9471cdf6909d8a4e8392b73940ca136c34eb4d'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-ppc64le'; 			sha256='9850f6ad445d1014a156c33ac7f9074fffd3358db304ef5b4e4509355a4d9fb9'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-riscv64'; 			sha256='07529564e5b2f1f6e33fbf947700f9118a727dde2d8486c3e2115bc4fb42d86a'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-s390x'; 			sha256='871b4a746765334a1a0b56700525d5ef7f83adcafbb193734e238c8ac102eccc'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 20 Jan 2023 00:39:34 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Fri, 20 Jan 2023 00:39:37 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 20 Jan 2023 00:39:37 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 20 Jan 2023 00:39:38 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 20 Jan 2023 00:39:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 20 Jan 2023 00:39:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 20 Jan 2023 00:39:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Jan 2023 00:39:38 GMT
CMD ["sh"]
# Fri, 20 Jan 2023 00:39:44 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 20 Jan 2023 00:39:45 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 20 Jan 2023 00:39:48 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-23.0.0-rc.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-23.0.0-rc.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-23.0.0-rc.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-23.0.0-rc.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 20 Jan 2023 00:39:49 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 20 Jan 2023 00:39:49 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 20 Jan 2023 00:39:49 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 20 Jan 2023 00:39:50 GMT
VOLUME [/var/lib/docker]
# Fri, 20 Jan 2023 00:39:50 GMT
EXPOSE 2375 2376
# Fri, 20 Jan 2023 00:39:50 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 20 Jan 2023 00:39:50 GMT
CMD []
# Fri, 20 Jan 2023 00:39:54 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 20 Jan 2023 00:39:55 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 20 Jan 2023 00:39:55 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 20 Jan 2023 00:39:58 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-23.0.0-rc.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-23.0.0-rc.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 20 Jan 2023 00:39:58 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 20 Jan 2023 00:39:58 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 20 Jan 2023 00:39:58 GMT
USER rootless
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
	-	`sha256:b04448b5ab866ce58e9045d830cb22adf7a6c9df14a32becf446504b2d08771b`  
		Last Modified: Fri, 20 Jan 2023 00:41:21 GMT  
		Size: 15.3 MB (15286237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58febb98d86a1f75bb161b40593029154b51a95f04498668a9302916e4cb8b0b`  
		Last Modified: Fri, 20 Jan 2023 00:41:20 GMT  
		Size: 14.4 MB (14430978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849c5d6785d0ecaa4727a5add37695e51832be46b4c225d70414e286c4cb9493`  
		Last Modified: Fri, 20 Jan 2023 00:41:20 GMT  
		Size: 13.1 MB (13080438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc652dd57da3d14699c3eecc24dc127767b41edd435e6bc6747d1234839d8c5a`  
		Last Modified: Fri, 20 Jan 2023 00:41:19 GMT  
		Size: 550.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a858be319c6c1582f5b54f5e0921db2c4b5161065531f18e273131445c24fb66`  
		Last Modified: Fri, 20 Jan 2023 00:41:18 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d880c535d51decbb91e1f37749562e75643b62c3a60e6161c725b64def51fd8`  
		Last Modified: Fri, 20 Jan 2023 00:41:18 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e43c39ad478ab9bc5e8aab96ecfb27dbabcd995dc2fef47b459aaeaac1a927e`  
		Last Modified: Fri, 20 Jan 2023 00:41:36 GMT  
		Size: 7.0 MB (6991132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176d3a312663d33ec37832d6d93059f3c7bc193a667d295ac72b02de6344a06f`  
		Last Modified: Fri, 20 Jan 2023 00:41:34 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111c7af3af42ba5327975c0da39b615385791eb30cf4cd163c62de02451e2682`  
		Last Modified: Fri, 20 Jan 2023 00:41:40 GMT  
		Size: 46.9 MB (46897347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a31d0aa096257021d7eccc18249ebf7780c03e908f89e77d2c54ab6bee89cd`  
		Last Modified: Fri, 20 Jan 2023 00:41:34 GMT  
		Size: 1.0 KB (1044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1474c4e70bc86ed8ec20a98a9cde90e49089955e9082a1799492a9833ad36c`  
		Last Modified: Fri, 20 Jan 2023 00:41:34 GMT  
		Size: 2.7 KB (2744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbad7960ef48f4206bde84eca9c6cf332f446ad8193609b6fe448b5155865fad`  
		Last Modified: Fri, 20 Jan 2023 00:42:05 GMT  
		Size: 1.4 MB (1401563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e962133f836065978b06b60f2212b6216633a4bc7a44c530d5664a4b616dbbd8`  
		Last Modified: Fri, 20 Jan 2023 00:42:05 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfede1bb1fe5c06dc005ad3dbc191662463f13b01640401471795e908a6455c`  
		Last Modified: Fri, 20 Jan 2023 00:42:05 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf8b3e25e1c44cbf05c6e29a3387a6e18b2c0ba9051d6891f06ada94aa7bdfc`  
		Last Modified: Fri, 20 Jan 2023 00:42:08 GMT  
		Size: 22.2 MB (22232244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a11bf74a0366f08f60d2ad82dd0545188202758be859331a10a72ba284bfae`  
		Last Modified: Fri, 20 Jan 2023 00:42:05 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
