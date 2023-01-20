## `docker:dind`

```console
$ docker pull docker@sha256:03f2d563100b9776283de1e18f10a1f0b66d2fdc7918831bf8db1cda767d6b37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:a2b673f671ab5480f0fcb80e332180f28ccad642ff33b63ff7211fbfd0ae2d39
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109760223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d828bdfa17fe751c45151e332232fd397e42a69a0948f8c86d0d22ea169355a`
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
# Mon, 09 Jan 2023 21:13:35 GMT
ENV DOCKER_VERSION=20.10.22
# Mon, 09 Jan 2023 21:13:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.22.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.22.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.22.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.22.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 20 Jan 2023 01:20:06 GMT
ENV DOCKER_BUILDX_VERSION=0.10.0
# Fri, 20 Jan 2023 01:20:08 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-amd64'; 			sha256='f76047e43cd2526a870b9cf385effc7c9642c1a17d144559c43545525415867d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v6'; 			sha256='dc037b64e14388cbf5441d3b23a3f1ccd9a56a47007555ce681d89b70d411d31'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v7'; 			sha256='19b82ba259d83cc75b12bddb1cdc0712dd276f8763d0a65ded2048193973260b'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm64'; 			sha256='abf375431775d46139312591aa9471cdf6909d8a4e8392b73940ca136c34eb4d'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-ppc64le'; 			sha256='9850f6ad445d1014a156c33ac7f9074fffd3358db304ef5b4e4509355a4d9fb9'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-riscv64'; 			sha256='07529564e5b2f1f6e33fbf947700f9118a727dde2d8486c3e2115bc4fb42d86a'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-s390x'; 			sha256='871b4a746765334a1a0b56700525d5ef7f83adcafbb193734e238c8ac102eccc'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 20 Jan 2023 01:20:08 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Fri, 20 Jan 2023 01:20:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 20 Jan 2023 01:20:11 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 20 Jan 2023 01:20:11 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 20 Jan 2023 01:20:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 20 Jan 2023 01:20:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 20 Jan 2023 01:20:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Jan 2023 01:20:12 GMT
CMD ["sh"]
# Fri, 20 Jan 2023 01:20:18 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 20 Jan 2023 01:20:18 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 20 Jan 2023 01:20:23 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.22.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.22.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.22.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.22.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 20 Jan 2023 01:20:23 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 20 Jan 2023 01:20:24 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 20 Jan 2023 01:20:24 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 20 Jan 2023 01:20:24 GMT
VOLUME [/var/lib/docker]
# Fri, 20 Jan 2023 01:20:24 GMT
EXPOSE 2375 2376
# Fri, 20 Jan 2023 01:20:24 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 20 Jan 2023 01:20:24 GMT
CMD []
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
	-	`sha256:0ba836ede3c52b4e50be778327aae06076bede29bc2ccd9f317f54c2268167f9`  
		Last Modified: Mon, 09 Jan 2023 21:16:13 GMT  
		Size: 14.0 MB (13982943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43effd36e4809575b4afdbd0092aa8894be7952c8ac021a5fbf04032f30b752`  
		Last Modified: Fri, 20 Jan 2023 01:22:39 GMT  
		Size: 16.0 MB (15988693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dae86dd7677992032fff70c782b41da11936b7e70b3f842845ebfa6cdd3ac62`  
		Last Modified: Fri, 20 Jan 2023 01:22:39 GMT  
		Size: 14.5 MB (14490919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a864069484effd9eb21e3328b3de0bea8e2bd56dbeba6cfd8da4a7f864dd2645`  
		Last Modified: Fri, 20 Jan 2023 01:22:36 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5bbb95ca560840b64b9cce12d6c8eef06efe74ffd8c0a07fec77387a747d1c`  
		Last Modified: Fri, 20 Jan 2023 01:22:36 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb5fc05f46f58df95b79ce722692de5e9710d159decb3409afb269b3c4c9fc6`  
		Last Modified: Fri, 20 Jan 2023 01:22:36 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196e7d5eb78a9137836998d1c3e88b871bfeb90830aa75e95084418e303e0c76`  
		Last Modified: Fri, 20 Jan 2023 01:23:06 GMT  
		Size: 6.8 MB (6837899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39a243097f562ce0693cfb87118b8089a817ffcf46521865f3eac5552748e8e`  
		Last Modified: Fri, 20 Jan 2023 01:23:04 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d72ffcb08653bc4e43414e5984456d4cc94656aea3c5c51f7f21af41d4b037`  
		Last Modified: Fri, 20 Jan 2023 01:23:13 GMT  
		Size: 53.0 MB (53018057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8986d996ca863d26156ec91d0a0dfdb8bfdb639dce49a8211b505928a83085`  
		Last Modified: Fri, 20 Jan 2023 01:23:05 GMT  
		Size: 1.0 KB (1040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e94533688370d613c689d1d77869416314135928d6eaa299afcedec34a5181e5`  
		Last Modified: Fri, 20 Jan 2023 01:23:05 GMT  
		Size: 2.7 KB (2742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:59a3b27f3ad9f7526b78be474ea21a30931ac0664cb4c4e6c302cbfe36d15a8d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101225500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80dbcb0b93a21ee8ab8cdc09fbe60a7021dcffed1bb7f380e492e669602f534e`
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
# Mon, 09 Jan 2023 17:29:40 GMT
ENV DOCKER_VERSION=20.10.22
# Mon, 09 Jan 2023 17:29:42 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.22.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.22.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.22.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.22.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 20 Jan 2023 00:40:04 GMT
ENV DOCKER_BUILDX_VERSION=0.10.0
# Fri, 20 Jan 2023 00:40:06 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-amd64'; 			sha256='f76047e43cd2526a870b9cf385effc7c9642c1a17d144559c43545525415867d'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v6'; 			sha256='dc037b64e14388cbf5441d3b23a3f1ccd9a56a47007555ce681d89b70d411d31'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm-v7'; 			sha256='19b82ba259d83cc75b12bddb1cdc0712dd276f8763d0a65ded2048193973260b'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-arm64'; 			sha256='abf375431775d46139312591aa9471cdf6909d8a4e8392b73940ca136c34eb4d'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-ppc64le'; 			sha256='9850f6ad445d1014a156c33ac7f9074fffd3358db304ef5b4e4509355a4d9fb9'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-riscv64'; 			sha256='07529564e5b2f1f6e33fbf947700f9118a727dde2d8486c3e2115bc4fb42d86a'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.10.0/buildx-v0.10.0.linux-s390x'; 			sha256='871b4a746765334a1a0b56700525d5ef7f83adcafbb193734e238c8ac102eccc'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 20 Jan 2023 00:40:06 GMT
ENV DOCKER_COMPOSE_VERSION=2.15.1
# Fri, 20 Jan 2023 00:40:08 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-x86_64'; 			sha256='bcfd9ea51dee4c19dccdfaeef0e7956ef68bf14f3d175933742061a7271ef0f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv6'; 			sha256='a8934600100af88f535eb50b45c7d8d2ac37835221803ba2910e0b167b3af22e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-armv7'; 			sha256='e5b03ac1258ad4243af0ac4afcb1c6cc8c9956b2483a50309cdb38cdb8387e37'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-aarch64'; 			sha256='14d31297794868520cb2e61b543bb1c821aaa484af22b397904314ae8227f6a2'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-ppc64le'; 			sha256='bdada874a26d382b20ced7c170707a1ebcf9f20d7d6f394b962076968473ca9c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-riscv64'; 			sha256='9cc1b9c8de313a1e43b8f3dcca47c29eeb87af3de24c67448c463bf882166430'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.15.1/docker-compose-linux-s390x'; 			sha256='cf311824af115d0bece5d5d60a73464912dad07cdd00fdaa469dabbcad60f289'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 20 Jan 2023 00:40:08 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 20 Jan 2023 00:40:09 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 20 Jan 2023 00:40:09 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 20 Jan 2023 00:40:09 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 20 Jan 2023 00:40:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Jan 2023 00:40:09 GMT
CMD ["sh"]
# Fri, 20 Jan 2023 00:40:14 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 20 Jan 2023 00:40:15 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 20 Jan 2023 00:40:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.22.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.22.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.22.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.22.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 20 Jan 2023 00:40:19 GMT
ENV DIND_COMMIT=1f32e3c95d72a29b3eaacba156ed675dba976cb5
# Fri, 20 Jan 2023 00:40:19 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 20 Jan 2023 00:40:19 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 20 Jan 2023 00:40:19 GMT
VOLUME [/var/lib/docker]
# Fri, 20 Jan 2023 00:40:19 GMT
EXPOSE 2375 2376
# Fri, 20 Jan 2023 00:40:20 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 20 Jan 2023 00:40:20 GMT
CMD []
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
	-	`sha256:3e5567070d966674de4065d4af430ca10957d42583f6fb752fa8a33d1cbaafc1`  
		Last Modified: Mon, 09 Jan 2023 17:32:10 GMT  
		Size: 12.7 MB (12743371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6f3c97d07e38522af5329f629558b34f9e9a68b1ef94246f7a3bcd870be1e9`  
		Last Modified: Fri, 20 Jan 2023 00:42:32 GMT  
		Size: 14.4 MB (14430979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a4a674f6e98114f79bdc8151c65d9c6b93e207aab226fefee0abd2392db20b`  
		Last Modified: Fri, 20 Jan 2023 00:42:32 GMT  
		Size: 13.1 MB (13080442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e7693e8166197c5e8b265d4d1d5f84590269e5c2656e49b687042ac7e8e75f`  
		Last Modified: Fri, 20 Jan 2023 00:42:30 GMT  
		Size: 549.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438407297ba78c2317f0ad1b4e113891ac121c5cc8cd5a9c89126c0e469a3d46`  
		Last Modified: Fri, 20 Jan 2023 00:42:30 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6640ddd118acdbdc238024236fbc83f7b2399ff41b8788289135f90d7448ec91`  
		Last Modified: Fri, 20 Jan 2023 00:42:30 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f580a0c8689696ea520f59a9365be3122c3aecc2569bc653159018d8c4002f`  
		Last Modified: Fri, 20 Jan 2023 00:42:58 GMT  
		Size: 7.0 MB (6991111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519b44710f9d79d8650fe6cab9eadf83f8b621f45d1fedf2cd191cb171199fff`  
		Last Modified: Fri, 20 Jan 2023 00:42:57 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e788afee8640d90f0af6dd8a5d9582a8273e15fbcd0e337f0506b74cd89d2bf7`  
		Last Modified: Fri, 20 Jan 2023 00:43:03 GMT  
		Size: 48.7 MB (48676625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa409900e3820d4b498446fc0d6a135e5dc1156362116dbfc31e7497906b282d`  
		Last Modified: Fri, 20 Jan 2023 00:42:57 GMT  
		Size: 1.0 KB (1043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dbdccccf4101c3cef91bdd015bb01ebadccee46b4e4d08f98fec5094dcb1d8d`  
		Last Modified: Fri, 20 Jan 2023 00:42:57 GMT  
		Size: 2.7 KB (2743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
