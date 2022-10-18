## `docker:rc-cli`

```console
$ docker pull docker@sha256:10fd65aa0df0ec3c1b71f21ef5190d9f4cab68e9b513e11587df64f2e16c83db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-cli` - linux; amd64

```console
$ docker pull docker@sha256:bf99671394d847b44da0a2e94951d8cd2ef160fba8f3f488236b43aabb30c84c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43234067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54733b3f038d80a78b480a916016e49580c06f9354e6dad390c1261caf8bf328`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:19:24 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 06 Oct 2022 20:19:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:19:24 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Thu, 06 Oct 2022 20:19:28 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Thu, 06 Oct 2022 20:19:28 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Thu, 06 Oct 2022 20:19:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Tue, 18 Oct 2022 21:19:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.12.0
# Tue, 18 Oct 2022 21:19:34 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-x86_64'; 			sha256='2054f3a24cb6814b390bd22c95fa37af7675831e37776bb1473a29a912d48b4b'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-armv6'; 			sha256='81e1d70b82873145faf802d3c8c46d5c35373d3665586d263ecf28a9df25a308'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-armv7'; 			sha256='63f94bcea4f2b6e9abeba90ac81620b1b0cab116b40890f0a68619fd26e3eb3f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-aarch64'; 			sha256='3708946bf5d78db23502e95a7ef1f716c16060e098b28acbe604a38b3ab3a51a'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-ppc64le'; 			sha256='263c827f0222dee0738a38ada22d5a4776d4a46874f34c114d7975e24e8c7bbe'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-riscv64'; 			sha256='65c7c1cda3ab6de7fb8f9b12d67d63b94a1355cc014e4ce5c7504809cb8db2e8'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-s390x'; 			sha256='b8087688da06c3c95e0cb518880053783951b47e3757be24788e34d5617128e4'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 18 Oct 2022 21:19:34 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 18 Oct 2022 21:19:34 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 18 Oct 2022 21:19:35 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 18 Oct 2022 21:19:35 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 18 Oct 2022 21:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Oct 2022 21:19:35 GMT
CMD ["sh"]
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
	-	`sha256:b71bbd92cafae45d57d7d9c872764c3a3422ad5f461234db0e28c7189364fa07`  
		Last Modified: Thu, 06 Oct 2022 20:21:29 GMT  
		Size: 8.7 MB (8706446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cb11473cfe767f03d6b5a80d0ed644adbdd3dc57dba9a0fa887785607dd9b2`  
		Last Modified: Thu, 06 Oct 2022 20:21:25 GMT  
		Size: 15.2 MB (15204105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3644c6eeb00850bbf74917a0e09ecf85505fb4d2f2322791d87073ae023478a0`  
		Last Modified: Tue, 18 Oct 2022 21:21:21 GMT  
		Size: 14.5 MB (14479516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12a2af0a6cbd461dc287c9436d5636ac8fef243499106329958511f0bc073be`  
		Last Modified: Tue, 18 Oct 2022 21:21:18 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ceb7292918b5774d28813c1b8e99357e1cd9fecaa6fc4e2d506ed863cf7f424`  
		Last Modified: Tue, 18 Oct 2022 21:21:18 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f82e98831b33138f9b0e266151a07cf24f6881e9357e86fca6e675c2b46291d`  
		Last Modified: Tue, 18 Oct 2022 21:21:20 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:5494003836ac27ccdb941f15225f1c8417c7d05e6feea5088bb61255959cbf4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39602917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad9b5671b3d57d2411d92129e4079e1699fdbe65536596790e789dee51ab6889`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:57:19 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Thu, 06 Oct 2022 19:57:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:57:21 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Thu, 06 Oct 2022 19:57:26 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Thu, 06 Oct 2022 19:57:27 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Thu, 06 Oct 2022 19:57:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Tue, 18 Oct 2022 21:39:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.12.0
# Tue, 18 Oct 2022 21:39:44 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-x86_64'; 			sha256='2054f3a24cb6814b390bd22c95fa37af7675831e37776bb1473a29a912d48b4b'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-armv6'; 			sha256='81e1d70b82873145faf802d3c8c46d5c35373d3665586d263ecf28a9df25a308'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-armv7'; 			sha256='63f94bcea4f2b6e9abeba90ac81620b1b0cab116b40890f0a68619fd26e3eb3f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-aarch64'; 			sha256='3708946bf5d78db23502e95a7ef1f716c16060e098b28acbe604a38b3ab3a51a'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-ppc64le'; 			sha256='263c827f0222dee0738a38ada22d5a4776d4a46874f34c114d7975e24e8c7bbe'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-riscv64'; 			sha256='65c7c1cda3ab6de7fb8f9b12d67d63b94a1355cc014e4ce5c7504809cb8db2e8'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.12.0/docker-compose-linux-s390x'; 			sha256='b8087688da06c3c95e0cb518880053783951b47e3757be24788e34d5617128e4'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 18 Oct 2022 21:39:46 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 18 Oct 2022 21:39:47 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 18 Oct 2022 21:39:47 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 18 Oct 2022 21:39:48 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 18 Oct 2022 21:39:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 18 Oct 2022 21:39:50 GMT
CMD ["sh"]
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
	-	`sha256:2839662109c3662f36d20d4f9e06dda4da895298bd450b424415319f4261f84b`  
		Last Modified: Thu, 06 Oct 2022 20:00:59 GMT  
		Size: 8.0 MB (8048674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9684c7523557099cadb09af30feb21c5970402c4ca96feae5c8f72f46bd3760`  
		Last Modified: Thu, 06 Oct 2022 20:00:57 GMT  
		Size: 13.8 MB (13764592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5d4aafcf79092338f789826adccfbcbd1289d5972bffbef267565b15ba0d88`  
		Last Modified: Tue, 18 Oct 2022 21:43:12 GMT  
		Size: 13.1 MB (13069601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d3d89fd763b5af81e51de3720f8174c1930ebd19640540fed78e1aabb9e4f`  
		Last Modified: Tue, 18 Oct 2022 21:43:10 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:392f5ddebde995a0fac40451fa2bd7fc1be6bab97b53bc32e090683a7d881c5a`  
		Last Modified: Tue, 18 Oct 2022 21:43:10 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcf4732c18ac14eb8dae24ecb756152e3ad5e4acf54ea63120243e23bcf8962`  
		Last Modified: Tue, 18 Oct 2022 21:43:10 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
