## `docker:23-cli`

```console
$ docker pull docker@sha256:ae9763d037a0a1a9c2e88e5ccb89c6a3774549241a8405f6f60002dd93ca8caf
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23-cli` - linux; amd64

```console
$ docker pull docker@sha256:90397e74f9996b32f282d82d6f5eaec6792bb966c3c686a4beb4c76a3c9ff650
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.0 MB (56956449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc476c1f5f0c8f03e018dd6fb5eeb3fe7c13cc1b1748e8b7649aedeb0426f7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 17:04:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 21 Sep 2023 17:04:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Thu, 21 Sep 2023 17:04:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
ENV DOCKER_COMPOSE_VERSION=2.22.0
# Thu, 21 Sep 2023 17:04:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-x86_64'; 			sha256='e849450f1c5c20123aa7d63291e2a818b7a117f2e03e432853ece463dd09e67a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv6'; 			sha256='46cabb4363c5fa66e63c6055b1d0a6fe2c7995350e48f14816a752ae4132231d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv7'; 			sha256='1a0d500eaae3c4ddbfdeb566896207c0628a671065b95d0e8907bca58f91d312'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-aarch64'; 			sha256='572a22000d408fb524258b379bf272a007c8da977c3e8d47c34f4e45dd7b1932'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-ppc64le'; 			sha256='4d1a3e89fdb7641422dc5cbcab48fd2da337b03265cb5ac2858c3425bacf952c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-riscv64'; 			sha256='c45193b98c54e5a898e6b9095f70b0487599f19ce25b579ed2fcc3f868415aff'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-s390x'; 			sha256='716aded74df512728638f1fe53170c46d94c1a085bc5a24108ce7101bc37bd81'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 21 Sep 2023 17:04:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 17:04:14 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0a23e03dd7fa9d249a121b5eaf370bbf9c12a36649b5f21964bfd84fb14e453`  
		Last Modified: Wed, 27 Sep 2023 00:51:16 GMT  
		Size: 2.0 MB (2014282 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:227cce67a311f387a6a2f28751ff8ebc0fdadb14e7593f3025f4f2f9724601bb`  
		Last Modified: Wed, 27 Sep 2023 00:51:16 GMT  
		Size: 16.3 MB (16250859 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f10196a5e68fd819edc7db5cb621a42fd5eebb37ce1768a51eda0a52e947a28e`  
		Last Modified: Wed, 27 Sep 2023 00:51:16 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d2e820ce6683dc1607bc46439ec3efa445052b9339f7d0e9a9e9489de8c969e0`  
		Last Modified: Wed, 27 Sep 2023 00:51:17 GMT  
		Size: 17.8 MB (17828718 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0c2cd27d5f372750c9123d9e3da52a99466f701e60aeaf2d158b3079e87485ab`  
		Last Modified: Wed, 27 Sep 2023 00:51:17 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4273225e53ee222802075fd40e214dd4f9ddfc3c3609c05086a6a61914faf112`  
		Last Modified: Wed, 27 Sep 2023 00:51:17 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c106ed73da7e17527369a74fc9d6637714142e438c9c8ba431118adde9c2134`  
		Last Modified: Wed, 27 Sep 2023 00:51:18 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-cli` - unknown; unknown

```console
$ docker pull docker@sha256:556fdf32450aa8122245ed2591455265befaf9c34b26a7f96e2d7ccc05427b81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.3 KB (544297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbb110e32f0c53d052eec8ad98a9fac411b46d68734a9b849afe6da5a33606ee`

```dockerfile
```

-	Layers:
	-	`sha256:f9b8d5ae0387f2de3ed3b204af13efd134585081830b5b0c79c3e0b512acf870`  
		Last Modified: Wed, 27 Sep 2023 00:51:15 GMT  
		Size: 508.8 KB (508798 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:ab4064657c0220ecfa1524ea5643e528e3d05a8d905bfc07f475766d70cf4efd`  
		Last Modified: Wed, 27 Sep 2023 00:51:15 GMT  
		Size: 35.5 KB (35499 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:0a53374da871bc37fcf70c22c4855b8852267be29e1164e86e4cac86d966dc01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52734610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ba10935ab1229dd464c6b2088760443849819b6394d266dedd4b859fdf7224f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Thu, 21 Sep 2023 17:04:14 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
ENV DOCKER_VERSION=23.0.6
# Thu, 21 Sep 2023 17:04:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Thu, 21 Sep 2023 17:04:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
ENV DOCKER_COMPOSE_VERSION=2.22.0
# Thu, 21 Sep 2023 17:04:14 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-x86_64'; 			sha256='e849450f1c5c20123aa7d63291e2a818b7a117f2e03e432853ece463dd09e67a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv6'; 			sha256='46cabb4363c5fa66e63c6055b1d0a6fe2c7995350e48f14816a752ae4132231d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv7'; 			sha256='1a0d500eaae3c4ddbfdeb566896207c0628a671065b95d0e8907bca58f91d312'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-aarch64'; 			sha256='572a22000d408fb524258b379bf272a007c8da977c3e8d47c34f4e45dd7b1932'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-ppc64le'; 			sha256='4d1a3e89fdb7641422dc5cbcab48fd2da337b03265cb5ac2858c3425bacf952c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-riscv64'; 			sha256='c45193b98c54e5a898e6b9095f70b0487599f19ce25b579ed2fcc3f868415aff'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-s390x'; 			sha256='716aded74df512728638f1fe53170c46d94c1a085bc5a24108ce7101bc37bd81'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 21 Sep 2023 17:04:14 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 21 Sep 2023 17:04:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Sep 2023 17:04:14 GMT
CMD ["sh"]
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
	-	`sha256:e5fa0183f177eef4fbf1985af430c61c77b95421f027eea28f816b0cd1422c2a`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.3 MB (15325086 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ee7e69ab8affe56e6a48d95a413242bda38be403d58d989c83afd66e5ecddeb`  
		Last Modified: Mon, 07 Aug 2023 22:43:59 GMT  
		Size: 15.8 MB (15768048 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6395a2002efaa93792f407e54bc7d2387cb057519bbc23131d195282f6f4ff64`  
		Last Modified: Wed, 27 Sep 2023 02:36:57 GMT  
		Size: 16.3 MB (16284431 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a53825e360f9fad725dcb2b7bd81b1a5a2e66099425a90a15cb069cc28a005c3`  
		Last Modified: Wed, 27 Sep 2023 02:36:56 GMT  
		Size: 548.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d36e24d4e8429f6ac39f7cf1b326c2e86c9423785fa55533943628442b0311f`  
		Last Modified: Wed, 27 Sep 2023 02:36:56 GMT  
		Size: 1.0 KB (1026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9342e50e52776a999048d7e85b45939a42e13c223bc7e8a696a3476a4bf6356e`  
		Last Modified: Wed, 27 Sep 2023 02:36:56 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-cli` - unknown; unknown

```console
$ docker pull docker@sha256:961bcd598b976ce5eddcc54083c92acf4e97593e9e342e38d2b93274b7c361a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.2 KB (544191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0da37d18fdc672c37247e0a3c228444e4056b57e081fe5ede97d1c8f4154d7fa`

```dockerfile
```

-	Layers:
	-	`sha256:8e2e87bdfeb66d6f839801218c55e3ff36bf15f5a33dfec9e020057a83119ffe`  
		Last Modified: Wed, 27 Sep 2023 02:36:56 GMT  
		Size: 508.8 KB (508846 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:bc6429ee8d0cd8e46fc209e62c9cff972be8d193f0f4e2b5c329ace7992c0c9a`  
		Last Modified: Wed, 27 Sep 2023 02:36:56 GMT  
		Size: 35.3 KB (35345 bytes)  
		MIME: application/vnd.in-toto+json
