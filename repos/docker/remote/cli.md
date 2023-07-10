## `docker:cli`

```console
$ docker pull docker@sha256:2691dca173f0e947a0f26666117b3c408ef5d3aca3b0966e69b143b95e0ce6a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `docker:cli` - linux; amd64

```console
$ docker pull docker@sha256:2f8dae1ab1fc361a92fa8d1403e842832e79ac5f58a0ff25fd6e1e6dcddc9a39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.2 MB (57237369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:761c8b24ac0ac28e2d38bb871f1323cd13e56b08a32616fc47b58a0049d4f11b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Fri, 07 Jul 2023 21:23:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
ENV DOCKER_VERSION=24.0.4
# Fri, 07 Jul 2023 21:23:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.4.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.4.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.4.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.4.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
ENV DOCKER_BUILDX_VERSION=0.11.1
# Fri, 07 Jul 2023 21:23:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-amd64'; 			sha256='34927047282ef9052f57809fe94783b2dc0ab556fdd60c2c0b7f4e6e5f05a53b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-arm-v6'; 			sha256='ec7b60a4946c7c0fdaa3a44590adc08a0ead0ecca860358c57ca62d3e9a3a0be'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-arm-v7'; 			sha256='d122ec20622a744419fea021fd4850edc56d816b5cbc746d1f90184dbc227fec'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-arm64'; 			sha256='1649de43c6477eb8bf615f0817932e69e500ce530422bed47c9f3a689baeb788'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-ppc64le'; 			sha256='78cfc6cdb3982770ce4e922e62c42ee0750b4b2837349661d20834356f004d16'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-riscv64'; 			sha256='1d932a0925e9aee66c85cb7a351e9dbd210294ccb8d01208bf953108ad321f4d'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-s390x'; 			sha256='89466f278264f597d3c81e5230ab5795b2578ad62d2c7e8f8be398546e02c3d7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Fri, 07 Jul 2023 21:23:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Jul 2023 21:23:59 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Jul 2023 21:23:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7d0e1aee3d7ae6d265ee545cbab734bf74984f2c92ce1e9de99384496437d9`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 2.0 MB (2014369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616dc7f2241d214810794d133404c6c0fce720828611e22602fb0509d3b7dc6c`  
		Last Modified: Thu, 15 Jun 2023 05:27:05 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f83d66c9f2978256f5af482db96fc7c7c0c35e61a85ad5580a2078ea66adf9`  
		Last Modified: Mon, 10 Jul 2023 19:28:02 GMT  
		Size: 16.4 MB (16389603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b33ab92a6bb08bb76c708fb88854a9fe667c52493e06ba6f39f340c17491754`  
		Last Modified: Mon, 10 Jul 2023 19:28:01 GMT  
		Size: 17.5 MB (17453588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e091e6db8ccf84685d49f5429b4bca56733cae16117ce10d51af7e4168768a85`  
		Last Modified: Mon, 10 Jul 2023 19:28:02 GMT  
		Size: 18.0 MB (17980104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69e3e72a714f8f0b60ca672941346e4d0cfe8d6d2e9a0e7a568f7eed2b5faa8`  
		Last Modified: Mon, 10 Jul 2023 19:27:59 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62495c93088e3c717033098919f24b09eed011099e873533cfb9f1cb5d2b4f43`  
		Last Modified: Mon, 10 Jul 2023 19:27:59 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a28e0955540b02407a13f57c53e2a83a688f8c57a419fd99bae5bd7b907a50`  
		Last Modified: Mon, 10 Jul 2023 19:27:59 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:3d6cdd02719ed42d67ff5317d4864f209b7f4469649c0cb152f84b0bbd36730d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52863190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a1de6c0a50a598e412fda5cf05e50f9fd75f94141ddab4ce8e5a6b39c09471e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Fri, 07 Jul 2023 21:23:59 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
ENV DOCKER_VERSION=24.0.4
# Fri, 07 Jul 2023 21:23:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.4.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.4.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.4.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.4.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
ENV DOCKER_BUILDX_VERSION=0.11.1
# Fri, 07 Jul 2023 21:23:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-amd64'; 			sha256='34927047282ef9052f57809fe94783b2dc0ab556fdd60c2c0b7f4e6e5f05a53b'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-arm-v6'; 			sha256='ec7b60a4946c7c0fdaa3a44590adc08a0ead0ecca860358c57ca62d3e9a3a0be'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-arm-v7'; 			sha256='d122ec20622a744419fea021fd4850edc56d816b5cbc746d1f90184dbc227fec'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-arm64'; 			sha256='1649de43c6477eb8bf615f0817932e69e500ce530422bed47c9f3a689baeb788'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-ppc64le'; 			sha256='78cfc6cdb3982770ce4e922e62c42ee0750b4b2837349661d20834356f004d16'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-riscv64'; 			sha256='1d932a0925e9aee66c85cb7a351e9dbd210294ccb8d01208bf953108ad321f4d'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.1/buildx-v0.11.1.linux-s390x'; 			sha256='89466f278264f597d3c81e5230ab5795b2578ad62d2c7e8f8be398546e02c3d7'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
ENV DOCKER_COMPOSE_VERSION=2.19.1
# Fri, 07 Jul 2023 21:23:59 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-x86_64'; 			sha256='8d3ecd3e48c598ba2e2d8eb3b59380f74c8c0c46259008fcd16d0dc058aaebd1'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv6'; 			sha256='78639fa8323f0f60cd8b45a882bbb63cc630b44a7187e922195855cb64607d8f'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-armv7'; 			sha256='bc9646ecf835e5e2665b7de6455c07cb21d4e892a4c212f9ca9f3024a26ff880'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-aarch64'; 			sha256='35db0e5207c66e002bfde3cab84e907aa7e552812803bebebf990487729eb2bf'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-ppc64le'; 			sha256='9c79eada1314e63734eb33e9d1815b5f494c357b45ac1c3ec035188ee616f215'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-riscv64'; 			sha256='bcca185b3f1f2e6dbb392149f52676075b1e42ba64a3ed6508c2f9fc1b60c634'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.19.1/docker-compose-linux-s390x'; 			sha256='152e40b9f600b84223b8c2f217c45ed4813af8cdd98017cdcbdb35b81423f8d9'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 07 Jul 2023 21:23:59 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Fri, 07 Jul 2023 21:23:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Jul 2023 21:23:59 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e640e1526600576ae628fd21f3470e3216d9579d4b14b1032c2ed619de68e53`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 2.0 MB (2024530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db2eba5565b7a07c4d4ea27b5423aca276dfd220175588874377309ecab83ecc`  
		Last Modified: Wed, 14 Jun 2023 22:40:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19aadc22366563d3dabd7151e690b7bfe4b2f1db8f3419a507fb07e013b6f96`  
		Last Modified: Mon, 10 Jul 2023 19:41:27 GMT  
		Size: 15.4 MB (15435078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3735e18644abe5b6483de79fac3e9bf4e56cfdca38ab4d1d0bd71552bfec33`  
		Last Modified: Mon, 10 Jul 2023 19:41:25 GMT  
		Size: 15.8 MB (15759509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ff2d68d7514f6633a0b765da479fa2a9f56c4b2eff488f472a555ac69c046b`  
		Last Modified: Mon, 10 Jul 2023 19:41:26 GMT  
		Size: 16.3 MB (16312995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f01674a2c78d6ecabc631c5ac90300c3c6cb449a11c2b1e87c1e45e5727e54b`  
		Last Modified: Mon, 10 Jul 2023 19:41:23 GMT  
		Size: 548.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e35865a1f9af4158e05b5dd7bcba02617497747619dbeae6c2243dfbf73d0f1`  
		Last Modified: Mon, 10 Jul 2023 19:41:23 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdcee27edcecd206ff11f9113b9220745dda8c0d9735ad41b5dd888d6a20027`  
		Last Modified: Mon, 10 Jul 2023 19:41:23 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
