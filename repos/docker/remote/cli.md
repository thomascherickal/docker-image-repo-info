## `docker:cli`

```console
$ docker pull docker@sha256:24337de8d3d8e9ef43c4261d5a63c8243f345046e9a595f6abe9965cb084947d
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:cli` - linux; amd64

```console
$ docker pull docker@sha256:e25e39e7693e0bfca0595a68407d8c52c34841a0d5cfc7ee3ab3ee27ab613ac8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.3 MB (57252535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c93b90e8844566bd9e23ef4a94bfb402b0483d02f77df3e6a6314213b8bb87ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:f0b599822d6b02dd6e83654b9bac43433a82c86df5daf847261ce4c3078c9c36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **535.2 KB (535211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a09c6579a33be3ada161e438f1a3b6eed91b0e38e0ec1cd4dd26dc19aa71a7ad`

```dockerfile
```

-	Layers:
	-	`sha256:56713251b62105fa48022fc8c35d7dc455ab29da9d57dce754f630225e1ad4ed`  
		Last Modified: Fri, 28 Jul 2023 22:18:33 GMT  
		Size: 499.3 KB (499344 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7a4aacab7498b6f970025ce66ad791a33295321fd3b06d12fcaf5b97a310aa85`  
		Last Modified: Fri, 28 Jul 2023 22:18:33 GMT  
		Size: 35.9 KB (35867 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b9cb4acc78f2dc0884e1dc01e2009d9ac22adf9abfb02e4096747c5ad963be4e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52881367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56cd16c9eab27aae1e7449756896e5ddb29709b25b71552d41f85aa6b9c1e59a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

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

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:d296d00612d3483b94e7c0fc806a379587bc22075306842ffd3600a59b18b845
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.8 KB (541828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74991e76fb4b8dd2ca57cdae8fce10581d2ae1b94419276c5080a96c4b2c9cc5`

```dockerfile
```

-	Layers:
	-	`sha256:36a92bcf4f3b0e9cf5c7695f0d0cd16ccaf7197797a35880da35c9da09fb7d6a`  
		Last Modified: Mon, 07 Aug 2023 22:18:57 GMT  
		Size: 506.0 KB (506023 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:114e845150c204a2e4baa3988c79e902caf0d23825aae48f81cb16ed8abf4036`  
		Last Modified: Mon, 07 Aug 2023 22:18:56 GMT  
		Size: 35.8 KB (35805 bytes)  
		MIME: application/vnd.in-toto+json
