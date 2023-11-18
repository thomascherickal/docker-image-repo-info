## `docker:dind`

```console
$ docker pull docker@sha256:39920e7f8b71f33db3d145a1fb1fa8349ae97cc6dd64b738a2b77e9eddbd9999
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

### `docker:dind` - linux; amd64

```console
$ docker pull docker@sha256:f1a13839fe17d00249d5ccc439b0088c5398fe34fd81838c778488418312ed25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.5 MB (120477663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daefcf9ccf3b4e852a7d5342d50510b80bfd2851eed822e43163aa3b9130d588`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_VERSION=24.0.7
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.1
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-x86_64'; 			sha256='4f9b5313cf3eb1651b65aa6fc2fe1f59eb3812b7566f7c1b853be429b81bf3ab'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv6'; 			sha256='44b679381da55d1a673e5e638ac6d34f81e38e58ac656c530e27bb57a0ef930d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv7'; 			sha256='347b65d0cec622976bb753550d2708c8c9c760d55c1b5952a6800f5fadd4781c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-aarch64'; 			sha256='27b3cb1f066cdba191c4df96255a3d7178294763c9d67fba528f769968fc2e65'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-ppc64le'; 			sha256='76981fe4b032385752c5bb07144a22a7dfb599da15eca6fa1775e94364833475'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-riscv64'; 			sha256='1ee27dd153bd796686ece5d1829266b9b0db0a2ed67e7dbef023457da6dc5761'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-s390x'; 			sha256='9ee5fd812e7e52c08b95cd59673b956f2248343c2fb51eb8bcf635b02cfcbee4'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Oct 2023 17:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
CMD ["sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
VOLUME [/var/lib/docker]
# Thu, 26 Oct 2023 17:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
CMD []
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:979f7a62ca1b0f26f7216ee59c6bdcf4859e083dd69cac904eb848d6b0a6acaf`  
		Last Modified: Fri, 17 Nov 2023 19:18:07 GMT  
		Size: 2.0 MB (2014289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f4fb700ef54461cfa02571ae0db9a0dc1e0cdb5577484a6d75e68dc38e8acc1`  
		Last Modified: Tue, 07 Mar 2017 15:01:14 GMT  
		Size: 32.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb84691a0857a35ac421d9727216f628a445eb0a51b15fe358bb5ccc883bdf8b`  
		Last Modified: Fri, 17 Nov 2023 19:18:08 GMT  
		Size: 16.4 MB (16400387 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:18b1b5d57ca7f028ced000f2742414974ed47fca18e35c787c2481e06219330f`  
		Last Modified: Fri, 17 Nov 2023 19:18:08 GMT  
		Size: 17.2 MB (17195301 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ce1e8d1970d0cd635371a3abe4300938c772434fcb64b1e53accdcf3962b031a`  
		Last Modified: Fri, 17 Nov 2023 19:18:08 GMT  
		Size: 17.8 MB (17812801 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ffc5f9802ef4b0a26bcb0bc25d32bf7c840134c83f139428054b4ba37d42aa7`  
		Last Modified: Fri, 17 Nov 2023 19:18:08 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d3856c109dcb3a78be07a124a74a1765378fb7456e58f4dbe88f634d0be2c44b`  
		Last Modified: Fri, 17 Nov 2023 19:18:09 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:49f0f622e61c8d2f505db9498e6fcd4b9ec8de101df0f4b2913dbd2e48ca5a8e`  
		Last Modified: Fri, 17 Nov 2023 19:18:09 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:81640b6a1021c6828166788052c061732c96d1add80a64b74eefc080a7f1cece`  
		Last Modified: Fri, 17 Nov 2023 20:16:41 GMT  
		Size: 9.3 MB (9274445 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c7513b915291239007f63584483041cb500f46d660c6f9f0e0d664fecb3f376`  
		Last Modified: Fri, 17 Nov 2023 20:16:40 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6aa916c3993404360565c5e8220ee2bf73271c69b6779b0f697f16f37588e5f3`  
		Last Modified: Fri, 17 Nov 2023 20:16:41 GMT  
		Size: 54.4 MB (54371643 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47a389dfac47e969b8f8dbcd1c7ed89ce41d0343c7b1fd606905fb6b3b353d2f`  
		Last Modified: Fri, 17 Nov 2023 20:16:41 GMT  
		Size: 1.0 KB (1035 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7832b6a0e0521f2b4fe0e7eebb3c9117d727611b32c7bc533553796449df8e0a`  
		Last Modified: Fri, 17 Nov 2023 20:16:41 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind` - unknown; unknown

```console
$ docker pull docker@sha256:69128d5e712724cf10dc5f751ee9b5baa40e6be6469d7d83e107d6837b24f553
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **708.9 KB (708902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4222d16add8de875a660fb380d2cc28cf64815529cef11ea8464664ab7a8791d`

```dockerfile
```

-	Layers:
	-	`sha256:e2af790d78036e679b513f1d3b15dc1a6ec07bd6adc5ed7571f5dba2896dea05`  
		Last Modified: Fri, 17 Nov 2023 20:16:40 GMT  
		Size: 678.8 KB (678774 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:12ea8a9911214a4a0e7f4761d446a83b16bef1b1b868b16d4e8e1737c1e737da`  
		Last Modified: Fri, 17 Nov 2023 20:16:40 GMT  
		Size: 30.1 KB (30128 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:dind` - linux; arm variant v6

```console
$ docker pull docker@sha256:ce9cd3b55d27edb74bbf9d0405639e0fed5feb31deee5c6abe8be0a76f6d3046
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113320917 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17b87b3979b1d02a7136bf657c5d8e84570f6291c8689c19413fb3ef25ffc405`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_VERSION=24.0.7
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.1
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-x86_64'; 			sha256='4f9b5313cf3eb1651b65aa6fc2fe1f59eb3812b7566f7c1b853be429b81bf3ab'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv6'; 			sha256='44b679381da55d1a673e5e638ac6d34f81e38e58ac656c530e27bb57a0ef930d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv7'; 			sha256='347b65d0cec622976bb753550d2708c8c9c760d55c1b5952a6800f5fadd4781c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-aarch64'; 			sha256='27b3cb1f066cdba191c4df96255a3d7178294763c9d67fba528f769968fc2e65'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-ppc64le'; 			sha256='76981fe4b032385752c5bb07144a22a7dfb599da15eca6fa1775e94364833475'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-riscv64'; 			sha256='1ee27dd153bd796686ece5d1829266b9b0db0a2ed67e7dbef023457da6dc5761'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-s390x'; 			sha256='9ee5fd812e7e52c08b95cd59673b956f2248343c2fb51eb8bcf635b02cfcbee4'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Oct 2023 17:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
CMD ["sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
VOLUME [/var/lib/docker]
# Thu, 26 Oct 2023 17:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
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
	-	`sha256:9b83996d78fa3bf1f1f666c6867d86d9ec6df58b6779c0b69c27930534055f0a`  
		Last Modified: Fri, 17 Nov 2023 19:21:13 GMT  
		Size: 15.1 MB (15132561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5954e168cb50fb104f1abe5e1ab8f36cb2d56137292f600f518364011e3df1b`  
		Last Modified: Fri, 17 Nov 2023 19:21:13 GMT  
		Size: 16.1 MB (16099973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59352722cf28ac9eafad40b318890adcfcc45ca36c24eaa8a24be23e3137f244`  
		Last Modified: Fri, 17 Nov 2023 19:21:12 GMT  
		Size: 16.8 MB (16837156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5ce78514e9981ef39658f3b4afea0c61e21bbdde86bc4a608c6810bdfbf369`  
		Last Modified: Fri, 17 Nov 2023 19:21:09 GMT  
		Size: 543.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b175b9744b544bd3652735bf0ccfa9a4199600e79e61a38daf26dc2a640bba`  
		Last Modified: Fri, 17 Nov 2023 19:21:09 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38324ca8c3baecca94d04ce5aab9f7e62ff1a716662e2536e33fb3de99f7c8e4`  
		Last Modified: Fri, 17 Nov 2023 19:21:09 GMT  
		Size: 116.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b07d1b41691e6f7e9103211f92a03437519423b3d243021573e7252b59b622c`  
		Last Modified: Fri, 17 Nov 2023 20:20:31 GMT  
		Size: 9.0 MB (9046103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada21dc00a4dab675ea1ac34061978729e230cb72c7e297801e18880a3c139ed`  
		Last Modified: Fri, 17 Nov 2023 20:20:30 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6429b794052ea0f8a320a377aea4519619972612a84d4618f54a3515a2a8e6d0`  
		Last Modified: Fri, 17 Nov 2023 20:20:38 GMT  
		Size: 51.0 MB (50964385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd47f1b7ac5b36db315b8c36578852f560de76994908782a4f8762203f38466`  
		Last Modified: Fri, 17 Nov 2023 20:20:30 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7110e4dcec0ed056369a445af43e7ef302d2520a5371db38fc2078cfef73a9f2`  
		Last Modified: Fri, 17 Nov 2023 20:20:30 GMT  
		Size: 2.8 KB (2791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:dind` - linux; arm variant v7

```console
$ docker pull docker@sha256:ad99ac8b57925d1b4b9e7dc2fe249437641cc3d67ab34b4e189a8fe73e700775
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.0 MB (111997920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5c7e73afca77c3b674473c2894ca6524ef2a52144eadabb77000e00af5ea15b`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_VERSION=24.0.7
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.1
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-x86_64'; 			sha256='4f9b5313cf3eb1651b65aa6fc2fe1f59eb3812b7566f7c1b853be429b81bf3ab'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv6'; 			sha256='44b679381da55d1a673e5e638ac6d34f81e38e58ac656c530e27bb57a0ef930d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv7'; 			sha256='347b65d0cec622976bb753550d2708c8c9c760d55c1b5952a6800f5fadd4781c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-aarch64'; 			sha256='27b3cb1f066cdba191c4df96255a3d7178294763c9d67fba528f769968fc2e65'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-ppc64le'; 			sha256='76981fe4b032385752c5bb07144a22a7dfb599da15eca6fa1775e94364833475'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-riscv64'; 			sha256='1ee27dd153bd796686ece5d1829266b9b0db0a2ed67e7dbef023457da6dc5761'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-s390x'; 			sha256='9ee5fd812e7e52c08b95cd59673b956f2248343c2fb51eb8bcf635b02cfcbee4'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Oct 2023 17:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
CMD ["sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
VOLUME [/var/lib/docker]
# Thu, 26 Oct 2023 17:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
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
	-	`sha256:734588fa8ce31adf2dc94210cd8342f969f8b0e95bce00cca1ee11f8caeb8f81`  
		Last Modified: Fri, 27 Oct 2023 16:51:50 GMT  
		Size: 15.1 MB (15127058 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:be094786016ada203d28b6bd689aaa0c804ba33e6aae16aeace1a803c87d448c`  
		Last Modified: Fri, 17 Nov 2023 19:26:56 GMT  
		Size: 16.1 MB (16084089 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:918b5dce7a165d8ae0f32a894dc0ce6fd964f498c3ce545c7b94207b38e01f7b`  
		Last Modified: Fri, 17 Nov 2023 19:26:56 GMT  
		Size: 16.8 MB (16822958 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:516bb921a63bc30108055d28d31cbab7bb58cc9665fa52bec5d2ac1df1419a23`  
		Last Modified: Fri, 17 Nov 2023 19:26:55 GMT  
		Size: 543.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8b4aa870626a08b046d24d42ecae1f1580993e0b580d6039f2ff4f2d12d9d18`  
		Last Modified: Fri, 17 Nov 2023 19:26:55 GMT  
		Size: 1.0 KB (1019 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b262fdb80d4f76e5f44e601bc327cffb63bfe1761ee1d29a54293cf0ed6b48a7`  
		Last Modified: Fri, 17 Nov 2023 19:26:56 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:550c6d8fbe4881f50468cb713a52ccd20a82181128a43134e17913bab1711308`  
		Last Modified: Fri, 17 Nov 2023 20:26:28 GMT  
		Size: 8.2 MB (8217487 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:97ab26cc476dfbaabd49c7e55ae4eb42f2fa202ac9ed2196444c7b2353258c15`  
		Last Modified: Fri, 17 Nov 2023 20:26:28 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9477513991387f4c6a61790606b807f684169fe5b5d0641980c51cc6eb78cb0f`  
		Last Modified: Fri, 17 Nov 2023 20:26:30 GMT  
		Size: 51.0 MB (50964342 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f9101132d5eb8483d660d1f05eed458df56e2b56c5f5e3e5e2648e081f8cc37c`  
		Last Modified: Fri, 17 Nov 2023 20:26:28 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d024d05fd1ebd03798b6c47766e20b22d0529cb6273cb92a9b756715e737ae51`  
		Last Modified: Fri, 17 Nov 2023 20:26:29 GMT  
		Size: 2.8 KB (2790 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind` - unknown; unknown

```console
$ docker pull docker@sha256:22340d024bf0d73a44a14094db9ca1cff2c1b986a41f49c20a6d93beb91becc3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **709.2 KB (709190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8b0be4761c168d2d9c016a0e3ea09f144d5d399af3dbbe25c2020309e47ff8c`

```dockerfile
```

-	Layers:
	-	`sha256:3a76eab50d36380b37b8d3294a06d66a2a2de1a0d3d46f448af55c87f933178a`  
		Last Modified: Fri, 17 Nov 2023 20:26:27 GMT  
		Size: 678.9 KB (678858 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7f400c71e56574d7a2b05eeeada508d7678d1c10ce28d3bbc2831cc0bf9aef96`  
		Last Modified: Fri, 17 Nov 2023 20:26:27 GMT  
		Size: 30.3 KB (30332 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:dind` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:b20b11cc1aaabeda6af5ab8bce86de98276efd160005cb6690ef78d594de51a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111797483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be10b2a855378c946b2abd0349a919842b2ed33256731e75e1a7dba8a3eb3209`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_VERSION=24.0.7
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.1
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-x86_64'; 			sha256='4f9b5313cf3eb1651b65aa6fc2fe1f59eb3812b7566f7c1b853be429b81bf3ab'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv6'; 			sha256='44b679381da55d1a673e5e638ac6d34f81e38e58ac656c530e27bb57a0ef930d'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-armv7'; 			sha256='347b65d0cec622976bb753550d2708c8c9c760d55c1b5952a6800f5fadd4781c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-aarch64'; 			sha256='27b3cb1f066cdba191c4df96255a3d7178294763c9d67fba528f769968fc2e65'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-ppc64le'; 			sha256='76981fe4b032385752c5bb07144a22a7dfb599da15eca6fa1775e94364833475'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-riscv64'; 			sha256='1ee27dd153bd796686ece5d1829266b9b0db0a2ed67e7dbef023457da6dc5761'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.1/docker-compose-linux-s390x'; 			sha256='9ee5fd812e7e52c08b95cd59673b956f2248343c2fb51eb8bcf635b02cfcbee4'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Thu, 26 Oct 2023 17:04:13 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
CMD ["sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/stable/x86_64/docker-24.0.7.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/stable/armel/docker-24.0.7.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/stable/armhf/docker-24.0.7.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/stable/aarch64/docker-24.0.7.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
ENV DIND_COMMIT=d58df1fc6c866447ce2cd129af10e5b507705624
# Thu, 26 Oct 2023 17:04:13 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Thu, 26 Oct 2023 17:04:13 GMT
VOLUME [/var/lib/docker]
# Thu, 26 Oct 2023 17:04:13 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Thu, 26 Oct 2023 17:04:13 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Thu, 26 Oct 2023 17:04:13 GMT
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
	-	`sha256:99624a4fd86a4c6eda9530ba81d64e854494d3513e2b65182d975a3e73659f6a`  
		Last Modified: Fri, 27 Oct 2023 17:27:58 GMT  
		Size: 15.4 MB (15449538 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7f8d0b91b302e88cfdcf7ce318907c82d76a6158db3fbc7d2a269b8cf13135b3`  
		Last Modified: Fri, 17 Nov 2023 19:28:11 GMT  
		Size: 15.6 MB (15640599 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e31780ec4a8a2b24c00bffc2484d7f0ea31b9fc4adf2a6e98c84b9de4e40b60`  
		Last Modified: Fri, 17 Nov 2023 19:28:11 GMT  
		Size: 16.3 MB (16270028 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d899e0bff32f93f270d42551378813842bde4572beb443c52c879a80e0eb399c`  
		Last Modified: Fri, 17 Nov 2023 19:28:11 GMT  
		Size: 542.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89404bff69902dc2e075f68f78bdc5cce83ac1c0921917e0aeb4805978821dc8`  
		Last Modified: Fri, 17 Nov 2023 19:28:10 GMT  
		Size: 1.0 KB (1018 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e97f59fef71f84faf6f56411e944cbd8142cbf17b89564afb32a2353f443cd1c`  
		Last Modified: Fri, 17 Nov 2023 19:28:11 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9616ca4bc0cf47c676038d1ffe8c34890609627bfdc6a422ae7011d61b83cd5b`  
		Last Modified: Fri, 17 Nov 2023 20:27:41 GMT  
		Size: 9.4 MB (9362899 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7c904dd7e916461182d3e06043ea677c3134371fb0f66f35ffc50997dbc88a46`  
		Last Modified: Fri, 17 Nov 2023 20:27:40 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e12b927a57b7527c21f5c40fcb5411a48ed67eee331fcedc5a78a2b1e1ef50ff`  
		Last Modified: Fri, 17 Nov 2023 20:27:42 GMT  
		Size: 49.7 MB (49711206 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf6b0253fa4699c845dc51f482bbb4dcb9797a4e89c5838e7b2119a6d7ab2174`  
		Last Modified: Fri, 17 Nov 2023 20:27:40 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:894ce5b2ccc74d2860e7d7399f794f3d728eedc593488c640a5525e20f186203`  
		Last Modified: Fri, 17 Nov 2023 20:27:41 GMT  
		Size: 2.8 KB (2792 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:dind` - unknown; unknown

```console
$ docker pull docker@sha256:fd3342fb1d1ed572831ca609581ca669ba19061dda302fba26fb52c9c0bc536b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **709.0 KB (708995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c850ecbee42acd1f7b66748f636501667ae2391ea653e2a0d349b7ae9fb67331`

```dockerfile
```

-	Layers:
	-	`sha256:50d24caa41f8bcdbad2aa623555494f598879c181d019cd8111cbdd3c490536b`  
		Last Modified: Fri, 17 Nov 2023 20:27:40 GMT  
		Size: 678.8 KB (678797 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0736fd0ccdf6fffd94111232cfbbf1a88ce669c526828ad9ae07ee4f4d879ef3`  
		Last Modified: Fri, 17 Nov 2023 20:27:39 GMT  
		Size: 30.2 KB (30198 bytes)  
		MIME: application/vnd.in-toto+json
