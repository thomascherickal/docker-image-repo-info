## `docker:dind-rootless`

```console
$ docker pull docker@sha256:be37fd81568b8a1f6ff39a5fdfcc85fd9566c512194dcfc82880c9cf43f7bbf9
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:979ea05447c66ec192bd9473a5df008bc32a97125f171f6a349d64a1f23c3351
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.6 MB (140557623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83b2ab08eb145bb43c027b35c643f8a9fe30127c973cbc3f0817ac72fa6f20a`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Tue, 05 Sep 2023 23:04:32 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.22.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-x86_64'; 			sha256='e849450f1c5c20123aa7d63291e2a818b7a117f2e03e432853ece463dd09e67a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv6'; 			sha256='46cabb4363c5fa66e63c6055b1d0a6fe2c7995350e48f14816a752ae4132231d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv7'; 			sha256='1a0d500eaae3c4ddbfdeb566896207c0628a671065b95d0e8907bca58f91d312'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-aarch64'; 			sha256='572a22000d408fb524258b379bf272a007c8da977c3e8d47c34f4e45dd7b1932'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-ppc64le'; 			sha256='4d1a3e89fdb7641422dc5cbcab48fd2da337b03265cb5ac2858c3425bacf952c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-riscv64'; 			sha256='c45193b98c54e5a898e6b9095f70b0487599f19ce25b579ed2fcc3f868415aff'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-s390x'; 			sha256='716aded74df512728638f1fe53170c46d94c1a085bc5a24108ce7101bc37bd81'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
USER rootless
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
	-	`sha256:4101e3fd4622702cd6fd8400c297646c55a0cca6cdf3c00b55e39ac12cb4313f`  
		Last Modified: Thu, 28 Sep 2023 23:57:21 GMT  
		Size: 7.1 MB (7080468 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e27f630a38f0e6d85aedd015d883fd254c7a64f9dd009b7fd72ca4b631f7657c`  
		Last Modified: Thu, 28 Sep 2023 23:57:19 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62c9ea925f0c5f8bba8a5593154c3e1d5a84b186439a52a24d8a2503edec7f42`  
		Last Modified: Thu, 28 Sep 2023 23:57:24 GMT  
		Size: 54.4 MB (54351586 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e28d517cb2ce3b622fa933eb1572b6c818682ddc9562a1beac3909c27025bf08`  
		Last Modified: Thu, 28 Sep 2023 23:57:20 GMT  
		Size: 1.0 KB (1034 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a069f3d343dd4bffb49f0596ee0044a76162a48a148e84cca8fd10110d0da38e`  
		Last Modified: Thu, 28 Sep 2023 23:57:20 GMT  
		Size: 2.8 KB (2787 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cc0afc29227d8cf51082dbbf7cf5d33b621a96ce202be330d51c96ce4a31f3b4`  
		Last Modified: Fri, 29 Sep 2023 00:56:09 GMT  
		Size: 1.4 MB (1362150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e62e599cf58f63e80c987055ed41161f1b8b68720120a9d3e103e6f7fb1de58a`  
		Last Modified: Fri, 29 Sep 2023 00:56:09 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1e8e9a7a81fb42edf534149f3f86c1c04bf1935b0cbe7ef346acfdec66346fd2`  
		Last Modified: Fri, 29 Sep 2023 00:56:09 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:36cfb88dca21d17c684a40a1e5d6700eab5b9dbf8917850836335653460cb40a`  
		Last Modified: Fri, 29 Sep 2023 00:56:11 GMT  
		Size: 20.7 MB (20660316 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a39be0185f7d48a2e786443b48e601e25c789003b10244aee2090a5ca200fe5c`  
		Last Modified: Fri, 29 Sep 2023 00:56:10 GMT  
		Size: 187.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:88364d3a5bb21f498b5904e30b80a1fb616ce511dabc259340695912dea08150
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **776.1 KB (776089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2fa1df5be10b90384ff5c7bc5a7119e9ef2f9dff9ab67ebf886f158328f0499`

```dockerfile
```

-	Layers:
	-	`sha256:557394f9405b11ea1c13385caf6f3eb70085d8ca2e4662d89e74adf4a9b557b5`  
		Last Modified: Fri, 29 Sep 2023 00:56:08 GMT  
		Size: 745.0 KB (745005 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:19b2b2e04bb1b13008d70ba9e12e508bda7282b41ad0566bc765270252f010e7`  
		Last Modified: Fri, 29 Sep 2023 00:56:08 GMT  
		Size: 31.1 KB (31084 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:46bf3734c43d1aa15983b557c388a96929c4e4c807805362cbb70dcc263af2d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135767398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aded9b28dfda15a4645d7343672fa8abaaa0d7aee3d5b87b186d1decd9f3dd69`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_VERSION=24.0.6
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_BUILDX_VERSION=0.11.2
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-amd64'; 			sha256='311568ee69715abc46163fd688e56c77ab0144ff32e116d0f293bfc3470e75b7'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v6'; 			sha256='c1bab0c7374406d5069f60b291971d71161fbd3c00e8a8fb1b68b9053eda8a4e'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm-v7'; 			sha256='4defdf463ca2516d3f58fef69a6f78cbbb8baf16d936cdfc54df4a4be0d48f7f'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-arm64'; 			sha256='565e36085a35bba5104f37365ba796c111338eea1a0902b3a7ff42e2e1248815'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-ppc64le'; 			sha256='c5f5cb9957890873a537c7ff5c4eef36132339622baeabb37a4b9b7251ddf836'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-riscv64'; 			sha256='c0adc4b4625f7e3df7dcdec840568f918673f2ed4bcd03ca1e63ea2a5627ca35'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.11.2/buildx-v0.11.2.linux-s390x'; 			sha256='02916c76c3872fd0b3fa57e71403fee92b6be10f350b96a5ff99e7914dd277b8'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_COMPOSE_VERSION=2.22.0
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-x86_64'; 			sha256='e849450f1c5c20123aa7d63291e2a818b7a117f2e03e432853ece463dd09e67a'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv6'; 			sha256='46cabb4363c5fa66e63c6055b1d0a6fe2c7995350e48f14816a752ae4132231d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-armv7'; 			sha256='1a0d500eaae3c4ddbfdeb566896207c0628a671065b95d0e8907bca58f91d312'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-aarch64'; 			sha256='572a22000d408fb524258b379bf272a007c8da977c3e8d47c34f4e45dd7b1932'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-ppc64le'; 			sha256='4d1a3e89fdb7641422dc5cbcab48fd2da337b03265cb5ac2858c3425bacf952c'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-riscv64'; 			sha256='c45193b98c54e5a898e6b9095f70b0487599f19ce25b579ed2fcc3f868415aff'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.22.0/docker-compose-linux-s390x'; 			sha256='716aded74df512728638f1fe53170c46d94c1a085bc5a24108ce7101bc37bd81'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD ["sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.6.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.6.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/var/lib/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 05 Sep 2023 23:04:32 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 05 Sep 2023 23:04:32 GMT
CMD []
# Tue, 05 Sep 2023 23:04:32 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-rootless-extras-24.0.6.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-rootless-extras-24.0.6.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 05 Sep 2023 23:04:32 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 05 Sep 2023 23:04:32 GMT
USER rootless
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
	-	`sha256:3663a941bd50f2d9592c06a621cc798e7b67fcbe5019a7f00ce778d549483c1b`  
		Last Modified: Wed, 27 Sep 2023 02:42:52 GMT  
		Size: 9.4 MB (9362254 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee0c17d62831c53ccd819017cbfc2240a40bd0e45fad6a1fdb409c743a24e4ac`  
		Last Modified: Wed, 27 Sep 2023 02:42:52 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4762c49b05f7b0e4c93103ba69589263a18bc0df40a7651eec2874638635c177`  
		Last Modified: Wed, 27 Sep 2023 02:42:54 GMT  
		Size: 49.7 MB (49688241 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c629b58a6c3c89b3aa5a4c6841a0668933321ca1f65778963ddd83ecdefebd4`  
		Last Modified: Wed, 27 Sep 2023 02:42:52 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f06cf636ece24e41e358eee9f4d191a58ff476a8c57e8dc47ab56207720ac32c`  
		Last Modified: Wed, 27 Sep 2023 02:42:53 GMT  
		Size: 2.8 KB (2793 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c58e0d0e7bde08ca4c573188c6c2aa8566aa691bf932ea708d7cc5c67605505b`  
		Last Modified: Wed, 27 Sep 2023 02:51:18 GMT  
		Size: 1.4 MB (1413166 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bbc85c2ebc7dbf2d866b32ccb9a44dd908b95900f7d2f3ba142a204460948042`  
		Last Modified: Wed, 27 Sep 2023 02:51:18 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:11ca629dc49de655688e4ab8ee49a0392d4186f44abe7425c92006e2289b0c00`  
		Last Modified: Wed, 27 Sep 2023 02:51:18 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:faa241611c0bcbda79ee5910d0693356f8967c8eb3503c43fa4bdfdea6a68cf2`  
		Last Modified: Wed, 27 Sep 2023 02:51:20 GMT  
		Size: 22.4 MB (22448735 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2edb0e3ddaaf5edf566a1dd49b4561d081749eeec7a428ec6fab815c40af9213`  
		Last Modified: Wed, 27 Sep 2023 02:51:19 GMT  
		Size: 188.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:7da55854b83c324c6e726ac94471946c6a7a7c88c0676cb8e1915a1413ede2ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.0 MB (1037809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e59653609560da0678a897f020b2db30a78ffed783f30bd252254143ba36f50`

```dockerfile
```

-	Layers:
	-	`sha256:0849a3b3d6c8b1ade73a2b3dc382ac121c8244b0a4bd0ef52c85202992a076fd`  
		Last Modified: Wed, 27 Sep 2023 02:51:18 GMT  
		Size: 1.0 MB (1006658 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7114b107f8e246e884230b177ca3801630805c93484415feabd0ed8a6d964a9e`  
		Last Modified: Wed, 27 Sep 2023 02:51:17 GMT  
		Size: 31.2 KB (31151 bytes)  
		MIME: application/vnd.in-toto+json
