## `docker:rc-cli`

```console
$ docker pull docker@sha256:e39dcee58c540b4d98a2e8025e06fa8c07dde55e7fb3434f4239cf6de16d086b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-cli` - linux; amd64

```console
$ docker pull docker@sha256:5b44c84dd6bf9fd5bbe7a851272ac36e5c5695f49653b7e136fdf66e8dbed194
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38105780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:346ebc81e4ca5070e8cb5854d53cf5d4f2968c043e1893a0b7b69a73cc7c368d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:48 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 09 Aug 2022 18:20:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:20:49 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Tue, 09 Aug 2022 18:20:53 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 19 Aug 2022 00:19:27 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Fri, 19 Aug 2022 00:19:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Wed, 24 Aug 2022 23:17:11 GMT
ENV DOCKER_COMPOSE_VERSION=2.10.1
# Wed, 24 Aug 2022 23:17:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-x86_64'; 			sha256='dfe2e3f134cc053e020891a11c23a0923eb49ee35556ec40b37d098eaa5a55f6'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-armv6'; 			sha256='8f9e1ccf35763b292443112795418b3ec9e8df46f8d78ca2c92d44645a90b88f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-armv7'; 			sha256='4a1bd3d72ff2d21248f5e1a32cdabc81aca9d613ce0eee661ac3cb6815db1258'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-aarch64'; 			sha256='2598b299693d3ef6087a8faa02e91e29bc2f4515347a0cf4c9ea18967584f153'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-ppc64le'; 			sha256='4866a6df1bc35eda103b0d32b357e2da4aae0b4eff96dd19ea4c1d6ddbc43e9f'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-riscv64'; 			sha256='8211dc32f228ac6d8685c2d07f579654771af3e792ebc6cc8a212536229630c3'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.10.1/docker-compose-linux-s390x'; 			sha256='56b70071f7ab4acf7387cb3ce8492ec084650b435a2f483d355931bfa5536496'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Wed, 24 Aug 2022 23:17:13 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Wed, 24 Aug 2022 23:17:13 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Wed, 24 Aug 2022 23:17:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 24 Aug 2022 23:17:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Wed, 24 Aug 2022 23:17:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Aug 2022 23:17:14 GMT
CMD ["sh"]
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
	-	`sha256:3d957832b8a49136f6d95f00340a0c764c8cd051be7514885f8fca6a80053215`  
		Last Modified: Tue, 09 Aug 2022 18:22:45 GMT  
		Size: 8.7 MB (8706435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd48969715b862016850752e05193de3fe3dbc355a5f277cece7c52d69f4793`  
		Last Modified: Fri, 19 Aug 2022 00:21:18 GMT  
		Size: 15.2 MB (15204103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b457a3085999b1f501d0ed7b62e86a90d0b41563715f55c0189ff8da5c007b`  
		Last Modified: Wed, 24 Aug 2022 23:18:55 GMT  
		Size: 9.4 MB (9351261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ec4ab43f121c4c4e549d22fddada81a818a1cbac485f30587df7bdef77cee6`  
		Last Modified: Wed, 24 Aug 2022 23:18:53 GMT  
		Size: 552.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd175e05748624b79db41ddd232e7b6d47c0fcdebb51b1c188dae04a77e8d7d0`  
		Last Modified: Wed, 24 Aug 2022 23:18:53 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cce2b1610321ba2cb3bfb55feaf77a750e23a26bdfcc16eee4b21c1df6e901`  
		Last Modified: Wed, 24 Aug 2022 23:18:53 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e3dab745f8a4eb17d85913e5621b23b4d7de5508784221a6652fa893e4fbe7fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35131702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34d04297fe7b1e38990a8965629b6da4987d85b2feed380ee7d233ced387ad7c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:24:48 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 09 Aug 2022 18:24:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:24:50 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Tue, 09 Aug 2022 18:24:54 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Fri, 19 Aug 2022 02:45:35 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Fri, 19 Aug 2022 02:45:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Fri, 19 Aug 2022 02:45:40 GMT
ENV DOCKER_COMPOSE_VERSION=2.9.0
# Fri, 19 Aug 2022 02:45:43 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-x86_64'; 			sha256='3be9ce88ecba41b734e3fc8e59a9b11531133761414a78827d1615aadb5ef1f5'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-armv6'; 			sha256='2ea0f36350f81ae66db2b8c12104de6ed974a328557a4967857ee6e8df4b8f26'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-armv7'; 			sha256='658db542e40c8063cdafc23f650493bedc10b41b6d6fb581b7866bfeb5ffb0ba'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-aarch64'; 			sha256='6d227b060b2bc3dc5f315a07ae4f647f042755691e2da905b1a21e60a8ae3ddf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-ppc64le'; 			sha256='101ea490283f3c862e9bb4e7ef2a3fb38393cf2139f2b78e7a7423c91ad0c1fa'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.9.0/docker-compose-linux-s390x'; 			sha256='0826c101e1d1a070e8ab8d7649c0da3cb9e6ecf1e717c545188243be6e676d00'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Fri, 19 Aug 2022 02:45:45 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Fri, 19 Aug 2022 02:45:46 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Fri, 19 Aug 2022 02:45:46 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 19 Aug 2022 02:45:47 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Fri, 19 Aug 2022 02:45:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 19 Aug 2022 02:45:49 GMT
CMD ["sh"]
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
	-	`sha256:1503a42e3097b1eaf3bbc5e72622fc4950bd97ec2439372d2daf9fe4324a21b5`  
		Last Modified: Tue, 09 Aug 2022 18:28:30 GMT  
		Size: 8.0 MB (8048680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f94397c525f39d44ef3fda3b0bba921a889eb33ccc36156f3ba73a88804a75`  
		Last Modified: Fri, 19 Aug 2022 02:49:05 GMT  
		Size: 13.8 MB (13764592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311538882b04c9b6b05cbd9a008312b873e96b40b5a5bd5fc7adcb51606178f9`  
		Last Modified: Fri, 19 Aug 2022 02:49:00 GMT  
		Size: 8.6 MB (8598409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc89d05e92b84ee59806020196a71c1815589db858a239a729365c2aaa5180e`  
		Last Modified: Fri, 19 Aug 2022 02:48:58 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b52dd222b17c2d6faf2f97029132855f5b4bc0e14edf8831c6f63487ac4f7e0`  
		Last Modified: Fri, 19 Aug 2022 02:48:58 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6447a6dbdbc25eb730d268bf14790d370fb47facb6a1fafa43e3640d36fde8f`  
		Last Modified: Fri, 19 Aug 2022 02:48:58 GMT  
		Size: 117.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
