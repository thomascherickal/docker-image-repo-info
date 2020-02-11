<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:0.9`](#consul09)
-	[`consul:0.9.4`](#consul094)
-	[`consul:1.0`](#consul10)
-	[`consul:1.0.8`](#consul108)
-	[`consul:1.1`](#consul11)
-	[`consul:1.1.1`](#consul111)
-	[`consul:1.2`](#consul12)
-	[`consul:1.2.4`](#consul124)
-	[`consul:1.3`](#consul13)
-	[`consul:1.3.1`](#consul131)
-	[`consul:1.4`](#consul14)
-	[`consul:1.4.5`](#consul145)
-	[`consul:1.5`](#consul15)
-	[`consul:1.5.3`](#consul153)
-	[`consul:1.6`](#consul16)
-	[`consul:1.6.3`](#consul163)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.0`](#consul170)
-	[`consul:latest`](#consullatest)

## `consul:0.9`

```console
$ docker pull consul@sha256:0ccee2cf2dd6b09d6a09e03c84b03858e58119641109590686ee9f3ce893b0cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:0.9` - linux; amd64

```console
$ docker pull consul@sha256:c5dc83dce10cde85e81b69e35ea41e0bbdacdf0a548dabd001482075ae27a395
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14581666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8940e357b6bdbb1c47c1a1632c7765b284b627a69262bc6fd6181b33931ad45a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:17:29 GMT
ENV CONSUL_VERSION=0.9.4
# Thu, 23 Jan 2020 17:17:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:17:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:17:35 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:17:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:17:38 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:17:38 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:17:38 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:17:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:17:39 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:17:39 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:17:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddad4b3e0ff70fc3cd94dd63ff91a03452fd185e7c590e4cfd9f13c2b0b0172`  
		Last Modified: Thu, 23 Jan 2020 17:20:28 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcd1743e6f6912b7484b82019b94682e0c2ec57af17ed92b27af365cf97e79f`  
		Last Modified: Thu, 23 Jan 2020 17:20:36 GMT  
		Size: 11.8 MB (11814266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f42004c8c977650144f1b96957d7e31a2c97a656cf0fc836289cde24a86b8d`  
		Last Modified: Thu, 23 Jan 2020 17:20:28 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d50e5c336e354355843c8bca67d6ff1cf681eff136a085a8c951d29ee554762`  
		Last Modified: Thu, 23 Jan 2020 17:20:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fe4da42f21bfdd71a1427a509b2eb94632875b29740619b390bd23e54e4d49`  
		Last Modified: Thu, 23 Jan 2020 17:20:28 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:bb8e6f59a7196d6405ac7e6293d86cec887b4609f7311272dd7f2ed9097695f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13744162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb3f246af9963198e54e6f334293a78785d65fb09fc9b342fee3aff4f530c20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:42 GMT
ENV CONSUL_VERSION=0.9.4
# Thu, 23 Jan 2020 17:16:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:16:44 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:16:50 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:53 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:55 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:56 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:56 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:58 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:58 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:17:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854b831dcefb1e3c6c6c72dcc21f1b7dffe51ce73d852e0df725225dfbdf6b0c`  
		Last Modified: Thu, 23 Jan 2020 17:20:57 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306547b4e8c79bcf2c1947fca7e322211f2bf48b1a0c9f46d2872a890d2f71ed`  
		Last Modified: Thu, 23 Jan 2020 17:21:01 GMT  
		Size: 11.2 MB (11193200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ed30e2f82c08e31da237145b68a7b3bfeee7e27eeab2396080fb106ade9289`  
		Last Modified: Thu, 23 Jan 2020 17:20:57 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794bd9dc1bc28bfdcd78e8f248d76431158d7674e5627b75a61dd3d69e15eb35`  
		Last Modified: Thu, 23 Jan 2020 17:20:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffa9084bad223d93fd996ba4b4af2035e32ac6389a057e8c9dc5d60f3c68565`  
		Last Modified: Thu, 23 Jan 2020 17:20:57 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:702520973c43b475f43e292c994868f8736c5f66f12add272f58705572f358f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13789386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d36b08285c9d7d26d8bf2782a491bc712d3a3d0cba7bb7af3e09e441db0606d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:23:54 GMT
ENV CONSUL_VERSION=0.9.4
# Thu, 23 Jan 2020 17:23:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:23:57 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:24:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:24:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:24:06 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:24:07 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:24:08 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:24:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:24:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:24:10 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:24:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9a35ae03d22d598f34c3da928c9df1b7e124636713866ad031f0da661fc4f5`  
		Last Modified: Thu, 23 Jan 2020 17:27:53 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddbce5dac2f91e5b3d055229e892fac0dfd28a357d6e4be602155d6d692bd1d`  
		Last Modified: Thu, 23 Jan 2020 17:28:00 GMT  
		Size: 11.1 MB (11092860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c15a21030316cfbc6b490af6c31965c1a7e756af92f28e3805c3a893ab9cbf7`  
		Last Modified: Thu, 23 Jan 2020 17:27:53 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7416948ef4f56d8d07606ce587d84828afd30f04dd99ff2b78c23f5c0acdbaf`  
		Last Modified: Thu, 23 Jan 2020 17:27:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0d01e82b8ff8965f3b7e8cb102cc13b16924bac20e67c8b57963f94952703`  
		Last Modified: Thu, 23 Jan 2020 17:27:54 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9` - linux; 386

```console
$ docker pull consul@sha256:d47f059c497241f0847c65ea47e8595209b52498080c61a3b92639584ac80f56
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.3 MB (14265094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb59f4234c90595badcd63154fcc9a6d3ec45cbdeb98477538660d26f4e21fb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:59:27 GMT
ENV CONSUL_VERSION=0.9.4
# Thu, 23 Jan 2020 17:59:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:59:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:59:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:59:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:59:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:59:36 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:59:36 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:59:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:59:37 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:59:37 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:59:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e28e104d0ec20f8507ad7393233a90e5a59b3a8a7bfdb344d6f5b54faf51bf`  
		Last Modified: Thu, 23 Jan 2020 18:03:01 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c6bf3b72589a0a1af90d2d4a402f80ec3b27850c95eb6a93b13306ccdeb4eb`  
		Last Modified: Thu, 23 Jan 2020 18:03:04 GMT  
		Size: 11.5 MB (11493344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc49be4f803f13c7fbb59691dcb257e9266d93e4ae95158a9504f54e58ca55b`  
		Last Modified: Thu, 23 Jan 2020 18:03:01 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905ab9645182a27f3c345763724f3bfdaa8e4c4dc4bf1fd13a763bba44405f2d`  
		Last Modified: Thu, 23 Jan 2020 18:03:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b6f0235f5391c85df9475e86e5789c3f12b78772df346376a5683f192136ad`  
		Last Modified: Thu, 23 Jan 2020 18:03:01 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:0.9.4`

```console
$ docker pull consul@sha256:0ccee2cf2dd6b09d6a09e03c84b03858e58119641109590686ee9f3ce893b0cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:0.9.4` - linux; amd64

```console
$ docker pull consul@sha256:c5dc83dce10cde85e81b69e35ea41e0bbdacdf0a548dabd001482075ae27a395
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14581666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8940e357b6bdbb1c47c1a1632c7765b284b627a69262bc6fd6181b33931ad45a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:17:29 GMT
ENV CONSUL_VERSION=0.9.4
# Thu, 23 Jan 2020 17:17:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:17:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:17:35 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:17:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:17:38 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:17:38 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:17:38 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:17:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:17:39 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:17:39 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:17:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:17:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddad4b3e0ff70fc3cd94dd63ff91a03452fd185e7c590e4cfd9f13c2b0b0172`  
		Last Modified: Thu, 23 Jan 2020 17:20:28 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcd1743e6f6912b7484b82019b94682e0c2ec57af17ed92b27af365cf97e79f`  
		Last Modified: Thu, 23 Jan 2020 17:20:36 GMT  
		Size: 11.8 MB (11814266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f42004c8c977650144f1b96957d7e31a2c97a656cf0fc836289cde24a86b8d`  
		Last Modified: Thu, 23 Jan 2020 17:20:28 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d50e5c336e354355843c8bca67d6ff1cf681eff136a085a8c951d29ee554762`  
		Last Modified: Thu, 23 Jan 2020 17:20:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fe4da42f21bfdd71a1427a509b2eb94632875b29740619b390bd23e54e4d49`  
		Last Modified: Thu, 23 Jan 2020 17:20:28 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:bb8e6f59a7196d6405ac7e6293d86cec887b4609f7311272dd7f2ed9097695f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.7 MB (13744162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb3f246af9963198e54e6f334293a78785d65fb09fc9b342fee3aff4f530c20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:42 GMT
ENV CONSUL_VERSION=0.9.4
# Thu, 23 Jan 2020 17:16:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:16:44 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:16:50 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:53 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:55 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:56 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:56 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:58 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:58 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:17:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854b831dcefb1e3c6c6c72dcc21f1b7dffe51ce73d852e0df725225dfbdf6b0c`  
		Last Modified: Thu, 23 Jan 2020 17:20:57 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:306547b4e8c79bcf2c1947fca7e322211f2bf48b1a0c9f46d2872a890d2f71ed`  
		Last Modified: Thu, 23 Jan 2020 17:21:01 GMT  
		Size: 11.2 MB (11193200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ed30e2f82c08e31da237145b68a7b3bfeee7e27eeab2396080fb106ade9289`  
		Last Modified: Thu, 23 Jan 2020 17:20:57 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794bd9dc1bc28bfdcd78e8f248d76431158d7674e5627b75a61dd3d69e15eb35`  
		Last Modified: Thu, 23 Jan 2020 17:20:57 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fffa9084bad223d93fd996ba4b4af2035e32ac6389a057e8c9dc5d60f3c68565`  
		Last Modified: Thu, 23 Jan 2020 17:20:57 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:702520973c43b475f43e292c994868f8736c5f66f12add272f58705572f358f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13789386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d36b08285c9d7d26d8bf2782a491bc712d3a3d0cba7bb7af3e09e441db0606d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:23:54 GMT
ENV CONSUL_VERSION=0.9.4
# Thu, 23 Jan 2020 17:23:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:23:57 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:24:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:24:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:24:06 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:24:07 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:24:08 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:24:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:24:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:24:10 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:24:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:24:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9a35ae03d22d598f34c3da928c9df1b7e124636713866ad031f0da661fc4f5`  
		Last Modified: Thu, 23 Jan 2020 17:27:53 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ddbce5dac2f91e5b3d055229e892fac0dfd28a357d6e4be602155d6d692bd1d`  
		Last Modified: Thu, 23 Jan 2020 17:28:00 GMT  
		Size: 11.1 MB (11092860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c15a21030316cfbc6b490af6c31965c1a7e756af92f28e3805c3a893ab9cbf7`  
		Last Modified: Thu, 23 Jan 2020 17:27:53 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7416948ef4f56d8d07606ce587d84828afd30f04dd99ff2b78c23f5c0acdbaf`  
		Last Modified: Thu, 23 Jan 2020 17:27:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb0d01e82b8ff8965f3b7e8cb102cc13b16924bac20e67c8b57963f94952703`  
		Last Modified: Thu, 23 Jan 2020 17:27:54 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:0.9.4` - linux; 386

```console
$ docker pull consul@sha256:d47f059c497241f0847c65ea47e8595209b52498080c61a3b92639584ac80f56
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.3 MB (14265094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb59f4234c90595badcd63154fcc9a6d3ec45cbdeb98477538660d26f4e21fb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:59:27 GMT
ENV CONSUL_VERSION=0.9.4
# Thu, 23 Jan 2020 17:59:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:59:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:59:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:59:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:59:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:59:36 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:59:36 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:59:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:59:37 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:59:37 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:59:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:59:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e28e104d0ec20f8507ad7393233a90e5a59b3a8a7bfdb344d6f5b54faf51bf`  
		Last Modified: Thu, 23 Jan 2020 18:03:01 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c6bf3b72589a0a1af90d2d4a402f80ec3b27850c95eb6a93b13306ccdeb4eb`  
		Last Modified: Thu, 23 Jan 2020 18:03:04 GMT  
		Size: 11.5 MB (11493344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc49be4f803f13c7fbb59691dcb257e9266d93e4ae95158a9504f54e58ca55b`  
		Last Modified: Thu, 23 Jan 2020 18:03:01 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905ab9645182a27f3c345763724f3bfdaa8e4c4dc4bf1fd13a763bba44405f2d`  
		Last Modified: Thu, 23 Jan 2020 18:03:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b6f0235f5391c85df9475e86e5789c3f12b78772df346376a5683f192136ad`  
		Last Modified: Thu, 23 Jan 2020 18:03:01 GMT  
		Size: 1.7 KB (1681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.0`

```console
$ docker pull consul@sha256:6dfe59a6eca40d39904497df186beacc460bc97107537893b6ffc7bfe5d471ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.0` - linux; amd64

```console
$ docker pull consul@sha256:9942f0518293aa00ae0d6439f5074bd48e83b0e4e9f21e18ba3e9976668b7dbd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16595618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cbb12477735f3eb626b19b811ea28e7149aeafd5f47563becb8aa6b6fc9a88e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:17:14 GMT
ENV CONSUL_VERSION=1.0.8
# Thu, 23 Jan 2020 17:17:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:17:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:17:20 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:17:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:17:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:17:23 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:17:23 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:17:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:17:23 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:17:24 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:17:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:17:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a735925e960bfb965103741eb84a295fcd5a8859074cadd495564d41ce2c6`  
		Last Modified: Thu, 23 Jan 2020 17:20:19 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eecfab37a9845176e6c457eead6da1e495088da00c448e95556de198a9d5a99`  
		Last Modified: Thu, 23 Jan 2020 17:20:23 GMT  
		Size: 13.8 MB (13828214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c3d997d679c833acef18a377aabb870578d73991dd031501b59520d5b1068`  
		Last Modified: Thu, 23 Jan 2020 17:20:19 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f7ba4eb550de2fd79fc9f84acc66a0de6bec680408ead05b69ab53fc158329`  
		Last Modified: Thu, 23 Jan 2020 17:20:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ce656d5b4660e3baf0c4e5b9537bf8dc221ebae1bb581ca049ed997398eee`  
		Last Modified: Thu, 23 Jan 2020 17:20:19 GMT  
		Size: 1.7 KB (1680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0` - linux; arm variant v6

```console
$ docker pull consul@sha256:cc89fd19e453397c57e0451c4a7a4d7db54b175e42858b35b7f1aebeafd730c0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15926667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9037cd2470cdb71acfef5a1627ee8d2bb3ef2742db339ef60073063dfc7a2a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:19 GMT
ENV CONSUL_VERSION=1.0.8
# Thu, 23 Jan 2020 17:16:20 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:16:22 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:16:28 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:30 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:32 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:33 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:33 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:35 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:35 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186acd312e9e59bf3b9a5b024914b87f35f843b8f388827bfc4f84aa0510c940`  
		Last Modified: Thu, 23 Jan 2020 17:20:37 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dee013255c0d4e0d203a1d151b14bb417741defd468d275e505c6b2957c0151`  
		Last Modified: Thu, 23 Jan 2020 17:20:48 GMT  
		Size: 13.4 MB (13375710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f197567f26dfffcf465ec22016d743c240f1742c21f784e1d9aa95596837e2a9`  
		Last Modified: Thu, 23 Jan 2020 17:20:37 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dc207a98544d19759df4f997934adbd0cb65ffafaa08d510dadb79b5a1a0da`  
		Last Modified: Thu, 23 Jan 2020 17:20:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb98875b7668a8136a3b9df28acd1b058a357e11c4106157440a8f4b9b9a0fc`  
		Last Modified: Thu, 23 Jan 2020 17:20:37 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a4ad77f0ab5e582b7fbbfd0b5c24a3ba0ddcc6958e17cab54a39a46a59aab36c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15937701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:615191e2ff98d07c86cf3a061b752808ba17abd0932c3ad79c9b8a88bc10f478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:23:29 GMT
ENV CONSUL_VERSION=1.0.8
# Thu, 23 Jan 2020 17:23:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:23:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:23:37 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:23:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:23:41 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:23:42 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:23:42 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:23:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:23:44 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:23:44 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:23:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:23:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f67b753ffa58715006a169c5bc0fc97254389a09fc4d2994d6ecfa462ad612`  
		Last Modified: Thu, 23 Jan 2020 17:27:41 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca863c51b1fd31d8934a25dcedc9a2ecbce9637b5f5eeca7e05791f31c928827`  
		Last Modified: Thu, 23 Jan 2020 17:27:46 GMT  
		Size: 13.2 MB (13241178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d957ab1b179315468f071fd09af8b8cf4ecb5c5738227aabb8e21f30ba0f6c15`  
		Last Modified: Thu, 23 Jan 2020 17:27:41 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48b27b30d4ccd928a8dfa42042e7addf3b950bf32e1611f2db862000773c793`  
		Last Modified: Thu, 23 Jan 2020 17:27:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5be6bcaf9e62af8f545358f75e3aceb0d225ce628d5d51f05ac1cb6a467a5a`  
		Last Modified: Thu, 23 Jan 2020 17:27:41 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0` - linux; 386

```console
$ docker pull consul@sha256:eec42fbe7a5f7f043e1af590ea0533abedb5a204a894bc735c2c122fecb8bfb6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16488428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bbd5461bb6ea13f0abd570bd9a4cd2caffc61df225e0e62c52f8c1971fcb026`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:59:11 GMT
ENV CONSUL_VERSION=1.0.8
# Thu, 23 Jan 2020 17:59:12 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:59:13 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:59:18 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:59:20 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:59:21 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:59:21 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:59:21 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:59:22 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:59:22 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:59:22 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:59:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:59:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2459459b1e06b453537cb5cdc1c91abde65c212806250cd3434495e8d9746bd`  
		Last Modified: Thu, 23 Jan 2020 18:02:52 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a172dbf767ea0f19741367696429fedee78a328523a3297ce4131bf0ba20fa0`  
		Last Modified: Thu, 23 Jan 2020 18:02:56 GMT  
		Size: 13.7 MB (13716677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1deb4fe7d28fbabc3e88bc7e11924e99f47212d82ff0a190bf0fce82b2c1b61`  
		Last Modified: Thu, 23 Jan 2020 18:02:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba751cfcae186a3b77e919f182dd66f8012525efea263a9dd93b27ccc23acec`  
		Last Modified: Thu, 23 Jan 2020 18:02:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f9745a993429207fdd3da320a6917081221d49a762e551896031ebd63f08b4`  
		Last Modified: Thu, 23 Jan 2020 18:02:52 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.0.8`

```console
$ docker pull consul@sha256:6dfe59a6eca40d39904497df186beacc460bc97107537893b6ffc7bfe5d471ea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.0.8` - linux; amd64

```console
$ docker pull consul@sha256:9942f0518293aa00ae0d6439f5074bd48e83b0e4e9f21e18ba3e9976668b7dbd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16595618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cbb12477735f3eb626b19b811ea28e7149aeafd5f47563becb8aa6b6fc9a88e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:17:14 GMT
ENV CONSUL_VERSION=1.0.8
# Thu, 23 Jan 2020 17:17:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:17:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:17:20 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:17:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:17:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:17:23 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:17:23 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:17:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:17:23 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:17:24 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:17:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:17:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299a735925e960bfb965103741eb84a295fcd5a8859074cadd495564d41ce2c6`  
		Last Modified: Thu, 23 Jan 2020 17:20:19 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eecfab37a9845176e6c457eead6da1e495088da00c448e95556de198a9d5a99`  
		Last Modified: Thu, 23 Jan 2020 17:20:23 GMT  
		Size: 13.8 MB (13828214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94c3d997d679c833acef18a377aabb870578d73991dd031501b59520d5b1068`  
		Last Modified: Thu, 23 Jan 2020 17:20:19 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f7ba4eb550de2fd79fc9f84acc66a0de6bec680408ead05b69ab53fc158329`  
		Last Modified: Thu, 23 Jan 2020 17:20:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66ce656d5b4660e3baf0c4e5b9537bf8dc221ebae1bb581ca049ed997398eee`  
		Last Modified: Thu, 23 Jan 2020 17:20:19 GMT  
		Size: 1.7 KB (1680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:cc89fd19e453397c57e0451c4a7a4d7db54b175e42858b35b7f1aebeafd730c0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15926667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9037cd2470cdb71acfef5a1627ee8d2bb3ef2742db339ef60073063dfc7a2a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:19 GMT
ENV CONSUL_VERSION=1.0.8
# Thu, 23 Jan 2020 17:16:20 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:16:22 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:16:28 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:30 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:32 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:33 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:33 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:35 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:35 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186acd312e9e59bf3b9a5b024914b87f35f843b8f388827bfc4f84aa0510c940`  
		Last Modified: Thu, 23 Jan 2020 17:20:37 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dee013255c0d4e0d203a1d151b14bb417741defd468d275e505c6b2957c0151`  
		Last Modified: Thu, 23 Jan 2020 17:20:48 GMT  
		Size: 13.4 MB (13375710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f197567f26dfffcf465ec22016d743c240f1742c21f784e1d9aa95596837e2a9`  
		Last Modified: Thu, 23 Jan 2020 17:20:37 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20dc207a98544d19759df4f997934adbd0cb65ffafaa08d510dadb79b5a1a0da`  
		Last Modified: Thu, 23 Jan 2020 17:20:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb98875b7668a8136a3b9df28acd1b058a357e11c4106157440a8f4b9b9a0fc`  
		Last Modified: Thu, 23 Jan 2020 17:20:37 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a4ad77f0ab5e582b7fbbfd0b5c24a3ba0ddcc6958e17cab54a39a46a59aab36c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15937701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:615191e2ff98d07c86cf3a061b752808ba17abd0932c3ad79c9b8a88bc10f478`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:23:29 GMT
ENV CONSUL_VERSION=1.0.8
# Thu, 23 Jan 2020 17:23:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:23:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:23:37 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:23:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:23:41 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:23:42 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:23:42 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:23:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:23:44 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:23:44 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:23:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:23:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f67b753ffa58715006a169c5bc0fc97254389a09fc4d2994d6ecfa462ad612`  
		Last Modified: Thu, 23 Jan 2020 17:27:41 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca863c51b1fd31d8934a25dcedc9a2ecbce9637b5f5eeca7e05791f31c928827`  
		Last Modified: Thu, 23 Jan 2020 17:27:46 GMT  
		Size: 13.2 MB (13241178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d957ab1b179315468f071fd09af8b8cf4ecb5c5738227aabb8e21f30ba0f6c15`  
		Last Modified: Thu, 23 Jan 2020 17:27:41 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48b27b30d4ccd928a8dfa42042e7addf3b950bf32e1611f2db862000773c793`  
		Last Modified: Thu, 23 Jan 2020 17:27:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5be6bcaf9e62af8f545358f75e3aceb0d225ce628d5d51f05ac1cb6a467a5a`  
		Last Modified: Thu, 23 Jan 2020 17:27:41 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.0.8` - linux; 386

```console
$ docker pull consul@sha256:eec42fbe7a5f7f043e1af590ea0533abedb5a204a894bc735c2c122fecb8bfb6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.5 MB (16488428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bbd5461bb6ea13f0abd570bd9a4cd2caffc61df225e0e62c52f8c1971fcb026`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:59:11 GMT
ENV CONSUL_VERSION=1.0.8
# Thu, 23 Jan 2020 17:59:12 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:59:13 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:59:18 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:59:20 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:59:21 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:59:21 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:59:21 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:59:22 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:59:22 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:59:22 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:59:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:59:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2459459b1e06b453537cb5cdc1c91abde65c212806250cd3434495e8d9746bd`  
		Last Modified: Thu, 23 Jan 2020 18:02:52 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a172dbf767ea0f19741367696429fedee78a328523a3297ce4131bf0ba20fa0`  
		Last Modified: Thu, 23 Jan 2020 18:02:56 GMT  
		Size: 13.7 MB (13716677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1deb4fe7d28fbabc3e88bc7e11924e99f47212d82ff0a190bf0fce82b2c1b61`  
		Last Modified: Thu, 23 Jan 2020 18:02:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba751cfcae186a3b77e919f182dd66f8012525efea263a9dd93b27ccc23acec`  
		Last Modified: Thu, 23 Jan 2020 18:02:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f9745a993429207fdd3da320a6917081221d49a762e551896031ebd63f08b4`  
		Last Modified: Thu, 23 Jan 2020 18:02:52 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.1`

```console
$ docker pull consul@sha256:621caed58c4a96754e6afe22b18d3fdb67913de050a87bd02581881674c96174
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.1` - linux; amd64

```console
$ docker pull consul@sha256:aedb271ea421fd2ee887a277561f91aae8d16974fafc83e9ebc661b98c81d3b3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18060530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c84316bdbffdd5d803370f5bb4aee5ca44095cca1945a0497ea1f5ed9cee6b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:59 GMT
ENV CONSUL_VERSION=1.1.1
# Thu, 23 Jan 2020 17:16:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:17:00 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:17:05 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:17:07 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:17:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:17:08 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:17:08 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:17:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:17:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:17:09 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:17:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:17:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc1e00ae4e082537fd3e9c26ce3f3b4f8f2228a8253ce4708d780b1204de609`  
		Last Modified: Thu, 23 Jan 2020 17:20:02 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b6c21e5e36bcf90f10f67bebf2da4ab0231b886781a5eb881a4d6e1cb085ee`  
		Last Modified: Thu, 23 Jan 2020 17:20:15 GMT  
		Size: 15.3 MB (15293128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bfa000875e68bccfd819005555b8933cac08802ca05c3513233a6cb83ed901`  
		Last Modified: Thu, 23 Jan 2020 17:20:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39c82f8ebb31874c3a37c3ca7f52ea3e32927c59376c2627c03052c416137ac`  
		Last Modified: Thu, 23 Jan 2020 17:20:02 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29feee2c223abf0f89639b4626ea25459b42054765d588bd4aca36a9725ff32f`  
		Last Modified: Thu, 23 Jan 2020 17:20:02 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:11fd3230febfb254a16f69866b640e987174f53ee0bf084453f04299845cee26
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17390436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3037c26c8fd768c875d792d7ab8763bade1a17801f3911303392ccc251bdd65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:15:47 GMT
ENV CONSUL_VERSION=1.1.1
# Thu, 23 Jan 2020 17:15:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:15:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:15:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:00 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:03 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:03 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:05 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:06 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efad57ac4529242042432c3beb25813b9239ce0eb32980b726fd6bee919cd97`  
		Last Modified: Thu, 23 Jan 2020 17:20:21 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bbb5bc0c29c10b5736bfd0526aa7f8eba57738287c11a97c92def596067c35`  
		Last Modified: Thu, 23 Jan 2020 17:20:29 GMT  
		Size: 14.8 MB (14839473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328738b02390dd29907c91e6187289227201c3b44e0b24776c82f11cc175abf`  
		Last Modified: Thu, 23 Jan 2020 17:20:21 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef802b35c22d6e8ccd8788e7aa6dd115ff4bbf79e96620b57f34bad79971624b`  
		Last Modified: Thu, 23 Jan 2020 17:20:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a832ef5bba7cb3d8c6cbe4451e8ff08d3d34b6094ff3bdc7083a29af90c2f87`  
		Last Modified: Thu, 23 Jan 2020 17:20:21 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:02eb2dde0d018065a76a70cae855a202c84ac6a3110b68618d48a53ba29a96cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17374078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d935f232d5588eafa4f0684f9df8dd18019458d059d7cb013dac2211e4004a82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:23:04 GMT
ENV CONSUL_VERSION=1.1.1
# Thu, 23 Jan 2020 17:23:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:23:06 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:23:11 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:23:14 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:23:15 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:23:16 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:23:17 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:23:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:23:19 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:23:19 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:23:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:23:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de208071910e8a219ffff4644d9cfe2b6d6c0dfe7f65e1e2f4efeda76e44fe0`  
		Last Modified: Thu, 23 Jan 2020 17:27:29 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025019ed2ed7b39bcc56028d228b5687941f0f9af8ec077d779fc0046d53a5b8`  
		Last Modified: Thu, 23 Jan 2020 17:27:35 GMT  
		Size: 14.7 MB (14677552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ee18ebf1c4e1ec04ee4d405e4bb74eda52a1c7b53bd50bd1285fce31ecb7f0`  
		Last Modified: Thu, 23 Jan 2020 17:27:29 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b0fd5160a24d544362517f237ec81e53f1fe7f662b783da54679338246a5c9`  
		Last Modified: Thu, 23 Jan 2020 17:27:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59490a75b95de035d3d2c2d69fe7d92a3165c0552dcabeaa8e9c765b9385201f`  
		Last Modified: Thu, 23 Jan 2020 17:27:30 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1` - linux; 386

```console
$ docker pull consul@sha256:b4131fd85a6c86d3248a71e5609330fc01a13c17526f0316cc8b2ac94fbfc267
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17959975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9431061faec05289ecb87ac46fe7da6554798549174e72e2377d7ca6b7d2620c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:58:56 GMT
ENV CONSUL_VERSION=1.1.1
# Thu, 23 Jan 2020 17:58:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:58:57 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:59:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:59:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:59:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:59:05 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:59:06 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:59:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:59:06 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:59:06 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:59:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:59:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad526349440d06d2b77bae7e150dd7ddf7874fe8b2532ae8e08193530ad18c`  
		Last Modified: Thu, 23 Jan 2020 18:02:37 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dad09e78a9dce26a88857fb7bcf07cc8347bab877493b3ddf98b7f1e32d4aab`  
		Last Modified: Thu, 23 Jan 2020 18:02:48 GMT  
		Size: 15.2 MB (15188228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e037efe3a33ca80b41d58b1698e3123db25b01d684e8114b45110a17f5588d4`  
		Last Modified: Thu, 23 Jan 2020 18:02:37 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b09f7726e3bb974dd7333c165f085d73209516f71124496ee3da9213470b92`  
		Last Modified: Thu, 23 Jan 2020 18:02:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134c1517c8a63c25a7b7e55df71fc2d057311bee9cf62dcd0f3a27d2253d2833`  
		Last Modified: Thu, 23 Jan 2020 18:02:36 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.1.1`

```console
$ docker pull consul@sha256:621caed58c4a96754e6afe22b18d3fdb67913de050a87bd02581881674c96174
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.1.1` - linux; amd64

```console
$ docker pull consul@sha256:aedb271ea421fd2ee887a277561f91aae8d16974fafc83e9ebc661b98c81d3b3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.1 MB (18060530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c84316bdbffdd5d803370f5bb4aee5ca44095cca1945a0497ea1f5ed9cee6b1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:59 GMT
ENV CONSUL_VERSION=1.1.1
# Thu, 23 Jan 2020 17:16:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:17:00 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:17:05 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:17:07 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:17:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:17:08 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:17:08 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:17:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:17:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:17:09 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:17:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:17:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc1e00ae4e082537fd3e9c26ce3f3b4f8f2228a8253ce4708d780b1204de609`  
		Last Modified: Thu, 23 Jan 2020 17:20:02 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b6c21e5e36bcf90f10f67bebf2da4ab0231b886781a5eb881a4d6e1cb085ee`  
		Last Modified: Thu, 23 Jan 2020 17:20:15 GMT  
		Size: 15.3 MB (15293128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bfa000875e68bccfd819005555b8933cac08802ca05c3513233a6cb83ed901`  
		Last Modified: Thu, 23 Jan 2020 17:20:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39c82f8ebb31874c3a37c3ca7f52ea3e32927c59376c2627c03052c416137ac`  
		Last Modified: Thu, 23 Jan 2020 17:20:02 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29feee2c223abf0f89639b4626ea25459b42054765d588bd4aca36a9725ff32f`  
		Last Modified: Thu, 23 Jan 2020 17:20:02 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:11fd3230febfb254a16f69866b640e987174f53ee0bf084453f04299845cee26
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17390436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3037c26c8fd768c875d792d7ab8763bade1a17801f3911303392ccc251bdd65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:15:47 GMT
ENV CONSUL_VERSION=1.1.1
# Thu, 23 Jan 2020 17:15:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:15:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:15:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:00 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:03 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:03 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:05 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:06 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efad57ac4529242042432c3beb25813b9239ce0eb32980b726fd6bee919cd97`  
		Last Modified: Thu, 23 Jan 2020 17:20:21 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bbb5bc0c29c10b5736bfd0526aa7f8eba57738287c11a97c92def596067c35`  
		Last Modified: Thu, 23 Jan 2020 17:20:29 GMT  
		Size: 14.8 MB (14839473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b328738b02390dd29907c91e6187289227201c3b44e0b24776c82f11cc175abf`  
		Last Modified: Thu, 23 Jan 2020 17:20:21 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef802b35c22d6e8ccd8788e7aa6dd115ff4bbf79e96620b57f34bad79971624b`  
		Last Modified: Thu, 23 Jan 2020 17:20:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a832ef5bba7cb3d8c6cbe4451e8ff08d3d34b6094ff3bdc7083a29af90c2f87`  
		Last Modified: Thu, 23 Jan 2020 17:20:21 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1.1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:02eb2dde0d018065a76a70cae855a202c84ac6a3110b68618d48a53ba29a96cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17374078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d935f232d5588eafa4f0684f9df8dd18019458d059d7cb013dac2211e4004a82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:23:04 GMT
ENV CONSUL_VERSION=1.1.1
# Thu, 23 Jan 2020 17:23:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:23:06 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:23:11 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:23:14 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:23:15 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:23:16 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:23:17 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:23:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:23:19 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:23:19 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:23:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:23:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de208071910e8a219ffff4644d9cfe2b6d6c0dfe7f65e1e2f4efeda76e44fe0`  
		Last Modified: Thu, 23 Jan 2020 17:27:29 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025019ed2ed7b39bcc56028d228b5687941f0f9af8ec077d779fc0046d53a5b8`  
		Last Modified: Thu, 23 Jan 2020 17:27:35 GMT  
		Size: 14.7 MB (14677552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ee18ebf1c4e1ec04ee4d405e4bb74eda52a1c7b53bd50bd1285fce31ecb7f0`  
		Last Modified: Thu, 23 Jan 2020 17:27:29 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b0fd5160a24d544362517f237ec81e53f1fe7f662b783da54679338246a5c9`  
		Last Modified: Thu, 23 Jan 2020 17:27:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59490a75b95de035d3d2c2d69fe7d92a3165c0552dcabeaa8e9c765b9385201f`  
		Last Modified: Thu, 23 Jan 2020 17:27:30 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.1.1` - linux; 386

```console
$ docker pull consul@sha256:b4131fd85a6c86d3248a71e5609330fc01a13c17526f0316cc8b2ac94fbfc267
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.0 MB (17959975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9431061faec05289ecb87ac46fe7da6554798549174e72e2377d7ca6b7d2620c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:58:56 GMT
ENV CONSUL_VERSION=1.1.1
# Thu, 23 Jan 2020 17:58:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:58:57 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:59:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:59:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:59:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:59:05 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:59:06 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:59:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:59:06 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:59:06 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:59:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:59:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ad526349440d06d2b77bae7e150dd7ddf7874fe8b2532ae8e08193530ad18c`  
		Last Modified: Thu, 23 Jan 2020 18:02:37 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dad09e78a9dce26a88857fb7bcf07cc8347bab877493b3ddf98b7f1e32d4aab`  
		Last Modified: Thu, 23 Jan 2020 18:02:48 GMT  
		Size: 15.2 MB (15188228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e037efe3a33ca80b41d58b1698e3123db25b01d684e8114b45110a17f5588d4`  
		Last Modified: Thu, 23 Jan 2020 18:02:37 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b09f7726e3bb974dd7333c165f085d73209516f71124496ee3da9213470b92`  
		Last Modified: Thu, 23 Jan 2020 18:02:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134c1517c8a63c25a7b7e55df71fc2d057311bee9cf62dcd0f3a27d2253d2833`  
		Last Modified: Thu, 23 Jan 2020 18:02:36 GMT  
		Size: 1.7 KB (1676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.2`

```console
$ docker pull consul@sha256:1bbf8bd54bb525d5140dca3b40b59278bc145399150fb981383a4f932ca9a917
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.2` - linux; amd64

```console
$ docker pull consul@sha256:c72e7c8e3423ebbe3313ef8903fd00c3f1f3b6f41ed5578698ad64a1299fea50
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28360024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67f00a3cbd8ae9cb81252ee2890ab2a8779ee614a4d9820e8fb0332b1cd72b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:41 GMT
ENV CONSUL_VERSION=1.2.4
# Thu, 23 Jan 2020 17:16:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:16:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:16:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:51 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:51 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:51 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:52 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:52 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:52 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05236fbe333350c71e205c5a48e5c1498c79fcc4370068a86859fdb4dcc8ba6`  
		Last Modified: Thu, 23 Jan 2020 17:19:50 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25b9e9afae6f3f1764ac7c3dcc7c599ee824ebf4c24ad86fb8b6f926a5d2c36`  
		Last Modified: Thu, 23 Jan 2020 17:19:58 GMT  
		Size: 25.6 MB (25592623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6805bf2501087e0ba3f659513f496a23990d725531ab0be38fae74a3c831fa9`  
		Last Modified: Thu, 23 Jan 2020 17:19:50 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f551ea7fa1939e487e14e28cf0e6ccfa55439ef8c7a52e644e88924f0fcf71`  
		Last Modified: Thu, 23 Jan 2020 17:19:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecee1f7625c248fca92b3d57e5f1f2a39180057b479eb182d0329f7cdc371a`  
		Last Modified: Thu, 23 Jan 2020 17:19:50 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2` - linux; arm variant v6

```console
$ docker pull consul@sha256:5bcdbe8cb32a9083956f0b7c73708b06ea3ecda4c9a82ec3a2a065f1be142827
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27345494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bed1c57a821e8719fc0040f1d5bdce49b0d98a2725f6cef43bb4cc51b5ec4f2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:15:18 GMT
ENV CONSUL_VERSION=1.2.4
# Thu, 23 Jan 2020 17:15:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:15:21 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:15:30 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:15:32 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:15:35 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:15:36 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:15:37 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:15:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:15:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:15:39 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:15:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:15:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777e8f49895857c87e493bc96c7d816cf8d631dfb46090fc63ac54e4a553d225`  
		Last Modified: Thu, 23 Jan 2020 17:19:53 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27960aa4e4ec1be7ee1d54b3ce3be997e5135c28ffa0fdd09738f71404c526a7`  
		Last Modified: Thu, 23 Jan 2020 17:20:14 GMT  
		Size: 24.8 MB (24794531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4348673972808b9b99a46dcf4826a70fbe0ed56a055b7783dc7f116d60018a8a`  
		Last Modified: Thu, 23 Jan 2020 17:19:53 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcd33f8b4f96a4102e6530093ea079919be6cf0e4a16fa0c24ddefdd0b2a925`  
		Last Modified: Thu, 23 Jan 2020 17:19:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15efe0eb58c62036403da9985481fad70e64912971093c7e053a4d8db4919141`  
		Last Modified: Thu, 23 Jan 2020 17:19:53 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:001ecb2e473fecff4a92b05a066f68a15daf84b3c3c1d0c0d07ab6de3b9720c5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27144711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81dbc650e06f84574778ad7203e4618603b88765f3b1c016f0981bc283d3ac77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:22:35 GMT
ENV CONSUL_VERSION=1.2.4
# Thu, 23 Jan 2020 17:22:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:22:38 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:22:46 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:22:48 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:22:51 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:22:53 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:22:55 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:22:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:22:56 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:22:57 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:22:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f5b3b590a3b748748a66708d7f62a3b4fad4f172cbbfd22d6d9283cc7abf8`  
		Last Modified: Thu, 23 Jan 2020 17:27:14 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4691413d5a5f19170da5084a3cb6131835489f7868f17153fd895f9f27acc43a`  
		Last Modified: Thu, 23 Jan 2020 17:27:22 GMT  
		Size: 24.4 MB (24448187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644a1a197a254512b001fe802115f9b0b9e87a389e7205e3ec998dfca101653b`  
		Last Modified: Thu, 23 Jan 2020 17:27:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05aa6ffb25367f0b6e471b03152190e5b08c2c92c5ba63c4463b9f456840939`  
		Last Modified: Thu, 23 Jan 2020 17:27:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b8fc21306eef0dc0bc89ab67ad9de13287b2bc4d3418e563ed13d2ad2edd57`  
		Last Modified: Thu, 23 Jan 2020 17:27:14 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2` - linux; 386

```console
$ docker pull consul@sha256:55ae78ed844e1fe1b10ecf8cad8610d343a8cd6c187b77b536598db71afbc55e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28101526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231a7f0e397326a62df15b2e8fa29af56629f4f59added0f4566fe1258070761`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:58:37 GMT
ENV CONSUL_VERSION=1.2.4
# Thu, 23 Jan 2020 17:58:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:58:39 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:58:46 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:58:47 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:58:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:58:49 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:58:49 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:58:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:58:50 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:58:50 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:58:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:58:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1a81c440a928076734343ae0d0305bcdb6b89c9673880830ff21765ba17fb2`  
		Last Modified: Thu, 23 Jan 2020 18:02:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3bd4b339ff56435e28ae940ad054b7a1aa18cfd0fe7ee4a1597295e91d739d`  
		Last Modified: Thu, 23 Jan 2020 18:02:33 GMT  
		Size: 25.3 MB (25329777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec5dc5c03058dd1d186b213bd1da50fd0ba170da6ce5213ce5b41f35a102940`  
		Last Modified: Thu, 23 Jan 2020 18:02:17 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1af486929c272991fce7e9b5394b3231a8f2722c8a7cb143d14c78eaa2ee27c`  
		Last Modified: Thu, 23 Jan 2020 18:02:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d7211a286501aa32bb50df58d09e6844fca34e5088cdbc09a0de722972ffe2`  
		Last Modified: Thu, 23 Jan 2020 18:02:17 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.2.4`

```console
$ docker pull consul@sha256:1bbf8bd54bb525d5140dca3b40b59278bc145399150fb981383a4f932ca9a917
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.2.4` - linux; amd64

```console
$ docker pull consul@sha256:c72e7c8e3423ebbe3313ef8903fd00c3f1f3b6f41ed5578698ad64a1299fea50
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.4 MB (28360024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b67f00a3cbd8ae9cb81252ee2890ab2a8779ee614a4d9820e8fb0332b1cd72b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:41 GMT
ENV CONSUL_VERSION=1.2.4
# Thu, 23 Jan 2020 17:16:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:16:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:16:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:51 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:51 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:51 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:52 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:52 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:52 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05236fbe333350c71e205c5a48e5c1498c79fcc4370068a86859fdb4dcc8ba6`  
		Last Modified: Thu, 23 Jan 2020 17:19:50 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25b9e9afae6f3f1764ac7c3dcc7c599ee824ebf4c24ad86fb8b6f926a5d2c36`  
		Last Modified: Thu, 23 Jan 2020 17:19:58 GMT  
		Size: 25.6 MB (25592623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6805bf2501087e0ba3f659513f496a23990d725531ab0be38fae74a3c831fa9`  
		Last Modified: Thu, 23 Jan 2020 17:19:50 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f551ea7fa1939e487e14e28cf0e6ccfa55439ef8c7a52e644e88924f0fcf71`  
		Last Modified: Thu, 23 Jan 2020 17:19:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecee1f7625c248fca92b3d57e5f1f2a39180057b479eb182d0329f7cdc371a`  
		Last Modified: Thu, 23 Jan 2020 17:19:50 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:5bcdbe8cb32a9083956f0b7c73708b06ea3ecda4c9a82ec3a2a065f1be142827
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.3 MB (27345494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bed1c57a821e8719fc0040f1d5bdce49b0d98a2725f6cef43bb4cc51b5ec4f2c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:15:18 GMT
ENV CONSUL_VERSION=1.2.4
# Thu, 23 Jan 2020 17:15:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:15:21 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:15:30 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:15:32 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:15:35 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:15:36 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:15:37 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:15:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:15:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:15:39 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:15:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:15:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777e8f49895857c87e493bc96c7d816cf8d631dfb46090fc63ac54e4a553d225`  
		Last Modified: Thu, 23 Jan 2020 17:19:53 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27960aa4e4ec1be7ee1d54b3ce3be997e5135c28ffa0fdd09738f71404c526a7`  
		Last Modified: Thu, 23 Jan 2020 17:20:14 GMT  
		Size: 24.8 MB (24794531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4348673972808b9b99a46dcf4826a70fbe0ed56a055b7783dc7f116d60018a8a`  
		Last Modified: Thu, 23 Jan 2020 17:19:53 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bcd33f8b4f96a4102e6530093ea079919be6cf0e4a16fa0c24ddefdd0b2a925`  
		Last Modified: Thu, 23 Jan 2020 17:19:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15efe0eb58c62036403da9985481fad70e64912971093c7e053a4d8db4919141`  
		Last Modified: Thu, 23 Jan 2020 17:19:53 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:001ecb2e473fecff4a92b05a066f68a15daf84b3c3c1d0c0d07ab6de3b9720c5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.1 MB (27144711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81dbc650e06f84574778ad7203e4618603b88765f3b1c016f0981bc283d3ac77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:22:35 GMT
ENV CONSUL_VERSION=1.2.4
# Thu, 23 Jan 2020 17:22:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:22:38 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:22:46 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:22:48 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:22:51 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:22:53 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:22:55 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:22:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:22:56 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:22:57 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:22:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:22:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598f5b3b590a3b748748a66708d7f62a3b4fad4f172cbbfd22d6d9283cc7abf8`  
		Last Modified: Thu, 23 Jan 2020 17:27:14 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4691413d5a5f19170da5084a3cb6131835489f7868f17153fd895f9f27acc43a`  
		Last Modified: Thu, 23 Jan 2020 17:27:22 GMT  
		Size: 24.4 MB (24448187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644a1a197a254512b001fe802115f9b0b9e87a389e7205e3ec998dfca101653b`  
		Last Modified: Thu, 23 Jan 2020 17:27:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05aa6ffb25367f0b6e471b03152190e5b08c2c92c5ba63c4463b9f456840939`  
		Last Modified: Thu, 23 Jan 2020 17:27:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b8fc21306eef0dc0bc89ab67ad9de13287b2bc4d3418e563ed13d2ad2edd57`  
		Last Modified: Thu, 23 Jan 2020 17:27:14 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.2.4` - linux; 386

```console
$ docker pull consul@sha256:55ae78ed844e1fe1b10ecf8cad8610d343a8cd6c187b77b536598db71afbc55e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.1 MB (28101526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231a7f0e397326a62df15b2e8fa29af56629f4f59added0f4566fe1258070761`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:58:37 GMT
ENV CONSUL_VERSION=1.2.4
# Thu, 23 Jan 2020 17:58:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:58:39 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:58:46 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:58:47 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:58:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:58:49 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:58:49 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:58:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:58:50 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:58:50 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:58:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:58:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f1a81c440a928076734343ae0d0305bcdb6b89c9673880830ff21765ba17fb2`  
		Last Modified: Thu, 23 Jan 2020 18:02:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3bd4b339ff56435e28ae940ad054b7a1aa18cfd0fe7ee4a1597295e91d739d`  
		Last Modified: Thu, 23 Jan 2020 18:02:33 GMT  
		Size: 25.3 MB (25329777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec5dc5c03058dd1d186b213bd1da50fd0ba170da6ce5213ce5b41f35a102940`  
		Last Modified: Thu, 23 Jan 2020 18:02:17 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1af486929c272991fce7e9b5394b3231a8f2722c8a7cb143d14c78eaa2ee27c`  
		Last Modified: Thu, 23 Jan 2020 18:02:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d7211a286501aa32bb50df58d09e6844fca34e5088cdbc09a0de722972ffe2`  
		Last Modified: Thu, 23 Jan 2020 18:02:17 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.3`

```console
$ docker pull consul@sha256:06a32635c96c494f6fb1ffe19bf8282c1d7756c43797838a6303d8fbec1a123a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.3` - linux; amd64

```console
$ docker pull consul@sha256:1bedb45a13dccadfe00d032b7432f5069e76fd6726e94946879f9531c5f5b1c8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38563269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a1b14382a5b435edfcb5a194a60406bd861fabb75effcfe278f0f7ccd58965`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:23 GMT
ENV CONSUL_VERSION=1.3.1
# Thu, 23 Jan 2020 17:16:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:16:25 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:16:31 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:32 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:33 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:34 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:34 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:34 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:35 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f35c11f4344ff830f784baa710a9b2c18b608b3e72ef47fba038762e7307b9`  
		Last Modified: Thu, 23 Jan 2020 17:19:37 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a8452a9f508b85fc7f8488e1bd2a5f1532616c4cfbe2e0144698bd6b50ea4a`  
		Last Modified: Thu, 23 Jan 2020 17:19:46 GMT  
		Size: 35.8 MB (35795870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a940220db4bbb696ce4e3c8c9c0aaa2d8a3143974fc01516b8fc0c739f85b5e`  
		Last Modified: Thu, 23 Jan 2020 17:19:37 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadae00f277c0b29d5edbc5976825a70e9597afe0b6711ec2af29a7ff13dcf88`  
		Last Modified: Thu, 23 Jan 2020 17:19:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5793fa9cc319a37def4538c53d0961fb328e2272d8176a9f5afe8c94672ed`  
		Last Modified: Thu, 23 Jan 2020 17:19:37 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3` - linux; arm variant v6

```console
$ docker pull consul@sha256:5ef1319bd7a263270f59c26effda15b49fcb966f06bda10f5a27d376bea7f60b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36396340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:594f4f4e206acc4fc744be3f65faad59ad6a1e1b7ef759b651c3420d7c9546ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:14:49 GMT
ENV CONSUL_VERSION=1.3.1
# Thu, 23 Jan 2020 17:14:49 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:14:51 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:15:00 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:15:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:15:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:15:06 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:15:07 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:15:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:15:08 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:15:09 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:15:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a02987bf44bbc2f4fb69b5226821e70a597fed6797d36077dfa7dbe0b50eaca`  
		Last Modified: Thu, 23 Jan 2020 17:19:16 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28909407896d89d87b7d3fb6a4b1d9fb536192af0a4463fb0b079b34c09932a`  
		Last Modified: Thu, 23 Jan 2020 17:19:46 GMT  
		Size: 33.8 MB (33845376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86640b27c00eda372e090c2b3958859b4b4bdef466ef3609bae0a83c894602`  
		Last Modified: Thu, 23 Jan 2020 17:19:16 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb71324ee15e936e48a5dd52fad393d014b125e731a446cb58234377476396e`  
		Last Modified: Thu, 23 Jan 2020 17:19:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004e0734cbfc1821974cd2c8f8eaa09a980947f398fa7c04f94dd06716442ee7`  
		Last Modified: Thu, 23 Jan 2020 17:19:16 GMT  
		Size: 1.7 KB (1680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2418b650cb5ea9bc4af38e5e0b249567bcee490ff3b46312100e3b51be757be3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36217075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb81762c89f3e79d1b604d9b61afed84e8b1ff1f6e81ee99adc217167dd0635`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:22:01 GMT
ENV CONSUL_VERSION=1.3.1
# Thu, 23 Jan 2020 17:22:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:22:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:22:13 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:22:17 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:22:19 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:22:20 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:22:21 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:22:22 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:22:22 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:22:23 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:22:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:22:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98012cd647e1d27e020c00fae0d589a965b7ecc830bda18c66aceb6ac72fae7`  
		Last Modified: Thu, 23 Jan 2020 17:27:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023f9aef35688822464cb5df3ee78a055a71ef63161969bd0f04bd25abdd79bc`  
		Last Modified: Thu, 23 Jan 2020 17:27:06 GMT  
		Size: 33.5 MB (33520552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599be1f23dcb5d8099d3eb5e0e46e58bbaa2c66143a7c9c76c7be5d5c05fc344`  
		Last Modified: Thu, 23 Jan 2020 17:27:01 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2c8ee332607e9b33817745e2162932c2b13cf5ccdb02cc8aa6ab1c14ef4f40`  
		Last Modified: Thu, 23 Jan 2020 17:27:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4b8b1de504b0c2fa582f0ad0f528fbfe2695451a47c5ca49febfd321c31d9f`  
		Last Modified: Thu, 23 Jan 2020 17:27:00 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3` - linux; 386

```console
$ docker pull consul@sha256:ece6f70acf01fbf44448083c8eb1fffe36ccc889431a65d99c95fa84275b0795
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37753218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc81f3a1fa153c5812e3e18e6674d20dbb7882920c43dee14456e452c6df6a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:58:19 GMT
ENV CONSUL_VERSION=1.3.1
# Thu, 23 Jan 2020 17:58:20 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:58:21 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:58:29 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:58:30 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:58:31 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:58:31 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:58:31 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:58:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:58:32 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:58:32 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:58:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6429398394daf9c5675c1d2d4e0f6f2e97715b33e3e439ff29348043af8f904b`  
		Last Modified: Thu, 23 Jan 2020 18:02:00 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ce5a9615357a61c09307434244d0fe228a029646aceb378b436864576e47a9`  
		Last Modified: Thu, 23 Jan 2020 18:02:12 GMT  
		Size: 35.0 MB (34981468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34637512a02add9c32eea89b47a2660309f28caab4d0ab1c33863b954bfe7eb0`  
		Last Modified: Thu, 23 Jan 2020 18:02:00 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffb6a8eb4c30dcb6d68c00ebe83ece845dd8798739c95bc70a5ec9a9b535c39`  
		Last Modified: Thu, 23 Jan 2020 18:02:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c4ec2dbdd9e56da11f75bbc533e0a59d89eae92e24986cf5e6f7588711e4ab`  
		Last Modified: Thu, 23 Jan 2020 18:02:01 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.3.1`

```console
$ docker pull consul@sha256:06a32635c96c494f6fb1ffe19bf8282c1d7756c43797838a6303d8fbec1a123a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.3.1` - linux; amd64

```console
$ docker pull consul@sha256:1bedb45a13dccadfe00d032b7432f5069e76fd6726e94946879f9531c5f5b1c8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38563269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34a1b14382a5b435edfcb5a194a60406bd861fabb75effcfe278f0f7ccd58965`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:23 GMT
ENV CONSUL_VERSION=1.3.1
# Thu, 23 Jan 2020 17:16:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:16:25 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:16:31 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:32 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:33 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:34 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:34 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:34 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:35 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f35c11f4344ff830f784baa710a9b2c18b608b3e72ef47fba038762e7307b9`  
		Last Modified: Thu, 23 Jan 2020 17:19:37 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a8452a9f508b85fc7f8488e1bd2a5f1532616c4cfbe2e0144698bd6b50ea4a`  
		Last Modified: Thu, 23 Jan 2020 17:19:46 GMT  
		Size: 35.8 MB (35795870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a940220db4bbb696ce4e3c8c9c0aaa2d8a3143974fc01516b8fc0c739f85b5e`  
		Last Modified: Thu, 23 Jan 2020 17:19:37 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadae00f277c0b29d5edbc5976825a70e9597afe0b6711ec2af29a7ff13dcf88`  
		Last Modified: Thu, 23 Jan 2020 17:19:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b5793fa9cc319a37def4538c53d0961fb328e2272d8176a9f5afe8c94672ed`  
		Last Modified: Thu, 23 Jan 2020 17:19:37 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:5ef1319bd7a263270f59c26effda15b49fcb966f06bda10f5a27d376bea7f60b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36396340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:594f4f4e206acc4fc744be3f65faad59ad6a1e1b7ef759b651c3420d7c9546ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:14:49 GMT
ENV CONSUL_VERSION=1.3.1
# Thu, 23 Jan 2020 17:14:49 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:14:51 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:15:00 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:15:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:15:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:15:06 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:15:07 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:15:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:15:08 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:15:09 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:15:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a02987bf44bbc2f4fb69b5226821e70a597fed6797d36077dfa7dbe0b50eaca`  
		Last Modified: Thu, 23 Jan 2020 17:19:16 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d28909407896d89d87b7d3fb6a4b1d9fb536192af0a4463fb0b079b34c09932a`  
		Last Modified: Thu, 23 Jan 2020 17:19:46 GMT  
		Size: 33.8 MB (33845376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86640b27c00eda372e090c2b3958859b4b4bdef466ef3609bae0a83c894602`  
		Last Modified: Thu, 23 Jan 2020 17:19:16 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb71324ee15e936e48a5dd52fad393d014b125e731a446cb58234377476396e`  
		Last Modified: Thu, 23 Jan 2020 17:19:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004e0734cbfc1821974cd2c8f8eaa09a980947f398fa7c04f94dd06716442ee7`  
		Last Modified: Thu, 23 Jan 2020 17:19:16 GMT  
		Size: 1.7 KB (1680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3.1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2418b650cb5ea9bc4af38e5e0b249567bcee490ff3b46312100e3b51be757be3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36217075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb81762c89f3e79d1b604d9b61afed84e8b1ff1f6e81ee99adc217167dd0635`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:22:01 GMT
ENV CONSUL_VERSION=1.3.1
# Thu, 23 Jan 2020 17:22:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:22:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:22:13 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:22:17 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:22:19 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:22:20 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:22:21 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:22:22 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:22:22 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:22:23 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:22:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:22:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98012cd647e1d27e020c00fae0d589a965b7ecc830bda18c66aceb6ac72fae7`  
		Last Modified: Thu, 23 Jan 2020 17:27:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023f9aef35688822464cb5df3ee78a055a71ef63161969bd0f04bd25abdd79bc`  
		Last Modified: Thu, 23 Jan 2020 17:27:06 GMT  
		Size: 33.5 MB (33520552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599be1f23dcb5d8099d3eb5e0e46e58bbaa2c66143a7c9c76c7be5d5c05fc344`  
		Last Modified: Thu, 23 Jan 2020 17:27:01 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2c8ee332607e9b33817745e2162932c2b13cf5ccdb02cc8aa6ab1c14ef4f40`  
		Last Modified: Thu, 23 Jan 2020 17:27:01 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d4b8b1de504b0c2fa582f0ad0f528fbfe2695451a47c5ca49febfd321c31d9f`  
		Last Modified: Thu, 23 Jan 2020 17:27:00 GMT  
		Size: 1.7 KB (1675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.3.1` - linux; 386

```console
$ docker pull consul@sha256:ece6f70acf01fbf44448083c8eb1fffe36ccc889431a65d99c95fa84275b0795
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37753218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcc81f3a1fa153c5812e3e18e6674d20dbb7882920c43dee14456e452c6df6a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:58:19 GMT
ENV CONSUL_VERSION=1.3.1
# Thu, 23 Jan 2020 17:58:20 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:58:21 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:58:29 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:58:30 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:58:31 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:58:31 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:58:31 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:58:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:58:32 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:58:32 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:58:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:58:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6429398394daf9c5675c1d2d4e0f6f2e97715b33e3e439ff29348043af8f904b`  
		Last Modified: Thu, 23 Jan 2020 18:02:00 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ce5a9615357a61c09307434244d0fe228a029646aceb378b436864576e47a9`  
		Last Modified: Thu, 23 Jan 2020 18:02:12 GMT  
		Size: 35.0 MB (34981468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34637512a02add9c32eea89b47a2660309f28caab4d0ab1c33863b954bfe7eb0`  
		Last Modified: Thu, 23 Jan 2020 18:02:00 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffb6a8eb4c30dcb6d68c00ebe83ece845dd8798739c95bc70a5ec9a9b535c39`  
		Last Modified: Thu, 23 Jan 2020 18:02:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c4ec2dbdd9e56da11f75bbc533e0a59d89eae92e24986cf5e6f7588711e4ab`  
		Last Modified: Thu, 23 Jan 2020 18:02:01 GMT  
		Size: 1.7 KB (1679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.4`

```console
$ docker pull consul@sha256:739cdd4593f17528f3e32e3a23ec0669d3971804f6108566ac5a6f8ee2f3cbd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.4` - linux; amd64

```console
$ docker pull consul@sha256:068a9a19ecd914c3364c5633917b72a898b461923ff56dd7500aa926f421c4b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39199490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad32393b859a2a3bdd3411af9926171c1f5c96558f796a03dce84b164c314613`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:05 GMT
ENV CONSUL_VERSION=1.4.5
# Thu, 23 Jan 2020 17:16:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:16:07 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:16:13 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:14 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:15 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:16 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:16 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:16 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:16 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:17 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:17 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7651bd62600c8b706e5120d2fe48d72e94904be0cc8d1a82d4d3f5de592b37`  
		Last Modified: Thu, 23 Jan 2020 17:19:00 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae6d22bb36b77217cd3fb3e007589cbfaf4076d1a1ad009150594dd270334d9`  
		Last Modified: Thu, 23 Jan 2020 17:19:32 GMT  
		Size: 36.4 MB (36432087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9697a7a1e3d9f33fe5891a4a3afab1ca81826b415f1575967c96fb7426b8d45e`  
		Last Modified: Thu, 23 Jan 2020 17:19:00 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5d89b529d3cc118de1dbf8c3b2554bc84510eb7afa942267aa3ffc94f94923`  
		Last Modified: Thu, 23 Jan 2020 17:19:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71722bc46238839f701198cdccdf1bd8330aa287d814044f6721c15038d9baeb`  
		Last Modified: Thu, 23 Jan 2020 17:19:00 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:ab75f66a4ad33a10e28ce3e51e872c4fe7b302e37c0fddc5c618ae6da514e6eb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36975580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f63b1297f708521ba3e05b70089d259eff0ee5318e8bbefa465a490ae16027`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:14:16 GMT
ENV CONSUL_VERSION=1.4.5
# Thu, 23 Jan 2020 17:14:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:14:19 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:14:30 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:14:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:14:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:14:37 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:14:38 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:14:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:14:39 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:14:40 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:14:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:14:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d61f6ab4ed74a2b32488b7ffce1af37fcea5abb15e679cc9675c0398761579`  
		Last Modified: Thu, 23 Jan 2020 17:18:40 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0563b308a3030c66030ea1d98b04a7caf1442855e3c3f21fe8f23f55902fbb57`  
		Last Modified: Thu, 23 Jan 2020 17:19:09 GMT  
		Size: 34.4 MB (34424623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad9d4fb0eb14f6b5144898dc40b616477b5aecfd8b589817f2d51f64dfc1a84`  
		Last Modified: Thu, 23 Jan 2020 17:18:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2ee9f3cfb50c34287e9649f9383bdbf1f7b30150d463e3d679fdaaa5bad269`  
		Last Modified: Thu, 23 Jan 2020 17:18:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11944222aa768729a26901bac254b94d0ec9abf89575f732ad5f5a906b49beb`  
		Last Modified: Thu, 23 Jan 2020 17:18:39 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:9d0b270062ca7bfc7e3cce9fe333356a8d3c748f272eb600c3ac4d0976838d67
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36791030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2a735556e7041d4de6c339d8f68ebbbd3ec4154495c5a96212c0d99b02ad11c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:21:29 GMT
ENV CONSUL_VERSION=1.4.5
# Thu, 23 Jan 2020 17:21:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:21:33 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:21:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:21:43 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:21:47 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:21:48 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:21:49 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:21:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:21:52 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:21:53 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:21:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152e314dadf8047c6af841428cd8f0e500b91d95d966b8e359644f2b59e20dbf`  
		Last Modified: Thu, 23 Jan 2020 17:26:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006c1a2a8bff1a062065f40aabd554fd4b8c518b856b9545969d48cd15c3a6c2`  
		Last Modified: Thu, 23 Jan 2020 17:26:50 GMT  
		Size: 34.1 MB (34094503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0eba5dacc287ff2bb7a9e2e93aaeb71bd297a017e6857df3e238c1e4edd348`  
		Last Modified: Thu, 23 Jan 2020 17:26:18 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1336cd3d92ebf35a59362b380985997672ab714945382c8bbf5638881135ed0a`  
		Last Modified: Thu, 23 Jan 2020 17:26:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6439e5bb7c9d7f3da8a7dd4a24467cf249e7bffef27f589c62012510b3d48cd0`  
		Last Modified: Thu, 23 Jan 2020 17:26:17 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4` - linux; 386

```console
$ docker pull consul@sha256:136a172563c1a39cf215aed205474181599a60cf830ce2aa7f79f9a0cec121de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38367962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:986008d7de1372a3b1e6fa343b29829d9fe2f9419ba42c69847459fe733d53f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:58:01 GMT
ENV CONSUL_VERSION=1.4.5
# Thu, 23 Jan 2020 17:58:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:58:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:58:10 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:58:11 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:58:12 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:58:13 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:58:13 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:58:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:58:14 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:58:14 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:58:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:58:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf4fb8aaef477a64085202e76cfa3a4b336bda58dd40505fe06a6f80c3dda57`  
		Last Modified: Thu, 23 Jan 2020 18:01:18 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b0d12ab73e75ad122a874d563c7703c128d1861023b88b6e86e08203a64cb7`  
		Last Modified: Thu, 23 Jan 2020 18:01:55 GMT  
		Size: 35.6 MB (35596213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5d2601c1d67b51aaaf916a12b754c5d0fa6d13f4626da4f66393dc52db6b19`  
		Last Modified: Thu, 23 Jan 2020 18:01:18 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ee2a7bd7fa8c4cb9174ff9a83ae335edea4bd8f20816ad40bf66ad42e9cbc4`  
		Last Modified: Thu, 23 Jan 2020 18:01:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c5102099f6c8e71eae7acfff693c1aff4047511f823502af13e5e959eca7ce`  
		Last Modified: Thu, 23 Jan 2020 18:01:18 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.4.5`

```console
$ docker pull consul@sha256:739cdd4593f17528f3e32e3a23ec0669d3971804f6108566ac5a6f8ee2f3cbd4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.4.5` - linux; amd64

```console
$ docker pull consul@sha256:068a9a19ecd914c3364c5633917b72a898b461923ff56dd7500aa926f421c4b8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39199490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad32393b859a2a3bdd3411af9926171c1f5c96558f796a03dce84b164c314613`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:16:05 GMT
ENV CONSUL_VERSION=1.4.5
# Thu, 23 Jan 2020 17:16:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:16:07 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:16:13 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:16:14 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:16:15 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:16:16 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:16:16 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:16:16 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:16:16 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:17 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:17 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7651bd62600c8b706e5120d2fe48d72e94904be0cc8d1a82d4d3f5de592b37`  
		Last Modified: Thu, 23 Jan 2020 17:19:00 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae6d22bb36b77217cd3fb3e007589cbfaf4076d1a1ad009150594dd270334d9`  
		Last Modified: Thu, 23 Jan 2020 17:19:32 GMT  
		Size: 36.4 MB (36432087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9697a7a1e3d9f33fe5891a4a3afab1ca81826b415f1575967c96fb7426b8d45e`  
		Last Modified: Thu, 23 Jan 2020 17:19:00 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5d89b529d3cc118de1dbf8c3b2554bc84510eb7afa942267aa3ffc94f94923`  
		Last Modified: Thu, 23 Jan 2020 17:19:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71722bc46238839f701198cdccdf1bd8330aa287d814044f6721c15038d9baeb`  
		Last Modified: Thu, 23 Jan 2020 17:19:00 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4.5` - linux; arm variant v6

```console
$ docker pull consul@sha256:ab75f66a4ad33a10e28ce3e51e872c4fe7b302e37c0fddc5c618ae6da514e6eb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.0 MB (36975580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95f63b1297f708521ba3e05b70089d259eff0ee5318e8bbefa465a490ae16027`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:14:16 GMT
ENV CONSUL_VERSION=1.4.5
# Thu, 23 Jan 2020 17:14:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:14:19 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:14:30 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:14:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:14:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:14:37 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:14:38 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:14:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:14:39 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:14:40 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:14:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:14:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d61f6ab4ed74a2b32488b7ffce1af37fcea5abb15e679cc9675c0398761579`  
		Last Modified: Thu, 23 Jan 2020 17:18:40 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0563b308a3030c66030ea1d98b04a7caf1442855e3c3f21fe8f23f55902fbb57`  
		Last Modified: Thu, 23 Jan 2020 17:19:09 GMT  
		Size: 34.4 MB (34424623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad9d4fb0eb14f6b5144898dc40b616477b5aecfd8b589817f2d51f64dfc1a84`  
		Last Modified: Thu, 23 Jan 2020 17:18:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2ee9f3cfb50c34287e9649f9383bdbf1f7b30150d463e3d679fdaaa5bad269`  
		Last Modified: Thu, 23 Jan 2020 17:18:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11944222aa768729a26901bac254b94d0ec9abf89575f732ad5f5a906b49beb`  
		Last Modified: Thu, 23 Jan 2020 17:18:39 GMT  
		Size: 1.7 KB (1674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4.5` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:9d0b270062ca7bfc7e3cce9fe333356a8d3c748f272eb600c3ac4d0976838d67
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36791030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2a735556e7041d4de6c339d8f68ebbbd3ec4154495c5a96212c0d99b02ad11c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:21:29 GMT
ENV CONSUL_VERSION=1.4.5
# Thu, 23 Jan 2020 17:21:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:21:33 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:21:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:21:43 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:21:47 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:21:48 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:21:49 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:21:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:21:52 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:21:53 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:21:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:21:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:152e314dadf8047c6af841428cd8f0e500b91d95d966b8e359644f2b59e20dbf`  
		Last Modified: Thu, 23 Jan 2020 17:26:18 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006c1a2a8bff1a062065f40aabd554fd4b8c518b856b9545969d48cd15c3a6c2`  
		Last Modified: Thu, 23 Jan 2020 17:26:50 GMT  
		Size: 34.1 MB (34094503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0eba5dacc287ff2bb7a9e2e93aaeb71bd297a017e6857df3e238c1e4edd348`  
		Last Modified: Thu, 23 Jan 2020 17:26:18 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1336cd3d92ebf35a59362b380985997672ab714945382c8bbf5638881135ed0a`  
		Last Modified: Thu, 23 Jan 2020 17:26:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6439e5bb7c9d7f3da8a7dd4a24467cf249e7bffef27f589c62012510b3d48cd0`  
		Last Modified: Thu, 23 Jan 2020 17:26:17 GMT  
		Size: 1.7 KB (1677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.4.5` - linux; 386

```console
$ docker pull consul@sha256:136a172563c1a39cf215aed205474181599a60cf830ce2aa7f79f9a0cec121de
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38367962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:986008d7de1372a3b1e6fa343b29829d9fe2f9419ba42c69847459fe733d53f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:58:01 GMT
ENV CONSUL_VERSION=1.4.5
# Thu, 23 Jan 2020 17:58:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:58:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:58:10 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:58:11 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:58:12 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:58:13 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:58:13 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:58:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:58:14 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:58:14 GMT
COPY file:2fc9ee792fd5d6e21568c1fcc92d825866250fafd9f3c82331ad98c840b3dd45 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:58:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:58:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bf4fb8aaef477a64085202e76cfa3a4b336bda58dd40505fe06a6f80c3dda57`  
		Last Modified: Thu, 23 Jan 2020 18:01:18 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b0d12ab73e75ad122a874d563c7703c128d1861023b88b6e86e08203a64cb7`  
		Last Modified: Thu, 23 Jan 2020 18:01:55 GMT  
		Size: 35.6 MB (35596213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5d2601c1d67b51aaaf916a12b754c5d0fa6d13f4626da4f66393dc52db6b19`  
		Last Modified: Thu, 23 Jan 2020 18:01:18 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ee2a7bd7fa8c4cb9174ff9a83ae335edea4bd8f20816ad40bf66ad42e9cbc4`  
		Last Modified: Thu, 23 Jan 2020 18:01:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c5102099f6c8e71eae7acfff693c1aff4047511f823502af13e5e959eca7ce`  
		Last Modified: Thu, 23 Jan 2020 18:01:18 GMT  
		Size: 1.7 KB (1678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.5`

```console
$ docker pull consul@sha256:6d69c850a686ff66704d18d17afa961fa637f199359c7c2b315dd505a6f83c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.5` - linux; amd64

```console
$ docker pull consul@sha256:9417ce87d497f80f8282d3b74f74c511f41f903b7178d4b3a894dd15e265fe03
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44182203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ce9a832eeab346273f7d1afffc1b80f770c2cf945c42ec159a183fc7ef989b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:15:47 GMT
ENV CONSUL_VERSION=1.5.3
# Thu, 23 Jan 2020 17:15:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:15:49 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:15:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:15:57 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:15:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:15:59 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:15:59 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:15:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:15:59 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:00 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4fdbcc757f800c98634ea57a90e25a5d71c8085047e7ef27a211baf791fbdf`  
		Last Modified: Thu, 23 Jan 2020 17:18:28 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c44a9b8d9f471fc81fea2fc3f754811b086921ce0e6ddc722666eeee59f4eab`  
		Last Modified: Thu, 23 Jan 2020 17:18:55 GMT  
		Size: 41.4 MB (41414773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b242415903bd0e91c2cf4db11a46a35e8ce72ce17cfb5bbc04c8ce1b4b37352`  
		Last Modified: Thu, 23 Jan 2020 17:18:29 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c602c8120e311bf687ab5541322da039164743f236c5d4dc8043b482e1662d`  
		Last Modified: Thu, 23 Jan 2020 17:18:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085df52b698732618e7ef9a5ab9ddb19f16a7225fb7e3b18757b7356529e85e8`  
		Last Modified: Thu, 23 Jan 2020 17:18:28 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5` - linux; arm variant v6

```console
$ docker pull consul@sha256:38b52a245cbb80b790c1a8029e767bc434161ab386e27c2d7f82086d7cdadc31
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41568465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2bdf49bc46e402782cbe73b1bb62e703924eba6c6c7fac502cd64529ac3fa0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:13:41 GMT
ENV CONSUL_VERSION=1.5.3
# Thu, 23 Jan 2020 17:13:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:13:44 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:13:54 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:13:59 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:14:01 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:14:02 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:14:03 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:14:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:14:05 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:14:05 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:14:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:14:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1269d2d3c5158e948002340c38c38b6d89059db8677d1bbe82f948e02f3f0e2f`  
		Last Modified: Thu, 23 Jan 2020 17:18:10 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a735959ed46320f4a53f6d633965338fdc7da8bd8c64d0012f54d836ec8fa4e`  
		Last Modified: Thu, 23 Jan 2020 17:18:32 GMT  
		Size: 39.0 MB (39017477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2bd33cde350fba4407d450904b97cb4bcb0356d424554678fe111717d75ab7`  
		Last Modified: Thu, 23 Jan 2020 17:18:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df83aad6548933382b2d463d9ad4fcb04bcfa0bb9ee98987970f4d0f18f001c4`  
		Last Modified: Thu, 23 Jan 2020 17:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44789f2d596b74a4fd589b2f8253b9ce35ff7b674008bfe12ecc78c59fb8afcb`  
		Last Modified: Thu, 23 Jan 2020 17:18:09 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b93c8d7effcca6871ef3dc097b014579924e0e9e53562e153104c61467e2794f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41736776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d71d8a623b84732d5eb46672cbd1526aa74216b8d824250ef3bebf908db4f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:20:53 GMT
ENV CONSUL_VERSION=1.5.3
# Thu, 23 Jan 2020 17:20:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:20:58 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:21:06 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:21:09 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:21:12 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:21:13 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:21:14 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:21:15 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:21:15 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:21:16 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:21:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66847b9d670332a71d6ede4a344d51162e0bdc6abd08a754f4de9c778ccfa1e4`  
		Last Modified: Thu, 23 Jan 2020 17:25:59 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add30ea62b96d1847e5af034c9942292447570d2feec35e349a29f3735569813`  
		Last Modified: Thu, 23 Jan 2020 17:26:11 GMT  
		Size: 39.0 MB (39040224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be64c310d7e9e83c8eadea0c99bce2a7949b115ceb55cc1470be31aaa8f7d21`  
		Last Modified: Thu, 23 Jan 2020 17:25:59 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5a2cf4964adaae1e25835708056bd14251cab62851cffa4452be09bd8c04a8`  
		Last Modified: Thu, 23 Jan 2020 17:25:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f808e5522e7eb3f5020ce3a4b64f87a4511c14ef14229c479ac2796d10ff6d52`  
		Last Modified: Thu, 23 Jan 2020 17:25:59 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5` - linux; 386

```console
$ docker pull consul@sha256:3daff066c6231a9e9a0db506e8900e21e3f89193224838ab4be57a60f3570c14
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59dfe8338725130aa16669baef8a2dd21a4aebc5920b38e385f39a2a1c1ce5f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:57:43 GMT
ENV CONSUL_VERSION=1.5.3
# Thu, 23 Jan 2020 17:57:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:57:44 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:57:52 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:57:53 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:57:54 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:57:55 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:57:55 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:57:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:57:56 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:57:56 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:57:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:57:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5913bfdca346aa9c11eeafbea739f57e9b501ec0be2257fe0c997407c42f173d`  
		Last Modified: Thu, 23 Jan 2020 18:00:59 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa88ea0f6d80e829b1a82dc650fc5741398eff79c7fc2dcd3b44f9fa1c3a6cd1`  
		Last Modified: Thu, 23 Jan 2020 18:01:13 GMT  
		Size: 40.3 MB (40322432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a9f17c58fd993aa84360a71b3371b4dfe488a53062fbd6f6e83805ea1935f4`  
		Last Modified: Thu, 23 Jan 2020 18:00:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3799343516d02a56471eea7f8e2ae52325ae738036ab58264dc344500870cdd`  
		Last Modified: Thu, 23 Jan 2020 18:00:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e7be14b5eab676cf5ef281cfcce68aaf208e9fc1d54c8c281f832f563781b`  
		Last Modified: Thu, 23 Jan 2020 18:00:59 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.5.3`

```console
$ docker pull consul@sha256:6d69c850a686ff66704d18d17afa961fa637f199359c7c2b315dd505a6f83c1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.5.3` - linux; amd64

```console
$ docker pull consul@sha256:9417ce87d497f80f8282d3b74f74c511f41f903b7178d4b3a894dd15e265fe03
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44182203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5ce9a832eeab346273f7d1afffc1b80f770c2cf945c42ec159a183fc7ef989b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:15:47 GMT
ENV CONSUL_VERSION=1.5.3
# Thu, 23 Jan 2020 17:15:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:15:49 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:15:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:15:57 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:15:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:15:59 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:15:59 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:15:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:15:59 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:16:00 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:16:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:16:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4fdbcc757f800c98634ea57a90e25a5d71c8085047e7ef27a211baf791fbdf`  
		Last Modified: Thu, 23 Jan 2020 17:18:28 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c44a9b8d9f471fc81fea2fc3f754811b086921ce0e6ddc722666eeee59f4eab`  
		Last Modified: Thu, 23 Jan 2020 17:18:55 GMT  
		Size: 41.4 MB (41414773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b242415903bd0e91c2cf4db11a46a35e8ce72ce17cfb5bbc04c8ce1b4b37352`  
		Last Modified: Thu, 23 Jan 2020 17:18:29 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c602c8120e311bf687ab5541322da039164743f236c5d4dc8043b482e1662d`  
		Last Modified: Thu, 23 Jan 2020 17:18:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085df52b698732618e7ef9a5ab9ddb19f16a7225fb7e3b18757b7356529e85e8`  
		Last Modified: Thu, 23 Jan 2020 17:18:28 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5.3` - linux; arm variant v6

```console
$ docker pull consul@sha256:38b52a245cbb80b790c1a8029e767bc434161ab386e27c2d7f82086d7cdadc31
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41568465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2bdf49bc46e402782cbe73b1bb62e703924eba6c6c7fac502cd64529ac3fa0d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:13:41 GMT
ENV CONSUL_VERSION=1.5.3
# Thu, 23 Jan 2020 17:13:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:13:44 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:13:54 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:13:59 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:14:01 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:14:02 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:14:03 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:14:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:14:05 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:14:05 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:14:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:14:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1269d2d3c5158e948002340c38c38b6d89059db8677d1bbe82f948e02f3f0e2f`  
		Last Modified: Thu, 23 Jan 2020 17:18:10 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a735959ed46320f4a53f6d633965338fdc7da8bd8c64d0012f54d836ec8fa4e`  
		Last Modified: Thu, 23 Jan 2020 17:18:32 GMT  
		Size: 39.0 MB (39017477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2bd33cde350fba4407d450904b97cb4bcb0356d424554678fe111717d75ab7`  
		Last Modified: Thu, 23 Jan 2020 17:18:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df83aad6548933382b2d463d9ad4fcb04bcfa0bb9ee98987970f4d0f18f001c4`  
		Last Modified: Thu, 23 Jan 2020 17:18:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44789f2d596b74a4fd589b2f8253b9ce35ff7b674008bfe12ecc78c59fb8afcb`  
		Last Modified: Thu, 23 Jan 2020 17:18:09 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5.3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b93c8d7effcca6871ef3dc097b014579924e0e9e53562e153104c61467e2794f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41736776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78d71d8a623b84732d5eb46672cbd1526aa74216b8d824250ef3bebf908db4f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:20:53 GMT
ENV CONSUL_VERSION=1.5.3
# Thu, 23 Jan 2020 17:20:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:20:58 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:21:06 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:21:09 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:21:12 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:21:13 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:21:14 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:21:15 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:21:15 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:21:16 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:21:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:21:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66847b9d670332a71d6ede4a344d51162e0bdc6abd08a754f4de9c778ccfa1e4`  
		Last Modified: Thu, 23 Jan 2020 17:25:59 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add30ea62b96d1847e5af034c9942292447570d2feec35e349a29f3735569813`  
		Last Modified: Thu, 23 Jan 2020 17:26:11 GMT  
		Size: 39.0 MB (39040224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be64c310d7e9e83c8eadea0c99bce2a7949b115ceb55cc1470be31aaa8f7d21`  
		Last Modified: Thu, 23 Jan 2020 17:25:59 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5a2cf4964adaae1e25835708056bd14251cab62851cffa4452be09bd8c04a8`  
		Last Modified: Thu, 23 Jan 2020 17:25:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f808e5522e7eb3f5020ce3a4b64f87a4511c14ef14229c479ac2796d10ff6d52`  
		Last Modified: Thu, 23 Jan 2020 17:25:59 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.5.3` - linux; 386

```console
$ docker pull consul@sha256:3daff066c6231a9e9a0db506e8900e21e3f89193224838ab4be57a60f3570c14
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59dfe8338725130aa16669baef8a2dd21a4aebc5920b38e385f39a2a1c1ce5f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 23 Jan 2020 17:57:43 GMT
ENV CONSUL_VERSION=1.5.3
# Thu, 23 Jan 2020 17:57:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 23 Jan 2020 17:57:44 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 23 Jan 2020 17:57:52 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 23 Jan 2020 17:57:53 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 23 Jan 2020 17:57:54 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 23 Jan 2020 17:57:55 GMT
VOLUME [/consul/data]
# Thu, 23 Jan 2020 17:57:55 GMT
EXPOSE 8300
# Thu, 23 Jan 2020 17:57:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 23 Jan 2020 17:57:56 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 23 Jan 2020 17:57:56 GMT
COPY file:1c5f16053db7ac80ca2606114b1597e5421edf31162ea24a1ae8b059f48426f0 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 17:57:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 17:57:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5913bfdca346aa9c11eeafbea739f57e9b501ec0be2257fe0c997407c42f173d`  
		Last Modified: Thu, 23 Jan 2020 18:00:59 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa88ea0f6d80e829b1a82dc650fc5741398eff79c7fc2dcd3b44f9fa1c3a6cd1`  
		Last Modified: Thu, 23 Jan 2020 18:01:13 GMT  
		Size: 40.3 MB (40322432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a9f17c58fd993aa84360a71b3371b4dfe488a53062fbd6f6e83805ea1935f4`  
		Last Modified: Thu, 23 Jan 2020 18:00:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3799343516d02a56471eea7f8e2ae52325ae738036ab58264dc344500870cdd`  
		Last Modified: Thu, 23 Jan 2020 18:00:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05e7be14b5eab676cf5ef281cfcce68aaf208e9fc1d54c8c281f832f563781b`  
		Last Modified: Thu, 23 Jan 2020 18:00:59 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6`

```console
$ docker pull consul@sha256:8f735b1a7e6a62a345f805007def31bfd13b1b4d53424a861579d98b707de39d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6` - linux; amd64

```console
$ docker pull consul@sha256:9719a04f1286207bd9d1137eb455f25b83f8f933fd3340a48575278aa60314ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.7 MB (44663448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20001a3c09ce9a8954664e53fb2aa5fe5dd4250d5514f2c8ce08a8dad4e29c3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 23:21:14 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 23:21:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 23:21:15 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 23:21:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 23:21:20 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 23:21:21 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 23:21:21 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 23:21:21 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 23:21:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 23:21:22 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 23:21:22 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:21:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15878aef4423da9c80b5154606f4a0edc686cfb4f7719e8794db6a75c639062`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820bbf6db48b6a1ff342c75d812575732f08c4e444c55c304c4a736d7e1af442`  
		Last Modified: Thu, 30 Jan 2020 23:22:03 GMT  
		Size: 41.9 MB (41896017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6579edfb575b355796b593c7df28f53bda4913268db8ede91376ae2b7b82c3`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c55b5d5c6fc6ec75e25392111f1c3ee83044db3eae3c93071d9c38822b30ad`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095ef6f46849595eebb9d3f8c84990031e39f48d0b3517a83b6a6725919f0f0`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:5ab2fef70e77f6e74f961592ac6524d910449b09b83c1719c4da038f7715ac57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42056255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30d4cf4f0c21d1a8941470f2f7c05c22b670bbecac59c40ab833654ebd03b452`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 22:49:36 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 22:49:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 22:49:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 22:49:53 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 22:49:56 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 22:49:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 22:49:58 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 22:49:59 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 22:50:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 22:50:00 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 22:50:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 22:50:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 22:50:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3314d47720c9584ee0058003e4a40324cfa5a583a7009b003e7b2bf54e529d13`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df56066a99ad7031843fead4ba5e0eb60321f7789177a58db50a7a35b014f4a6`  
		Last Modified: Thu, 30 Jan 2020 22:51:01 GMT  
		Size: 39.5 MB (39505263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ed1e2fc130b8287684adcdc4b25acad567b6ee0262f7199e777e153d8ec1e7`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca1e99ee8f05dc3d93b818f2ef7534b472dfbb93d1da9e00dea82989631a4fa`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e15540eb9740c670106e005722202785736cb7bc4ed0df8a4b69e0f6c1164`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:861982fdd0ac25e652b2e6826431914551e1c9e42d8ab9d4432d99de8067ef87
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40233390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65c324f1a611a67554d77dad7fd28c7e82579f4afcf3135deb5d1825b5fba3b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 23:41:52 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 23:41:52 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 23:41:54 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 23:42:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 23:42:05 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 23:42:06 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 23:42:07 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 23:42:08 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 23:42:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 23:42:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 23:42:09 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:42:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd54316b1a2275e02125180270d62c994c05b452ee1192077712929179c4ad20`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24752c9fa8daf4a8dd6d5b7fa4abadb21a7d6ab863703b288e104d5e11b3a82`  
		Last Modified: Thu, 30 Jan 2020 23:43:05 GMT  
		Size: 37.5 MB (37536832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a12bd03b47a600aa4835cdf5f88965f8db747f01fae3a11449142873d19834`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a77e605d49684b179ffe2f5dea21961d99e60da2b0b876aaaf2a7dc2196628`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45affe15f8b6ab3cf5ec967697a9ac5b3446adc386b0dd3e6a3693b6bbba361`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; 386

```console
$ docker pull consul@sha256:549ea841e06954b67c4b052de945f8a3253d351d47cdf4fcfb2be40a24e1481a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43579250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64e5c2c0d75cd2c03f4dd16a32b159be185e6cb329fc27a7df7ac3d08c4e417d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 23:38:26 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 23:38:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 23:38:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 23:38:35 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 23:38:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 23:38:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 23:38:37 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 23:38:37 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 23:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 23:38:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 23:38:38 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:38:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc3496eeac5f321e785a5ca9b93bd32a04a4e40a032eb3b941f7ee3aca94992`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861631e7c94fde584b123379f277599f7f80b275ad7e0f2d094652a89008255b`  
		Last Modified: Thu, 30 Jan 2020 23:39:23 GMT  
		Size: 40.8 MB (40807471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb5de2cfbd714048b01c7f59056c4afb7f10b60e4360a0e7c0e3bd3e419ffe`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8044e4a22554f0829c001a0fdbb1e5935c36daa69a7eaf998084ff9e5e501917`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaf104116bc40f1e20c49e0674f1bfaccbf04309c77fe6b53c03cd2a1858a32`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6.3`

```console
$ docker pull consul@sha256:8f735b1a7e6a62a345f805007def31bfd13b1b4d53424a861579d98b707de39d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6.3` - linux; amd64

```console
$ docker pull consul@sha256:9719a04f1286207bd9d1137eb455f25b83f8f933fd3340a48575278aa60314ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.7 MB (44663448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20001a3c09ce9a8954664e53fb2aa5fe5dd4250d5514f2c8ce08a8dad4e29c3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 23:21:14 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 23:21:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 23:21:15 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 23:21:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 23:21:20 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 23:21:21 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 23:21:21 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 23:21:21 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 23:21:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 23:21:22 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 23:21:22 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:21:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15878aef4423da9c80b5154606f4a0edc686cfb4f7719e8794db6a75c639062`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820bbf6db48b6a1ff342c75d812575732f08c4e444c55c304c4a736d7e1af442`  
		Last Modified: Thu, 30 Jan 2020 23:22:03 GMT  
		Size: 41.9 MB (41896017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6579edfb575b355796b593c7df28f53bda4913268db8ede91376ae2b7b82c3`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c55b5d5c6fc6ec75e25392111f1c3ee83044db3eae3c93071d9c38822b30ad`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095ef6f46849595eebb9d3f8c84990031e39f48d0b3517a83b6a6725919f0f0`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.3` - linux; arm variant v6

```console
$ docker pull consul@sha256:5ab2fef70e77f6e74f961592ac6524d910449b09b83c1719c4da038f7715ac57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42056255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30d4cf4f0c21d1a8941470f2f7c05c22b670bbecac59c40ab833654ebd03b452`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 22:49:36 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 22:49:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 22:49:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 22:49:53 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 22:49:56 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 22:49:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 22:49:58 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 22:49:59 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 22:50:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 22:50:00 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 22:50:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 22:50:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 22:50:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3314d47720c9584ee0058003e4a40324cfa5a583a7009b003e7b2bf54e529d13`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df56066a99ad7031843fead4ba5e0eb60321f7789177a58db50a7a35b014f4a6`  
		Last Modified: Thu, 30 Jan 2020 22:51:01 GMT  
		Size: 39.5 MB (39505263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ed1e2fc130b8287684adcdc4b25acad567b6ee0262f7199e777e153d8ec1e7`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca1e99ee8f05dc3d93b818f2ef7534b472dfbb93d1da9e00dea82989631a4fa`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e15540eb9740c670106e005722202785736cb7bc4ed0df8a4b69e0f6c1164`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:861982fdd0ac25e652b2e6826431914551e1c9e42d8ab9d4432d99de8067ef87
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40233390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65c324f1a611a67554d77dad7fd28c7e82579f4afcf3135deb5d1825b5fba3b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 23:41:52 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 23:41:52 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 23:41:54 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 23:42:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 23:42:05 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 23:42:06 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 23:42:07 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 23:42:08 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 23:42:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 23:42:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 23:42:09 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:42:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd54316b1a2275e02125180270d62c994c05b452ee1192077712929179c4ad20`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24752c9fa8daf4a8dd6d5b7fa4abadb21a7d6ab863703b288e104d5e11b3a82`  
		Last Modified: Thu, 30 Jan 2020 23:43:05 GMT  
		Size: 37.5 MB (37536832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a12bd03b47a600aa4835cdf5f88965f8db747f01fae3a11449142873d19834`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a77e605d49684b179ffe2f5dea21961d99e60da2b0b876aaaf2a7dc2196628`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45affe15f8b6ab3cf5ec967697a9ac5b3446adc386b0dd3e6a3693b6bbba361`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.3` - linux; 386

```console
$ docker pull consul@sha256:549ea841e06954b67c4b052de945f8a3253d351d47cdf4fcfb2be40a24e1481a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43579250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64e5c2c0d75cd2c03f4dd16a32b159be185e6cb329fc27a7df7ac3d08c4e417d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 23:38:26 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 23:38:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 23:38:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 23:38:35 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 23:38:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 23:38:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 23:38:37 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 23:38:37 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 23:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 23:38:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 23:38:38 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:38:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc3496eeac5f321e785a5ca9b93bd32a04a4e40a032eb3b941f7ee3aca94992`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861631e7c94fde584b123379f277599f7f80b275ad7e0f2d094652a89008255b`  
		Last Modified: Thu, 30 Jan 2020 23:39:23 GMT  
		Size: 40.8 MB (40807471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb5de2cfbd714048b01c7f59056c4afb7f10b60e4360a0e7c0e3bd3e419ffe`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8044e4a22554f0829c001a0fdbb1e5935c36daa69a7eaf998084ff9e5e501917`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaf104116bc40f1e20c49e0674f1bfaccbf04309c77fe6b53c03cd2a1858a32`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7`

**does not exist** (yet?)

## `consul:1.7.0`

**does not exist** (yet?)

## `consul:latest`

```console
$ docker pull consul@sha256:8f735b1a7e6a62a345f805007def31bfd13b1b4d53424a861579d98b707de39d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:9719a04f1286207bd9d1137eb455f25b83f8f933fd3340a48575278aa60314ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.7 MB (44663448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20001a3c09ce9a8954664e53fb2aa5fe5dd4250d5514f2c8ce08a8dad4e29c3e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:17 GMT
ADD file:f4f85ec73d7cc949662413419f8eafb31dabaa6e12cd21b7c8d5a9ef0d5b9681 in / 
# Thu, 23 Jan 2020 16:53:17 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:15:11 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 23:21:14 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 23:21:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 23:21:15 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 23:21:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 23:21:20 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 23:21:21 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 23:21:21 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 23:21:21 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 23:21:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 23:21:22 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 23:21:22 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:21:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:21:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9123ac7c32f74759e6283f04dbf571f18246abe5bb2c779efcb32cd50f3ff13c`  
		Last Modified: Thu, 23 Jan 2020 16:53:45 GMT  
		Size: 2.8 MB (2764173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15878aef4423da9c80b5154606f4a0edc686cfb4f7719e8794db6a75c639062`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820bbf6db48b6a1ff342c75d812575732f08c4e444c55c304c4a736d7e1af442`  
		Last Modified: Thu, 30 Jan 2020 23:22:03 GMT  
		Size: 41.9 MB (41896017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6579edfb575b355796b593c7df28f53bda4913268db8ede91376ae2b7b82c3`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c55b5d5c6fc6ec75e25392111f1c3ee83044db3eae3c93071d9c38822b30ad`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7095ef6f46849595eebb9d3f8c84990031e39f48d0b3517a83b6a6725919f0f0`  
		Last Modified: Thu, 30 Jan 2020 23:21:56 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:5ab2fef70e77f6e74f961592ac6524d910449b09b83c1719c4da038f7715ac57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42056255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30d4cf4f0c21d1a8941470f2f7c05c22b670bbecac59c40ab833654ebd03b452`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:38 GMT
ADD file:7e840db4b1f91900bcc3693359908c82f531fc44027d4d5327ef598e8710ed0f in / 
# Thu, 23 Jan 2020 16:53:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:12:38 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 22:49:36 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 22:49:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 22:49:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 22:49:53 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 22:49:56 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 22:49:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 22:49:58 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 22:49:59 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 22:50:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 22:50:00 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 22:50:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 22:50:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 22:50:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c8737e28b1ca4452315b0127f7c6f4ad64f0c4695a3b52b1a4a3d2d17d3bbd5`  
		Last Modified: Thu, 23 Jan 2020 16:54:15 GMT  
		Size: 2.5 MB (2547672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3314d47720c9584ee0058003e4a40324cfa5a583a7009b003e7b2bf54e529d13`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df56066a99ad7031843fead4ba5e0eb60321f7789177a58db50a7a35b014f4a6`  
		Last Modified: Thu, 30 Jan 2020 22:51:01 GMT  
		Size: 39.5 MB (39505263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ed1e2fc130b8287684adcdc4b25acad567b6ee0262f7199e777e153d8ec1e7`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca1e99ee8f05dc3d93b818f2ef7534b472dfbb93d1da9e00dea82989631a4fa`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500e15540eb9740c670106e005722202785736cb7bc4ed0df8a4b69e0f6c1164`  
		Last Modified: Thu, 30 Jan 2020 22:50:50 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:861982fdd0ac25e652b2e6826431914551e1c9e42d8ab9d4432d99de8067ef87
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40233390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65c324f1a611a67554d77dad7fd28c7e82579f4afcf3135deb5d1825b5fba3b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:58 GMT
ADD file:92767b5525acd9dbf8657931d32bdcc7cc504cdc33c95e84a75e478b00569bab in / 
# Thu, 23 Jan 2020 16:54:59 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:19:49 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 23:41:52 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 23:41:52 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 23:41:54 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 23:42:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 23:42:05 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 23:42:06 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 23:42:07 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 23:42:08 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 23:42:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 23:42:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 23:42:09 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:42:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:42:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:eb93038481ddcf86a625b70f7551cdc583e38886f206fe7e40ad644008efa815`  
		Last Modified: Thu, 23 Jan 2020 16:55:31 GMT  
		Size: 2.7 MB (2693238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd54316b1a2275e02125180270d62c994c05b452ee1192077712929179c4ad20`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24752c9fa8daf4a8dd6d5b7fa4abadb21a7d6ab863703b288e104d5e11b3a82`  
		Last Modified: Thu, 30 Jan 2020 23:43:05 GMT  
		Size: 37.5 MB (37536832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86a12bd03b47a600aa4835cdf5f88965f8db747f01fae3a11449142873d19834`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a77e605d49684b179ffe2f5dea21961d99e60da2b0b876aaaf2a7dc2196628`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45affe15f8b6ab3cf5ec967697a9ac5b3446adc386b0dd3e6a3693b6bbba361`  
		Last Modified: Thu, 30 Jan 2020 23:42:54 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:549ea841e06954b67c4b052de945f8a3253d351d47cdf4fcfb2be40a24e1481a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43579250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64e5c2c0d75cd2c03f4dd16a32b159be185e6cb329fc27a7df7ac3d08c4e417d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:05 GMT
ADD file:4e7195ad2b3e9b85e4596b4a73719eb294f2a293a05b7b8e6096c4cfac0c6fde in / 
# Thu, 23 Jan 2020 16:53:05 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 17:57:03 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 30 Jan 2020 23:38:26 GMT
ENV CONSUL_VERSION=1.6.3
# Thu, 30 Jan 2020 23:38:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Jan 2020 23:38:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Jan 2020 23:38:35 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Jan 2020 23:38:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Jan 2020 23:38:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Jan 2020 23:38:37 GMT
VOLUME [/consul/data]
# Thu, 30 Jan 2020 23:38:37 GMT
EXPOSE 8300
# Thu, 30 Jan 2020 23:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Jan 2020 23:38:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Jan 2020 23:38:38 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Jan 2020 23:38:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Jan 2020 23:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fd25584d30bfc37afa2d99f41ef0a7055a4f2923907582dd992194fb4aa13f1c`  
		Last Modified: Thu, 23 Jan 2020 16:53:27 GMT  
		Size: 2.8 MB (2768519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc3496eeac5f321e785a5ca9b93bd32a04a4e40a032eb3b941f7ee3aca94992`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861631e7c94fde584b123379f277599f7f80b275ad7e0f2d094652a89008255b`  
		Last Modified: Thu, 30 Jan 2020 23:39:23 GMT  
		Size: 40.8 MB (40807471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabb5de2cfbd714048b01c7f59056c4afb7f10b60e4360a0e7c0e3bd3e419ffe`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8044e4a22554f0829c001a0fdbb1e5935c36daa69a7eaf998084ff9e5e501917`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaf104116bc40f1e20c49e0674f1bfaccbf04309c77fe6b53c03cd2a1858a32`  
		Last Modified: Thu, 30 Jan 2020 23:39:14 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
