## `docker:24-cli`

```console
$ docker pull docker@sha256:d5452c2f0fbd383a439022a4e3cd9d19f8eb5bf5bf96749e3213a92d152beb4c
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 5
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:24-cli` - linux; amd64

```console
$ docker pull docker@sha256:e92b413794dfb6fb51d36353d1be137544d5d9402ab15edee67d99f5f5cf590f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57096372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5af48b26d175b77fd5907bdf79e2b105d5500eba302907ed5c0ea00459e316d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 18:22:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_VERSION=24.0.6
# Fri, 29 Sep 2023 18:22:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Fri, 29 Sep 2023 18:22:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_COMPOSE_VERSION=2.22.0
# Fri, 29 Sep 2023 18:22:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-x86_64'; 			sha256='e849450f1c5c20123aa7d63291e2a818b7a117f2e03e432853ece463dd09e67a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv6'; 			sha256='46cabb4363c5fa66e63c6055b1d0a6fe2c7995350e48f14816a752ae4132231d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv7'; 			sha256='1a0d500eaae3c4ddbfdeb566896207c0628a671065b95d0e8907bca58f91d312'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-aarch64'; 			sha256='572a22000d408fb524258b379bf272a007c8da977c3e8d47c34f4e45dd7b1932'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-ppc64le'; 			sha256='4d1a3e89fdb7641422dc5cbcab48fd2da337b03265cb5ac2858c3425bacf952c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-riscv64'; 			sha256='c45193b98c54e5a898e6b9095f70b0487599f19ce25b579ed2fcc3f868415aff'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-s390x'; 			sha256='716aded74df512728638f1fe53170c46d94c1a085bc5a24108ce7101bc37bd81'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 29 Sep 2023 18:22:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 18:22:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6c3b1865084b87380a1c759579197510e1d62c242d4a8f44eb10669961b8219f`  
		Last Modified: Tue, 03 Oct 2023 00:56:09 GMT  
		Size: 2.0 MB (2014278 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:54a726528b5b556fa0b25410027bdb9ab9b0971e15b122767cc40b554f5281ff`  
		Last Modified: Tue, 03 Oct 2023 00:56:10 GMT  
		Size: 16.4 MB (16390432 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a5753e84c889d7939d3759cf7d503ad708909256ed1e587a5f2033da02f5a2c`  
		Last Modified: Tue, 03 Oct 2023 00:56:10 GMT  
		Size: 17.5 MB (17459266 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64810bdae73788879e15e0f00287bfc19b6c11f62110828f56dd9d1338b2f7ed`  
		Last Modified: Tue, 03 Oct 2023 00:56:10 GMT  
		Size: 17.8 MB (17828718 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1018d1edcb4a39296e4b933c8bf65263bf92297ec6d5859382968b4445b609b6`  
		Last Modified: Tue, 03 Oct 2023 00:56:10 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f597a6889ca7d62a500c8c00f32b7c523af0425b4a848482c58c780c207b14ba`  
		Last Modified: Tue, 03 Oct 2023 00:56:11 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89aff94efcc876dd56b6e14ecb14f58e6055a1afdb024fa79528f3c0e64a1142`  
		Last Modified: Tue, 03 Oct 2023 00:56:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:24-cli` - unknown; unknown

```console
$ docker pull docker@sha256:829f24ab4d1614cd9dbb2588697fb809523b6b3ee28ef5e9afe6eb007217fc07
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.3 KB (398259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b08e8161bb74aac4937e59ebc3c3f13aa6f05f03d7d27c91eb2e4906075addbb`

```dockerfile
```

-	Layers:
	-	`sha256:662b5bacacbc647fccc962a360a80c4b6a214fa9bb145888f6253e564b090b3a`  
		Last Modified: Tue, 03 Oct 2023 00:56:09 GMT  
		Size: 362.5 KB (362476 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:5369a9b4c558f70f756c1f427d8790ea6a2a9298f64faacd93fc5a94bd77f5de`  
		Last Modified: Tue, 03 Oct 2023 00:56:09 GMT  
		Size: 35.8 KB (35783 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:24-cli` - linux; arm variant v6

```console
$ docker pull docker@sha256:ab73690b61c9bcbf41dfedbc13a8539043400b78cfe544e94b848d7f7f91a138
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53613747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa523813fab8e27d14c5ec90d4a63ebe71d91da9d018692a551aed0d4550dc93`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 18:22:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_VERSION=24.0.6
# Fri, 29 Sep 2023 18:22:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Fri, 29 Sep 2023 18:22:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_COMPOSE_VERSION=2.22.0
# Fri, 29 Sep 2023 18:22:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-x86_64'; 			sha256='e849450f1c5c20123aa7d63291e2a818b7a117f2e03e432853ece463dd09e67a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv6'; 			sha256='46cabb4363c5fa66e63c6055b1d0a6fe2c7995350e48f14816a752ae4132231d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv7'; 			sha256='1a0d500eaae3c4ddbfdeb566896207c0628a671065b95d0e8907bca58f91d312'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-aarch64'; 			sha256='572a22000d408fb524258b379bf272a007c8da977c3e8d47c34f4e45dd7b1932'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-ppc64le'; 			sha256='4d1a3e89fdb7641422dc5cbcab48fd2da337b03265cb5ac2858c3425bacf952c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-riscv64'; 			sha256='c45193b98c54e5a898e6b9095f70b0487599f19ce25b579ed2fcc3f868415aff'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-s390x'; 			sha256='716aded74df512728638f1fe53170c46d94c1a085bc5a24108ce7101bc37bd81'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 29 Sep 2023 18:22:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 18:22:05 GMT
CMD ["sh"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608526548bfc9b9f9d78884918653f8ae17b49fd4e6fa1ca52ab837d1f4dbdaf`  
		Last Modified: Tue, 03 Oct 2023 00:57:00 GMT  
		Size: 2.1 MB (2088611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca4348b56d5f1b183cae111d92be2491bd1d0eb5274a7afa1815f2718d0acbc`  
		Last Modified: Tue, 03 Oct 2023 00:57:02 GMT  
		Size: 15.1 MB (15122154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ece89c3e55993fcdf039970f3ebb3e0f452cfb1882f5d0cecb372ed77961885`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.4 MB (16403196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbb5bd24945e00202545942ce697624a135e76faa8ae183433a28792329ae85`  
		Last Modified: Tue, 03 Oct 2023 00:57:01 GMT  
		Size: 16.9 MB (16852788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a9c16a47e6e57d671f3717e39355f4ee39b3238d97ac00baf498e53e6170cf`  
		Last Modified: Tue, 03 Oct 2023 00:56:58 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ccad03f2bb06a2fe8d15271ecee1edd473687c5b2d99b74937cb2584c86b44`  
		Last Modified: Tue, 03 Oct 2023 00:56:58 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffac5b4954a22669ccfcf48b4b5471d9ab0664a4aecaa540eda45281aae63db9`  
		Last Modified: Tue, 03 Oct 2023 00:56:58 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:24-cli` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:106881fc5255fd994b13af5e4526213e951a0285cb5dd735e6312e0d2e1c8d3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52849290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9caf38d29093ea430f65702e5763b6b1bf946828ddc84f590e5f14f09d294f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 18:22:05 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_VERSION=24.0.6
# Fri, 29 Sep 2023 18:22:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Fri, 29 Sep 2023 18:22:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_COMPOSE_VERSION=2.22.0
# Fri, 29 Sep 2023 18:22:05 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-x86_64'; 			sha256='e849450f1c5c20123aa7d63291e2a818b7a117f2e03e432853ece463dd09e67a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv6'; 			sha256='46cabb4363c5fa66e63c6055b1d0a6fe2c7995350e48f14816a752ae4132231d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv7'; 			sha256='1a0d500eaae3c4ddbfdeb566896207c0628a671065b95d0e8907bca58f91d312'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-aarch64'; 			sha256='572a22000d408fb524258b379bf272a007c8da977c3e8d47c34f4e45dd7b1932'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-ppc64le'; 			sha256='4d1a3e89fdb7641422dc5cbcab48fd2da337b03265cb5ac2858c3425bacf952c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-riscv64'; 			sha256='c45193b98c54e5a898e6b9095f70b0487599f19ce25b579ed2fcc3f868415aff'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-s390x'; 			sha256='716aded74df512728638f1fe53170c46d94c1a085bc5a24108ce7101bc37bd81'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Fri, 29 Sep 2023 18:22:05 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Fri, 29 Sep 2023 18:22:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 18:22:05 GMT
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

### `docker:24-cli` - unknown; unknown

```console
$ docker pull docker@sha256:e87c187c569fb1d27c2ba2aec6bc1c285632c3775f50267dcc766ca0de73a401
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.1 KB (398120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8e66d35cf977070cfa8385c08865e8df7127e4ed482c74232463f13a686e5f0`

```dockerfile
```

-	Layers:
	-	`sha256:2984dd2157317124f685bcb1bb979f923d0004827282e99e11254605055fbb80`  
		Last Modified: Tue, 03 Oct 2023 00:57:39 GMT  
		Size: 362.5 KB (362491 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:85322377545cccedf0e839df55b6557a268b0f67c967e3272e13d2dbfc2c3275`  
		Last Modified: Tue, 03 Oct 2023 00:57:39 GMT  
		Size: 35.6 KB (35629 bytes)  
		MIME: application/vnd.in-toto+json
