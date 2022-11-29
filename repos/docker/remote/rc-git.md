## `docker:rc-git`

```console
$ docker pull docker@sha256:c41b4c4f3d088725b44048c7f83c097f69b452515f69f31482e2cbfdf817f53b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-git` - linux; amd64

```console
$ docker pull docker@sha256:0c98158ad3457365ec561d644c34dec5ee5ee4e18c3e6a56dcfb4bd95e741356
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48255568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f615304fcea74018be74e76e58425396ae1be93df99a063fe5f0346d610e3f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Tue, 29 Nov 2022 01:27:01 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 29 Nov 2022 01:27:02 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Tue, 29 Nov 2022 01:27:02 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Tue, 29 Nov 2022 01:27:06 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Tue, 29 Nov 2022 01:27:06 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Tue, 29 Nov 2022 01:27:08 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Tue, 29 Nov 2022 01:27:08 GMT
ENV DOCKER_COMPOSE_VERSION=2.13.0
# Tue, 29 Nov 2022 01:27:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-x86_64'; 			sha256='943ff254867e1c23cd6414d7255790daddc7ab69013dd79ba5c172410cbafb14'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-armv6'; 			sha256='c188afabb4565145beaf3ccd025d04428f7ba543616fb7042190d267ffb3df77'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-armv7'; 			sha256='7f985bf4b61f70b17a3c7da2d4cedb7e8fb13bc7c67d5e6e2fd23dd28212d61a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-aarch64'; 			sha256='4a920b7d5fe5011dd466fa87ea3b47ee5f224b5770337188daee359ec606eb20'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-ppc64le'; 			sha256='2aaa046eb055d2b0ccbdeac2c22f2bf927adb4c328b912a458686bf0861322d1'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-riscv64'; 			sha256='f8690e1c715a1bd87316cdd4e1ba1c0144f02eaa9f037075a471d926af133306'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-s390x'; 			sha256='e48830b80893ac41d8f7198f6660f23c24c4a7cde3b95593e534ff7bb3ee0a03'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 29 Nov 2022 01:27:11 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 29 Nov 2022 01:27:11 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 29 Nov 2022 01:27:11 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 29 Nov 2022 01:27:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 29 Nov 2022 01:27:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Nov 2022 01:27:12 GMT
CMD ["sh"]
# Tue, 29 Nov 2022 01:27:37 GMT
RUN apk add --no-cache git
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
	-	`sha256:167876a5be069f24a780c6f691232a898b42897a71a944c290b9ddbc8db9108d`  
		Last Modified: Tue, 29 Nov 2022 01:29:01 GMT  
		Size: 8.7 MB (8706448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbb609ba54efd37f7c5e2c41163e4e2406ba2867404a804a9a1a9fbad592523`  
		Last Modified: Tue, 29 Nov 2022 01:28:59 GMT  
		Size: 15.2 MB (15204113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae228767305225c5f1ad1c52b7846c2096f04343671bb80f190e37df6e56248`  
		Last Modified: Tue, 29 Nov 2022 01:28:59 GMT  
		Size: 14.8 MB (14772084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bcbab2f2af646ac72e7ceba31c9181da88accfad001077177c3b2fb6cf2fdaf`  
		Last Modified: Tue, 29 Nov 2022 01:28:57 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3008c4589e88141459cec163d170d5943082dd2f57db66f7ea98ad0f5e9f20b`  
		Last Modified: Tue, 29 Nov 2022 01:28:57 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e7b7dc2cac27d013ad3eed069f3c0906564c04efaf4ebddf62894acb3917df`  
		Last Modified: Tue, 29 Nov 2022 01:28:57 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9220d0d3263f37543c3884a283d83f06dbf3aa19577ac30d5fe42d300259ec93`  
		Last Modified: Tue, 29 Nov 2022 01:30:01 GMT  
		Size: 4.1 MB (4136245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:749f9dbeee22706b11f76bf056e7ed37dca3f7427f9f48004c1048f9cf0f9b8f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44632091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f55b82598f5a5d7f6ae925e6023ccf8a8dabf7eba55d968e28b39f40695fd3d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Tue, 22 Nov 2022 22:39:21 GMT
ADD file:685b5edadf1d5bf0aeb2aec35f810d83876e6d2ea0903b213f75a9c5f0dc5901 in / 
# Tue, 22 Nov 2022 22:39:21 GMT
CMD ["/bin/sh"]
# Tue, 29 Nov 2022 01:42:08 GMT
RUN apk add --no-cache 		ca-certificates 		libc6-compat 		openssh-client
# Tue, 29 Nov 2022 01:42:08 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf
# Tue, 29 Nov 2022 01:42:08 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Tue, 29 Nov 2022 01:42:11 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-22.06.0-beta.0.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-22.06.0-beta.0.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-22.06.0-beta.0.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-22.06.0-beta.0.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Tue, 29 Nov 2022 01:42:11 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Tue, 29 Nov 2022 01:42:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Tue, 29 Nov 2022 01:42:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.13.0
# Tue, 29 Nov 2022 01:42:19 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-x86_64'; 			sha256='943ff254867e1c23cd6414d7255790daddc7ab69013dd79ba5c172410cbafb14'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-armv6'; 			sha256='c188afabb4565145beaf3ccd025d04428f7ba543616fb7042190d267ffb3df77'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-armv7'; 			sha256='7f985bf4b61f70b17a3c7da2d4cedb7e8fb13bc7c67d5e6e2fd23dd28212d61a'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-aarch64'; 			sha256='4a920b7d5fe5011dd466fa87ea3b47ee5f224b5770337188daee359ec606eb20'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-ppc64le'; 			sha256='2aaa046eb055d2b0ccbdeac2c22f2bf927adb4c328b912a458686bf0861322d1'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-riscv64'; 			sha256='f8690e1c715a1bd87316cdd4e1ba1c0144f02eaa9f037075a471d926af133306'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.13.0/docker-compose-linux-s390x'; 			sha256='e48830b80893ac41d8f7198f6660f23c24c4a7cde3b95593e534ff7bb3ee0a03'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Tue, 29 Nov 2022 01:42:19 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Tue, 29 Nov 2022 01:42:20 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Tue, 29 Nov 2022 01:42:20 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 29 Nov 2022 01:42:20 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Tue, 29 Nov 2022 01:42:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 29 Nov 2022 01:42:20 GMT
CMD ["sh"]
# Tue, 29 Nov 2022 01:42:53 GMT
RUN apk add --no-cache git
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
	-	`sha256:80b845a285d7e5030c4ad0ef7da9967f0d0a1303715750be254e670890a3d095`  
		Last Modified: Tue, 29 Nov 2022 01:44:15 GMT  
		Size: 8.0 MB (8048675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ce1ba28fe13a4eaba8fa7079f76a9adb36b95cbf782e3cfbc6184b190e0e7d`  
		Last Modified: Tue, 29 Nov 2022 01:44:13 GMT  
		Size: 13.8 MB (13764573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd2e5db61656c1d6d318a052e618ddba3952a2dcfe849c1ba0a240a5e877242`  
		Last Modified: Tue, 29 Nov 2022 01:44:13 GMT  
		Size: 13.3 MB (13340966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3914d84383639f092a0def7de25e474a1fdff07be17b87ec08e9a6e6083de8`  
		Last Modified: Tue, 29 Nov 2022 01:44:12 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a67779c9d3023e01dce6bb48bff56b5ed7e25cf50b444c40618b7ed23fdca4c2`  
		Last Modified: Tue, 29 Nov 2022 01:44:12 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24cd408bf04685f6ea022294a828d274eac495e938b608fb407ea3b2be0b5cfc`  
		Last Modified: Tue, 29 Nov 2022 01:44:12 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953c58510d5330913c4a3f8df8647ea44b16551a4f6a0c8fa6de44a0699a8c59`  
		Last Modified: Tue, 29 Nov 2022 01:45:13 GMT  
		Size: 4.2 MB (4180118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
