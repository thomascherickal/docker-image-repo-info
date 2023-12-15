## `docker:25-rc-dind-rootless`

```console
$ docker pull docker@sha256:247bce94aec510f2236ed1353f0cd898112e66f2a4626c9f6dc14389bc563471
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 4
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown

### `docker:25-rc-dind-rootless` - linux; amd64

```console
$ docker pull docker@sha256:402f7fed1f84de7c771f7501f0a7598f347f4f71a29fa889a8a65ce91e9b48bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141891092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83140112e2582356325aa1cc8e8e8b5183c8bda9a4e741d978c3ea8441dca03`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Tue, 12 Dec 2023 23:39:18 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENV DOCKER_VERSION=25.0.0-beta.2
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.3
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-x86_64'; 			sha256='a836e807951db448f991f303cddcc9a4ec69f4a49d58bc7d536cb91c77c04c33'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv6'; 			sha256='b712693945360155842b578beace00effa723b604bfe1ccd6421645523e15d86'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv7'; 			sha256='4068bcbe1dd90034c8fe8d2c65b600ba793fc19bdb65db3c2dbf80b8a078de6c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-aarch64'; 			sha256='71f38f0923b8a9b80ad02c823ec3207d94677547aa5c618ca41b81d29fe6b9d9'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-ppc64le'; 			sha256='6110b0d30baee103c98ca5503bea24acb9d52bd333a67d3bf3c57d383c585c62'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-riscv64'; 			sha256='3ac26e5f272deb1364c9b8760af44c4dbd87d6faa42fc53bfec95885cfa8ae77'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-s390x'; 			sha256='2886dd4eddaea1eeb03537bdc596ec8947eb3ef7908c955284f8aad9170d3098'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Dec 2023 23:39:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Dec 2023 23:39:18 GMT
CMD ["sh"]
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	apk add --no-cache iptables-legacy; 	mkdir -p /usr/local/sbin/.iptables-legacy; 	for f in 		iptables 		iptables-save 		iptables-restore 		ip6tables 		ip6tables-save 		ip6tables-restore 	; do 		b="/sbin/${f/tables/tables-legacy}"; 		"$b" --version; 		ln -svT "$b" "/usr/local/sbin/.iptables-legacy/$f"; 	done; 	export PATH="/usr/local/sbin/.iptables-legacy:$PATH"; 	iptables --version | grep legacy # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENV DIND_COMMIT=65cfcc28ab37cb75e1560e4b4738719c07c6618e
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Dec 2023 23:39:18 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 12 Dec 2023 23:39:18 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Dec 2023 23:39:18 GMT
CMD []
# Tue, 12 Dec 2023 23:39:18 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 12 Dec 2023 23:39:18 GMT
USER rootless
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
	-	`sha256:a68b83bca30c94369721eb7282bdeb7fe328c1f9871ff6ddbf0e85659ecf46c4`  
		Last Modified: Fri, 15 Dec 2023 19:42:04 GMT  
		Size: 974.0 KB (974031 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bc9f1574defb650cbabc0bd70326503db8bfbdaf17291eb712bbf01b65fb0337`  
		Last Modified: Fri, 15 Dec 2023 19:42:03 GMT  
		Size: 116.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0abab6421f726137efdb320a567300d43d55151b259c4f82661ad31130a00300`  
		Last Modified: Fri, 15 Dec 2023 19:42:03 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2fbfbc2e2c6a4d638986d6d0e2aa7fa44ce3f02a48066ddb96cbbc99d7d9cde0`  
		Last Modified: Fri, 15 Dec 2023 19:42:05 GMT  
		Size: 20.9 MB (20862827 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9176ac0d2d229979ea5c2b5219b75e6f5f705331d728a71aaf8a8bec036de15b`  
		Last Modified: Fri, 15 Dec 2023 19:42:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:25-rc-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:78ca5b7f82e064947e939076dd48a2536e0147c298d38a02327919149545eb3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.0 KB (759006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ff133ed0e15db3f51bb3bb9c0ae5b5926ca2fb69eb2de97cdea2954314aa056`

```dockerfile
```

-	Layers:
	-	`sha256:62cdb08284ab0d86c98efb0688923c2dfaebc0c2c91245e96c740e8dca94b990`  
		Last Modified: Fri, 15 Dec 2023 19:42:03 GMT  
		Size: 727.1 KB (727062 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:af675e28e1be56140cf80caa93ecaaac96840580a858ff26823417ac4d6427c4`  
		Last Modified: Fri, 15 Dec 2023 19:42:03 GMT  
		Size: 31.9 KB (31944 bytes)  
		MIME: application/vnd.in-toto+json

### `docker:25-rc-dind-rootless` - linux; arm64 variant v8

```console
$ docker pull docker@sha256:16dda6576f6c87873a6a65a9e5daaadae17f588cd67851707b17501634f1f360
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.7 MB (135731956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c05ce124f5c520149a3ce7ea516d8c3a7a8c4e502cf72000625a7346f0de3fca`
-	Entrypoint: `["dockerd-entrypoint.sh"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Dec 2023 23:39:18 GMT
RUN apk add --no-cache 		ca-certificates 		openssh-client # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN [ -e /etc/nsswitch.conf ] && grep '^hosts: files dns' /etc/nsswitch.conf # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENV DOCKER_VERSION=25.0.0-beta.2
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		'docker/docker' 	; 	rm docker.tgz; 		docker --version # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENV DOCKER_BUILDX_VERSION=0.12.0
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-amd64'; 			sha256='7c393b92c148a0ce26c76a2abc99960be1d1097f0471978d41dc51d0c1a4471e'; 			;; 		'armhf') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v6'; 			sha256='62d9162f526c3bb7f67768a5b0d81a8b3ad0371406dfc1f0775e4f62dfca7fe1'; 			;; 		'armv7') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm-v7'; 			sha256='d941d6a5b072de775222d31d9f8467b4c1b1f56e3b08d1b78f828a9244c16464'; 			;; 		'aarch64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-arm64'; 			sha256='781caebb36551b035cb9dcfaf91088543d09c73c4a2549341e6417d86b8bbb50'; 			;; 		'ppc64le') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-ppc64le'; 			sha256='ab5bda4532528d6b0801c877999fce9def10c6a37624673fd13c668fdcde16b7'; 			;; 		'riscv64') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-riscv64'; 			sha256='a2b846919c44128c6db9165ad24545e7e10035b6f0ad01559fcfbb2a13017127'; 			;; 		's390x') 			url='https://github.com/docker/buildx/releases/download/v0.12.0/buildx-v0.12.0.linux-s390x'; 			sha256='81c2ada65624e2ac6bb4123f3a3bb933d04cfb08aa45fc55dd201ba523d96d30'; 			;; 		*) echo >&2 "warning: unsupported 'docker-buildx' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-buildx' "$url"; 	echo "$sha256 *"'docker-buildx' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-buildx'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-buildx' "$plugin"; 	chmod +x "$plugin"; 		docker buildx version # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENV DOCKER_COMPOSE_VERSION=2.23.3
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-x86_64'; 			sha256='a836e807951db448f991f303cddcc9a4ec69f4a49d58bc7d536cb91c77c04c33'; 			;; 		'armhf') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv6'; 			sha256='b712693945360155842b578beace00effa723b604bfe1ccd6421645523e15d86'; 			;; 		'armv7') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-armv7'; 			sha256='4068bcbe1dd90034c8fe8d2c65b600ba793fc19bdb65db3c2dbf80b8a078de6c'; 			;; 		'aarch64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-aarch64'; 			sha256='71f38f0923b8a9b80ad02c823ec3207d94677547aa5c618ca41b81d29fe6b9d9'; 			;; 		'ppc64le') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-ppc64le'; 			sha256='6110b0d30baee103c98ca5503bea24acb9d52bd333a67d3bf3c57d383c585c62'; 			;; 		'riscv64') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-riscv64'; 			sha256='3ac26e5f272deb1364c9b8760af44c4dbd87d6faa42fc53bfec95885cfa8ae77'; 			;; 		's390x') 			url='https://github.com/docker/compose/releases/download/v2.23.3/docker-compose-linux-s390x'; 			sha256='2886dd4eddaea1eeb03537bdc596ec8947eb3ef7908c955284f8aad9170d3098'; 			;; 		*) echo >&2 "warning: unsupported 'docker-compose' architecture ($apkArch); skipping"; exit 0 ;; 	esac; 		wget -O 'docker-compose' "$url"; 	echo "$sha256 *"'docker-compose' | sha256sum -c -; 		plugin='/usr/local/libexec/docker/cli-plugins/docker-compose'; 	mkdir -p "$(dirname "$plugin")"; 	mv -vT 'docker-compose' "$plugin"; 	chmod +x "$plugin"; 		ln -sv "$plugin" /usr/local/bin/; 	docker-compose --version; 	docker compose version # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
COPY modprobe.sh /usr/local/bin/modprobe # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENV DOCKER_TLS_CERTDIR=/certs
# Tue, 12 Dec 2023 23:39:18 GMT
RUN mkdir /certs /certs/client && chmod 1777 /certs /certs/client # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Dec 2023 23:39:18 GMT
CMD ["sh"]
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	apk add --no-cache 		btrfs-progs 		e2fsprogs 		e2fsprogs-extra 		ip6tables 		iptables 		openssl 		shadow-uidmap 		xfsprogs 		xz 		pigz 	; 	if zfs="$(apk info --no-cache --quiet zfs)" && [ -n "$zfs" ]; then 		apk add --no-cache zfs; 	fi # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	apk add --no-cache iptables-legacy; 	mkdir -p /usr/local/sbin/.iptables-legacy; 	for f in 		iptables 		iptables-save 		iptables-restore 		ip6tables 		ip6tables-save 		ip6tables-restore 	; do 		b="/sbin/${f/tables/tables-legacy}"; 		"$b" --version; 		ln -svT "$b" "/usr/local/sbin/.iptables-legacy/$f"; 	done; 	export PATH="/usr/local/sbin/.iptables-legacy:$PATH"; 	iptables --version | grep legacy # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	addgroup -S dockremap; 	adduser -S -G dockremap dockremap; 	echo 'dockremap:165536:65536' >> /etc/subuid; 	echo 'dockremap:165536:65536' >> /etc/subgid # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-25.0.0-beta.2.tgz'; 			;; 		'armhf') 			url='https://download.docker.com/linux/static/test/armel/docker-25.0.0-beta.2.tgz'; 			;; 		'armv7') 			url='https://download.docker.com/linux/static/test/armhf/docker-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'docker.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'docker.tgz' "$url"; 		tar --extract 		--file docker.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		--no-same-owner 		--exclude 'docker/docker' 	; 	rm docker.tgz; 		dockerd --version; 	containerd --version; 	ctr --version; 	runc --version # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
ENV DIND_COMMIT=65cfcc28ab37cb75e1560e4b4738719c07c6618e
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	wget -O /usr/local/bin/dind "https://raw.githubusercontent.com/docker/docker/${DIND_COMMIT}/hack/dind"; 	chmod +x /usr/local/bin/dind # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
COPY dockerd-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
VOLUME [/var/lib/docker]
# Tue, 12 Dec 2023 23:39:18 GMT
EXPOSE map[2375/tcp:{} 2376/tcp:{}]
# Tue, 12 Dec 2023 23:39:18 GMT
ENTRYPOINT ["dockerd-entrypoint.sh"]
# Tue, 12 Dec 2023 23:39:18 GMT
CMD []
# Tue, 12 Dec 2023 23:39:18 GMT
RUN apk add --no-cache iproute2 fuse-overlayfs # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN mkdir /run/user && chmod 1777 /run/user # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	adduser -h /home/rootless -g 'Rootless' -D -u 1000 rootless; 	echo 'rootless:100000:65536' >> /etc/subuid; 	echo 'rootless:100000:65536' >> /etc/subgid # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			url='https://download.docker.com/linux/static/test/x86_64/docker-rootless-extras-25.0.0-beta.2.tgz'; 			;; 		'aarch64') 			url='https://download.docker.com/linux/static/test/aarch64/docker-rootless-extras-25.0.0-beta.2.tgz'; 			;; 		*) echo >&2 "error: unsupported 'rootless.tgz' architecture ($apkArch)"; exit 1 ;; 	esac; 		wget -O 'rootless.tgz' "$url"; 		tar --extract 		--file rootless.tgz 		--strip-components 1 		--directory /usr/local/bin/ 		'docker-rootless-extras/rootlesskit' 		'docker-rootless-extras/rootlesskit-docker-proxy' 		'docker-rootless-extras/vpnkit' 	; 	rm rootless.tgz; 		rootlesskit --version; 	vpnkit --version # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
RUN set -eux; 	mkdir -p /home/rootless/.local/share/docker; 	chown -R rootless:rootless /home/rootless/.local/share/docker # buildkit
# Tue, 12 Dec 2023 23:39:18 GMT
VOLUME [/home/rootless/.local/share/docker]
# Tue, 12 Dec 2023 23:39:18 GMT
USER rootless
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
	-	`sha256:7f02fbf2ed8fce5b8dbcf506b3431abd0fce65d4c10c6b8625c6652d07de8760`  
		Last Modified: Fri, 15 Dec 2023 19:53:35 GMT  
		Size: 1.0 MB (1016219 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:591fcca901c77cb2dbd53c1d2bceb8059b7d03ee1c9127fa87f44a4d238a5d27`  
		Last Modified: Fri, 15 Dec 2023 19:53:34 GMT  
		Size: 115.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:553ab0cbf3342a4d600b6f39ed7f5949034c081e5405be25b0185a3bdd706adf`  
		Last Modified: Fri, 15 Dec 2023 19:53:35 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cd580303f5033a3684ac577fd2d720b24be56566bdc4367fbd68ea90c5c6c9bf`  
		Last Modified: Fri, 15 Dec 2023 19:53:36 GMT  
		Size: 22.7 MB (22729178 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ad87b37face86e0762ece67959932a7f0dd41566b9d652146257e7ca5b02e1a5`  
		Last Modified: Fri, 15 Dec 2023 19:53:35 GMT  
		Size: 189.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `docker:25-rc-dind-rootless` - unknown; unknown

```console
$ docker pull docker@sha256:fa8576fd81a6a1d318019eff377fc9bc4426dc8f0e6a0f61fa12214dcb5ac327
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **759.1 KB (759077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bde418813affb652105e5592cc1efa5dc81d4dd8820feeb1d1e7998dd1d76525`

```dockerfile
```

-	Layers:
	-	`sha256:7133e0a2e061718c008fe149daa8daf8cae779cb5c29a69ceda9ee4eea8d1c04`  
		Last Modified: Fri, 15 Dec 2023 19:53:34 GMT  
		Size: 727.1 KB (727071 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:0790df993b093290b1a0ee35dca7a42f8e0205101803eb39211eb6c33c4a4f0e`  
		Last Modified: Fri, 15 Dec 2023 19:53:34 GMT  
		Size: 32.0 KB (32006 bytes)  
		MIME: application/vnd.in-toto+json
