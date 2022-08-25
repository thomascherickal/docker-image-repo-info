## `docker:20-dind-rootless`

```console
$ docker pull docker@sha256:99f93651781013800c23d17d050c3fec5a35b4984cb3cca3f3a51896f918b25b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:20-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:7ccff4077962658efd875c1a60ffeb93f1cf89f3d8b19c59489845890ffc3cee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.5 MB (122490843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfc77595689c5335f8abfb97f13cb018f288b721b77bea9cdc68df296e2cbb5b`
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
# Tue, 09 Aug 2022 18:21:25 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 09 Aug 2022 18:21:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 19 Aug 2022 00:19:59 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Fri, 19 Aug 2022 00:20:03 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 24 Aug 2022 23:17:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.10.1
# Wed, 24 Aug 2022 23:17:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-x86_64'; 			sha256='dfe2e3f134cc053e020891a11c23a0923eb49ee35556ec40b37d098eaa5a55f6'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-armv6'; 			sha256='8f9e1ccf35763b292443112795418b3ec9e8df46f8d78ca2c92d44645a90b88f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-armv7'; 			sha256='4a1bd3d72ff2d21248f5e1a32cdabc81aca9d613ce0eee661ac3cb6815db1258'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-aarch64'; 			sha256='2598b299693d3ef6087a8faa02e91e29bc2f4515347a0cf4c9ea18967584f153'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-ppc64le'; 			sha256='4866a6df1bc35eda103b0d32b357e2da4aae0b4eff96dd19ea4c1d6ddbc43e9f'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-riscv64'; 			sha256='8211dc32f228ac6d8685c2d07f579654771af3e792ebc6cc8a212536229630c3'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-s390x'; 			sha256='56b70071f7ab4acf7387cb3ce8492ec084650b435a2f483d355931bfa5536496'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 24 Aug 2022 23:17:44 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 24 Aug 2022 23:17:44 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 24 Aug 2022 23:17:44 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 24 Aug 2022 23:17:45 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 24 Aug 2022 23:17:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 23:17:45 GMT
CMD ["sh"]
# Wed, 24 Aug 2022 23:17:51 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Wed, 24 Aug 2022 23:17:52 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Wed, 24 Aug 2022 23:17:56 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Wed, 24 Aug 2022 23:17:56 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Wed, 24 Aug 2022 23:17:57 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Wed, 24 Aug 2022 23:17:57 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Wed, 24 Aug 2022 23:17:57 GMT
VOLUME [/var/lib/docker]
# Wed, 24 Aug 2022 23:17:57 GMT
EXPOSE 2375 2376
# Wed, 24 Aug 2022 23:17:57 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Wed, 24 Aug 2022 23:17:57 GMT
CMD []
# Wed, 24 Aug 2022 23:18:02 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Wed, 24 Aug 2022 23:18:02 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Wed, 24 Aug 2022 23:18:03 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Wed, 24 Aug 2022 23:18:04 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Wed, 24 Aug 2022 23:18:05 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Wed, 24 Aug 2022 23:18:05 GMT
VOLUME [/home/rootless/.local/share/docker]
# Wed, 24 Aug 2022 23:18:05 GMT
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
	-	`sha256:e001120e1cd4a7ea1ec2535b3ff388987a6bf3f3bd1568ba33de8157170276df`  
		Last Modified: Tue, 09 Aug 2022 18:24:12 GMT  
		Size: 13.7 MB (13668392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3ada922ff1d635680390f511fa096205beea3f4dc80a7fd4774133e9a572a7`  
		Last Modified: Fri, 19 Aug 2022 00:22:45 GMT  
		Size: 15.2 MB (15204102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145c17e0135eeca4e3fadf84680735cb7f810cc5cf01cfc143b191c1b637ef81`  
		Last Modified: Wed, 24 Aug 2022 23:20:17 GMT  
		Size: 9.4 MB (9351241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5eb6ef0bbbe94a8a957afb7d5832d7fe41c4f94e6fc884b52b68fc0c0a04c3`  
		Last Modified: Wed, 24 Aug 2022 23:20:15 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00ffea85b5c1b1b52801d09c10c6cffa1c28c21dc180fbcd089592e9c6131d3`  
		Last Modified: Wed, 24 Aug 2022 23:20:15 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:113b1213dc52b092b87de1089cb15b8adc29f96a8fb9387e925ceea9fa86be6e`  
		Last Modified: Wed, 24 Aug 2022 23:20:15 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f543a97eff74258cfa0bc9ce89e2fc84b6ddbd9fbe9cc3b215600f1acd3b306d`  
		Last Modified: Wed, 24 Aug 2022 23:20:48 GMT  
		Size: 6.9 MB (6863658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc80a42a6100ada105aefa979a4a6e1e0cf126c60c33118c1f0ba65f8bdd3e2`  
		Last Modified: Wed, 24 Aug 2022 23:20:47 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30add30b85c757eb1e889d4cb4edfef01f58261801e0052e8e60bf84cba631d`  
		Last Modified: Wed, 24 Aug 2022 23:20:56 GMT  
		Size: 51.8 MB (51847193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480bb92d7e2b89cdfa8c40753cd50df484a74e2027fbdd6261fa95631c799559`  
		Last Modified: Wed, 24 Aug 2022 23:20:47 GMT  
		Size: 962.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a7e85779826e36589da5b3ef62aa31bee5097f9fc49c57a3102f636f91f191`  
		Last Modified: Wed, 24 Aug 2022 23:20:47 GMT  
		Size: 2.8 KB (2755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b8eb8df22d6429f2391a80dd7c8f256d443dbf9e66cc8f0c67e58518843e6f`  
		Last Modified: Wed, 24 Aug 2022 23:21:15 GMT  
		Size: 1.4 MB (1358653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9e4e5f47a9ce9e7362830b2a8ee65b45e4f8cde48490e383d1b45f3fe6f0ef`  
		Last Modified: Wed, 24 Aug 2022 23:21:15 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e621f0ff948229dae96455dd29ff8b7c16d66cb3e49491ee94fb38dc5881b3d`  
		Last Modified: Wed, 24 Aug 2022 23:21:15 GMT  
		Size: 1.3 KB (1347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe5db740055792bdcc4c5a924c87064bceb42980689501ad69a0046e4d0d02`  
		Last Modified: Wed, 24 Aug 2022 23:21:18 GMT  
		Size: 19.3 MB (19346867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4930164ed0d7217ff4b664c3cbb22cb91ab2d92730d08c531a63cc02f47b57b`  
		Last Modified: Wed, 24 Aug 2022 23:21:15 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:59f980d12a75003922c41e8fa7d836791afc73ea8d410529419d183d40a22b19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.4 MB (116398352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c85b57e4caa46c5da7297775a32510cf2f8aa4e1d574466d338734d5f670b65e`
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
# Tue, 09 Aug 2022 18:25:59 GMT
ENV DOCKER_VERSION=20.10.17
# Tue, 09 Aug 2022 18:26:06 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 19 Aug 2022 02:46:39 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Fri, 19 Aug 2022 02:46:41 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 19 Aug 2022 02:46:42 GMT
ENV DOCKER_COMPOSE_VERSION=2.9.0
# Fri, 19 Aug 2022 02:46:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-x86_64'; 			sha256='3be9ce88ecba41b734e3fc8e59a9b11531133761414a78827d1615aadb5ef1f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-armv6'; 			sha256='2ea0f36350f81ae66db2b8c12104de6ed974a328557a4967857ee6e8df4b8f26'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-armv7'; 			sha256='658db542e40c8063cdafc23f650493bedc10b41b6d6fb581b7866bfeb5ffb0ba'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-aarch64'; 			sha256='6d227b060b2bc3dc5f315a07ae4f647f042755691e2da905b1a21e60a8ae3ddf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-ppc64le'; 			sha256='101ea490283f3c862e9bb4e7ef2a3fb38393cf2139f2b78e7a7423c91ad0c1fa'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-s390x'; 			sha256='0826c101e1d1a070e8ab8d7649c0da3cb9e6ecf1e717c545188243be6e676d00'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 19 Aug 2022 02:46:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 19 Aug 2022 02:46:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 19 Aug 2022 02:46:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 19 Aug 2022 02:46:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 19 Aug 2022 02:46:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 02:46:49 GMT
CMD ["sh"]
# Fri, 19 Aug 2022 02:47:00 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi
# Fri, 19 Aug 2022 02:47:01 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid
# Fri, 19 Aug 2022 02:47:07 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-20.10.17.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-20.10.17.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version
# Fri, 19 Aug 2022 02:47:08 GMT
ENV DIND_COMMIT=42b1175eda071c0e9121e1d64345928384a93df1
# Fri, 19 Aug 2022 02:47:09 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind
# Fri, 19 Aug 2022 02:47:11 GMT
COPY file:45c7926c5d79023b457ad24274c893b1fc21f241bed46421dc901b8237045f17 in /usr/local/bin/ 
# Fri, 19 Aug 2022 02:47:11 GMT
VOLUME [/var/lib/docker]
# Fri, 19 Aug 2022 02:47:12 GMT
EXPOSE 2375 2376
# Fri, 19 Aug 2022 02:47:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Fri, 19 Aug 2022 02:47:14 GMT
CMD []
# Fri, 19 Aug 2022 02:47:22 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs
# Fri, 19 Aug 2022 02:47:23 GMT
RUN mkdir /run/user && chmod 1777 /run/user
# Fri, 19 Aug 2022 02:47:24 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid
# Fri, 19 Aug 2022 02:47:27 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-20.10.17.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-20.10.17.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version
# Fri, 19 Aug 2022 02:47:27 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker
# Fri, 19 Aug 2022 02:47:28 GMT
VOLUME [/home/rootless/.local/share/docker]
# Fri, 19 Aug 2022 02:47:29 GMT
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
	-	`sha256:596c126c4e7f951be440ca6dc23043be252de5144fad72341963255f4d1f60e1`  
		Last Modified: Tue, 09 Aug 2022 18:30:10 GMT  
		Size: 12.5 MB (12500816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe8becc8c0570807fac1996ee4346147c87042c21f1be006ff348008880d3d4`  
		Last Modified: Fri, 19 Aug 2022 02:50:38 GMT  
		Size: 13.8 MB (13764592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dca5527bf3fb8918e39e523aa168f1bab5d9b926b8302c93763d9156f8ecdea`  
		Last Modified: Fri, 19 Aug 2022 02:50:38 GMT  
		Size: 8.6 MB (8598409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6710481aa5e9c602ca476a9061d6e78c17ef0388c648efb60a2834d8a3fdfad7`  
		Last Modified: Fri, 19 Aug 2022 02:50:36 GMT  
		Size: 546.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19993a91c415f84a4ebdd716da60ffc4cc9096c53e430c52331dd38d6d88b1c6`  
		Last Modified: Fri, 19 Aug 2022 02:50:36 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fd4df8b90d9d74bf9c03774d5db0961f53700a6299eafe69ea841e564736a6`  
		Last Modified: Fri, 19 Aug 2022 02:50:36 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44ef34fa29d09df7c7ae5130ea306125de3efbe7aaceaa2bada198e5979692a`  
		Last Modified: Fri, 19 Aug 2022 02:51:16 GMT  
		Size: 6.7 MB (6736616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba0636b4dc55d85f1824147c7b18b44b3bb005eafbcff5c00053ba4341533cf6`  
		Last Modified: Fri, 19 Aug 2022 02:51:15 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:086d3bf4cf4ab773ec95b68b719cccea07000f9e41da4760f1eb09cec9196db6`  
		Last Modified: Fri, 19 Aug 2022 02:51:22 GMT  
		Size: 47.5 MB (47523610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814ef71da9cadbec7a5ba319531fe4582b894d67bdc4f316c4aa0e66223d29b`  
		Last Modified: Fri, 19 Aug 2022 02:51:15 GMT  
		Size: 956.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4769496d1ea8e03e98491eaff548ebfa0eaf45c1a16f8fc2a2b1ef41e3f51ca5`  
		Last Modified: Fri, 19 Aug 2022 02:51:15 GMT  
		Size: 2.7 KB (2748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad63a8ef4d9cf2b1666cb02caef6dd25ed3cb39acf472c2799280767ac737e6`  
		Last Modified: Fri, 19 Aug 2022 02:51:45 GMT  
		Size: 1.4 MB (1370596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2803f1e58b835ffb326e792d519a570da824bc9347e99b0e42d0823a9af9351`  
		Last Modified: Fri, 19 Aug 2022 02:51:45 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e0555f25aa3a74ffc9b7573baca598a42ffd95ac19aeec2b2882e71e39d3f9`  
		Last Modified: Fri, 19 Aug 2022 02:51:45 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977f8eea1066a3ffbaf6a2f966a927a8af19e4c953d544ca26895ce418c1cdec`  
		Last Modified: Fri, 19 Aug 2022 02:51:48 GMT  
		Size: 21.2 MB (21177071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb02597032181ce9b3da35b9e6134b4bd324b8d98efbb5e411c6aff01494213`  
		Last Modified: Fri, 19 Aug 2022 02:51:45 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
