## `docker:23-git`

```console
$ docker pull docker@sha256:7adc97903031eea62fdb217b301c4f638a44d02e58f1255ef79429126e42f574
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:23-git` - linux; amd64

```console
$ docker pull docker@sha256:5559bba76cd2482a12e29ceb3a78867d5b5eb488867d5135200066567bf8ad12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122976700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:706a3b31ab84af0354f137a6b38a9275161e5eb16306013db944fb4272d811d3`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-x86_64'; 			sha256='b9385dabb7931636a3afc0aee94625ebff3bb29584493a87804afb6ebaf2d916'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv6'; 			sha256='39cef332454d1c7a26e12f8d9ee297908d1da9cb71112ede1816c550766ddb8e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv7'; 			sha256='139275f3453761b46f0837a4e4c2a00883b778abee997e299c52e1bcf3d8fc9f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-aarch64'; 			sha256='e63a24e57d2104a09b37ee6aa04c76f4ae85bdf7a59e1bf79adc6d5f55340a31'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-ppc64le'; 			sha256='9c08eb875a7ffd4a832a585540a4c9c81da5dcab263ec3e704ab1d62b573636f'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-riscv64'; 			sha256='5a3bff32ecf0a5a38a83afeb3dc2effd8ca3d52eb2e07ec000334663d493055b'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-s390x'; 			sha256='297be6a0ece070ae95d5caf91a23b89dc1b2563e928db80eee480d7018919ee6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
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
	-	`sha256:d42d2b0a5c2295606a1cfc119ea62fc1ac5d8976df977641ae78c200c424cf76`  
		Last Modified: Mon, 31 Jul 2023 21:50:43 GMT  
		Size: 9.3 MB (9266204 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:044c6cac6229b417ac5ef611f845fd1553e70137789c3c4fab541ad37345a799`  
		Last Modified: Mon, 31 Jul 2023 21:50:42 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:597a5cd0881525f7ded046c9c317ea06ef3771bdc96da65219ff449d2f26d087`  
		Last Modified: Mon, 31 Jul 2023 21:50:47 GMT  
		Size: 51.7 MB (51657422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fc6fd83155b7486ba43c2df471d93e141361eeb6f5e14f56b34ba46ba395354`  
		Last Modified: Mon, 31 Jul 2023 21:50:42 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d9b9e0a716ac27aef7c9f9b165735b0a75d7333f9b0539e1d0508575ab5fbc7a`  
		Last Modified: Mon, 31 Jul 2023 21:50:43 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c8aaae80151e16e799244e2d5e83e2531ce9006f43734b5152356c85611e2cac`  
		Last Modified: Mon, 31 Jul 2023 22:05:57 GMT  
		Size: 4.9 MB (4935226 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-git` - unknown; unknown

```console
$ docker pull docker@sha256:4c6656b479f934d3791b3ddf2dde9a98d4c8c481650d1580fecf694302fce4b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **812.0 KB (811963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fea76e1cedb41b8318eec6f1a1a56c5493e161ad088ca0ae7eabeca1c6dab78`

```dockerfile
```

-	Layers:
	-	`sha256:b88713d5db088cf1b3ce39a25d67206cae5f6b66638d73fe8bef1769640b5b3c`  
		Last Modified: Mon, 31 Jul 2023 22:05:57 GMT  
		Size: 799.4 KB (799350 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:40f9a78a200e71adbc7574c4d19e2eccba058ef789ef76d6e866c56215e9474f`  
		Last Modified: Mon, 31 Jul 2023 22:05:57 GMT  
		Size: 12.6 KB (12613 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:23-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b4423e69da44672fde7267d61db77c102c05660115162c48ac20dfd56ef51ff4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.2 MB (114208810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408c64166097740c98ce08ac0d528ccc578c3720ac42659d0367546ff536c4ce`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 16 May 2023 17:59:38 GMT
ADD file:289c2fac17119508ced527225d445747cd177111b4a0018a6b04948ecb3b5e29 in / 
# Tue, 16 May 2023 17:59:38 GMT
CMD ["/bin/sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_VERSION=23.0.6
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_COMPOSE_VERSION=2.20.2
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-x86_64'; 			sha256='b9385dabb7931636a3afc0aee94625ebff3bb29584493a87804afb6ebaf2d916'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv6'; 			sha256='39cef332454d1c7a26e12f8d9ee297908d1da9cb71112ede1816c550766ddb8e'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-armv7'; 			sha256='139275f3453761b46f0837a4e4c2a00883b778abee997e299c52e1bcf3d8fc9f'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-aarch64'; 			sha256='e63a24e57d2104a09b37ee6aa04c76f4ae85bdf7a59e1bf79adc6d5f55340a31'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-ppc64le'; 			sha256='9c08eb875a7ffd4a832a585540a4c9c81da5dcab263ec3e704ab1d62b573636f'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-riscv64'; 			sha256='5a3bff32ecf0a5a38a83afeb3dc2effd8ca3d52eb2e07ec000334663d493055b'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-linux-s390x'; 			sha256='297be6a0ece070ae95d5caf91a23b89dc1b2563e928db80eee480d7018919ee6'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 16 May 2023 17:59:38 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD ["sh"]
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-23.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-23.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-23.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-23.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 16 May 2023 17:59:38 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 16 May 2023 17:59:38 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 16 May 2023 17:59:38 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 16 May 2023 17:59:38 GMT
VOLUME [/var/lib/docker]
# Tue, 16 May 2023 17:59:38 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 16 May 2023 17:59:38 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 16 May 2023 17:59:38 GMT
CMD []
# Tue, 16 May 2023 17:59:38 GMT
RUN apk add --no-cache git # buildkit
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
	-	`sha256:848981db39f52f9f6985d5cddbb14c147d693e0685ed148669ad7a9163eb2327`  
		Last Modified: Mon, 31 Jul 2023 18:26:51 GMT  
		Size: 9.4 MB (9359365 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7ce5edd10000b139cd3b8576c13114e5165d1ad716d73a99782a58db3fc62c9`  
		Last Modified: Mon, 31 Jul 2023 18:26:50 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:de53d5d758ff4892567265e18dd4646ae6ca92b815abef3302df8f21a8c14004`  
		Last Modified: Mon, 31 Jul 2023 18:26:54 GMT  
		Size: 47.1 MB (47053308 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b061d4f2b252dbe0daebf9e1bb19479cea27827bf5f174bb94983b739bea6af`  
		Last Modified: Mon, 31 Jul 2023 18:26:51 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c1cc68b8290f08e636b7999c7d4998aa66cfca4cd8ece0022d5c4129384c51c0`  
		Last Modified: Mon, 31 Jul 2023 18:26:51 GMT  
		Size: 2.8 KB (2787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b014092d1a99123d738785a01d2f6052fe61e6ed3498eb1d52fa15e47082260`  
		Last Modified: Mon, 31 Jul 2023 19:07:13 GMT  
		Size: 5.0 MB (5021547 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:23-git` - unknown; unknown

```console
$ docker pull docker@sha256:d10931824139faba87f02a1a4be36a6ed4be48d9cb97ac3d0e29e4b78fdd4ea7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **802.4 KB (802377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b85cd422504d0c58270385bba640260676ac35c2ac829981ea47644fa60dfae8`

```dockerfile
```

-	Layers:
	-	`sha256:e6d38558fdbc018d39125188c646b210e53a933f7578c10ee9be0c7b8804b1c1`  
		Last Modified: Mon, 31 Jul 2023 19:07:13 GMT  
		Size: 791.9 KB (791931 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:28b012a2295fc94be2b199b503f772f0d214bdd9c89ee2b2f65284b0a15034c9`  
		Last Modified: Mon, 31 Jul 2023 19:07:13 GMT  
		Size: 10.4 KB (10446 bytes)  
		MIME: application/vnd.in-toto+json
