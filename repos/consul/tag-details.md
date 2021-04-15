<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.7`](#consul17)
-	[`consul:1.7.13`](#consul1713)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.9`](#consul189)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.4`](#consul194)
-	[`consul:latest`](#consullatest)

## `consul:1.7`

```console
$ docker pull consul@sha256:2af038c167dfff98963be6727fa7dc7a487403a0f0b897196d991d9fb3cc66e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:30ad554f5a8982d32c5e3a15dfbae7ea2c9cc64f5127268424e6939665d4cf91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43160412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf47c0a5e27ce0fd0330b0abd671f0193b161334f73fc8139a99da2590c7c64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:14:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 20:15:13 GMT
ARG CONSUL_VERSION=1.7.13
# Wed, 14 Apr 2021 20:15:14 GMT
LABEL org.opencontainers.image.version=1.7.13
# Wed, 14 Apr 2021 20:15:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 20:15:16 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 20:15:29 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 20:15:32 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 20:15:34 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:15:34 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 20:15:34 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 20:15:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 20:15:35 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 20:15:36 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 20:15:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:15:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5ed97676b653ef31ffb62e1b4d3751a736bf7a83bded02548bdb3f3fff6fb7`  
		Last Modified: Wed, 14 Apr 2021 20:16:34 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2273ceb2040d0c6bbfeb44d44ac4b4ba59904ba883f51ae7a749e9a4bd32b1cf`  
		Last Modified: Wed, 14 Apr 2021 20:16:40 GMT  
		Size: 40.4 MB (40356554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878d8b2cdae5fa78631f47c83c8463fbaf82c376eadcdaca82ef4134c8b5e9e9`  
		Last Modified: Wed, 14 Apr 2021 20:16:34 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57137307e8e1e0cbad26268b2907caf0c5abf38dde25ab89757f6b0d6c1c145`  
		Last Modified: Wed, 14 Apr 2021 20:16:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7764ccadb29e0b518de2a54376e6648629e2005c3ec2ca5eab39e50e9ad78c15`  
		Last Modified: Wed, 14 Apr 2021 20:16:34 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:7ba3825092a6944745259ee247bc09df7da5671d364c7b0dafa8b59be91ed892
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.9 MB (38854078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e32b37fc718609862a981c494dfb75175b965d3b28bb27998f40410495a787`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:48:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:51:10 GMT
ARG CONSUL_VERSION=1.7.13
# Wed, 14 Apr 2021 19:51:11 GMT
LABEL org.opencontainers.image.version=1.7.13
# Wed, 14 Apr 2021 19:51:12 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:51:16 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:51:26 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:51:33 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:51:35 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:51:36 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:51:37 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:51:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:51:39 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:51:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:51:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3a1eed412d11a6c86e3a59a88c1d4afde737b156e96e7115c49f3716e944c`  
		Last Modified: Wed, 14 Apr 2021 19:52:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5145989ff5143d2455c02a88e85cb9e8060d48599bee48ae2b27bc221c0db104`  
		Last Modified: Wed, 14 Apr 2021 19:52:50 GMT  
		Size: 36.2 MB (36245532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e8b95f02943856f687e75b0e1d615a18032bce8371513d00845779fd8577bb`  
		Last Modified: Wed, 14 Apr 2021 19:52:40 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d8f73ee3427e122fbb378ae7cc6159f8610a2e2ae5e3bc8ffc6165e772bf1d`  
		Last Modified: Wed, 14 Apr 2021 19:52:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eb22a1d3bc66b7665462628e60d62b1cc27d406380d4187a41dcf06096389b`  
		Last Modified: Wed, 14 Apr 2021 19:52:40 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1afafb751bd0a85b255a51b60db53d646ac6bf61395d7f408212a9d4031981b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39071149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d02eb9fc189c0ec658af38a9baf46dc258de16998316cf5ebedf505539e849ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:22:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:24:03 GMT
ARG CONSUL_VERSION=1.7.13
# Wed, 14 Apr 2021 19:24:04 GMT
LABEL org.opencontainers.image.version=1.7.13
# Wed, 14 Apr 2021 19:24:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:24:08 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:24:15 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:24:18 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:24:20 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:24:21 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:24:22 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:24:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:24:24 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:24:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:24:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:24:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9f734f535e02dbd4e906c37c98f41711a2e686b87be5c4e5b4cd0209425de3`  
		Last Modified: Wed, 14 Apr 2021 19:25:26 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd7e39bb1820fdec3015b10ee854d61c1d26efac1a4d168f2ae8b240ee42c31`  
		Last Modified: Wed, 14 Apr 2021 19:25:33 GMT  
		Size: 36.4 MB (36357165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0b4f3df551660cfb737ba89506d0cce8d9b2903afb4ee7e04b97d37e477e04`  
		Last Modified: Wed, 14 Apr 2021 19:25:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f94cfd07f9c44ebe79b4b829856c413af484bc30a473f8b94d4fd5a5c4fc58`  
		Last Modified: Wed, 14 Apr 2021 19:25:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf32e2d0ec7733fe6fc7cf834e221ec44257147f5c7631a0a54c80ef996f713`  
		Last Modified: Wed, 14 Apr 2021 19:25:25 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:e36f2b17709f22341fb80d892f852fb2a653c1c3c05eb09b4ec4a0443f017727
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41967695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad2c4ba0498e14730d0e35f973293145c985da63b8a5289dee1adb533ec8d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 18:56:07 GMT
ARG CONSUL_VERSION=1.7.13
# Wed, 14 Apr 2021 18:56:07 GMT
LABEL org.opencontainers.image.version=1.7.13
# Wed, 14 Apr 2021 18:56:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 18:56:08 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 18:56:13 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 18:56:14 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 18:56:15 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 18:56:15 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 18:56:15 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 18:56:16 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 18:56:16 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 18:56:16 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 18:56:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 18:56:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e51d0cf9f34fc8ef57ae4d7f8312d898899a7d394e62f68c75668c7c392af5d`  
		Last Modified: Wed, 14 Apr 2021 18:57:41 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a6cfb7bf36bcf37242b07431d6db85c7c63f17226062c385c77e9aebfeb560`  
		Last Modified: Wed, 14 Apr 2021 18:57:47 GMT  
		Size: 39.2 MB (39168609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007d5a25290063f49c42946d7bd8a9269aff393731dd02c47b246baa64f1f86e`  
		Last Modified: Wed, 14 Apr 2021 18:57:41 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bf9d5f8cc42a78be8dc2b92dd3c8b70e13f968a11a13a4e8971d74f16410cd`  
		Last Modified: Wed, 14 Apr 2021 18:57:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421f9d51d4bba68eec8dd875989856dac5f1b65093cc8b72f8c54cd55d3901e`  
		Last Modified: Wed, 14 Apr 2021 18:57:41 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.13`

```console
$ docker pull consul@sha256:2af038c167dfff98963be6727fa7dc7a487403a0f0b897196d991d9fb3cc66e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.13` - linux; amd64

```console
$ docker pull consul@sha256:30ad554f5a8982d32c5e3a15dfbae7ea2c9cc64f5127268424e6939665d4cf91
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43160412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf47c0a5e27ce0fd0330b0abd671f0193b161334f73fc8139a99da2590c7c64`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:14:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 20:15:13 GMT
ARG CONSUL_VERSION=1.7.13
# Wed, 14 Apr 2021 20:15:14 GMT
LABEL org.opencontainers.image.version=1.7.13
# Wed, 14 Apr 2021 20:15:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 20:15:16 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 20:15:29 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 20:15:32 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 20:15:34 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:15:34 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 20:15:34 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 20:15:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 20:15:35 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 20:15:36 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 20:15:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:15:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5ed97676b653ef31ffb62e1b4d3751a736bf7a83bded02548bdb3f3fff6fb7`  
		Last Modified: Wed, 14 Apr 2021 20:16:34 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2273ceb2040d0c6bbfeb44d44ac4b4ba59904ba883f51ae7a749e9a4bd32b1cf`  
		Last Modified: Wed, 14 Apr 2021 20:16:40 GMT  
		Size: 40.4 MB (40356554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878d8b2cdae5fa78631f47c83c8463fbaf82c376eadcdaca82ef4134c8b5e9e9`  
		Last Modified: Wed, 14 Apr 2021 20:16:34 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57137307e8e1e0cbad26268b2907caf0c5abf38dde25ab89757f6b0d6c1c145`  
		Last Modified: Wed, 14 Apr 2021 20:16:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7764ccadb29e0b518de2a54376e6648629e2005c3ec2ca5eab39e50e9ad78c15`  
		Last Modified: Wed, 14 Apr 2021 20:16:34 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.13` - linux; arm variant v6

```console
$ docker pull consul@sha256:7ba3825092a6944745259ee247bc09df7da5671d364c7b0dafa8b59be91ed892
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.9 MB (38854078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e32b37fc718609862a981c494dfb75175b965d3b28bb27998f40410495a787`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:48:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:51:10 GMT
ARG CONSUL_VERSION=1.7.13
# Wed, 14 Apr 2021 19:51:11 GMT
LABEL org.opencontainers.image.version=1.7.13
# Wed, 14 Apr 2021 19:51:12 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:51:16 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:51:26 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:51:33 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:51:35 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:51:36 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:51:37 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:51:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:51:39 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:51:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:51:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f3a1eed412d11a6c86e3a59a88c1d4afde737b156e96e7115c49f3716e944c`  
		Last Modified: Wed, 14 Apr 2021 19:52:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5145989ff5143d2455c02a88e85cb9e8060d48599bee48ae2b27bc221c0db104`  
		Last Modified: Wed, 14 Apr 2021 19:52:50 GMT  
		Size: 36.2 MB (36245532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e8b95f02943856f687e75b0e1d615a18032bce8371513d00845779fd8577bb`  
		Last Modified: Wed, 14 Apr 2021 19:52:40 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d8f73ee3427e122fbb378ae7cc6159f8610a2e2ae5e3bc8ffc6165e772bf1d`  
		Last Modified: Wed, 14 Apr 2021 19:52:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eb22a1d3bc66b7665462628e60d62b1cc27d406380d4187a41dcf06096389b`  
		Last Modified: Wed, 14 Apr 2021 19:52:40 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.13` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1afafb751bd0a85b255a51b60db53d646ac6bf61395d7f408212a9d4031981b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39071149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d02eb9fc189c0ec658af38a9baf46dc258de16998316cf5ebedf505539e849ba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:22:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:24:03 GMT
ARG CONSUL_VERSION=1.7.13
# Wed, 14 Apr 2021 19:24:04 GMT
LABEL org.opencontainers.image.version=1.7.13
# Wed, 14 Apr 2021 19:24:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:24:08 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:24:15 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:24:18 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:24:20 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:24:21 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:24:22 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:24:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:24:24 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:24:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:24:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:24:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a9f734f535e02dbd4e906c37c98f41711a2e686b87be5c4e5b4cd0209425de3`  
		Last Modified: Wed, 14 Apr 2021 19:25:26 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd7e39bb1820fdec3015b10ee854d61c1d26efac1a4d168f2ae8b240ee42c31`  
		Last Modified: Wed, 14 Apr 2021 19:25:33 GMT  
		Size: 36.4 MB (36357165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af0b4f3df551660cfb737ba89506d0cce8d9b2903afb4ee7e04b97d37e477e04`  
		Last Modified: Wed, 14 Apr 2021 19:25:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f94cfd07f9c44ebe79b4b829856c413af484bc30a473f8b94d4fd5a5c4fc58`  
		Last Modified: Wed, 14 Apr 2021 19:25:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf32e2d0ec7733fe6fc7cf834e221ec44257147f5c7631a0a54c80ef996f713`  
		Last Modified: Wed, 14 Apr 2021 19:25:25 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.13` - linux; 386

```console
$ docker pull consul@sha256:e36f2b17709f22341fb80d892f852fb2a653c1c3c05eb09b4ec4a0443f017727
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41967695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ad2c4ba0498e14730d0e35f973293145c985da63b8a5289dee1adb533ec8d82`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 18:56:07 GMT
ARG CONSUL_VERSION=1.7.13
# Wed, 14 Apr 2021 18:56:07 GMT
LABEL org.opencontainers.image.version=1.7.13
# Wed, 14 Apr 2021 18:56:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 18:56:08 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 18:56:13 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 18:56:14 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 18:56:15 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 18:56:15 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 18:56:15 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 18:56:16 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 18:56:16 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 18:56:16 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 18:56:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 18:56:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e51d0cf9f34fc8ef57ae4d7f8312d898899a7d394e62f68c75668c7c392af5d`  
		Last Modified: Wed, 14 Apr 2021 18:57:41 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a6cfb7bf36bcf37242b07431d6db85c7c63f17226062c385c77e9aebfeb560`  
		Last Modified: Wed, 14 Apr 2021 18:57:47 GMT  
		Size: 39.2 MB (39168609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007d5a25290063f49c42946d7bd8a9269aff393731dd02c47b246baa64f1f86e`  
		Last Modified: Wed, 14 Apr 2021 18:57:41 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bf9d5f8cc42a78be8dc2b92dd3c8b70e13f968a11a13a4e8971d74f16410cd`  
		Last Modified: Wed, 14 Apr 2021 18:57:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b421f9d51d4bba68eec8dd875989856dac5f1b65093cc8b72f8c54cd55d3901e`  
		Last Modified: Wed, 14 Apr 2021 18:57:41 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:be906b8395cfd33c25c5ed051c53a0c2541de551542ca9d527ea6f6149279a15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:7413f2c739c98bd5e121a1798c6d3ed8ddde4a6f1cf217d906506194e361ecaa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46547774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9a2d4e8475b5b96d88239a7230443bbdf6a94db78890b48c106ab2888b517a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:14:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 20:14:47 GMT
ARG CONSUL_VERSION=1.8.9
# Wed, 14 Apr 2021 20:14:47 GMT
LABEL org.opencontainers.image.version=1.8.9
# Wed, 14 Apr 2021 20:14:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 20:14:50 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 20:14:58 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 20:15:01 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 20:15:03 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:15:04 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 20:15:04 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 20:15:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 20:15:05 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 20:15:06 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 20:15:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:15:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2962128d5213477b100c792f668fe1f1103252fd597434b13dc41bf9aaa95e25`  
		Last Modified: Wed, 14 Apr 2021 20:16:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2addd9ed0763874bcfdcdfe2339e0bf96666431e7318124c962eecfbb8f87fc`  
		Last Modified: Wed, 14 Apr 2021 20:16:22 GMT  
		Size: 43.7 MB (43743917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af9b3772486b7b78774a0e4ad9efd7080ce3a172ada2fd7c2f2ca15d51ae8`  
		Last Modified: Wed, 14 Apr 2021 20:16:16 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfac59635651856ebd2c485c363c92af2ffbdda250f82ba4b796cb821728679`  
		Last Modified: Wed, 14 Apr 2021 20:16:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb95be59f804ebdb96880ff7575de9e00793c0bac23012a6cc6874fb2e91310d`  
		Last Modified: Wed, 14 Apr 2021 20:16:17 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:f415e69dbe0b469b1a45ec89bd780df9ecd8232cea5950e0e5cbe00d774502d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41809057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12bf896288482d481c892aaf8f22bc2e60def0956ae675646b38ff1911499d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:48:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:50:25 GMT
ARG CONSUL_VERSION=1.8.9
# Wed, 14 Apr 2021 19:50:27 GMT
LABEL org.opencontainers.image.version=1.8.9
# Wed, 14 Apr 2021 19:50:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:50:30 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:50:44 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:50:50 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:50:52 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:50:53 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:50:54 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:50:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:50:56 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:50:58 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:50:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79562b0ef2bda58f27e4b920ddaa4ddc06cd0d151574f31a8a8ec47a27ac1430`  
		Last Modified: Wed, 14 Apr 2021 19:52:21 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7eed33841774d06dd98c6a8dd9beb4ece0f327917850b2963823afc2f5499dd`  
		Last Modified: Wed, 14 Apr 2021 19:52:32 GMT  
		Size: 39.2 MB (39200512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ed9e781c2e19d39661d4026e5623c93357d61c685dfebd75a8d813ba16e302`  
		Last Modified: Wed, 14 Apr 2021 19:52:21 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0a6b728d534a358b5f763a61c5357a9270143aec90cdb4cc6f9aa93b0202dd`  
		Last Modified: Wed, 14 Apr 2021 19:52:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320278702380eb051dbb92f49c37b21fefd396f82a0caf3eadbd668d4fa4d5c7`  
		Last Modified: Wed, 14 Apr 2021 19:52:21 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:efa6e7ca940f6a14444b4f84ed7ed23db7cda69629c641a0c0962295b920ce85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41982267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e5d398fd2f340fc1b4b2dc2ba57d5c86e6b32367860efb35cab1023fd376027`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:22:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:23:26 GMT
ARG CONSUL_VERSION=1.8.9
# Wed, 14 Apr 2021 19:23:28 GMT
LABEL org.opencontainers.image.version=1.8.9
# Wed, 14 Apr 2021 19:23:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:23:31 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:23:38 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:23:41 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:23:44 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:23:45 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:23:46 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:23:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:23:48 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:23:49 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:23:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:23:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b5571393035c4757df133370d5c2d1c7b9a5c0b6a1c991e2644048a71814b8`  
		Last Modified: Wed, 14 Apr 2021 19:25:09 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c763675dd4ef92e3623c1b49e892cf59de5e3f3d14a3c6a675fbfa98481ac`  
		Last Modified: Wed, 14 Apr 2021 19:25:17 GMT  
		Size: 39.3 MB (39268281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcaec3c757f98193db9c9837ddcf261f3bab3eddd4ccb6dc42ed48ee79e688c`  
		Last Modified: Wed, 14 Apr 2021 19:25:09 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf224d390c88605c93f6484c31f95889a6ff4e4ab16e07d708f02c58efd3442a`  
		Last Modified: Wed, 14 Apr 2021 19:25:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501b62f777fbc16d208c09cb46bda23b3e53e0a58aa442a55605985dbaa056b`  
		Last Modified: Wed, 14 Apr 2021 19:25:09 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:5dce80a9c00ce04e6bc012d8f02f948f3b1b3ca069668d0403228fc9e8cd2268
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46072303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:432bba23041c7d8beaa473e2b676c66eb2d8a60b83fb61ec6cce850b6b1d33ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 18:55:53 GMT
ARG CONSUL_VERSION=1.8.9
# Wed, 14 Apr 2021 18:55:53 GMT
LABEL org.opencontainers.image.version=1.8.9
# Wed, 14 Apr 2021 18:55:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 18:55:54 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 18:55:59 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 18:56:00 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 18:56:01 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 18:56:01 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 18:56:01 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 18:56:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 18:56:02 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 18:56:02 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 18:56:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 18:56:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8db9ae0b7b83ba7b1defb913bc9dbed81c21def51442f927dd0e716b89f6f5`  
		Last Modified: Wed, 14 Apr 2021 18:57:22 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da24a16fbc35b0e5b01d6803bd687e835baedd549845c2b3c6db5065b23b3a`  
		Last Modified: Wed, 14 Apr 2021 18:57:29 GMT  
		Size: 43.3 MB (43273215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57cf0eb793920b9309d2f2d5887c0f9956e4f4ac3544e91ea1a0db4a358df60`  
		Last Modified: Wed, 14 Apr 2021 18:57:22 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa6e9893eb45f30ce4ae14c4d89e283a022f5a46bd1cfab3498da4c718d7d93`  
		Last Modified: Wed, 14 Apr 2021 18:57:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a179f593ded316386fbf4301a8eb438e4495471af99b86246711ff5af6109021`  
		Last Modified: Wed, 14 Apr 2021 18:57:22 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.9`

```console
$ docker pull consul@sha256:be906b8395cfd33c25c5ed051c53a0c2541de551542ca9d527ea6f6149279a15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.9` - linux; amd64

```console
$ docker pull consul@sha256:7413f2c739c98bd5e121a1798c6d3ed8ddde4a6f1cf217d906506194e361ecaa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46547774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a9a2d4e8475b5b96d88239a7230443bbdf6a94db78890b48c106ab2888b517a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:14:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 20:14:47 GMT
ARG CONSUL_VERSION=1.8.9
# Wed, 14 Apr 2021 20:14:47 GMT
LABEL org.opencontainers.image.version=1.8.9
# Wed, 14 Apr 2021 20:14:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 20:14:50 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 20:14:58 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 20:15:01 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 20:15:03 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:15:04 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 20:15:04 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 20:15:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 20:15:05 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 20:15:06 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 20:15:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:15:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2962128d5213477b100c792f668fe1f1103252fd597434b13dc41bf9aaa95e25`  
		Last Modified: Wed, 14 Apr 2021 20:16:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2addd9ed0763874bcfdcdfe2339e0bf96666431e7318124c962eecfbb8f87fc`  
		Last Modified: Wed, 14 Apr 2021 20:16:22 GMT  
		Size: 43.7 MB (43743917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af9b3772486b7b78774a0e4ad9efd7080ce3a172ada2fd7c2f2ca15d51ae8`  
		Last Modified: Wed, 14 Apr 2021 20:16:16 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bfac59635651856ebd2c485c363c92af2ffbdda250f82ba4b796cb821728679`  
		Last Modified: Wed, 14 Apr 2021 20:16:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb95be59f804ebdb96880ff7575de9e00793c0bac23012a6cc6874fb2e91310d`  
		Last Modified: Wed, 14 Apr 2021 20:16:17 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:f415e69dbe0b469b1a45ec89bd780df9ecd8232cea5950e0e5cbe00d774502d2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41809057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12bf896288482d481c892aaf8f22bc2e60def0956ae675646b38ff1911499d8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:48:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:50:25 GMT
ARG CONSUL_VERSION=1.8.9
# Wed, 14 Apr 2021 19:50:27 GMT
LABEL org.opencontainers.image.version=1.8.9
# Wed, 14 Apr 2021 19:50:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:50:30 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:50:44 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:50:50 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:50:52 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:50:53 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:50:54 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:50:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:50:56 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:50:58 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:50:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79562b0ef2bda58f27e4b920ddaa4ddc06cd0d151574f31a8a8ec47a27ac1430`  
		Last Modified: Wed, 14 Apr 2021 19:52:21 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7eed33841774d06dd98c6a8dd9beb4ece0f327917850b2963823afc2f5499dd`  
		Last Modified: Wed, 14 Apr 2021 19:52:32 GMT  
		Size: 39.2 MB (39200512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ed9e781c2e19d39661d4026e5623c93357d61c685dfebd75a8d813ba16e302`  
		Last Modified: Wed, 14 Apr 2021 19:52:21 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0a6b728d534a358b5f763a61c5357a9270143aec90cdb4cc6f9aa93b0202dd`  
		Last Modified: Wed, 14 Apr 2021 19:52:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320278702380eb051dbb92f49c37b21fefd396f82a0caf3eadbd668d4fa4d5c7`  
		Last Modified: Wed, 14 Apr 2021 19:52:21 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:efa6e7ca940f6a14444b4f84ed7ed23db7cda69629c641a0c0962295b920ce85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41982267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e5d398fd2f340fc1b4b2dc2ba57d5c86e6b32367860efb35cab1023fd376027`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:22:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:23:26 GMT
ARG CONSUL_VERSION=1.8.9
# Wed, 14 Apr 2021 19:23:28 GMT
LABEL org.opencontainers.image.version=1.8.9
# Wed, 14 Apr 2021 19:23:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:23:31 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:23:38 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:23:41 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:23:44 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:23:45 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:23:46 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:23:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:23:48 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:23:49 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:23:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:23:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b5571393035c4757df133370d5c2d1c7b9a5c0b6a1c991e2644048a71814b8`  
		Last Modified: Wed, 14 Apr 2021 19:25:09 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827c763675dd4ef92e3623c1b49e892cf59de5e3f3d14a3c6a675fbfa98481ac`  
		Last Modified: Wed, 14 Apr 2021 19:25:17 GMT  
		Size: 39.3 MB (39268281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bcaec3c757f98193db9c9837ddcf261f3bab3eddd4ccb6dc42ed48ee79e688c`  
		Last Modified: Wed, 14 Apr 2021 19:25:09 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf224d390c88605c93f6484c31f95889a6ff4e4ab16e07d708f02c58efd3442a`  
		Last Modified: Wed, 14 Apr 2021 19:25:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4501b62f777fbc16d208c09cb46bda23b3e53e0a58aa442a55605985dbaa056b`  
		Last Modified: Wed, 14 Apr 2021 19:25:09 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.9` - linux; 386

```console
$ docker pull consul@sha256:5dce80a9c00ce04e6bc012d8f02f948f3b1b3ca069668d0403228fc9e8cd2268
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.1 MB (46072303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:432bba23041c7d8beaa473e2b676c66eb2d8a60b83fb61ec6cce850b6b1d33ff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 18:55:53 GMT
ARG CONSUL_VERSION=1.8.9
# Wed, 14 Apr 2021 18:55:53 GMT
LABEL org.opencontainers.image.version=1.8.9
# Wed, 14 Apr 2021 18:55:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 18:55:54 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 18:55:59 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 18:56:00 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 18:56:01 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 18:56:01 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 18:56:01 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 18:56:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 18:56:02 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 18:56:02 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 18:56:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 18:56:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8db9ae0b7b83ba7b1defb913bc9dbed81c21def51442f927dd0e716b89f6f5`  
		Last Modified: Wed, 14 Apr 2021 18:57:22 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3da24a16fbc35b0e5b01d6803bd687e835baedd549845c2b3c6db5065b23b3a`  
		Last Modified: Wed, 14 Apr 2021 18:57:29 GMT  
		Size: 43.3 MB (43273215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57cf0eb793920b9309d2f2d5887c0f9956e4f4ac3544e91ea1a0db4a358df60`  
		Last Modified: Wed, 14 Apr 2021 18:57:22 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa6e9893eb45f30ce4ae14c4d89e283a022f5a46bd1cfab3498da4c718d7d93`  
		Last Modified: Wed, 14 Apr 2021 18:57:22 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a179f593ded316386fbf4301a8eb438e4495471af99b86246711ff5af6109021`  
		Last Modified: Wed, 14 Apr 2021 18:57:22 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:c7ac5b7a23cab94ce207da2722fe37666d6d31dd0de585798149f92a1bd59628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:0e1bf46d11fc1206b823adee771d4a828c1e43ffbc61eb0f3bd1b9c4c2e9555c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45660975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28efe5fcc0492ee7af47f817357211e3e0e079d76d208f83fb67190fc1005c24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:14:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 20:14:28 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 20:14:29 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 20:14:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 20:14:30 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 20:14:35 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 20:14:37 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 20:14:39 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:14:39 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 20:14:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 20:14:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:14:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6f7401278b6047ca51b04eaa48718d1ad2217d17cfa7aacd0f88cd75087ef`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42903c65e0ffb2011b9dd5455c10767b28d080882f7b5e147dfcdae436589415`  
		Last Modified: Wed, 14 Apr 2021 20:16:02 GMT  
		Size: 42.9 MB (42857116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7545c107e7a73790423708f86188c0f57b1f3047db4b363546f26dbf95b752d`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f837edf7afc74be22f4b914b3e9050371bcab6111de42aaf802c2711006836d`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d959978e907f3ffccec3ec6bcc1486bba7e9431b596593b89ed84b472ec89e27`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:57f0b9e1d87c0a5ef6946bbd6a1767d1630d5f3e238cd84e04312dbbb0472084
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40911088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d290d4e40b5f15fcadae2f208f0d12a0b2b75c21b0202d4ee126628c3e50db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:48:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:48:51 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 19:48:52 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 19:48:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:48:59 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:50:03 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:50:07 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:50:10 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:50:10 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:50:11 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:50:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:50:13 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:50:13 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:50:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:50:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab416f4b1ee1c7c4f0f327a9548c6fa41fc8b61b7ff80bb072ab5eafbfe81aa`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f9bff852385f80d92506250cb34641498caaf3ce2ce6774bdeb80d5fa1611f`  
		Last Modified: Wed, 14 Apr 2021 19:52:13 GMT  
		Size: 38.3 MB (38302542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45821997bb09bd9c2430bf007cca645d38ae22f9cd53c846f84f8ed54f70aa64`  
		Last Modified: Wed, 14 Apr 2021 19:52:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53516a4fc57619782eda8f42b4918106984adb2bdabaca7b3f7c1c0a65eeb0`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c919202793e92b538f208f3ee0e5f7e92e03111769f68f8ab0d94438916bca41`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:794c24fbbd979bf5af6af9630d7d9325aa6f01f668f4bca857204c5994c54b3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41126204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a825e2fced0b53948b4f9e7bfc5d1609481cc108c2d60c1c6fd96b2643c9736a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:22:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:22:51 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 19:22:52 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 19:22:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:22:56 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:23:03 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:23:06 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:23:09 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:23:10 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:23:11 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:23:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:23:13 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:23:14 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:23:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:23:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b96788e82b6af129f934f44e3be6e11bd50c5aa4aa7f153d5c23ccb0dc12cf`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:face225286cec8239bf7c33e3977ca020cbc18e6b8cd3865c520feb00357f466`  
		Last Modified: Wed, 14 Apr 2021 19:24:57 GMT  
		Size: 38.4 MB (38412219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fb33ef170a52b1969e77c98378e9677623a19a6c6c17b581a3b345a3f9d387`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3befdfcaca0963f39f847c37604e9867e38aaca2fa8bbfde33c3515e22ec18`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b246d545ee670f4fd4a8233c1a1fb4233cba1d92c226cf5fad4566571d125075`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:f7b2894fa2b2cce628874cb34c141e154a36af139a2ce7cf8ea879057ec1f36a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44978347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e6b7fa39b52e886a1bcecc2e7cca9076c09427848558ee7631e8b5a9a924e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 18:55:36 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 18:55:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 18:55:37 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 18:55:44 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 18:55:45 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 18:55:46 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 18:55:46 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 18:55:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 18:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 18:55:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3831ff37459cebceaf36d2175d922fea9abe8aa2d956f29596fcce2b12cc90d`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf5d944668f1ce4efe25c8da04427ff173e57ba09ae72f16313fe5fd01d77b`  
		Last Modified: Wed, 14 Apr 2021 18:56:48 GMT  
		Size: 42.2 MB (42179261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f75e489a23c08e7c8d80a390517626ae20d9bc1900e38f640c3ceb3c452289`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9108803843267de412c0c6aa141a1d17bc55047f1b59d3602ce336005d6a81`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77f9b370fadecaa06e11cd41a1054987b24cf57a0b49c6b4d3f1c4a64928e40`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.4`

```console
$ docker pull consul@sha256:c7ac5b7a23cab94ce207da2722fe37666d6d31dd0de585798149f92a1bd59628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.4` - linux; amd64

```console
$ docker pull consul@sha256:0e1bf46d11fc1206b823adee771d4a828c1e43ffbc61eb0f3bd1b9c4c2e9555c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45660975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28efe5fcc0492ee7af47f817357211e3e0e079d76d208f83fb67190fc1005c24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:14:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 20:14:28 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 20:14:29 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 20:14:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 20:14:30 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 20:14:35 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 20:14:37 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 20:14:39 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:14:39 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 20:14:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 20:14:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:14:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6f7401278b6047ca51b04eaa48718d1ad2217d17cfa7aacd0f88cd75087ef`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42903c65e0ffb2011b9dd5455c10767b28d080882f7b5e147dfcdae436589415`  
		Last Modified: Wed, 14 Apr 2021 20:16:02 GMT  
		Size: 42.9 MB (42857116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7545c107e7a73790423708f86188c0f57b1f3047db4b363546f26dbf95b752d`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f837edf7afc74be22f4b914b3e9050371bcab6111de42aaf802c2711006836d`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d959978e907f3ffccec3ec6bcc1486bba7e9431b596593b89ed84b472ec89e27`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:57f0b9e1d87c0a5ef6946bbd6a1767d1630d5f3e238cd84e04312dbbb0472084
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40911088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d290d4e40b5f15fcadae2f208f0d12a0b2b75c21b0202d4ee126628c3e50db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:48:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:48:51 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 19:48:52 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 19:48:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:48:59 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:50:03 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:50:07 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:50:10 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:50:10 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:50:11 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:50:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:50:13 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:50:13 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:50:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:50:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab416f4b1ee1c7c4f0f327a9548c6fa41fc8b61b7ff80bb072ab5eafbfe81aa`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f9bff852385f80d92506250cb34641498caaf3ce2ce6774bdeb80d5fa1611f`  
		Last Modified: Wed, 14 Apr 2021 19:52:13 GMT  
		Size: 38.3 MB (38302542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45821997bb09bd9c2430bf007cca645d38ae22f9cd53c846f84f8ed54f70aa64`  
		Last Modified: Wed, 14 Apr 2021 19:52:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53516a4fc57619782eda8f42b4918106984adb2bdabaca7b3f7c1c0a65eeb0`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c919202793e92b538f208f3ee0e5f7e92e03111769f68f8ab0d94438916bca41`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:794c24fbbd979bf5af6af9630d7d9325aa6f01f668f4bca857204c5994c54b3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41126204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a825e2fced0b53948b4f9e7bfc5d1609481cc108c2d60c1c6fd96b2643c9736a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:22:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:22:51 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 19:22:52 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 19:22:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:22:56 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:23:03 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:23:06 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:23:09 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:23:10 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:23:11 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:23:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:23:13 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:23:14 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:23:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:23:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b96788e82b6af129f934f44e3be6e11bd50c5aa4aa7f153d5c23ccb0dc12cf`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:face225286cec8239bf7c33e3977ca020cbc18e6b8cd3865c520feb00357f466`  
		Last Modified: Wed, 14 Apr 2021 19:24:57 GMT  
		Size: 38.4 MB (38412219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fb33ef170a52b1969e77c98378e9677623a19a6c6c17b581a3b345a3f9d387`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3befdfcaca0963f39f847c37604e9867e38aaca2fa8bbfde33c3515e22ec18`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b246d545ee670f4fd4a8233c1a1fb4233cba1d92c226cf5fad4566571d125075`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.4` - linux; 386

```console
$ docker pull consul@sha256:f7b2894fa2b2cce628874cb34c141e154a36af139a2ce7cf8ea879057ec1f36a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44978347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e6b7fa39b52e886a1bcecc2e7cca9076c09427848558ee7631e8b5a9a924e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 18:55:36 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 18:55:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 18:55:37 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 18:55:44 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 18:55:45 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 18:55:46 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 18:55:46 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 18:55:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 18:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 18:55:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3831ff37459cebceaf36d2175d922fea9abe8aa2d956f29596fcce2b12cc90d`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf5d944668f1ce4efe25c8da04427ff173e57ba09ae72f16313fe5fd01d77b`  
		Last Modified: Wed, 14 Apr 2021 18:56:48 GMT  
		Size: 42.2 MB (42179261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f75e489a23c08e7c8d80a390517626ae20d9bc1900e38f640c3ceb3c452289`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9108803843267de412c0c6aa141a1d17bc55047f1b59d3602ce336005d6a81`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77f9b370fadecaa06e11cd41a1054987b24cf57a0b49c6b4d3f1c4a64928e40`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:c7ac5b7a23cab94ce207da2722fe37666d6d31dd0de585798149f92a1bd59628
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:0e1bf46d11fc1206b823adee771d4a828c1e43ffbc61eb0f3bd1b9c4c2e9555c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45660975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28efe5fcc0492ee7af47f817357211e3e0e079d76d208f83fb67190fc1005c24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:14:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 20:14:28 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 20:14:29 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 20:14:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 20:14:30 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 20:14:35 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 20:14:37 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 20:14:39 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:14:39 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 20:14:40 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 20:14:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 20:14:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 20:14:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d6f7401278b6047ca51b04eaa48718d1ad2217d17cfa7aacd0f88cd75087ef`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42903c65e0ffb2011b9dd5455c10767b28d080882f7b5e147dfcdae436589415`  
		Last Modified: Wed, 14 Apr 2021 20:16:02 GMT  
		Size: 42.9 MB (42857116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7545c107e7a73790423708f86188c0f57b1f3047db4b363546f26dbf95b752d`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f837edf7afc74be22f4b914b3e9050371bcab6111de42aaf802c2711006836d`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d959978e907f3ffccec3ec6bcc1486bba7e9431b596593b89ed84b472ec89e27`  
		Last Modified: Wed, 14 Apr 2021 20:15:56 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:57f0b9e1d87c0a5ef6946bbd6a1767d1630d5f3e238cd84e04312dbbb0472084
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40911088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7d290d4e40b5f15fcadae2f208f0d12a0b2b75c21b0202d4ee126628c3e50db`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:48:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:48:51 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 19:48:52 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 19:48:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:48:59 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:50:03 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:50:07 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:50:10 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:50:10 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:50:11 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:50:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:50:13 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:50:13 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:50:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:50:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab416f4b1ee1c7c4f0f327a9548c6fa41fc8b61b7ff80bb072ab5eafbfe81aa`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f9bff852385f80d92506250cb34641498caaf3ce2ce6774bdeb80d5fa1611f`  
		Last Modified: Wed, 14 Apr 2021 19:52:13 GMT  
		Size: 38.3 MB (38302542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45821997bb09bd9c2430bf007cca645d38ae22f9cd53c846f84f8ed54f70aa64`  
		Last Modified: Wed, 14 Apr 2021 19:52:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf53516a4fc57619782eda8f42b4918106984adb2bdabaca7b3f7c1c0a65eeb0`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c919202793e92b538f208f3ee0e5f7e92e03111769f68f8ab0d94438916bca41`  
		Last Modified: Wed, 14 Apr 2021 19:52:03 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:794c24fbbd979bf5af6af9630d7d9325aa6f01f668f4bca857204c5994c54b3a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41126204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a825e2fced0b53948b4f9e7bfc5d1609481cc108c2d60c1c6fd96b2643c9736a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:22:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 19:22:51 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 19:22:52 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 19:22:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 19:22:56 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 19:23:03 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 19:23:06 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 19:23:09 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:23:10 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 19:23:11 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 19:23:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 19:23:13 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 19:23:14 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 19:23:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 19:23:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b96788e82b6af129f934f44e3be6e11bd50c5aa4aa7f153d5c23ccb0dc12cf`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:face225286cec8239bf7c33e3977ca020cbc18e6b8cd3865c520feb00357f466`  
		Last Modified: Wed, 14 Apr 2021 19:24:57 GMT  
		Size: 38.4 MB (38412219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fb33ef170a52b1969e77c98378e9677623a19a6c6c17b581a3b345a3f9d387`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3befdfcaca0963f39f847c37604e9867e38aaca2fa8bbfde33c3515e22ec18`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b246d545ee670f4fd4a8233c1a1fb4233cba1d92c226cf5fad4566571d125075`  
		Last Modified: Wed, 14 Apr 2021 19:24:48 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:f7b2894fa2b2cce628874cb34c141e154a36af139a2ce7cf8ea879057ec1f36a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44978347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e6b7fa39b52e886a1bcecc2e7cca9076c09427848558ee7631e8b5a9a924e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 14 Apr 2021 18:55:36 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 14 Apr 2021 18:55:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 14 Apr 2021 18:55:37 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 14 Apr 2021 18:55:44 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 14 Apr 2021 18:55:45 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 14 Apr 2021 18:55:46 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 18:55:46 GMT
VOLUME [/consul/data]
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8300
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 14 Apr 2021 18:55:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 14 Apr 2021 18:55:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 14 Apr 2021 18:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 14 Apr 2021 18:55:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3831ff37459cebceaf36d2175d922fea9abe8aa2d956f29596fcce2b12cc90d`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edaf5d944668f1ce4efe25c8da04427ff173e57ba09ae72f16313fe5fd01d77b`  
		Last Modified: Wed, 14 Apr 2021 18:56:48 GMT  
		Size: 42.2 MB (42179261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f75e489a23c08e7c8d80a390517626ae20d9bc1900e38f640c3ceb3c452289`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9108803843267de412c0c6aa141a1d17bc55047f1b59d3602ce336005d6a81`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77f9b370fadecaa06e11cd41a1054987b24cf57a0b49c6b4d3f1c4a64928e40`  
		Last Modified: Wed, 14 Apr 2021 18:56:42 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
