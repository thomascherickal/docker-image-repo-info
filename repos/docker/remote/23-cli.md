## `docker:23-cli`

```console
$ docker pull docker@sha256:5f85260f1c78cfd796463b51fd000ff9f033d88b7047739f79c6df9d0fb531d4
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23-cli` - linux; amd64

```console
$ docker pull docker@sha256:16737a2ba8f12e0289bf6b727e6ac377380e4667a6e5707b7963fced434e5e25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57112728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95eded59f32e7afc8ecaedb82316f296b68cf9b5b782541d95d011c6ad2dfbbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Wed, 19 Jul 2023 17:04:16 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 19 Jul 2023 17:04:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 17:04:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 17:04:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-x86_64'; 			sha256='b9385dabb7931636a3afc0aee94625ebff3bb29584493a87804afb6ebaf2d916'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv6'; 			sha256='39cef332454d1c7a26e12f8d9ee297908d1da9cb71112ede1816c550766ddb8e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv7'; 			sha256='139275f3453761b46f0837a4e4c2a00883b778abee997e299c52e1bcf3d8fc9f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-aarch64'; 			sha256='e63a24e57d2104a09b37ee6aa04c76f4ae85bdf7a59e1bf79adc6d5f55340a31'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-ppc64le'; 			sha256='9c08eb875a7ffd4a832a585540a4c9c81da5dcab263ec3e704ab1d62b573636f'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-riscv64'; 			sha256='5a3bff32ecf0a5a38a83afeb3dc2effd8ca3d52eb2e07ec000334663d493055b'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-s390x'; 			sha256='297be6a0ece070ae95d5caf91a23b89dc1b2563e928db80eee480d7018919ee6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 19 Jul 2023 17:04:16 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jul 2023 17:04:16 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7b009ac550c3e2a03a9064b92b7dfcee35a891a4e4d3d9bf1823121d28d2235`  
		Last Modified: Mon, 31 Jul 2023 21:05:20 GMT  
		Size: 2.0 MB (2014272 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:690c96a00a63b069dfab0d1669ffa06a5fad2cf7ea9a44b0272d8573cca502db`  
		Last Modified: Mon, 31 Jul 2023 21:05:21 GMT  
		Size: 16.3 MB (16250847 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bf3e29f935573f53f50b85dba19222de187cbe88adb55f83cdad7bc8450c1e79`  
		Last Modified: Mon, 31 Jul 2023 21:05:21 GMT  
		Size: 17.5 MB (17459265 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65713abcfd3dc1cb1543d9b31d777eecd5d3ee296c28a48cf7c1111e8b43985d`  
		Last Modified: Mon, 31 Jul 2023 21:05:21 GMT  
		Size: 18.0 MB (17988752 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fe0f80b5292f60962a86ccc66ec4d428dea37627ce4fd0ded032f23e1342618`  
		Last Modified: Mon, 31 Jul 2023 21:05:21 GMT  
		Size: 545.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:634b6ef888e513d197016b36ad562031fcb416a45641db552cd9d6bb99264d4e`  
		Last Modified: Mon, 31 Jul 2023 21:05:22 GMT  
		Size: 1.0 KB (1020 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e9f05d98f1d35b5cda3fd9bece2c54752959afc417af2b1b6164e357b0b69b8`  
		Last Modified: Mon, 31 Jul 2023 21:05:22 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-cli` - unknown; unknown

```console
$ docker pull docker@sha256:c834dd5ae29242c745b777be1c501682470751fc1bdd39afba0f2f475c710bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **534.6 KB (534629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37bdd4e2c2f822976cb9d013d5e9edf3e3103f546841d74f7be62b892cf3bd3`

```dockerfile
```

-	Layers:
	-	`sha256:72f8b0ced2687201272ffe5b478396302f8f112e8e361b5d2990d89628a5e753`  
		Last Modified: Mon, 31 Jul 2023 21:05:19 GMT  
		Size: 499.1 KB (499054 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d91061f5bfba288552235f78488e0bf1c3fcfe147f7e61d414241d38f12d7bc0`  
		Last Modified: Mon, 31 Jul 2023 21:05:19 GMT  
		Size: 35.6 KB (35575 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:ee9ef81c22cf3a88efd38ac37141af86a3ea4855a5aa9ce74b680a05e6938902
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52769472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3815741d33b57263dcf7d3131138c5f48841479c50dc19711a4df76da0c22e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Wed, 14 Jun 2023 20:48:58 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Wed, 14 Jun 2023 20:48:58 GMT
CMD ["/bin/sh"]
# Wed, 19 Jul 2023 17:04:16 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
ENV DOCKER_VERSION=23.0.6
# Wed, 19 Jul 2023 17:04:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Wed, 19 Jul 2023 17:04:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Wed, 19 Jul 2023 17:04:16 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-x86_64'; 			sha256='b9385dabb7931636a3afc0aee94625ebff3bb29584493a87804afb6ebaf2d916'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv6'; 			sha256='39cef332454d1c7a26e12f8d9ee297908d1da9cb71112ede1816c550766ddb8e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv7'; 			sha256='139275f3453761b46f0837a4e4c2a00883b778abee997e299c52e1bcf3d8fc9f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-aarch64'; 			sha256='e63a24e57d2104a09b37ee6aa04c76f4ae85bdf7a59e1bf79adc6d5f55340a31'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-ppc64le'; 			sha256='9c08eb875a7ffd4a832a585540a4c9c81da5dcab263ec3e704ab1d62b573636f'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-riscv64'; 			sha256='5a3bff32ecf0a5a38a83afeb3dc2effd8ca3d52eb2e07ec000334663d493055b'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-s390x'; 			sha256='297be6a0ece070ae95d5caf91a23b89dc1b2563e928db80eee480d7018919ee6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Wed, 19 Jul 2023 17:04:16 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Wed, 19 Jul 2023 17:04:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 19 Jul 2023 17:04:16 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:8c6d1654570f041603f4cef49c320c8f6f3e401324913009d92a19132cbf1ac0`  
		Last Modified: Wed, 14 Jun 2023 20:49:23 GMT  
		Size: 3.3 MB (3329251 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b5f9fdad9390b07a997877201870a12f621bb382a172bbb0ab30d45714d52ff`  
		Last Modified: Mon, 31 Jul 2023 16:26:17 GMT  
		Size: 2.0 MB (2024545 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b19fcc23e7ae7b7552136cc77b761b1322e21d733ba774f8f777109f4d6c904`  
		Last Modified: Mon, 31 Jul 2023 16:29:00 GMT  
		Size: 15.3 MB (15325084 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98705cb96065f56d01334f7f31820bdccd885abbbe961458ed70ff79141017e5`  
		Last Modified: Mon, 31 Jul 2023 16:29:00 GMT  
		Size: 15.8 MB (15768057 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b35edb5cc7a50d1c435828b1f1821e3dbcffb2ac57773793a81aece3cb94a3d0`  
		Last Modified: Mon, 31 Jul 2023 16:29:00 GMT  
		Size: 16.3 MB (16320824 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18279d02e647b43b46704668b8bc9ef16004e86378742abe187281f5091fd470`  
		Last Modified: Mon, 31 Jul 2023 16:28:59 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a040fa41835ede99fc08feb977a808bdedf94c10d3b048bfda8593e0b9a92f88`  
		Last Modified: Mon, 31 Jul 2023 16:29:00 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f933fc905ae9bf2867c48fca451185090540304229831fc8c8225dbb464ab9b2`  
		Last Modified: Mon, 31 Jul 2023 16:29:01 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-cli` - unknown; unknown

```console
$ docker pull docker@sha256:a578dc9c68718e0e4a58f6de285c729524b56ef9c1ed0e149f17b3630feb29eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **534.5 KB (534497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b99ef5b049d821fd8dbe53af06a5d2176b25413401265ea856f454d238bbd1c`

```dockerfile
```

-	Layers:
	-	`sha256:633dc7d838be66ab8e6f809934cad84a6c4455706dfdb8255534a03af595190d`  
		Last Modified: Mon, 31 Jul 2023 16:28:59 GMT  
		Size: 499.1 KB (499079 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:266965f4d7e492c776d8dd1e77267e4c007c54c0eca41ac164d58e0a5527a4a5`  
		Last Modified: Mon, 31 Jul 2023 16:28:59 GMT  
		Size: 35.4 KB (35418 bytes)  
		MIME: application/vnd.in-toto+json
