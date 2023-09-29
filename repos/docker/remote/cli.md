## `docker:cli`

```console
$ docker pull docker@sha256:25d3f6594113576d033a63601d1f5b7499e47eea7b12aa0132cefc5dcca9f9a6
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:cli` - linux; amd64

```console
$ docker pull docker@sha256:71fef5d661fa65800fd20a18b127da165ec3941b56fcbc2b34e81a92b8cfb204
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57096360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28fed4f37d07f371ec78324f52ee8c3c8b7c05930d32d83a7ea0d789a4189800`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 21 Sep 2023 17:05:55 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 21 Sep 2023 17:05:55 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 17:05:55 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
ENV DOCKER_VERSION=24.0.6
# Thu, 21 Sep 2023 17:05:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Thu, 21 Sep 2023 17:05:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.22.0
# Thu, 21 Sep 2023 17:05:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-x86_64'; 			sha256='e849450f1c5c20123aa7d63291e2a818b7a117f2e03e432853ece463dd09e67a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv6'; 			sha256='46cabb4363c5fa66e63c6055b1d0a6fe2c7995350e48f14816a752ae4132231d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv7'; 			sha256='1a0d500eaae3c4ddbfdeb566896207c0628a671065b95d0e8907bca58f91d312'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-aarch64'; 			sha256='572a22000d408fb524258b379bf272a007c8da977c3e8d47c34f4e45dd7b1932'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-ppc64le'; 			sha256='4d1a3e89fdb7641422dc5cbcab48fd2da337b03265cb5ac2858c3425bacf952c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-riscv64'; 			sha256='c45193b98c54e5a898e6b9095f70b0487599f19ce25b579ed2fcc3f868415aff'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-s390x'; 			sha256='716aded74df512728638f1fe53170c46d94c1a085bc5a24108ce7101bc37bd81'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 21 Sep 2023 17:05:55 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 17:05:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9a3b84f9d8d423361dc29f5318ddebd6822e36fda6a7311f9552a63cb8eef92`  
		Last Modified: Thu, 28 Sep 2023 22:50:45 GMT  
		Size: 2.0 MB (2014281 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e55f70a486915794c20cc8069b18eda66ec3ad4fc3e393361ae99e88ba75ac0`  
		Last Modified: Thu, 28 Sep 2023 22:50:46 GMT  
		Size: 16.4 MB (16390432 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5cde11686b6fc659bd672ba8ce623ac5ca01c69d8218e39dd606badef1de7a0e`  
		Last Modified: Thu, 28 Sep 2023 22:50:46 GMT  
		Size: 17.5 MB (17459269 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:16c4cc17db7f3f57c0bae50e5fd393fd68e38699f03a6c066c4d4604eecc4332`  
		Last Modified: Thu, 28 Sep 2023 22:50:47 GMT  
		Size: 17.8 MB (17828705 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:56e17aa0ca7f5f6173dbfade7886bf9acbc865d4ffb9a38208147d177035d17f`  
		Last Modified: Thu, 28 Sep 2023 22:50:46 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:04e17f377b828e4d21a41243d3d9f4dde9f454449e6b60f6101fa80a8eb8f15d`  
		Last Modified: Thu, 28 Sep 2023 22:50:47 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fdee13b2421d9f03b8fbd0e7c1446672777969c9355275da3c606fb3819ebe30`  
		Last Modified: Thu, 28 Sep 2023 22:50:47 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:09b59190435955ca1eecf0a898ffae1b044f09a11a77a36b54879dbb56388963
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.9 KB (544883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19ce0797a591e70d566766c8a22ddf8e01a7d4c5f61e60125deae68704b48a82`

```dockerfile
```

-	Layers:
	-	`sha256:b589d21f6ad3d6106c1cfa3e5c3bf0f83565d3f34fe2e542de2774af6d7aad9e`  
		Last Modified: Thu, 28 Sep 2023 22:50:45 GMT  
		Size: 509.1 KB (509090 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:96747f317f4018e5d40e49582b7abbc32d6c3a54263e329b48fc9c70408a0495`  
		Last Modified: Thu, 28 Sep 2023 22:50:45 GMT  
		Size: 35.8 KB (35793 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:16812d6908b000ee513dfe56b4ea7a03079c45b8730bb54cf52a29df856e3844
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52849290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8474d39a40918271d2543e2df8a56cfb0fcf4bd7b8a1c946a433c7c7caed9945`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 21 Sep 2023 17:05:55 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 21 Sep 2023 17:05:55 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 17:05:55 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
ENV DOCKER_VERSION=24.0.6
# Thu, 21 Sep 2023 17:05:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Thu, 21 Sep 2023 17:05:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
ENV DOCKER_COMPOSE_VERSION=2.22.0
# Thu, 21 Sep 2023 17:05:55 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-x86_64'; 			sha256='e849450f1c5c20123aa7d63291e2a818b7a117f2e03e432853ece463dd09e67a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv6'; 			sha256='46cabb4363c5fa66e63c6055b1d0a6fe2c7995350e48f14816a752ae4132231d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv7'; 			sha256='1a0d500eaae3c4ddbfdeb566896207c0628a671065b95d0e8907bca58f91d312'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-aarch64'; 			sha256='572a22000d408fb524258b379bf272a007c8da977c3e8d47c34f4e45dd7b1932'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-ppc64le'; 			sha256='4d1a3e89fdb7641422dc5cbcab48fd2da337b03265cb5ac2858c3425bacf952c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-riscv64'; 			sha256='c45193b98c54e5a898e6b9095f70b0487599f19ce25b579ed2fcc3f868415aff'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-s390x'; 			sha256='716aded74df512728638f1fe53170c46d94c1a085bc5a24108ce7101bc37bd81'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 21 Sep 2023 17:05:55 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 21 Sep 2023 17:05:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 17:05:55 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ecd494fa26a8aad94a0d22885340d6ee599258b2e67c6c22f91ed6221294435`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 2.0 MB (2024548 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:152366591504a2012a175b6773ee6dd24c70908a8974de4f78b436134dbcd209`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.4 MB (15438727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:002e729a1bea6f35c00510ee459c2c20ac218b3f9ddf24db1722f8ba114316a2`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4475640d4b9700b7c0796e86dd2a4f56d238090f5c88fefa616bc2c1996f6cad`  
		Last Modified: Fri, 29 Sep 2023 02:55:40 GMT  
		Size: 16.3 MB (16284423 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:479bb069c95302029a8fd7f34e2f92c9f722466cb004ec9a7de4f28b7b46b84b`  
		Last Modified: Fri, 29 Sep 2023 02:55:39 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:66610116e5414dd019279d78145cb14c323f0cbe81df8f7b5d64e397d9500453`  
		Last Modified: Fri, 29 Sep 2023 02:55:40 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c755325432ecc6f0291cdf9d6ed427a37394f0d038e681043f311699948f8efd`  
		Last Modified: Fri, 29 Sep 2023 02:55:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:d00eea979bd8b188fa22564105f72b6be14f798246aa7bd6aea2d5a949930fa2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.3 KB (398286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6da2c6c39ca0da2c789fb9e173280aa075521493da5dab4382325fac45b9f5d8`

```dockerfile
```

-	Layers:
	-	`sha256:237678a8be1380c37ec89f3b1599eed6aeb1b998faa11e00450f33cf85b350c6`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 362.5 KB (362491 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6022f7f2820805f45f8b13c3a71b642b0a5343df106814c64b269a6a06ed444b`  
		Last Modified: Fri, 29 Sep 2023 02:55:37 GMT  
		Size: 35.8 KB (35795 bytes)  
		MIME: application/vnd.in-toto+json
