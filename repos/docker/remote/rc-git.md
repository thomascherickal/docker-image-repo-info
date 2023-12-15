## `docker:rc-git`

```console
$ docker pull docker@sha256:80ba70d03c596576f1a060a9a87c245ddbeb79e50644681bef5443f9ede75365
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:rc-git` - linux; amd64

```console
$ docker pull docker@sha256:e6bc612e6df390f62b1ef9208e613afaf7dd7765763baaf4e233c827c4ebab2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125174122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:178b2b731e3d884f9acb42b3229fa56082c50689a540e43f0517365968efd552`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 13 Nov 2023 22:06:12 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.2
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.3
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-x86_64'; 			sha256='a836e807951db448f991f303cddcc9a4ec69f4a49d58bc7d536cb91c77c04c33'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv6'; 			sha256='b712693945360155842b578beace00effa723b604bfe1ccd6421645523e15d86'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv7'; 			sha256='4068bcbe1dd90034c8fe8d2c65b600ba793fc19bdb65db3c2dbf80b8a078de6c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-aarch64'; 			sha256='71f38f0923b8a9b80ad02c823ec3207d94677547aa5c618ca41b81d29fe6b9d9'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-ppc64le'; 			sha256='6110b0d30baee103c98ca5503bea24acb9d52bd333a67d3bf3c57d383c585c62'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-riscv64'; 			sha256='3ac26e5f272deb1364c9b8760af44c4dbd87d6faa42fc53bfec95885cfa8ae77'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-s390x'; 			sha256='2886dd4eddaea1eeb03537bdc596ec8947eb3ef7908c955284f8aad9170d3098'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache iptables-legacy; 	mkdir -p /usr/local/sbin/.iptables-legacy; 	for f in 		iptables 		iptables-save 		iptables-restore 		ip6tables 		ip6tables-save 		ip6tables-restore 	; do 		b="/sbin/${f/tables/tables-legacy}"; 		"$b" --version; 		ln -svT "$b" "/usr/local/sbin/.iptables-legacy/$f"; 	done; 	export PATH="/usr/local/sbin/.iptables-legacy:$PATH"; 	iptables --version | grep legacy # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DIND_COMMIT=65cfcc28ab37cb75e1560e4b4738719c07c6618e
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/var/lib/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD []
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fc52a27149e708d7ee7fe87e2bfb36b1580c10498ed79434486393d2c9007415`  
		Last Modified: Thu, 14 Dec 2023 21:51:24 GMT  
		Size: 2.0 MB (2011658 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4397437e724813265ed8dcc1f187149da017c621940458750e069700749853a0`  
		Last Modified: Thu, 14 Dec 2023 21:51:30 GMT  
		Size: 16.9 MB (16879771 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f04b53a848df22a93af5e6c6fc6072bfe986c97ecad16c149953ce2716eba678`  
		Last Modified: Thu, 14 Dec 2023 21:51:25 GMT  
		Size: 17.2 MB (17195295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69c523561410ee97dc4ae9a0eadfb4d1efe928954100f9a6fbdb4951fe74480c`  
		Last Modified: Thu, 14 Dec 2023 21:51:25 GMT  
		Size: 17.9 MB (17852073 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1ddf68211061c59d4d3f554d0b3856dfc4d5bf89b36c17a296434301bac63882`  
		Last Modified: Thu, 14 Dec 2023 21:51:25 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f88bf149788702cc862e90a3a38be008df21aa736389079123e782fcb711e582`  
		Last Modified: Thu, 14 Dec 2023 21:51:26 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a05634c6b39367f5f73d8114319bb26a0f0bed6ee347b80ce443555e2c14494`  
		Last Modified: Thu, 14 Dec 2023 21:51:26 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:398be9bc47df025b8bfcefa5879176cb2095a7ee1b0f737aff06b0c784898690`  
		Last Modified: Fri, 15 Dec 2023 19:20:11 GMT  
		Size: 7.1 MB (7068026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d98ca7dcf2ac7fedb36ad960c2538adf1fee42681b77d38a795e559729201217`  
		Last Modified: Fri, 15 Dec 2023 19:20:10 GMT  
		Size: 83.6 KB (83633 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:22947852c2693615e92f565b5a5db68f2a7c357831036cec061b8dae7959cfb0`  
		Last Modified: Fri, 15 Dec 2023 19:20:10 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a3998cddf436b674a89cd0d22372b6d7a416052c44e168d854ffa908012385c`  
		Last Modified: Fri, 15 Dec 2023 19:20:11 GMT  
		Size: 55.5 MB (55546290 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b4cf6cdcd929c4a65aa906f2691bef72d41663e652a3833f8f9edd3c5282ffe`  
		Last Modified: Fri, 15 Dec 2023 19:20:11 GMT  
		Size: 1.5 KB (1509 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c68fb67d207fbc7c3b2ac6039dde76b767bb4cd216bbc5213180b298632693c6`  
		Last Modified: Fri, 15 Dec 2023 19:20:11 GMT  
		Size: 2.9 KB (2872 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f88a99581a0851ea902e6377cc8adfe1241f6f26bb0d1c0d6737920397cfb1ea`  
		Last Modified: Fri, 15 Dec 2023 19:42:01 GMT  
		Size: 5.1 MB (5121513 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:rc-git` - unknown; unknown

```console
$ docker pull docker@sha256:1cf9f0634861ac4c7e4aec37de9232eadff7c10ac2ae04eca5f7b4d0ae9ed515
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **743.9 KB (743937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d87ddaad9ae7703609b15bbba714159470d2e7fc36c530411d58339b575986b`

```dockerfile
```

-	Layers:
	-	`sha256:27994f9306c043cacf30e37a6ee850cf2db734105edd82330ec4ae104c468412`  
		Last Modified: Fri, 15 Dec 2023 19:42:00 GMT  
		Size: 730.8 KB (730806 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:68c65906d35e6da134becdfda1e5fb3fd179df2bf65ea79cd93d0c326c384f05`  
		Last Modified: Fri, 15 Dec 2023 19:42:00 GMT  
		Size: 13.1 KB (13131 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:rc-git` - linux; arm variant v6

```console
$ docker pull docker@sha256:c6c90218d9a1f311730247f8ce9baab29c8761cae966bd44287946c962f67803
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.0 MB (117959553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:522b90d612421a9b0e2029c04cb818565702775d7a4cc4d27b12ee7787c3662b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 13 Nov 2023 22:06:12 GMT
ADD file:d43ed267a41631ce0e5a4ef5aac821a75300a83f85ecb6259f5616852f89e989 in / 
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.2
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.3
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-x86_64'; 			sha256='a836e807951db448f991f303cddcc9a4ec69f4a49d58bc7d536cb91c77c04c33'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv6'; 			sha256='b712693945360155842b578beace00effa723b604bfe1ccd6421645523e15d86'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv7'; 			sha256='4068bcbe1dd90034c8fe8d2c65b600ba793fc19bdb65db3c2dbf80b8a078de6c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-aarch64'; 			sha256='71f38f0923b8a9b80ad02c823ec3207d94677547aa5c618ca41b81d29fe6b9d9'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-ppc64le'; 			sha256='6110b0d30baee103c98ca5503bea24acb9d52bd333a67d3bf3c57d383c585c62'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-riscv64'; 			sha256='3ac26e5f272deb1364c9b8760af44c4dbd87d6faa42fc53bfec95885cfa8ae77'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-s390x'; 			sha256='2886dd4eddaea1eeb03537bdc596ec8947eb3ef7908c955284f8aad9170d3098'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache iptables-legacy; 	mkdir -p /usr/local/sbin/.iptables-legacy; 	for f in 		iptables 		iptables-save 		iptables-restore 		ip6tables 		ip6tables-save 		ip6tables-restore 	; do 		b="/sbin/${f/tables/tables-legacy}"; 		"$b" --version; 		ln -svT "$b" "/usr/local/sbin/.iptables-legacy/$f"; 	done; 	export PATH="/usr/local/sbin/.iptables-legacy:$PATH"; 	iptables --version | grep legacy # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DIND_COMMIT=65cfcc28ab37cb75e1560e4b4738719c07c6618e
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/var/lib/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD []
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:0803c38384d9fd0f9afaec8fd13d267547b660dcd46bb92a3d63c5d76e78b04c`  
		Last Modified: Fri, 08 Dec 2023 01:49:33 GMT  
		Size: 3.2 MB (3165143 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6e700a29d71792cc9368bd3cb3281d3b0873b32d1d8593483d3c20b3ef7c4bab`  
		Last Modified: Thu, 14 Dec 2023 21:55:41 GMT  
		Size: 2.1 MB (2099460 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cbdb0cea91510553c7d86c70a0f8cc5aaaa095b73dc7e0e1eda0232611f1dd77`  
		Last Modified: Thu, 14 Dec 2023 21:55:42 GMT  
		Size: 15.3 MB (15263644 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:373d0862416b6164530fb4cb48701610990e80409f1b6105f381d4a36d732d88`  
		Last Modified: Thu, 14 Dec 2023 21:55:42 GMT  
		Size: 16.1 MB (16099975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1904017fd425fca82fa83ff14832922083b0c99645713a256de4062b1aecb5ca`  
		Last Modified: Thu, 14 Dec 2023 21:55:42 GMT  
		Size: 16.9 MB (16867501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:32313784065eb91b679fe6d31831faef4d520330aef9ad851a4e081a0f7a35fd`  
		Last Modified: Thu, 14 Dec 2023 21:55:42 GMT  
		Size: 541.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c23502e1992998f8c7d88a860c2800d4088642b146267269834e572f8187443`  
		Last Modified: Thu, 14 Dec 2023 21:55:43 GMT  
		Size: 1.0 KB (1016 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:986ecac1281a73ae909ad3fc231886d7290a7f28333df2389300c6a0449cda6a`  
		Last Modified: Thu, 14 Dec 2023 21:55:43 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3fe79bc49d76bc5a4694742f93c5ef5a3766f993e285c5b692f24ac42236360f`  
		Last Modified: Thu, 14 Dec 2023 23:54:37 GMT  
		Size: 7.4 MB (7361975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:556f08f1f12a987de44e84cbb475b9accb129668d8feebfa52e77011e02dd28c`  
		Last Modified: Fri, 15 Dec 2023 19:23:58 GMT  
		Size: 82.6 KB (82606 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b78a1d4a2dfedda600e1d483f66d5ef8e4f9c6bf94d5064525484d063f8bd0eb`  
		Last Modified: Fri, 15 Dec 2023 19:23:58 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1cf06c66f62c9254e9cfad7a2b96034b200dfea703c311cbf13b88fe18033614`  
		Last Modified: Fri, 15 Dec 2023 19:24:00 GMT  
		Size: 51.9 MB (51910190 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:27f43c64df4effbc20bdd850c4b593cb90c7d2f1249e46351c9ca5238007464b`  
		Last Modified: Fri, 15 Dec 2023 19:23:59 GMT  
		Size: 1.5 KB (1516 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d0338f45b9d5ed16001ce18ff3409ce016d3046ef79a72ce8cde43395f45d097`  
		Last Modified: Fri, 15 Dec 2023 19:23:59 GMT  
		Size: 2.9 KB (2881 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1cf158870a2da62c7beaa95d5aa67b64965a4f6c5764dbfae7f9c8519d423c20`  
		Last Modified: Fri, 15 Dec 2023 19:46:00 GMT  
		Size: 5.1 MB (5101662 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:rc-git` - unknown; unknown

```console
$ docker pull docker@sha256:adad129723a1b3d1c443fafd72ea095c481f980210cfa675732518bbadba25ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.0 KB (13002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c02d9b840645ac5bb60f5995f380b7772a0c7251116b9c9d98e1a79d26797f7`

```dockerfile
```

-	Layers:
	-	`sha256:8cc7d5e94c2fc0516c62b8a68df0a19b17322919430be7b68affc55e8b02ed1e`  
		Last Modified: Fri, 15 Dec 2023 19:45:59 GMT  
		Size: 13.0 KB (13002 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:rc-git` - linux; arm variant v7

```console
$ docker pull docker@sha256:dc50b8998c43130519dc2b172bf2586098ae567f05262be3176675215f82a22b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.3 MB (116309366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c0cf2925472b19c8978cccc03f893b3f0bd1716caccbfb8dfec3477d0850a76`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 13 Nov 2023 22:06:12 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.2
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.3
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-x86_64'; 			sha256='a836e807951db448f991f303cddcc9a4ec69f4a49d58bc7d536cb91c77c04c33'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv6'; 			sha256='b712693945360155842b578beace00effa723b604bfe1ccd6421645523e15d86'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv7'; 			sha256='4068bcbe1dd90034c8fe8d2c65b600ba793fc19bdb65db3c2dbf80b8a078de6c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-aarch64'; 			sha256='71f38f0923b8a9b80ad02c823ec3207d94677547aa5c618ca41b81d29fe6b9d9'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-ppc64le'; 			sha256='6110b0d30baee103c98ca5503bea24acb9d52bd333a67d3bf3c57d383c585c62'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-riscv64'; 			sha256='3ac26e5f272deb1364c9b8760af44c4dbd87d6faa42fc53bfec95885cfa8ae77'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-s390x'; 			sha256='2886dd4eddaea1eeb03537bdc596ec8947eb3ef7908c955284f8aad9170d3098'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache iptables-legacy; 	mkdir -p /usr/local/sbin/.iptables-legacy; 	for f in 		iptables 		iptables-save 		iptables-restore 		ip6tables 		ip6tables-save 		ip6tables-restore 	; do 		b="/sbin/${f/tables/tables-legacy}"; 		"$b" --version; 		ln -svT "$b" "/usr/local/sbin/.iptables-legacy/$f"; 	done; 	export PATH="/usr/local/sbin/.iptables-legacy:$PATH"; 	iptables --version | grep legacy # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DIND_COMMIT=65cfcc28ab37cb75e1560e4b4738719c07c6618e
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/var/lib/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD []
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:40f7102b17e4ec828559672f3388bba1ec86d87e7aa09caba4b82fc6870b4fa6`  
		Last Modified: Thu, 14 Dec 2023 22:03:12 GMT  
		Size: 1.9 MB (1888652 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a3f5c26cb0f3d7c2ad130ec3d151eec30027fb088b454645e123d35cae26fcf`  
		Last Modified: Thu, 14 Dec 2023 22:03:13 GMT  
		Size: 15.3 MB (15261181 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df9016b3b5518df9a190626411d1f72e4909fb6fef37bade8595ec019de31cd2`  
		Last Modified: Thu, 14 Dec 2023 22:03:13 GMT  
		Size: 16.1 MB (16084090 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5868d43270c4d925062baabbcfaf74684668ddb1c112f683511857bf51cd24f6`  
		Last Modified: Thu, 14 Dec 2023 22:03:13 GMT  
		Size: 16.9 MB (16852961 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ba41a244d15efbb948349fde074672df1fe8f2bb05ce7a220bee3f99859cb7f`  
		Last Modified: Thu, 14 Dec 2023 22:03:14 GMT  
		Size: 542.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fbee32f98e9dcebe983ed4c420aa7b2fe36e4ec7689c5b765b07d692046dea86`  
		Last Modified: Thu, 14 Dec 2023 22:03:14 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89df2d8c7477228967e0a6447b948f99f8e5428ee8b105ae9b4528402bcfea24`  
		Last Modified: Thu, 14 Dec 2023 22:03:15 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f6273153d734f6da358dd23f9a6ea2db5651609fc63868248772814fa09c130`  
		Last Modified: Fri, 15 Dec 2023 00:01:42 GMT  
		Size: 6.6 MB (6649757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e676041cffef9995347cab8dd30a5786101056a08a8f92209c80253fa31fc768`  
		Last Modified: Fri, 15 Dec 2023 19:30:58 GMT  
		Size: 78.9 KB (78896 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12ae9bfc17586102ae9161d2d98570504abb53ee1eb51a3ac4a1f0d4ee8136e3`  
		Last Modified: Fri, 15 Dec 2023 19:30:58 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b9122ec39b1ed2a381579db7c9d3d3ed566b8a6a98414a40e34400540bd4947`  
		Last Modified: Fri, 15 Dec 2023 19:31:00 GMT  
		Size: 51.9 MB (51910212 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:65ed82be42e3579f884cff8f1abf3fa5250e23ce310ba467ee261f8676e80cc4`  
		Last Modified: Fri, 15 Dec 2023 19:30:58 GMT  
		Size: 1.5 KB (1514 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:35ad81f08e3623e9a0f1374f5636f9c251d259209be872d05d4c32400efa0df7`  
		Last Modified: Fri, 15 Dec 2023 19:30:59 GMT  
		Size: 2.9 KB (2878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ab899250d26ed35f10c7213750d618f00324fd9096e1b226c79ab1124816d9e4`  
		Last Modified: Fri, 15 Dec 2023 19:52:48 GMT  
		Size: 4.7 MB (4657521 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:rc-git` - unknown; unknown

```console
$ docker pull docker@sha256:81df3cd122b9f31af7df9861dde6cb16b981425599b336ebb100d155d6fe9f3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **746.5 KB (746523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dc82728e265b1d623a32263539648193e1d4b0eaf6c7b86905f1ea1fd054d6d`

```dockerfile
```

-	Layers:
	-	`sha256:e3c53215749f678da058607a863ee085bc6602b5b17a7519a828d752f26a8c9d`  
		Last Modified: Fri, 15 Dec 2023 19:52:47 GMT  
		Size: 733.3 KB (733306 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4cf1ceee9a20b14ec28726ba86a3174a5b148a89b926327c754a8a5832b66d9c`  
		Last Modified: Fri, 15 Dec 2023 19:52:47 GMT  
		Size: 13.2 KB (13217 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:rc-git` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:25996dc3ea841b8ddaa411b44dcb4d78c7425410cf54245a397e5458da6f6848
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117212429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51fa5fe68cdc6b45d78c6b8411d2f62eb6e82e3d852581ce66ba822274970656`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 13 Nov 2023 22:06:12 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.2
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.3
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-x86_64'; 			sha256='a836e807951db448f991f303cddcc9a4ec69f4a49d58bc7d536cb91c77c04c33'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv6'; 			sha256='b712693945360155842b578beace00effa723b604bfe1ccd6421645523e15d86'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv7'; 			sha256='4068bcbe1dd90034c8fe8d2c65b600ba793fc19bdb65db3c2dbf80b8a078de6c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-aarch64'; 			sha256='71f38f0923b8a9b80ad02c823ec3207d94677547aa5c618ca41b81d29fe6b9d9'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-ppc64le'; 			sha256='6110b0d30baee103c98ca5503bea24acb9d52bd333a67d3bf3c57d383c585c62'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-riscv64'; 			sha256='3ac26e5f272deb1364c9b8760af44c4dbd87d6faa42fc53bfec95885cfa8ae77'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-s390x'; 			sha256='2886dd4eddaea1eeb03537bdc596ec8947eb3ef7908c955284f8aad9170d3098'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD ["sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	apk add --no-cache iptables-legacy; 	mkdir -p /usr/local/sbin/.iptables-legacy; 	for f in 		iptables 		iptables-save 		iptables-restore 		ip6tables 		ip6tables-save 		ip6tables-restore 	; do 		b="/sbin/${f/tables/tables-legacy}"; 		"$b" --version; 		ln -svT "$b" "/usr/local/sbin/.iptables-legacy/$f"; 	done; 	export PATH="/usr/local/sbin/.iptables-legacy:$PATH"; 	iptables --version | grep legacy # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DIND_COMMIT=65cfcc28ab37cb75e1560e4b4738719c07c6618e
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/var/lib/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Mon, 13 Nov 2023 22:06:12 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
CMD []
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache git # buildkit
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d4959de38143abac793d31e4e8592696721305ff06281f8b9284aee380afcfe`  
		Last Modified: Thu, 14 Dec 2023 22:04:39 GMT  
		Size: 2.0 MB (2014899 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1dc2488df1b2820f1843853b994195973c9de6610e106b58701bbad49d6e9ca`  
		Last Modified: Thu, 14 Dec 2023 22:04:39 GMT  
		Size: 15.9 MB (15895347 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ace41f81de2f6058c5af45f615c6f1add39c259d8134b47c024d8c02963fcf2e`  
		Last Modified: Thu, 14 Dec 2023 22:04:39 GMT  
		Size: 15.6 MB (15640596 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:57287c3e3041b9ad611b61a753cbaac3feb12210e03adaf5ccbfc94c59b7c7f0`  
		Last Modified: Thu, 14 Dec 2023 22:04:39 GMT  
		Size: 16.3 MB (16302318 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc835c41ef1da3a2a00b6c9c4cae77e37480965760cfeff7b089404a181e3e9c`  
		Last Modified: Thu, 14 Dec 2023 22:04:40 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ffd0d560c0f9dcddd6576f8a6def5d010ab1c4c9e603d668e1746fb6f9fbc4e5`  
		Last Modified: Thu, 14 Dec 2023 22:04:41 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:739ad47860c9e713034bdbdf9393544297d64575fee6e53af41b8c6a8c2b3eee`  
		Last Modified: Thu, 14 Dec 2023 22:04:40 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eb960a25dcd6ded95375cf734eb882aea29001e46af8b9a12544591c625dfa19`  
		Last Modified: Fri, 15 Dec 2023 00:16:15 GMT  
		Size: 7.4 MB (7428532 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b03314a3b836481d0aac03d1e20f2ae943732c793099292fdda3cfdc8d0d204c`  
		Last Modified: Fri, 15 Dec 2023 19:31:26 GMT  
		Size: 93.1 KB (93073 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:aef74db21cd26fe2395cc2c881ece363e8afd44defd10e4217f463b0c9e299b0`  
		Last Modified: Fri, 15 Dec 2023 19:31:26 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b3405f023fb4562997c83102ed389f8c6125a5d7c40eb0c1a1b38c695129e67`  
		Last Modified: Fri, 15 Dec 2023 19:31:28 GMT  
		Size: 51.3 MB (51254976 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:af747d35186ec57ef6624163868d6325fd89bbd48485ac0235d3574f7226c684`  
		Last Modified: Fri, 15 Dec 2023 19:31:26 GMT  
		Size: 1.5 KB (1514 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e81b560f148ccaf4029b9d73dda9e61f1a7ae146e8063af6dae3724d7788377c`  
		Last Modified: Fri, 15 Dec 2023 19:31:27 GMT  
		Size: 2.9 KB (2878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c4319d1e358b0f165a2d1b044c94fd958be1deec353cce1d78b3158f28cf154`  
		Last Modified: Fri, 15 Dec 2023 20:28:42 GMT  
		Size: 5.2 MB (5227496 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:rc-git` - unknown; unknown

```console
$ docker pull docker@sha256:e79e144cbcb3c8b7fde0cd99f9594d822f848c637a58bdbc58f648a10966adbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **741.6 KB (741622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f00679d96a73e3ed1881ccb9dce9ada8f85a1118dab79ae1a33c16dd428e370`

```dockerfile
```

-	Layers:
	-	`sha256:4367be44e704cad4daa218d21401f58c99bc56228707ae4e5a27f7ea40fae20c`  
		Last Modified: Fri, 15 Dec 2023 20:28:42 GMT  
		Size: 730.8 KB (730815 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:34de2195d1d6d1d1bfebdc4ce13508996a479adfd262e442b8e9d306ab803165`  
		Last Modified: Fri, 15 Dec 2023 20:28:42 GMT  
		Size: 10.8 KB (10807 bytes)  
		MIME: application/vnd.in-toto+json
