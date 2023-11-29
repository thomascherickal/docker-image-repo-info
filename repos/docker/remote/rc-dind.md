## `docker:rc-dind`

```console
$ docker pull docker@sha256:4f4ea31a9464694593dd5a78635e97be98ff580e835151bb8bc1060456f816b5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 7
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:rc-dind` - linux; amd64

```console
$ docker pull docker@sha256:c98c2a9432faf823f7c6fcc3ae875dee79656b01cfc41c3f2ea06464f3d0abf9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.4 MB (122400220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d9c07d0e224eb0a1f8f01f145e1687957ca781ef5ff48d13be50631c201283d`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 23 Nov 2023 12:05:52 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.3
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-x86_64'; 			sha256='a836e807951db448f991f303cddcc9a4ec69f4a49d58bc7d536cb91c77c04c33'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv6'; 			sha256='b712693945360155842b578beace00effa723b604bfe1ccd6421645523e15d86'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv7'; 			sha256='4068bcbe1dd90034c8fe8d2c65b600ba793fc19bdb65db3c2dbf80b8a078de6c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-aarch64'; 			sha256='71f38f0923b8a9b80ad02c823ec3207d94677547aa5c618ca41b81d29fe6b9d9'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-ppc64le'; 			sha256='6110b0d30baee103c98ca5503bea24acb9d52bd333a67d3bf3c57d383c585c62'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-riscv64'; 			sha256='3ac26e5f272deb1364c9b8760af44c4dbd87d6faa42fc53bfec95885cfa8ae77'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-s390x'; 			sha256='2886dd4eddaea1eeb03537bdc596ec8947eb3ef7908c955284f8aad9170d3098'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Nov 2023 12:05:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Nov 2023 12:05:52 GMT
CMD ["sh"]
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
ENV DIND_COMMIT=65cfcc28ab37cb75e1560e4b4738719c07c6618e
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
VOLUME [/var/lib/docker]
# Tue, 28 Nov 2023 00:06:31 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 28 Nov 2023 00:06:31 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 28 Nov 2023 00:06:31 GMT
CMD []
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:01f8ea160d28fc413b17ecb203b120b569dde799e9059fb7c94131d9699cfab5`  
		Last Modified: Tue, 28 Nov 2023 19:12:06 GMT  
		Size: 2.0 MB (2014295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:762037293b6bfc04495775108a271e145c8e7ec89f99768f26de44f252cb8204`  
		Last Modified: Tue, 28 Nov 2023 19:12:06 GMT  
		Size: 16.9 MB (16890673 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5a67ae5ecd65e3c205313463fcc473c584cc80bb44adea4a622842d148e4ef1`  
		Last Modified: Tue, 28 Nov 2023 19:12:06 GMT  
		Size: 17.2 MB (17195300 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f4a1f2dd3d1952780873ef52e9d13a22a1e1e8bc6ce975e2975f3584587bd719`  
		Last Modified: Tue, 28 Nov 2023 19:12:06 GMT  
		Size: 17.9 MB (17852060 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b2b98bbdc2abf9d18c78d7b0e6b86557da1e145813816045fab8521a8d8eb1b`  
		Last Modified: Tue, 28 Nov 2023 19:12:06 GMT  
		Size: 544.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee2947d8c6c7030c66b5ab8c5fe2b88d8233706a85e9064958bb51e9a3d0bbf0`  
		Last Modified: Tue, 28 Nov 2023 19:12:07 GMT  
		Size: 1.0 KB (1017 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:40ac6231400308044cc8c92229dbb2dfacca2740c5ade765913a237bc0a6ced3`  
		Last Modified: Tue, 28 Nov 2023 19:12:07 GMT  
		Size: 114.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64314609d292b60c8d57472e6c51f914ee9bc6c390eabf8b598ff55ea1cac50e`  
		Last Modified: Tue, 28 Nov 2023 20:15:44 GMT  
		Size: 9.3 MB (9274436 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b62eb4931aea44ea6ec79fb53792f1569c7a4914caddbfbf95053e5908c26d6`  
		Last Modified: Tue, 28 Nov 2023 20:15:44 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:650a8f4c995bf1aa7fdb052d39cd9baaf0f0006dbe5507b5ba17bf30746d386d`  
		Last Modified: Tue, 28 Nov 2023 20:15:45 GMT  
		Size: 55.8 MB (55764184 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15b73b56c2cb208b5fb4aa1467741519ef754f80a58236eefeccf9c4472cea61`  
		Last Modified: Tue, 28 Nov 2023 20:15:45 GMT  
		Size: 1.5 KB (1512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9c40ed29a83f719ca1925819ab2222077ad7db1c5ab304f7599d76b3a59abcad`  
		Last Modified: Tue, 28 Nov 2023 20:15:45 GMT  
		Size: 2.8 KB (2789 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:rc-dind` - unknown; unknown

```console
$ docker pull docker@sha256:1aad20222adac09d9c11bafeccec75652142bb42d84033b0061fcf797fbb574e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.2 KB (702183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0369d025f404a7916e6d096f838542e0c7dc979b62891613ac4e448e646a9e6d`

```dockerfile
```

-	Layers:
	-	`sha256:e6bc2320ea9427d373bfe1fed66139c8817924049ad976c54b294f87193e7b57`  
		Last Modified: Tue, 28 Nov 2023 20:15:44 GMT  
		Size: 672.5 KB (672495 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a4402fc7fc87401c9bca5a39522bb606a9c68ebbd7cfaf79ab303a87fe01f9ac`  
		Last Modified: Tue, 28 Nov 2023 20:15:44 GMT  
		Size: 29.7 KB (29688 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:rc-dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:b3e772901bea2a82e83840707496f1303d66b135b410e15db412bada2aae3222
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114642945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5e12f0563ce264feee8ec35f7a686b0c8c074ca88fefa55302c7d87e67c44c2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 23 Nov 2023 12:05:52 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.3
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-x86_64'; 			sha256='a836e807951db448f991f303cddcc9a4ec69f4a49d58bc7d536cb91c77c04c33'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv6'; 			sha256='b712693945360155842b578beace00effa723b604bfe1ccd6421645523e15d86'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv7'; 			sha256='4068bcbe1dd90034c8fe8d2c65b600ba793fc19bdb65db3c2dbf80b8a078de6c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-aarch64'; 			sha256='71f38f0923b8a9b80ad02c823ec3207d94677547aa5c618ca41b81d29fe6b9d9'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-ppc64le'; 			sha256='6110b0d30baee103c98ca5503bea24acb9d52bd333a67d3bf3c57d383c585c62'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-riscv64'; 			sha256='3ac26e5f272deb1364c9b8760af44c4dbd87d6faa42fc53bfec95885cfa8ae77'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-s390x'; 			sha256='2886dd4eddaea1eeb03537bdc596ec8947eb3ef7908c955284f8aad9170d3098'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Nov 2023 12:05:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Nov 2023 12:05:52 GMT
CMD ["sh"]
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
ENV DIND_COMMIT=65cfcc28ab37cb75e1560e4b4738719c07c6618e
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
VOLUME [/var/lib/docker]
# Tue, 28 Nov 2023 00:06:31 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 28 Nov 2023 00:06:31 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 28 Nov 2023 00:06:31 GMT
CMD []
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749ab9fb78d5310f50a86ca9fc51b51ccfc7c6fb8285aea647b6faa49409ecf2`  
		Last Modified: Tue, 14 Nov 2023 02:37:28 GMT  
		Size: 2.1 MB (2088618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d4f6ffcef8dee3f9bf83e3bdcc8907643c5e1f91d44d8396286b5b8e58a5e1`  
		Last Modified: Tue, 14 Nov 2023 02:37:29 GMT  
		Size: 15.3 MB (15274900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8471a598c6c33331ad7a5058de5738de5952be7f17280bc35a3e18402a588bb`  
		Last Modified: Fri, 17 Nov 2023 19:20:33 GMT  
		Size: 16.1 MB (16099979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e709e56c9bc50331c45d66a725d813af385fe575a4cd02a742ad8d13fc89526f`  
		Last Modified: Tue, 28 Nov 2023 19:06:34 GMT  
		Size: 16.9 MB (16867551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b485294dbf1476f5cc410edef9cc048e3f9357efe86257ff66f9d3cb96a684`  
		Last Modified: Tue, 28 Nov 2023 19:06:31 GMT  
		Size: 547.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9176d32eed3c0d2c43ca40b6701ecd94cfb75db567c41f1c06ead045759ea6`  
		Last Modified: Tue, 28 Nov 2023 19:06:31 GMT  
		Size: 1.0 KB (1023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e119c223471d840c01d4a12e374f5f46ea19666a4c8d7d37621400ee886026ef`  
		Last Modified: Tue, 28 Nov 2023 19:06:31 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47405e621a2220fdbc9cdad50a60260b79fd425e122a4e9e9fcd4c861de4bb52`  
		Last Modified: Tue, 28 Nov 2023 19:36:48 GMT  
		Size: 9.0 MB (9046089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a833442813cc2d19d09fa0c6fb324fc3f9612f5b882ab2d0b949cadea43afc6`  
		Last Modified: Tue, 28 Nov 2023 19:36:47 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fec9455ab77e336f0bf63078412f3617b7dd5d8c42ed0e5657f5a716f583d9f`  
		Last Modified: Tue, 28 Nov 2023 19:36:55 GMT  
		Size: 52.1 MB (52113195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8b7d550419e325678ac6e360c7d6a82200c95b62762b08d710c9924d7410f8`  
		Last Modified: Tue, 28 Nov 2023 19:36:47 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b0629eb9d18bb4e2c5410b6542445c74325a678d0dce92eef3840e08ef1f15`  
		Last Modified: Tue, 28 Nov 2023 19:36:47 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:rc-dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:b53fbd1fb995db467cf31bb475c0e34a96b2a8852e816118ff5303a20074b00e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113319758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75dce5c745e64906440890ac4c1020ea47135c04f37fa65504b3ed48b1ddeaf8`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 23 Nov 2023 12:05:52 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.3
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-x86_64'; 			sha256='a836e807951db448f991f303cddcc9a4ec69f4a49d58bc7d536cb91c77c04c33'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv6'; 			sha256='b712693945360155842b578beace00effa723b604bfe1ccd6421645523e15d86'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv7'; 			sha256='4068bcbe1dd90034c8fe8d2c65b600ba793fc19bdb65db3c2dbf80b8a078de6c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-aarch64'; 			sha256='71f38f0923b8a9b80ad02c823ec3207d94677547aa5c618ca41b81d29fe6b9d9'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-ppc64le'; 			sha256='6110b0d30baee103c98ca5503bea24acb9d52bd333a67d3bf3c57d383c585c62'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-riscv64'; 			sha256='3ac26e5f272deb1364c9b8760af44c4dbd87d6faa42fc53bfec95885cfa8ae77'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-s390x'; 			sha256='2886dd4eddaea1eeb03537bdc596ec8947eb3ef7908c955284f8aad9170d3098'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Nov 2023 12:05:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Nov 2023 12:05:52 GMT
CMD ["sh"]
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
ENV DIND_COMMIT=65cfcc28ab37cb75e1560e4b4738719c07c6618e
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
VOLUME [/var/lib/docker]
# Tue, 28 Nov 2023 00:06:31 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 28 Nov 2023 00:06:31 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 28 Nov 2023 00:06:31 GMT
CMD []
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b7fbc844f0c4a3436052544093f56c4d5061b5302239d5e8f50afb7d503a29c`  
		Last Modified: Tue, 03 Oct 2023 00:57:56 GMT  
		Size: 1.9 MB (1875250 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e4d4284c771adbac8678f485d42c71da5e9465482941db8231f014420c8bd33c`  
		Last Modified: Tue, 14 Nov 2023 05:39:25 GMT  
		Size: 15.3 MB (15269601 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:add0974f57e0de4e10c6786a80dc2ac3db50e68d39b46cadaad22aaf65ae911f`  
		Last Modified: Fri, 17 Nov 2023 19:26:29 GMT  
		Size: 16.1 MB (16084089 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9f6e386e450b849a2ad4605089c261de62ef7ca32d710570f3dbe0b4d0f9d7bd`  
		Last Modified: Tue, 28 Nov 2023 19:12:25 GMT  
		Size: 16.9 MB (16852976 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ba0199a3437b3b596b08f3f040a87d12dae3245fa3a516d0ee1b637898303b8`  
		Last Modified: Tue, 28 Nov 2023 19:12:24 GMT  
		Size: 547.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f04824561e59156180dcf495f6932c8c69ad8b21c7c1546f811428de51c80d3f`  
		Last Modified: Tue, 28 Nov 2023 19:12:24 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a92be7404735a395ae4554a6a59ca455330daa95000534b9d80c3a7ad880c1c`  
		Last Modified: Tue, 28 Nov 2023 19:12:24 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a061213943cbbd22e11fefa35e7a1e095d9f0731a092eb581b1bf1e83bc1ab6d`  
		Last Modified: Tue, 28 Nov 2023 20:24:57 GMT  
		Size: 8.2 MB (8217358 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be0ffae7da1fa898ac1a2b5140cb5de59fb94794ded8bae47b36c2f8d8e2d905`  
		Last Modified: Tue, 28 Nov 2023 20:24:57 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca544a20b324562422ef4d16ae381f9e74e917bf0ae08e3823022b66a8e93001`  
		Last Modified: Tue, 28 Nov 2023 20:24:59 GMT  
		Size: 52.1 MB (52113253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0ae4fcaca00712663b24e834251ed5eed29e7edaf512335a787b22162fdd9f38`  
		Last Modified: Tue, 28 Nov 2023 20:24:57 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:103b8df363131d61f5a8a3eafba5c55b7c05a41c42cb9654db7c0135f948adc9`  
		Last Modified: Tue, 28 Nov 2023 20:24:58 GMT  
		Size: 2.8 KB (2793 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:rc-dind` - unknown; unknown

```console
$ docker pull docker@sha256:f0e813670cd88d6c954512697c88131e9eb912cb0b60975c58011d9d8fb909e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.4 KB (702440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76ee1cd36da9ac4df17eb23fe2e42ad70a026f7d1209462fdeec2767785e94c8`

```dockerfile
```

-	Layers:
	-	`sha256:23652ba6deaa9736d1f07399af78385aa5a68167d984fc0aa9cffd59f80d44cb`  
		Last Modified: Tue, 28 Nov 2023 20:24:56 GMT  
		Size: 672.6 KB (672563 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0a47d5240295271a745c44f5a9485c19f93c79ad8e965ce946b9baa460ba8cf8`  
		Last Modified: Tue, 28 Nov 2023 20:24:56 GMT  
		Size: 29.9 KB (29877 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:rc-dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:ec47c6f9662c1c0742e65750d0e2e91297638419d7e715ef4b46453ebf6cf21e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (113951563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c8ce2f60e9e55ba3ee1406da2ea9f85a0f89ff69fd17b4c04e3a2d8a07547d2`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 23 Nov 2023 12:05:52 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.3
# Thu, 23 Nov 2023 12:05:52 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-x86_64'; 			sha256='a836e807951db448f991f303cddcc9a4ec69f4a49d58bc7d536cb91c77c04c33'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv6'; 			sha256='b712693945360155842b578beace00effa723b604bfe1ccd6421645523e15d86'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv7'; 			sha256='4068bcbe1dd90034c8fe8d2c65b600ba793fc19bdb65db3c2dbf80b8a078de6c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-aarch64'; 			sha256='71f38f0923b8a9b80ad02c823ec3207d94677547aa5c618ca41b81d29fe6b9d9'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-ppc64le'; 			sha256='6110b0d30baee103c98ca5503bea24acb9d52bd333a67d3bf3c57d383c585c62'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-riscv64'; 			sha256='3ac26e5f272deb1364c9b8760af44c4dbd87d6faa42fc53bfec95885cfa8ae77'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-s390x'; 			sha256='2886dd4eddaea1eeb03537bdc596ec8947eb3ef7908c955284f8aad9170d3098'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 23 Nov 2023 12:05:52 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 23 Nov 2023 12:05:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Nov 2023 12:05:52 GMT
CMD ["sh"]
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
ENV DIND_COMMIT=65cfcc28ab37cb75e1560e4b4738719c07c6618e
# Tue, 28 Nov 2023 00:06:31 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 28 Nov 2023 00:06:31 GMT
VOLUME [/var/lib/docker]
# Tue, 28 Nov 2023 00:06:31 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 28 Nov 2023 00:06:31 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 28 Nov 2023 00:06:31 GMT
CMD []
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
	-	`sha256:b751039a3d1e1f4c5da518d2c0ab210d9dde6bb4b882239669c537ca0cca4750`  
		Last Modified: Tue, 14 Nov 2023 02:44:03 GMT  
		Size: 15.9 MB (15893478 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7628bbe10bd17a4da8529f7b50fad49a8ad91dd1fceb4aed606780b6729c45fc`  
		Last Modified: Fri, 17 Nov 2023 19:27:03 GMT  
		Size: 15.6 MB (15640603 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8945d88660ba0aa4e183e2ba6bebb45419d3d74294dcb976f52b11323ebad2a6`  
		Last Modified: Tue, 28 Nov 2023 19:12:57 GMT  
		Size: 16.3 MB (16302325 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:31a1117346a5d0218bd01d9be2e03f0a141c696808060ce326ba3244319b31ff`  
		Last Modified: Tue, 28 Nov 2023 19:12:56 GMT  
		Size: 548.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb20aabb1ed246c1e3e02385730a52d6ffd278bbde66c573e7c89c9f2c0f33e7`  
		Last Modified: Tue, 28 Nov 2023 19:12:56 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:38f04613519a4e69bf1dba4469c5739e9fbad69e0f3878165a3378e6a6f72fbe`  
		Last Modified: Tue, 28 Nov 2023 19:12:56 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a2018a1085e4d8677a17736be18cf876465c54ceaee4ee0b7fe38dc574b50b2f`  
		Last Modified: Tue, 28 Nov 2023 20:25:20 GMT  
		Size: 9.4 MB (9362878 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:511c0f34cc1124eb8b3b7a89518cfac105049ffb3d07ccb717a417505bff6868`  
		Last Modified: Tue, 28 Nov 2023 20:25:19 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad11f32fd029b3ba26f28d02eb6d81e807cc1b0332f97208a58e47a37942f3c6`  
		Last Modified: Tue, 28 Nov 2023 20:25:21 GMT  
		Size: 51.4 MB (51388576 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:348d435d8d578d64bd8949831fcc693b2185e33ad3c8ba64d547956d836e31e4`  
		Last Modified: Tue, 28 Nov 2023 20:25:19 GMT  
		Size: 1.5 KB (1515 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1fc30a0b6084479fa143b059c0e8ade7754781099a757305c5240d42f47c25`  
		Last Modified: Tue, 28 Nov 2023 20:25:20 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:rc-dind` - unknown; unknown

```console
$ docker pull docker@sha256:01063c2d64cbdc2589a7b0e48749d1b194de8428d8143ffa34feb80e6bcc19bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **702.3 KB (702267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93cb2a532c522e3680344a4aa147d918e6e2b133fd379e92800161dd49478d74`

```dockerfile
```

-	Layers:
	-	`sha256:2ec0cf9d00625899dfbd93b35af47b46d00e05cdf2fcbb954d7cb5e817a734a7`  
		Last Modified: Tue, 28 Nov 2023 20:25:19 GMT  
		Size: 672.5 KB (672514 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0265ecedc9a0910268bd06089961d298551e25c57dc4b0873f75dfa1b8acb242`  
		Last Modified: Tue, 28 Nov 2023 20:25:19 GMT  
		Size: 29.8 KB (29753 bytes)  
		MIME: application/vnd.in-toto+json
