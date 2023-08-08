## `docker:24-dind`

```console
$ docker pull docker@sha256:9ec413dbffb3e75b95d68a746a5ec3451afa6836cc5bce03a856a826c5ad0b12
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-dind` - linux; amd64

```console
$ docker pull docker@sha256:bbc57559ea5f6d7359f53c92bdfd386df0b1b0384591a24b7a6cf40b77343a4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.9 MB (120901309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fddd6ec43ab484d35772852bbeefbc825bc2b9846d121f1e87da42cfef62e00`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-x86_64'; 			sha256='b9385dabb7931636a3afc0aee94625ebff3bb29584493a87804afb6ebaf2d916'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv6'; 			sha256='39cef332454d1c7a26e12f8d9ee297908d1da9cb71112ede1816c550766ddb8e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv7'; 			sha256='139275f3453761b46f0837a4e4c2a00883b778abee997e299c52e1bcf3d8fc9f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-aarch64'; 			sha256='e63a24e57d2104a09b37ee6aa04c76f4ae85bdf7a59e1bf79adc6d5f55340a31'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-ppc64le'; 			sha256='9c08eb875a7ffd4a832a585540a4c9c81da5dcab263ec3e704ab1d62b573636f'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-riscv64'; 			sha256='5a3bff32ecf0a5a38a83afeb3dc2effd8ca3d52eb2e07ec000334663d493055b'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-s390x'; 			sha256='297be6a0ece070ae95d5caf91a23b89dc1b2563e928db80eee480d7018919ee6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a909a6dccb2a6d84f4f5aefc708bf3ffcc5d43ef0281708c595f1d3f126d395d`  
		Last Modified: Fri, 28 Jul 2023 22:18:34 GMT  
		Size: 2.0 MB (2014277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee5d1d3b3c0a84d62fbd574562a1be8d50b7c6851e2b212d3e42c3f30b9e1eb2`  
		Last Modified: Fri, 28 Jul 2023 22:18:34 GMT  
		Size: 16.4 MB (16390649 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5061ed9e3f18485a019cb2d5eb9c7b1326aa76691480c9625e80abb6dfde6411`  
		Last Modified: Fri, 28 Jul 2023 22:18:35 GMT  
		Size: 17.5 MB (17459268 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97b5a361640304d855b5be202f9e2a7baac4a963f393ff48d5dc21a934a7c938`  
		Last Modified: Fri, 28 Jul 2023 22:18:35 GMT  
		Size: 18.0 MB (17988753 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f429e55eceb384dfc466efa7a0bc3bdc698d14cc2d7909d823ba9753c3924fa`  
		Last Modified: Fri, 28 Jul 2023 22:18:35 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7288f1321468813ab59c5614b931a5a8065be8f4a2d9cb2e1969600eaad7e2c7`  
		Last Modified: Fri, 28 Jul 2023 22:18:36 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39e34e641f8b1404b00d5c672066c54226a8ead75c4f39bbf37460aabe01bcb4`  
		Last Modified: Fri, 28 Jul 2023 22:18:36 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6ee3b156fe6393577dc4490f97c6d2b08c98aeec04c383f1828ae55ae950d9e`  
		Last Modified: Mon, 31 Jul 2023 21:05:32 GMT  
		Size: 9.3 MB (9266083 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98627b255aea9d5c8ff48dcdc4a6c2a41aa1a7451424da9723839cbc01c852de`  
		Last Modified: Mon, 31 Jul 2023 21:05:31 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f191f06e12ea5246673afce7b10713011b94fe8a8c2791ddde91248c367a8f44`  
		Last Modified: Mon, 31 Jul 2023 21:05:34 GMT  
		Size: 54.4 MB (54377567 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6471e5d17b88d2bc79821a01015944da238bbbe1d0a4320c5dc2fa70ddc6a756`  
		Last Modified: Mon, 31 Jul 2023 21:05:31 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b911e1248ddca02330949a971f5040c1b34027ab3784f8b51ebfa0fcee296879`  
		Last Modified: Mon, 31 Jul 2023 21:05:32 GMT  
		Size: 2.8 KB (2793 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind` - unknown; unknown

```console
$ docker pull docker@sha256:31b162dbcfef47a911a9c3d68e295c259b383bd6d552864240020c7f6b7ec847
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **776.3 KB (776336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:652d54c363c041aebece1d249609e63241f3b2523369427ea1c0a90aac3028cc`

```dockerfile
```

-	Layers:
	-	`sha256:1c3d043296de8eb013796234706d299e81ff5c53c1a012face52859a043fad36`  
		Last Modified: Mon, 31 Jul 2023 21:05:30 GMT  
		Size: 746.2 KB (746174 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f47bb1d5cbdff10f55c1ac0de988bc80a7417e8ceac0c2493cf1d817f3fc9746`  
		Last Modified: Mon, 31 Jul 2023 21:05:30 GMT  
		Size: 30.2 KB (30162 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:a381661c34528b528daa8252d51e9060f480eac7225df1f8aed69ee05ba149e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109896531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b7cc94180e380149b5692a59a107aa8516cccaee9758004b09182b0e12ff729`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 24 Jul 2023 16:17:39 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["/bin/sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_VERSION=24.0.5
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-x86_64'; 			sha256='b9385dabb7931636a3afc0aee94625ebff3bb29584493a87804afb6ebaf2d916'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv6'; 			sha256='39cef332454d1c7a26e12f8d9ee297908d1da9cb71112ede1816c550766ddb8e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv7'; 			sha256='139275f3453761b46f0837a4e4c2a00883b778abee997e299c52e1bcf3d8fc9f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-aarch64'; 			sha256='e63a24e57d2104a09b37ee6aa04c76f4ae85bdf7a59e1bf79adc6d5f55340a31'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-ppc64le'; 			sha256='9c08eb875a7ffd4a832a585540a4c9c81da5dcab263ec3e704ab1d62b573636f'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-riscv64'; 			sha256='5a3bff32ecf0a5a38a83afeb3dc2effd8ca3d52eb2e07ec000334663d493055b'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-s390x'; 			sha256='297be6a0ece070ae95d5caf91a23b89dc1b2563e928db80eee480d7018919ee6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 24 Jul 2023 16:17:39 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD ["sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.5.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.5.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.5.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.5.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Mon, 24 Jul 2023 16:17:39 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 24 Jul 2023 16:17:39 GMT
VOLUME [/var/lib/docker]
# Mon, 24 Jul 2023 16:17:39 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 24 Jul 2023 16:17:39 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 24 Jul 2023 16:17:39 GMT
CMD []
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6852f3ef0b5f9b77c7c21abf9035ed77c331514fd6aa1498370a5dbd3e2048b5`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 2.0 MB (2024556 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:37278d121b4b21d7bddb02dabb1e78b7fc30c3f3a41e41d6f6967d040f3a1b54`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 15.4 MB (15435452 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c05b0ea06520d0d3c1e2b6753a684589ba3e17e586d4be8ad9ddfbb2d3b1d4c`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 15.8 MB (15768051 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b920faef0f924e0bc6293f765487b42850f8fcc7dc006e00acab7779365e7b3`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 16.3 MB (16320824 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8cfd071449c0a8d2d4ea27ffa825ac548273b41fc00b7dc76e13263f55c129ac`  
		Last Modified: Mon, 07 Aug 2023 22:18:58 GMT  
		Size: 548.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5bd8c360864191385b3ebd69155f1dfe1900d09f75ebfc489c01c86434583e8d`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 1.0 KB (1021 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b1fdce017755150f777e27def5147cfbc3441af3770996ea37fd694a0a07bbed`  
		Last Modified: Mon, 07 Aug 2023 22:18:59 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ccc68e27d20d81c5082a28faedb7feda3ac23db34bbbcc2caa1b82b1021eca9`  
		Last Modified: Mon, 07 Aug 2023 22:55:11 GMT  
		Size: 7.3 MB (7291162 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a2c99fcb4ebd1ddf039f1e83fc19e534b2ab9fedf7129a9eedbb875356f8c67`  
		Last Modified: Mon, 07 Aug 2023 22:55:10 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:42173ff4f85357bbcdbea0f5a420603cac5a52162f8d7b6cf30061397ce5fdfb`  
		Last Modified: Mon, 07 Aug 2023 22:55:13 GMT  
		Size: 49.7 MB (49718883 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:48772cf52f8ea3e9b59a7fa20a40f91c26df17d138fc892cc8f2c44cc87607d4`  
		Last Modified: Mon, 07 Aug 2023 22:55:10 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8520c3392243d65413eb8453582848ba7e8a5bdff7874268638054b34a07af7c`  
		Last Modified: Mon, 07 Aug 2023 22:55:11 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-dind` - unknown; unknown

```console
$ docker pull docker@sha256:7f4a66a5695dd5d1e8fc1c7ca73f75ab5c40011ea3385424e50f578097401fe4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **784.1 KB (784063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e2ab24c88ee978b7146023ce3b92a5f4c88aacbef25a5979dd9eaafe4e8ac05`

```dockerfile
```

-	Layers:
	-	`sha256:77eae467d5340b30f3a22026b8792902ba1c35a988b83d47ba017446f3a1e9da`  
		Last Modified: Mon, 07 Aug 2023 22:55:10 GMT  
		Size: 753.9 KB (753855 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b57138c25912cc8f4294f6c4e9d0d2ff9129eb47dc276e2e96be5a3e36d238ac`  
		Last Modified: Mon, 07 Aug 2023 22:55:10 GMT  
		Size: 30.2 KB (30208 bytes)  
		MIME: application/vnd.in-toto+json
