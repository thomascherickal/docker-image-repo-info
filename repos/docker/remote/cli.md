## `docker:cli`

```console
$ docker pull docker@sha256:49741c18e7e12da7650e4a6c753602e6211e8cb9e5adb51dff661c12167dad50
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:cli` - linux; amd64

```console
$ docker pull docker@sha256:3883944c14659c84ff09fcb089a178664f9df55dcceb545dd432e3cb0aad16e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57096025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c30fb26a5dc1c0a93f053b562cb5afb1e6a3e28f2338d0447314620dac8526b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
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
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:223dfaad4451024cb3c0e6863bfa426834fbe42c7ca5233bbcafccc0bbc016e2`  
		Last Modified: Wed, 27 Sep 2023 00:51:07 GMT  
		Size: 2.0 MB (2014281 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:559d22cffa1e3a7cef63dcd01975632757fbd3e822cdef7fa0c947a0cea2ecb5`  
		Last Modified: Wed, 27 Sep 2023 00:51:07 GMT  
		Size: 16.4 MB (16390435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a98f9133802becfd676d54d249bfb6ef346f4a78a923862bcf8954c51c32d20`  
		Last Modified: Wed, 27 Sep 2023 00:51:08 GMT  
		Size: 17.5 MB (17459265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f032ee91e44aebad24ce746ef5aa92619254e758637694939cc6fa457222bdce`  
		Last Modified: Wed, 27 Sep 2023 00:51:08 GMT  
		Size: 17.8 MB (17828719 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f96fb13784bf175c2d14b327c77267bb7ca4c70f8f88b885db759a4d68d51286`  
		Last Modified: Wed, 27 Sep 2023 00:51:08 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c2dad6e4571e602b1ba998dc0f48a9b939ee4c2f6a79b7d58f6225301f8b0cb0`  
		Last Modified: Wed, 27 Sep 2023 00:51:09 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eb6894b0142bdf94ab7001b6ed8cd7336eff64492f41a8e794774aab87595e86`  
		Last Modified: Wed, 27 Sep 2023 00:51:09 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:00174b06f8f57bb379a4d8901722b03f72e068c2cad0350b3235d37ebc5064f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.9 KB (544883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc8349ee0505e33c62d2f45d9d03dc68bb45dc667cfa860ad34e6fe9f38a74e9`

```dockerfile
```

-	Layers:
	-	`sha256:b31bc16187677e26e1653066913a17db34fcb3389ce44cb24f397bb66b80a2a6`  
		Last Modified: Wed, 27 Sep 2023 00:51:07 GMT  
		Size: 509.1 KB (509090 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:90c7a3ee737e5a0899cf04a81fd1a46a0424e8259d886b6c0a23fcb4ff8fdfa7`  
		Last Modified: Wed, 27 Sep 2023 00:51:07 GMT  
		Size: 35.8 KB (35793 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:e567f55138af168840ad90152c133cc3a61f653cd4e57053157a8f02ef135545
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52848253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b812e034efdb6875bc36f24e4ebe3b51e36bcefcbee0ce8ffb5d924b2095244`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
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
	-	`sha256:767c2a40dc41374be62f00886c074a5c66733ebfa45696a9b8765a285eed5c72`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.4 MB (15438722 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:011855a528fc2a658b48d2b14e37cf356d07a9b1c2cd8641c6a5e7cfa3ccafaf`  
		Last Modified: Wed, 06 Sep 2023 01:23:41 GMT  
		Size: 15.8 MB (15768059 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c5bc81d37c7ce6be347b9be40a203587efc2dbfdea6a46416b69a78aa34e934`  
		Last Modified: Wed, 27 Sep 2023 01:15:56 GMT  
		Size: 16.3 MB (16284432 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d2ffaaea26a94fbe2fec70dfc6c717fc5badfadaedb0a08ea58f9e3c852cd7f`  
		Last Modified: Wed, 27 Sep 2023 01:15:55 GMT  
		Size: 546.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21489bbfa60b9d7dd80c3dea7895312aa816ad54650d4af05287a4f0a1164e28`  
		Last Modified: Wed, 27 Sep 2023 01:15:55 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a037e423567a71c1142b9f7119f73226a5d6c8ed13f724dfb0d98f18c493b2fd`  
		Last Modified: Wed, 27 Sep 2023 01:15:55 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:cli` - unknown; unknown

```console
$ docker pull docker@sha256:98b4c9092631babdfdaa1e9a09b94550f711e23875664e346d7ebd093933d6d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **544.8 KB (544779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a814e40fc9a6c0c5e760fa6c34f1ec3e13bf7e2ec06b463b9756054500e551b0`

```dockerfile
```

-	Layers:
	-	`sha256:abccac56b5763d3195ecbc09c943558dfeea0379665d63679a5a95587dcc9cd4`  
		Last Modified: Wed, 27 Sep 2023 01:15:55 GMT  
		Size: 509.1 KB (509140 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:22177f8aeff7b1adae64f209c679393f1aa87c6ada12c0ef8af653067d01d943`  
		Last Modified: Wed, 27 Sep 2023 01:15:55 GMT  
		Size: 35.6 KB (35639 bytes)  
		MIME: application/vnd.in-toto+json
