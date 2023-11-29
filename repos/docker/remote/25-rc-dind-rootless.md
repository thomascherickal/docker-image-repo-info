## `docker:25-rc-dind-rootless`

```console
$ docker pull docker@sha256:9b13b95132714870ded8e774fefae6a7218047ede1e2363b1a2407c00569c912
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:25-rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:fc5f80cb56c07b140d92a53397ad30fd21b66aaa88e9b721e54eca37f5cd3d90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.6 MB (144648491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5397aa7b20cc5ab404011d8ffe3a42b6f6c958e5b579986ec70e40f7e20afc82`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
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
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
USER rootless
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
	-	`sha256:44d22a95ff0d7d175258783515a5a597f33501c884fbd4f9ee6d6eae324d9db1`  
		Last Modified: Tue, 28 Nov 2023 21:18:59 GMT  
		Size: 1.4 MB (1362186 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1d2819d3e09b6379daf2b02b754810f6c8a2868f712e40d2666ac4bf3503eced`  
		Last Modified: Tue, 28 Nov 2023 21:18:58 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07f4e48214c93a0d57173ac9075f052f0cda1bf3cf80c5445ddda2490ab51894`  
		Last Modified: Tue, 28 Nov 2023 21:18:59 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6594116ad2a930e3eb8ac1a631ff4565b46a10ac2641be2c0e44ee6fd3d6c2ec`  
		Last Modified: Tue, 28 Nov 2023 21:18:59 GMT  
		Size: 20.9 MB (20884457 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:962f72615d0ccae4f8b0265256686d54c85bb2c6e3e359fafdb0c7ef40684cfb`  
		Last Modified: Tue, 28 Nov 2023 21:19:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:25-rc-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:dbde9412c057732b262ee42b9be39430fae99707df7d31aceeb8f95e0b52f09d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **750.1 KB (750133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1dc906b78669c4d07e7aa462ab7a0100d69add9296a7abea2ca4b25ba4df25`

```dockerfile
```

-	Layers:
	-	`sha256:6b63cd9b98158d5d363f204611735fac1a6763d57879145e28950843fa62c46f`  
		Last Modified: Tue, 28 Nov 2023 21:18:59 GMT  
		Size: 719.3 KB (719275 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d8cef088615cc59ae554db9223b1ea3478392c854c2cdc916cd20095f3a80875`  
		Last Modified: Tue, 28 Nov 2023 21:18:58 GMT  
		Size: 30.9 KB (30858 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:25-rc-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:bae94839de9f902fb9319255cb2cfdd8ea72f67862016560d80e6f61d5d70df6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138112904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd1c833d63d0526e182b15d3c0d0f7f1b56801f6cc5da86e36d6e62961b1396`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 13 Nov 2023 22:06:12 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
ENV DOCKER_VERSION=25.0.0-beta.1
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
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
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.1.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.1.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
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
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-25.0.0-beta.1.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-25.0.0-beta.1.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Mon, 13 Nov 2023 22:06:12 GMT
VOLUME [/home/rootless/.local/share/docker]
# Mon, 13 Nov 2023 22:06:12 GMT
USER rootless
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
	-	`sha256:a0db174695dfee5585c198580fd539f88d24af2ed0eb51e3ce4c79f979e59ce5`  
		Last Modified: Tue, 28 Nov 2023 21:28:28 GMT  
		Size: 1.4 MB (1413161 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:102b77af16f88804391af84c25510385eee7e5cb20a227ce10f5e3fc4e69dd05`  
		Last Modified: Tue, 28 Nov 2023 21:28:28 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cb75e574fcfd8f904e1a479a4fb5e8610ad76e9e7c7ec7d18969604579f9a31e`  
		Last Modified: Tue, 28 Nov 2023 21:28:28 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:846c115f852ab263f08299899ca14a19eaf6df24743bdb066193c6657adb610c`  
		Last Modified: Tue, 28 Nov 2023 21:28:30 GMT  
		Size: 22.7 MB (22746550 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0846d35e3721121bf005fe66b61bbc262aa955017c70e6a545220b66124be10d`  
		Last Modified: Tue, 28 Nov 2023 21:28:29 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:25-rc-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:6b41a9d4409d71b2fba0c4936c21a1d608b0ffb3e05056eb50ab9ba4d0a3fba8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **750.2 KB (750198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db677b2ba4c917018853ffa2c2cc078d9e7504a7c9490b64c146c8998ee1b247`

```dockerfile
```

-	Layers:
	-	`sha256:bc8bfb2197cbc654564524e2882414cc1e727503d77c18a254007b55d8172b79`  
		Last Modified: Tue, 28 Nov 2023 21:28:28 GMT  
		Size: 719.3 KB (719284 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b1cc617e1d1373faf0a05debad83d3f403fe24e918dc28b048d2000322ec076a`  
		Last Modified: Tue, 28 Nov 2023 21:28:27 GMT  
		Size: 30.9 KB (30914 bytes)  
		MIME: application/vnd.in-toto+json
