## `docker:rc-git`

```console
$ docker pull docker@sha256:78b80e0da81fccd6232949354886b3c4df8e541efb627ba369157c89095955af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:rc-git` - linux; amd64

```console
$ docker pull docker@sha256:63df9ed692c2465e803c359de1ca4009ef51bc92ce5e00d1ae534306eade0a14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.5 MB (55471951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca0a2fabbdb738cabeb63b20ba478982a1c766aee1fcac643dc792b475488e0`
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
# Thu, 29 Dec 2022 17:20:55 GMT
ENV DOCKER_VERSION=23.0.0-rc.1
# Thu, 29 Dec 2022 17:20:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-23.0.0-rc.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-23.0.0-rc.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-23.0.0-rc.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-23.0.0-rc.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Thu, 29 Dec 2022 17:20:59 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Thu, 29 Dec 2022 17:21:01 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Thu, 29 Dec 2022 17:21:01 GMT
ENV DOCKER_COMPOSE_VERSION=2.14.2
# Thu, 29 Dec 2022 17:21:04 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-x86_64'; 			sha256='d056a8330a01f22c249b9fa03ad0d5be889b79b648cad43c8549eb4c3f8ff0ba'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-armv6'; 			sha256='164b04d5970f340eb6cb4da171b2dc0d12c345a6092c8ac2409b5fb4fc8af5e6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-armv7'; 			sha256='6e01028d97bc48bfd3894d9161586e74c0f37cf7d67a67ab7eafb351c2003cb3'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-aarch64'; 			sha256='48ef22ecea70b4b197def1c1bfd2e797f7117db5257f6e505e64f03fdc329a7e'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-ppc64le'; 			sha256='8cbceb45fc656ec9f9e24b8e61fda54d233ecc8f46cee8ef5ae5acfdcc7940d4'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-riscv64'; 			sha256='e9d612ff8d198911f93706f4eec2bb58abb24c0f869cff7d69f6a8e24ce05420'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-s390x'; 			sha256='9fec4a8628729766f4600ec0f8fb5aa760b6a20673e1abfb3d78f3b2eb02696a'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Thu, 29 Dec 2022 17:21:04 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 29 Dec 2022 17:21:04 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 29 Dec 2022 17:21:04 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Dec 2022 17:21:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 29 Dec 2022 17:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Dec 2022 17:21:05 GMT
CMD ["sh"]
# Thu, 29 Dec 2022 17:21:28 GMT
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
	-	`sha256:8eac26b9fd140bd6a8e7a448eb1e2a6f2b0c34a2f85980151d5ee6845f4b1370`  
		Last Modified: Thu, 29 Dec 2022 17:22:20 GMT  
		Size: 16.2 MB (16214837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24215b171d2c93b81105b4dad5d13c041ac51f8e59f4df9fd70bc315fcda7254`  
		Last Modified: Thu, 29 Dec 2022 17:22:19 GMT  
		Size: 15.2 MB (15204070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02493b48b4e9939467032f4cae0fdd77d792e8faaff5ddb539c1c4aa047b9938`  
		Last Modified: Thu, 29 Dec 2022 17:22:19 GMT  
		Size: 14.5 MB (14474933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf404cfad1e67cdc8ad9898d2b18d56caab953fa3e747d19ff6ed9b56f57bd01`  
		Last Modified: Thu, 29 Dec 2022 17:22:16 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388dc806e3bdbdb4aacc5825dd461ea8076e9ff9fc1eb63104071e73fb5240fe`  
		Last Modified: Thu, 29 Dec 2022 17:22:16 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3afb8c205814317afae4b25951e8ad4fa1840e8e1f177a168fff24c050589cb`  
		Last Modified: Thu, 29 Dec 2022 17:22:16 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae6543188cd90f3f44b17b72e45863546e539fcaa846e663bc577d01922a6ecc`  
		Last Modified: Thu, 29 Dec 2022 17:23:23 GMT  
		Size: 4.1 MB (4141432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a2532a8c0d91f685ca89a9ceea92b1305c3d90e192ac56751e818f57bc6b81ed
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51602053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f124dc45b0119c81bec43400f4f0d19d7c140d6f8a4ecdd8c0d670c5dd39aae2`
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
# Thu, 29 Dec 2022 16:39:22 GMT
ENV DOCKER_VERSION=23.0.0-rc.1
# Thu, 29 Dec 2022 16:39:25 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-23.0.0-rc.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-23.0.0-rc.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-23.0.0-rc.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-23.0.0-rc.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version
# Thu, 29 Dec 2022 16:39:25 GMT
ENV DOCKER_BUILDX_VERSION=0.9.1
# Thu, 29 Dec 2022 16:39:27 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-amd64'; 			sha256='a7fb95177792ca8ffc7243fad7bf2f33738b8b999a184b6201f002a63c43d136'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v6'; 			sha256='159925b4e679eb66e7f0312c7d57a97e68a418c1fa602a00dd8b29b6406768f0'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm-v7'; 			sha256='ba8e5359ce9ba24fec6da07f73591c1b20ac0797a2248b0ef8088f57ae3340fc'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-arm64'; 			sha256='bbf6a76bf9aef9c5759ff225b97ce23a24fc11e4fa3cdcae36e5dcf1de2cffc5'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-ppc64le'; 			sha256='1b2441886e556c720c1bf12f18f240113cc45f9eb404c0f162166ca1c96c1b60'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-riscv64'; 			sha256='c32372dad653fc70eb756b2cffd026e74425e807c01accaeed4559da881ff57c'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.9.1/buildx-v0.9.1.linux-s390x'; 			sha256='90b0ecf315d741888920dddeac9fe2e141123c4fe79465b7b10fe23521c9c366'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version
# Thu, 29 Dec 2022 16:39:27 GMT
ENV DOCKER_COMPOSE_VERSION=2.14.2
# Thu, 29 Dec 2022 16:39:29 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-x86_64'; 			sha256='d056a8330a01f22c249b9fa03ad0d5be889b79b648cad43c8549eb4c3f8ff0ba'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-armv6'; 			sha256='164b04d5970f340eb6cb4da171b2dc0d12c345a6092c8ac2409b5fb4fc8af5e6'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-armv7'; 			sha256='6e01028d97bc48bfd3894d9161586e74c0f37cf7d67a67ab7eafb351c2003cb3'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-aarch64'; 			sha256='48ef22ecea70b4b197def1c1bfd2e797f7117db5257f6e505e64f03fdc329a7e'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-ppc64le'; 			sha256='8cbceb45fc656ec9f9e24b8e61fda54d233ecc8f46cee8ef5ae5acfdcc7940d4'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-riscv64'; 			sha256='e9d612ff8d198911f93706f4eec2bb58abb24c0f869cff7d69f6a8e24ce05420'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.14.2/docker-compose-linux-s390x'; 			sha256='9fec4a8628729766f4600ec0f8fb5aa760b6a20673e1abfb3d78f3b2eb02696a'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version
# Thu, 29 Dec 2022 16:39:29 GMT
COPY file:abb137d24130e7fa2bdd38694af607361ecb688521e60965681e49460964a204 in /usr/local/bin/modprobe 
# Thu, 29 Dec 2022 16:39:29 GMT
COPY file:5b18768029dab8174c9d5957bb39560bde5ef6cba50fbbca222731a0059b449b in /usr/local/bin/ 
# Thu, 29 Dec 2022 16:39:29 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 29 Dec 2022 16:39:30 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client
# Thu, 29 Dec 2022 16:39:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 29 Dec 2022 16:39:30 GMT
CMD ["sh"]
# Thu, 29 Dec 2022 16:39:53 GMT
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
	-	`sha256:ca8cadd162baf4e6baf87c3b8cabea5aa1ca9ad5925c0fbc7686eb9c9d61c48c`  
		Last Modified: Thu, 29 Dec 2022 16:40:46 GMT  
		Size: 15.3 MB (15291665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948bd5e25ebbb11921d23a9ebf978a835132271c6e170c575db9e771a16e039b`  
		Last Modified: Thu, 29 Dec 2022 16:40:44 GMT  
		Size: 13.8 MB (13764578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05da3711b9b112f6fff6982087c7c04285205a70cf40ee2766f82daf71b2513e`  
		Last Modified: Thu, 29 Dec 2022 16:40:44 GMT  
		Size: 13.1 MB (13063335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c0fb4149c992de079195b0b9238101feeb261e3046608ef702ced782e6edbc`  
		Last Modified: Thu, 29 Dec 2022 16:40:42 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552d52e958dc8e24045b7bfd6b3358828885c902edc1373fcd818d38deae25f0`  
		Last Modified: Thu, 29 Dec 2022 16:40:42 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f05488781146c3fe9a3f16f0be735f1e1fd094428646aeae8e22f9119b87d4f`  
		Last Modified: Thu, 29 Dec 2022 16:40:42 GMT  
		Size: 150.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b992580cb98c983dc6bc9bf98141119db2132910637cc22f23d951a60dc440`  
		Last Modified: Thu, 29 Dec 2022 16:41:45 GMT  
		Size: 4.2 MB (4184715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
