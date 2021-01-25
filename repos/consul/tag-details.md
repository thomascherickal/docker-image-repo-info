<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.7`](#consul17)
-	[`consul:1.7.12`](#consul1712)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.8`](#consul188)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.2`](#consul192)
-	[`consul:latest`](#consullatest)

## `consul:1.7`

```console
$ docker pull consul@sha256:51ddb97b709ec18a85f28cb78d1c4e103fc587dc194a5cf82200e88e21212912
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:50439c535847f48f2342add5cf9aaaf016496e731eb3c4fb0c11709620509d6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43109101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe32aec0b0f038d08a7f84782312c88e6b7171c8a6f79685fb67a02cb0f4b5c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:24:04 GMT
ARG CONSUL_VERSION=1.7.12
# Mon, 25 Jan 2021 20:24:05 GMT
LABEL org.opencontainers.image.version=1.7.12
# Mon, 25 Jan 2021 20:24:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:24:06 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:24:51 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:24:52 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:24:53 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:24:53 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:24:53 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:24:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:24:54 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:24:54 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:24:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:24:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf7d2dee009868387b8b448e1725ed5731c55589fad6bfee448cec66ac4686f`  
		Last Modified: Mon, 25 Jan 2021 20:25:26 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a16589aaad004b5a97f0b9056b9ea8047356adc26383b3d981ca9baa9e09af`  
		Last Modified: Mon, 25 Jan 2021 20:25:32 GMT  
		Size: 40.3 MB (40306798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33b9fa1593d9007bd2f18b16eaac9f69f96091223e636a69816f773914adf4c`  
		Last Modified: Mon, 25 Jan 2021 20:25:26 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed4843ea8039966bb8a2cf3675f96efd773d51c34050618ebca5a0e3b16feeb`  
		Last Modified: Mon, 25 Jan 2021 20:25:26 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbbfb7dbebb8a330789e879a8e8939abb3cb349724be1056eeb9c929a87e46b`  
		Last Modified: Mon, 25 Jan 2021 20:25:26 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:51afa1fdf496c00db031287cd8af08c6b43cfd5666fc5e0d5b86a3b603438dfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38815714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3056e1aa63aa8fbe247a5dc7decc9c20eebf23a122ad3bc85288c6e260bcdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:53:34 GMT
ARG CONSUL_VERSION=1.7.12
# Mon, 25 Jan 2021 20:53:35 GMT
LABEL org.opencontainers.image.version=1.7.12
# Mon, 25 Jan 2021 20:53:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:53:37 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:53:45 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:53:47 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:53:49 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:53:50 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:53:50 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:53:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:53:52 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:53:52 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:53:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:53:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d7ac2ea51bd13bcdcb8bf35b5d3659154a068bb6466c08dc9725db0d08be55`  
		Last Modified: Mon, 25 Jan 2021 20:54:35 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a71a41b779a11e2e627356d87bf97ad04886489a4642840e01604170e71296`  
		Last Modified: Mon, 25 Jan 2021 20:54:45 GMT  
		Size: 36.2 MB (36208257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d654ff00f11118b4d81d8e9fbe5895683b4399f59c2196c1518fd581f70a7a4`  
		Last Modified: Mon, 25 Jan 2021 20:54:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a76c0c19bcef8b74865739203bc9ef980ab398632cfd85d1a50a5c79996d3`  
		Last Modified: Mon, 25 Jan 2021 20:54:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba8ba4f43a81aaebcd7acd20a2d0a30aeaf69c35d88f45756cd3dced0df1e0b`  
		Last Modified: Mon, 25 Jan 2021 20:54:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:3dd5414d3e357cee180a5d5b0b5ded59cbbe3f58d86ff2a896e60bece31e7748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39014250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee1e88e2e3c1204380983a5ab100cd4f77f157f3ff1c12050aad8bd971f5f26f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:45:03 GMT
ARG CONSUL_VERSION=1.7.12
# Mon, 25 Jan 2021 20:45:04 GMT
LABEL org.opencontainers.image.version=1.7.12
# Mon, 25 Jan 2021 20:45:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:45:06 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:45:13 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:45:15 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:45:17 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:45:17 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:45:18 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:45:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:45:19 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:45:20 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:45:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:45:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71edbaa7e2711d7dbfcc0d00dea8d2807b1556cd717f11c9b37bdf5b4e86c673`  
		Last Modified: Mon, 25 Jan 2021 20:46:00 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6022b28937fb8d2f674fd9f9a1e6a51cb2bda3e1a2a4abcf39efaae525d7908`  
		Last Modified: Mon, 25 Jan 2021 20:46:10 GMT  
		Size: 36.3 MB (36301907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba05ebb6019860c24b97bf6de882cf695de8c730555759cb8f20da0a68387448`  
		Last Modified: Mon, 25 Jan 2021 20:46:00 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909661f57a799173dfffe4bb2580cf6458fb64de26760462ec246193bc371fc2`  
		Last Modified: Mon, 25 Jan 2021 20:46:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dee198252988f3f04592790da2a3407c3fef07127517042ddabb05f95e796a4`  
		Last Modified: Mon, 25 Jan 2021 20:46:00 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:92e536fe5ed5a509dc811f4477395d14d24d9ecdfe969b6f36420cd9dcaa1e3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41906240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0647c945ad72ad85ddac82c55d20b2b1a6654a65b1b2c6d71c94cfa48b9228`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:39:19 GMT
ARG CONSUL_VERSION=1.7.12
# Mon, 25 Jan 2021 20:39:20 GMT
LABEL org.opencontainers.image.version=1.7.12
# Mon, 25 Jan 2021 20:39:20 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:39:21 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:39:27 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:39:28 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:39:29 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:39:29 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:39:29 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:39:29 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:39:30 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:39:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:39:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:39:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96c1a072a9a5756247b978c1d30715204575e6eba7b1ff88e79f677140727d`  
		Last Modified: Mon, 25 Jan 2021 20:40:08 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4f4261cf2fd9b211873bf3d884b42fd0d62522feb7384b0e23bae4a503ed4d`  
		Last Modified: Mon, 25 Jan 2021 20:40:15 GMT  
		Size: 39.1 MB (39108872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee4f6c10434d04698e504e5d5989ea46bc735bd442882c26d60486b5141f91`  
		Last Modified: Mon, 25 Jan 2021 20:40:08 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b86431373ca83887b6fd9a88665d91524b48b5bda24b5184b2785666dbc17e3`  
		Last Modified: Mon, 25 Jan 2021 20:40:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9900fbb3a1e6f50aeeb13ea2743bbef24c974738977935d231dd178fe5472313`  
		Last Modified: Mon, 25 Jan 2021 20:40:08 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.12`

```console
$ docker pull consul@sha256:51ddb97b709ec18a85f28cb78d1c4e103fc587dc194a5cf82200e88e21212912
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.12` - linux; amd64

```console
$ docker pull consul@sha256:50439c535847f48f2342add5cf9aaaf016496e731eb3c4fb0c11709620509d6c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43109101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe32aec0b0f038d08a7f84782312c88e6b7171c8a6f79685fb67a02cb0f4b5c4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:24:04 GMT
ARG CONSUL_VERSION=1.7.12
# Mon, 25 Jan 2021 20:24:05 GMT
LABEL org.opencontainers.image.version=1.7.12
# Mon, 25 Jan 2021 20:24:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:24:06 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:24:51 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:24:52 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:24:53 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:24:53 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:24:53 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:24:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:24:54 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:24:54 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:24:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:24:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf7d2dee009868387b8b448e1725ed5731c55589fad6bfee448cec66ac4686f`  
		Last Modified: Mon, 25 Jan 2021 20:25:26 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a16589aaad004b5a97f0b9056b9ea8047356adc26383b3d981ca9baa9e09af`  
		Last Modified: Mon, 25 Jan 2021 20:25:32 GMT  
		Size: 40.3 MB (40306798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33b9fa1593d9007bd2f18b16eaac9f69f96091223e636a69816f773914adf4c`  
		Last Modified: Mon, 25 Jan 2021 20:25:26 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed4843ea8039966bb8a2cf3675f96efd773d51c34050618ebca5a0e3b16feeb`  
		Last Modified: Mon, 25 Jan 2021 20:25:26 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbbfb7dbebb8a330789e879a8e8939abb3cb349724be1056eeb9c929a87e46b`  
		Last Modified: Mon, 25 Jan 2021 20:25:26 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.12` - linux; arm variant v6

```console
$ docker pull consul@sha256:51afa1fdf496c00db031287cd8af08c6b43cfd5666fc5e0d5b86a3b603438dfe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38815714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f3056e1aa63aa8fbe247a5dc7decc9c20eebf23a122ad3bc85288c6e260bcdd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:53:34 GMT
ARG CONSUL_VERSION=1.7.12
# Mon, 25 Jan 2021 20:53:35 GMT
LABEL org.opencontainers.image.version=1.7.12
# Mon, 25 Jan 2021 20:53:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:53:37 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:53:45 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:53:47 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:53:49 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:53:50 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:53:50 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:53:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:53:52 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:53:52 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:53:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:53:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d7ac2ea51bd13bcdcb8bf35b5d3659154a068bb6466c08dc9725db0d08be55`  
		Last Modified: Mon, 25 Jan 2021 20:54:35 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a71a41b779a11e2e627356d87bf97ad04886489a4642840e01604170e71296`  
		Last Modified: Mon, 25 Jan 2021 20:54:45 GMT  
		Size: 36.2 MB (36208257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d654ff00f11118b4d81d8e9fbe5895683b4399f59c2196c1518fd581f70a7a4`  
		Last Modified: Mon, 25 Jan 2021 20:54:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a76c0c19bcef8b74865739203bc9ef980ab398632cfd85d1a50a5c79996d3`  
		Last Modified: Mon, 25 Jan 2021 20:54:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba8ba4f43a81aaebcd7acd20a2d0a30aeaf69c35d88f45756cd3dced0df1e0b`  
		Last Modified: Mon, 25 Jan 2021 20:54:34 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.12` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:3dd5414d3e357cee180a5d5b0b5ded59cbbe3f58d86ff2a896e60bece31e7748
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39014250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee1e88e2e3c1204380983a5ab100cd4f77f157f3ff1c12050aad8bd971f5f26f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:45:03 GMT
ARG CONSUL_VERSION=1.7.12
# Mon, 25 Jan 2021 20:45:04 GMT
LABEL org.opencontainers.image.version=1.7.12
# Mon, 25 Jan 2021 20:45:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:45:06 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:45:13 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:45:15 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:45:17 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:45:17 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:45:18 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:45:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:45:19 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:45:20 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:45:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:45:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71edbaa7e2711d7dbfcc0d00dea8d2807b1556cd717f11c9b37bdf5b4e86c673`  
		Last Modified: Mon, 25 Jan 2021 20:46:00 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6022b28937fb8d2f674fd9f9a1e6a51cb2bda3e1a2a4abcf39efaae525d7908`  
		Last Modified: Mon, 25 Jan 2021 20:46:10 GMT  
		Size: 36.3 MB (36301907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba05ebb6019860c24b97bf6de882cf695de8c730555759cb8f20da0a68387448`  
		Last Modified: Mon, 25 Jan 2021 20:46:00 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909661f57a799173dfffe4bb2580cf6458fb64de26760462ec246193bc371fc2`  
		Last Modified: Mon, 25 Jan 2021 20:46:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dee198252988f3f04592790da2a3407c3fef07127517042ddabb05f95e796a4`  
		Last Modified: Mon, 25 Jan 2021 20:46:00 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.12` - linux; 386

```console
$ docker pull consul@sha256:92e536fe5ed5a509dc811f4477395d14d24d9ecdfe969b6f36420cd9dcaa1e3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41906240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd0647c945ad72ad85ddac82c55d20b2b1a6654a65b1b2c6d71c94cfa48b9228`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:39:19 GMT
ARG CONSUL_VERSION=1.7.12
# Mon, 25 Jan 2021 20:39:20 GMT
LABEL org.opencontainers.image.version=1.7.12
# Mon, 25 Jan 2021 20:39:20 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:39:21 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:39:27 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:39:28 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:39:29 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:39:29 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:39:29 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:39:29 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:39:30 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:39:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:39:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:39:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd96c1a072a9a5756247b978c1d30715204575e6eba7b1ff88e79f677140727d`  
		Last Modified: Mon, 25 Jan 2021 20:40:08 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4f4261cf2fd9b211873bf3d884b42fd0d62522feb7384b0e23bae4a503ed4d`  
		Last Modified: Mon, 25 Jan 2021 20:40:15 GMT  
		Size: 39.1 MB (39108872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ee4f6c10434d04698e504e5d5989ea46bc735bd442882c26d60486b5141f91`  
		Last Modified: Mon, 25 Jan 2021 20:40:08 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b86431373ca83887b6fd9a88665d91524b48b5bda24b5184b2785666dbc17e3`  
		Last Modified: Mon, 25 Jan 2021 20:40:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9900fbb3a1e6f50aeeb13ea2743bbef24c974738977935d231dd178fe5472313`  
		Last Modified: Mon, 25 Jan 2021 20:40:08 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:c5edd0c31e24e977ab491d95607eaf340f5075e8cf64582112c34022664464df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:80bb21c5855d4cd166e20a0772c4149ebede63942550e977d81b4f6f99d9552f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46505910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac338baca76a23a90dfc6e230ae0dc703a74023223a71da948fd9a4a378ed83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:23:50 GMT
ARG CONSUL_VERSION=1.8.8
# Mon, 25 Jan 2021 20:23:50 GMT
LABEL org.opencontainers.image.version=1.8.8
# Mon, 25 Jan 2021 20:23:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:23:51 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:23:57 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:23:58 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:23:59 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:23:59 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:23:59 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:23:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:23:59 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:24:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:24:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:24:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ab9c41b1e31fbc72c633729d4b69c88c30ad0683489eb4f2fad53ca97185a1`  
		Last Modified: Mon, 25 Jan 2021 20:25:12 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f7a91972d77f76f4ae16a66b19292f84eece8d9cfadc2d1dee0704dc604ac9`  
		Last Modified: Mon, 25 Jan 2021 20:25:19 GMT  
		Size: 43.7 MB (43703605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ca9d685cacebbe27a806e95e02c6b71b59c227d6117858be734ce5d1b007fa`  
		Last Modified: Mon, 25 Jan 2021 20:25:12 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255ba71969215e4615a01a0791c41c1e2967cb4b541149a563ddf8006cd49f33`  
		Last Modified: Mon, 25 Jan 2021 20:25:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac883b3d3e1b7306e1cfbaf383923b847bbf7fa0e6a3f8ba088120e357978f2d`  
		Last Modified: Mon, 25 Jan 2021 20:25:12 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:4a5921ae153c04cfa19e0e861daaeb17e1542c464d79209d15e08892c35a70ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41745171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e5207b5bd26a7bbcc3c1e6d048fbf8e543c439aa9d3e792ef8902a8eeab058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:53:07 GMT
ARG CONSUL_VERSION=1.8.8
# Mon, 25 Jan 2021 20:53:07 GMT
LABEL org.opencontainers.image.version=1.8.8
# Mon, 25 Jan 2021 20:53:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:53:10 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:53:19 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:53:21 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:53:22 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:53:23 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:53:23 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:53:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:53:25 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:53:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:53:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:53:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceafdbec34d90158018b6437340ca0f91196c0b9ccbce75e291d5566af8cc4ef`  
		Last Modified: Mon, 25 Jan 2021 20:54:17 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd8a4a5591a2a41cbd81643ecad0575a9bec05cb9f5f8508229e2e04675e1eb`  
		Last Modified: Mon, 25 Jan 2021 20:54:28 GMT  
		Size: 39.1 MB (39137710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d829b708d65aeb3715ec5f76b52dfef569fc93e9b090b8132556a198c29e63`  
		Last Modified: Mon, 25 Jan 2021 20:54:17 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4f8108cef6da2b219e4e6a390fe96a2d1496a08c47bd7d665460eadcc0eb50`  
		Last Modified: Mon, 25 Jan 2021 20:54:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c8035df1ad866d9d5aeb0cc353784e981f95de58626851fd93f3a1a37e8081`  
		Last Modified: Mon, 25 Jan 2021 20:54:18 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a38dedd646bc39eb737776832f79f5b9142cf4ca125a9ea9fa92e531c40f7851
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41925824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef627e9d90bf95113c67f7f5a70128ef09c2de0f66e44e56d0e64b45674c229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:44:36 GMT
ARG CONSUL_VERSION=1.8.8
# Mon, 25 Jan 2021 20:44:36 GMT
LABEL org.opencontainers.image.version=1.8.8
# Mon, 25 Jan 2021 20:44:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:44:39 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:44:45 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:44:47 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:44:49 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:44:50 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:44:51 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:44:52 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:44:52 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:44:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:44:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:44:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f58de96d8c5adae2483e134ca437fab696c00ea3aad0996258b92af82ddc73f`  
		Last Modified: Mon, 25 Jan 2021 20:45:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c23803397bc3770b83c77b2a13177d861e29b7f8074c3e496001f6983d4704`  
		Last Modified: Mon, 25 Jan 2021 20:45:52 GMT  
		Size: 39.2 MB (39213477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d53e7e0d05ccf30f7bc5f4396c47ae5ea5b44b3d4f66d09c21b77ca3a283158`  
		Last Modified: Mon, 25 Jan 2021 20:45:43 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b5608823b3ea48a8db3776ec5f5a96b2f26862e2b148c54123b263e4167151`  
		Last Modified: Mon, 25 Jan 2021 20:45:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f075c428cbc7fd7f37198c1b89bdc9a67bbfe41ef1759d22d0af9966188e8`  
		Last Modified: Mon, 25 Jan 2021 20:45:44 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:c339f960be249960830093ffdd1ec7ae133b99a3509a712fcd00132e2859752a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46004583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0acec72defb268603f1dcc9c80d0f5c0dd1ec262e7829183200bc0ba026a32c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:38:32 GMT
ARG CONSUL_VERSION=1.8.8
# Mon, 25 Jan 2021 20:38:32 GMT
LABEL org.opencontainers.image.version=1.8.8
# Mon, 25 Jan 2021 20:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:38:34 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:39:11 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:39:12 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:39:13 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:39:13 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:39:13 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:39:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:39:14 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:39:14 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:39:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95ca4b2e06c620c8cf4038e38efdda9a9e399c724768b29636080cb024fdde9`  
		Last Modified: Mon, 25 Jan 2021 20:39:51 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da2bbfdb7565df38ce8f1817e56da1145a5c8cb3935dc41f17db899de932844`  
		Last Modified: Mon, 25 Jan 2021 20:40:01 GMT  
		Size: 43.2 MB (43207215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdbeb14497a84a6e8de752b6313e54927f42d3e5df135b0eaeba4ce41ceb9e9`  
		Last Modified: Mon, 25 Jan 2021 20:39:51 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bbeabc044320ad2d286f774224baf0f73311ed19f128f8b0ef6710f944a51f`  
		Last Modified: Mon, 25 Jan 2021 20:39:51 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b35f26de1682bf170171fa8656779bcf2091e033539c4795783625afcd36522`  
		Last Modified: Mon, 25 Jan 2021 20:39:52 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.8`

```console
$ docker pull consul@sha256:c5edd0c31e24e977ab491d95607eaf340f5075e8cf64582112c34022664464df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.8` - linux; amd64

```console
$ docker pull consul@sha256:80bb21c5855d4cd166e20a0772c4149ebede63942550e977d81b4f6f99d9552f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46505910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac338baca76a23a90dfc6e230ae0dc703a74023223a71da948fd9a4a378ed83`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:23:50 GMT
ARG CONSUL_VERSION=1.8.8
# Mon, 25 Jan 2021 20:23:50 GMT
LABEL org.opencontainers.image.version=1.8.8
# Mon, 25 Jan 2021 20:23:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:23:51 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:23:57 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:23:58 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:23:59 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:23:59 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:23:59 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:23:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:23:59 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:24:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:24:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:24:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ab9c41b1e31fbc72c633729d4b69c88c30ad0683489eb4f2fad53ca97185a1`  
		Last Modified: Mon, 25 Jan 2021 20:25:12 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f7a91972d77f76f4ae16a66b19292f84eece8d9cfadc2d1dee0704dc604ac9`  
		Last Modified: Mon, 25 Jan 2021 20:25:19 GMT  
		Size: 43.7 MB (43703605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ca9d685cacebbe27a806e95e02c6b71b59c227d6117858be734ce5d1b007fa`  
		Last Modified: Mon, 25 Jan 2021 20:25:12 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255ba71969215e4615a01a0791c41c1e2967cb4b541149a563ddf8006cd49f33`  
		Last Modified: Mon, 25 Jan 2021 20:25:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac883b3d3e1b7306e1cfbaf383923b847bbf7fa0e6a3f8ba088120e357978f2d`  
		Last Modified: Mon, 25 Jan 2021 20:25:12 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:4a5921ae153c04cfa19e0e861daaeb17e1542c464d79209d15e08892c35a70ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41745171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e5207b5bd26a7bbcc3c1e6d048fbf8e543c439aa9d3e792ef8902a8eeab058`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:53:07 GMT
ARG CONSUL_VERSION=1.8.8
# Mon, 25 Jan 2021 20:53:07 GMT
LABEL org.opencontainers.image.version=1.8.8
# Mon, 25 Jan 2021 20:53:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:53:10 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:53:19 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:53:21 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:53:22 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:53:23 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:53:23 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:53:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:53:25 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:53:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:53:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:53:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceafdbec34d90158018b6437340ca0f91196c0b9ccbce75e291d5566af8cc4ef`  
		Last Modified: Mon, 25 Jan 2021 20:54:17 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd8a4a5591a2a41cbd81643ecad0575a9bec05cb9f5f8508229e2e04675e1eb`  
		Last Modified: Mon, 25 Jan 2021 20:54:28 GMT  
		Size: 39.1 MB (39137710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37d829b708d65aeb3715ec5f76b52dfef569fc93e9b090b8132556a198c29e63`  
		Last Modified: Mon, 25 Jan 2021 20:54:17 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4f8108cef6da2b219e4e6a390fe96a2d1496a08c47bd7d665460eadcc0eb50`  
		Last Modified: Mon, 25 Jan 2021 20:54:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c8035df1ad866d9d5aeb0cc353784e981f95de58626851fd93f3a1a37e8081`  
		Last Modified: Mon, 25 Jan 2021 20:54:18 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a38dedd646bc39eb737776832f79f5b9142cf4ca125a9ea9fa92e531c40f7851
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41925824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ef627e9d90bf95113c67f7f5a70128ef09c2de0f66e44e56d0e64b45674c229`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:44:36 GMT
ARG CONSUL_VERSION=1.8.8
# Mon, 25 Jan 2021 20:44:36 GMT
LABEL org.opencontainers.image.version=1.8.8
# Mon, 25 Jan 2021 20:44:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:44:39 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:44:45 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:44:47 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:44:49 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:44:50 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:44:51 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:44:52 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:44:52 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:44:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:44:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:44:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f58de96d8c5adae2483e134ca437fab696c00ea3aad0996258b92af82ddc73f`  
		Last Modified: Mon, 25 Jan 2021 20:45:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c23803397bc3770b83c77b2a13177d861e29b7f8074c3e496001f6983d4704`  
		Last Modified: Mon, 25 Jan 2021 20:45:52 GMT  
		Size: 39.2 MB (39213477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d53e7e0d05ccf30f7bc5f4396c47ae5ea5b44b3d4f66d09c21b77ca3a283158`  
		Last Modified: Mon, 25 Jan 2021 20:45:43 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b5608823b3ea48a8db3776ec5f5a96b2f26862e2b148c54123b263e4167151`  
		Last Modified: Mon, 25 Jan 2021 20:45:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0f075c428cbc7fd7f37198c1b89bdc9a67bbfe41ef1759d22d0af9966188e8`  
		Last Modified: Mon, 25 Jan 2021 20:45:44 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.8` - linux; 386

```console
$ docker pull consul@sha256:c339f960be249960830093ffdd1ec7ae133b99a3509a712fcd00132e2859752a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46004583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0acec72defb268603f1dcc9c80d0f5c0dd1ec262e7829183200bc0ba026a32c1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 25 Jan 2021 20:38:32 GMT
ARG CONSUL_VERSION=1.8.8
# Mon, 25 Jan 2021 20:38:32 GMT
LABEL org.opencontainers.image.version=1.8.8
# Mon, 25 Jan 2021 20:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 25 Jan 2021 20:38:34 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 25 Jan 2021 20:39:11 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 25 Jan 2021 20:39:12 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 25 Jan 2021 20:39:13 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 25 Jan 2021 20:39:13 GMT
VOLUME [/consul/data]
# Mon, 25 Jan 2021 20:39:13 GMT
EXPOSE 8300
# Mon, 25 Jan 2021 20:39:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 25 Jan 2021 20:39:14 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 25 Jan 2021 20:39:14 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jan 2021 20:39:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jan 2021 20:39:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95ca4b2e06c620c8cf4038e38efdda9a9e399c724768b29636080cb024fdde9`  
		Last Modified: Mon, 25 Jan 2021 20:39:51 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da2bbfdb7565df38ce8f1817e56da1145a5c8cb3935dc41f17db899de932844`  
		Last Modified: Mon, 25 Jan 2021 20:40:01 GMT  
		Size: 43.2 MB (43207215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdbeb14497a84a6e8de752b6313e54927f42d3e5df135b0eaeba4ce41ceb9e9`  
		Last Modified: Mon, 25 Jan 2021 20:39:51 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bbeabc044320ad2d286f774224baf0f73311ed19f128f8b0ef6710f944a51f`  
		Last Modified: Mon, 25 Jan 2021 20:39:51 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b35f26de1682bf170171fa8656779bcf2091e033539c4795783625afcd36522`  
		Last Modified: Mon, 25 Jan 2021 20:39:52 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:3b5c20f1ee6cb29741ec390cc4b3e50e02de0ead14b6ada5b1aa8461beb8e29a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:ef46003c8ca3069848803aafbc803b1a8ffcdcb97034cb34b5f4c4254b2505ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45598321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e1bcefc0b32c32a7ece6d078449b12f9c54bd7c1347200df223210bd62405c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:33:50 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:33:52 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:33:57 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:33:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:33:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:33:59 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:34:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:34:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622eed43c213ca04b014ca29d4bd443d339b4ce1697945724870f3f3be81c18b`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063beacf31e763c209cc2be56ab26891df2de15419c483ccd90f4b1d81e0665c`  
		Last Modified: Fri, 22 Jan 2021 00:34:30 GMT  
		Size: 42.8 MB (42796017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2fca495ba473b83faec23d60822f22d3f2a08ced7024784cd9ef938c2d93b5`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed07e71d77a7a297e5cf3bf86ef8e802e9e730e1ffbbee7b9c5d7d93e5936284`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e475fda5e48743650615e434915ecbfb2e215386499fd5936f757b762b1a8299`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:09433ed5adc26846cadd9d07b88b6ca6995452488be29937b4018e00d07b3a2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40846565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a259b57b45460fbaaae246878625657976c75a381d0dbbf8dcca5e5595a3024f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 21 Jan 2021 21:52:56 GMT
ARG CONSUL_VERSION=1.9.2
# Thu, 21 Jan 2021 21:52:57 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 21 Jan 2021 21:52:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Jan 2021 21:53:01 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Jan 2021 21:55:13 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Jan 2021 21:55:18 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Jan 2021 21:55:21 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Jan 2021 21:55:22 GMT
VOLUME [/consul/data]
# Thu, 21 Jan 2021 21:55:23 GMT
EXPOSE 8300
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Jan 2021 21:55:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Jan 2021 21:55:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:55:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886bcad55540156824b7334ba6968f2e2aef5edbbdb7c99ce6778a138e5346`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5537d2ff2a79a77ac5c53d677805c1fb4688881a633541faac2a3c4591000b`  
		Last Modified: Thu, 21 Jan 2021 21:56:19 GMT  
		Size: 38.2 MB (38239103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38219ace88131be232012db73dfa3543d0cb585db03a36434b3bedec8de7e2f`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02356861ba79b91256c9d428795d7d6aae4f95f07bb09cde3a5ba9a743bf390`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c65106acd946ef239362e33bcabf1b5d9e6adce96283311e72c2f1a928c0f33`  
		Last Modified: Thu, 21 Jan 2021 21:56:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:15a1f0753281fde2cb63a501ba190a53aa2fcf9a90db0f0976bc4c9368cfbd35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41065234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac31a930562e08820ffa23c05e3d66c84579594d7cda5eea1107bb6dbc84ca16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 01:15:22 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 01:15:22 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 01:15:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 01:15:25 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 01:15:32 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 01:15:34 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 01:15:36 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 01:15:37 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 01:15:37 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 01:15:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 01:15:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 01:15:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 01:15:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 01:15:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bada9d8146f78d35ba9058649f1a743f8f8effe6da47ad7f3efdc994ba55bf41`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305af6dcc21c7e5f99fe3059c3f621802851d0a1293fd8c14740b20bb5b75366`  
		Last Modified: Fri, 22 Jan 2021 01:16:19 GMT  
		Size: 38.4 MB (38352892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dabffb835fa239e023fa6571b5b645ff51b1d40439107a11604e828e316016`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd7d264e592997cfd404dd063958d86c708c1ce911ffcfcdd34bbb6ec0e5e79`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81738446441aadb1fd34a5df891bf9aca96ae3f40a41bbe34347cae246f212e6`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:bbf964de59b46d6aa23a0f0abfeacf8d92d66ce0974edf11fa883fd93d5bd05b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44918842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97373824e761cbabe5bb17cedd6494eebab31799e05d0cbea58aba0fe1b5a053`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:00:45 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:00:46 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:00:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:01:00 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:01:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:01:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a28b498a655e5f63890364a4aa4a6fa70282b3986dd0b8034ff978a8df9aebf`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc789b9b6618677a18b9813121f06f9537a1daf5ff84893bedf1a309edf4b96`  
		Last Modified: Fri, 22 Jan 2021 00:01:37 GMT  
		Size: 42.1 MB (42121475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d93e16ee5f3a25d893087303645ad2d1921100f838b7de5176e4ca260ae6ccc`  
		Last Modified: Fri, 22 Jan 2021 00:01:28 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291d8059ab881bb3fede51f0f18655ab4d0957d84c57d6b69d51d69582ab4c8e`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afdaec594273374dd2b6213921b5234defa2b8a3945b484db4e6863f2167968`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.2`

```console
$ docker pull consul@sha256:3b5c20f1ee6cb29741ec390cc4b3e50e02de0ead14b6ada5b1aa8461beb8e29a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.2` - linux; amd64

```console
$ docker pull consul@sha256:ef46003c8ca3069848803aafbc803b1a8ffcdcb97034cb34b5f4c4254b2505ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45598321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e1bcefc0b32c32a7ece6d078449b12f9c54bd7c1347200df223210bd62405c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:33:50 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:33:52 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:33:57 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:33:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:33:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:33:59 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:34:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:34:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622eed43c213ca04b014ca29d4bd443d339b4ce1697945724870f3f3be81c18b`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063beacf31e763c209cc2be56ab26891df2de15419c483ccd90f4b1d81e0665c`  
		Last Modified: Fri, 22 Jan 2021 00:34:30 GMT  
		Size: 42.8 MB (42796017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2fca495ba473b83faec23d60822f22d3f2a08ced7024784cd9ef938c2d93b5`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed07e71d77a7a297e5cf3bf86ef8e802e9e730e1ffbbee7b9c5d7d93e5936284`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e475fda5e48743650615e434915ecbfb2e215386499fd5936f757b762b1a8299`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.2` - linux; arm variant v6

```console
$ docker pull consul@sha256:09433ed5adc26846cadd9d07b88b6ca6995452488be29937b4018e00d07b3a2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40846565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a259b57b45460fbaaae246878625657976c75a381d0dbbf8dcca5e5595a3024f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 21 Jan 2021 21:52:56 GMT
ARG CONSUL_VERSION=1.9.2
# Thu, 21 Jan 2021 21:52:57 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 21 Jan 2021 21:52:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Jan 2021 21:53:01 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Jan 2021 21:55:13 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Jan 2021 21:55:18 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Jan 2021 21:55:21 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Jan 2021 21:55:22 GMT
VOLUME [/consul/data]
# Thu, 21 Jan 2021 21:55:23 GMT
EXPOSE 8300
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Jan 2021 21:55:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Jan 2021 21:55:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:55:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886bcad55540156824b7334ba6968f2e2aef5edbbdb7c99ce6778a138e5346`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5537d2ff2a79a77ac5c53d677805c1fb4688881a633541faac2a3c4591000b`  
		Last Modified: Thu, 21 Jan 2021 21:56:19 GMT  
		Size: 38.2 MB (38239103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38219ace88131be232012db73dfa3543d0cb585db03a36434b3bedec8de7e2f`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02356861ba79b91256c9d428795d7d6aae4f95f07bb09cde3a5ba9a743bf390`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c65106acd946ef239362e33bcabf1b5d9e6adce96283311e72c2f1a928c0f33`  
		Last Modified: Thu, 21 Jan 2021 21:56:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:15a1f0753281fde2cb63a501ba190a53aa2fcf9a90db0f0976bc4c9368cfbd35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41065234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac31a930562e08820ffa23c05e3d66c84579594d7cda5eea1107bb6dbc84ca16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 01:15:22 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 01:15:22 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 01:15:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 01:15:25 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 01:15:32 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 01:15:34 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 01:15:36 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 01:15:37 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 01:15:37 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 01:15:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 01:15:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 01:15:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 01:15:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 01:15:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bada9d8146f78d35ba9058649f1a743f8f8effe6da47ad7f3efdc994ba55bf41`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305af6dcc21c7e5f99fe3059c3f621802851d0a1293fd8c14740b20bb5b75366`  
		Last Modified: Fri, 22 Jan 2021 01:16:19 GMT  
		Size: 38.4 MB (38352892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dabffb835fa239e023fa6571b5b645ff51b1d40439107a11604e828e316016`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd7d264e592997cfd404dd063958d86c708c1ce911ffcfcdd34bbb6ec0e5e79`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81738446441aadb1fd34a5df891bf9aca96ae3f40a41bbe34347cae246f212e6`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.2` - linux; 386

```console
$ docker pull consul@sha256:bbf964de59b46d6aa23a0f0abfeacf8d92d66ce0974edf11fa883fd93d5bd05b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44918842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97373824e761cbabe5bb17cedd6494eebab31799e05d0cbea58aba0fe1b5a053`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:00:45 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:00:46 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:00:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:01:00 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:01:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:01:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a28b498a655e5f63890364a4aa4a6fa70282b3986dd0b8034ff978a8df9aebf`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc789b9b6618677a18b9813121f06f9537a1daf5ff84893bedf1a309edf4b96`  
		Last Modified: Fri, 22 Jan 2021 00:01:37 GMT  
		Size: 42.1 MB (42121475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d93e16ee5f3a25d893087303645ad2d1921100f838b7de5176e4ca260ae6ccc`  
		Last Modified: Fri, 22 Jan 2021 00:01:28 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291d8059ab881bb3fede51f0f18655ab4d0957d84c57d6b69d51d69582ab4c8e`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afdaec594273374dd2b6213921b5234defa2b8a3945b484db4e6863f2167968`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:3b5c20f1ee6cb29741ec390cc4b3e50e02de0ead14b6ada5b1aa8461beb8e29a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:ef46003c8ca3069848803aafbc803b1a8ffcdcb97034cb34b5f4c4254b2505ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45598321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e1bcefc0b32c32a7ece6d078449b12f9c54bd7c1347200df223210bd62405c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 13:01:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:33:50 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:33:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:33:52 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:33:57 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:33:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:33:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:33:59 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:33:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:34:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:34:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:34:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622eed43c213ca04b014ca29d4bd443d339b4ce1697945724870f3f3be81c18b`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063beacf31e763c209cc2be56ab26891df2de15419c483ccd90f4b1d81e0665c`  
		Last Modified: Fri, 22 Jan 2021 00:34:30 GMT  
		Size: 42.8 MB (42796017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2fca495ba473b83faec23d60822f22d3f2a08ced7024784cd9ef938c2d93b5`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed07e71d77a7a297e5cf3bf86ef8e802e9e730e1ffbbee7b9c5d7d93e5936284`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e475fda5e48743650615e434915ecbfb2e215386499fd5936f757b762b1a8299`  
		Last Modified: Fri, 22 Jan 2021 00:34:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:09433ed5adc26846cadd9d07b88b6ca6995452488be29937b4018e00d07b3a2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40846565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a259b57b45460fbaaae246878625657976c75a381d0dbbf8dcca5e5595a3024f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:15:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 21 Jan 2021 21:52:56 GMT
ARG CONSUL_VERSION=1.9.2
# Thu, 21 Jan 2021 21:52:57 GMT
LABEL org.opencontainers.image.version=1.9.2
# Thu, 21 Jan 2021 21:52:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Jan 2021 21:53:01 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Jan 2021 21:55:13 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Jan 2021 21:55:18 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Jan 2021 21:55:21 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Jan 2021 21:55:22 GMT
VOLUME [/consul/data]
# Thu, 21 Jan 2021 21:55:23 GMT
EXPOSE 8300
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Jan 2021 21:55:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Jan 2021 21:55:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Jan 2021 21:55:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:55:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886bcad55540156824b7334ba6968f2e2aef5edbbdb7c99ce6778a138e5346`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5537d2ff2a79a77ac5c53d677805c1fb4688881a633541faac2a3c4591000b`  
		Last Modified: Thu, 21 Jan 2021 21:56:19 GMT  
		Size: 38.2 MB (38239103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38219ace88131be232012db73dfa3543d0cb585db03a36434b3bedec8de7e2f`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02356861ba79b91256c9d428795d7d6aae4f95f07bb09cde3a5ba9a743bf390`  
		Last Modified: Thu, 21 Jan 2021 21:56:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c65106acd946ef239362e33bcabf1b5d9e6adce96283311e72c2f1a928c0f33`  
		Last Modified: Thu, 21 Jan 2021 21:56:09 GMT  
		Size: 1.7 KB (1712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:15a1f0753281fde2cb63a501ba190a53aa2fcf9a90db0f0976bc4c9368cfbd35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41065234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac31a930562e08820ffa23c05e3d66c84579594d7cda5eea1107bb6dbc84ca16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 00:36:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 01:15:22 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 01:15:22 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 01:15:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 01:15:25 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 01:15:32 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 01:15:34 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 01:15:36 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 01:15:37 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 01:15:37 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 01:15:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 01:15:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 01:15:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 01:15:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 01:15:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bada9d8146f78d35ba9058649f1a743f8f8effe6da47ad7f3efdc994ba55bf41`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305af6dcc21c7e5f99fe3059c3f621802851d0a1293fd8c14740b20bb5b75366`  
		Last Modified: Fri, 22 Jan 2021 01:16:19 GMT  
		Size: 38.4 MB (38352892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dabffb835fa239e023fa6571b5b645ff51b1d40439107a11604e828e316016`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd7d264e592997cfd404dd063958d86c708c1ce911ffcfcdd34bbb6ec0e5e79`  
		Last Modified: Fri, 22 Jan 2021 01:16:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81738446441aadb1fd34a5df891bf9aca96ae3f40a41bbe34347cae246f212e6`  
		Last Modified: Fri, 22 Jan 2021 01:16:10 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:bbf964de59b46d6aa23a0f0abfeacf8d92d66ce0974edf11fa883fd93d5bd05b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44918842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97373824e761cbabe5bb17cedd6494eebab31799e05d0cbea58aba0fe1b5a053`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 01:24:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 22 Jan 2021 00:00:45 GMT
ARG CONSUL_VERSION=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
LABEL org.opencontainers.image.version=1.9.2
# Fri, 22 Jan 2021 00:00:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 Jan 2021 00:00:46 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 Jan 2021 00:00:58 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 Jan 2021 00:00:59 GMT
# ARGS: CONSUL_VERSION=1.9.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 Jan 2021 00:01:00 GMT
VOLUME [/consul/data]
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8300
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 Jan 2021 00:01:00 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 Jan 2021 00:01:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 Jan 2021 00:01:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 Jan 2021 00:01:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a28b498a655e5f63890364a4aa4a6fa70282b3986dd0b8034ff978a8df9aebf`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc789b9b6618677a18b9813121f06f9537a1daf5ff84893bedf1a309edf4b96`  
		Last Modified: Fri, 22 Jan 2021 00:01:37 GMT  
		Size: 42.1 MB (42121475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d93e16ee5f3a25d893087303645ad2d1921100f838b7de5176e4ca260ae6ccc`  
		Last Modified: Fri, 22 Jan 2021 00:01:28 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291d8059ab881bb3fede51f0f18655ab4d0957d84c57d6b69d51d69582ab4c8e`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afdaec594273374dd2b6213921b5234defa2b8a3945b484db4e6863f2167968`  
		Last Modified: Fri, 22 Jan 2021 00:01:26 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
