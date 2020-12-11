<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.6`](#consul16)
-	[`consul:1.6.10`](#consul1610)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.10`](#consul1710)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.6`](#consul186)
-	[`consul:1.8.7-beta1`](#consul187-beta1)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.0`](#consul190)
-	[`consul:latest`](#consullatest)

## `consul:1.6`

```console
$ docker pull consul@sha256:e2c784c7f9820a3c1ef58e79a58afb08be8111b62a287e576fd1fed4c022163f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6` - linux; amd64

```console
$ docker pull consul@sha256:dd84a400239d14d8f1778a2a2a8cacb129382c1527afb6be972eaff722d3ca5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44791257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f54a78fa9cfb1418f1991fdf3c70b3d43538183d39fb205fad04a48c8dbb2fe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 02:56:33 GMT
ENV CONSUL_VERSION=1.6.10
# Fri, 11 Dec 2020 02:56:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 02:56:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 02:56:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 02:56:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 02:56:45 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:56:45 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 02:56:46 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 02:56:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 02:56:46 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 02:56:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 02:56:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 02:56:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637e1a6d2f2eb8b86a1165b06157992ac04f4f487e63929224ba58831d2f1389`  
		Last Modified: Fri, 11 Dec 2020 02:58:10 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81380126608683d3f3e322217e25bf30a385a0d65377739de011d33578bb05c5`  
		Last Modified: Fri, 11 Dec 2020 02:58:18 GMT  
		Size: 42.0 MB (41991077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6e3a4d48893837760d565dec5302d5439662035f273c6747f288936b81544`  
		Last Modified: Fri, 11 Dec 2020 02:58:10 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301a486e7cfbb4be1077de6adb467923208f0ee9ac3118e19b0cead9103d2a3`  
		Last Modified: Fri, 11 Dec 2020 02:58:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0368ea3a8ac9d3a3bca026da11b96f9ec8ce28a1cbd81aaa14606b42f4681`  
		Last Modified: Fri, 11 Dec 2020 02:58:10 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:08144fc23ebb35123bf31b1f4cd9b8480d51edc0428f91af96599733440e13b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40231619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580318a60f5c5a81c54adf1080cab6b86ad202c6b166efbe11288155faed1d69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:14:42 GMT
ENV CONSUL_VERSION=1.6.10
# Fri, 11 Dec 2020 03:14:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:14:46 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:14:58 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:15:02 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:15:04 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:15:05 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:15:06 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:15:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:15:08 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:15:09 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:15:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:15:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0718992863a38eff7e646240eba13de8a3fcaa1efdda46b5ddb354e4811fee72`  
		Last Modified: Fri, 11 Dec 2020 03:16:46 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aba9c95278ad90efba337bb3b2517be6de7c1a562b810c7db8f0c64183da62`  
		Last Modified: Fri, 11 Dec 2020 03:16:54 GMT  
		Size: 37.6 MB (37626335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59197aacf91a6d9a2e9eab91f55748287fff34b5b7815754b261c20e72f9be5e`  
		Last Modified: Fri, 11 Dec 2020 03:16:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10ee0507ad984cd367d13a7777508a41b0077a2714abc2fea8875c11f39d0f`  
		Last Modified: Fri, 11 Dec 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5c945e42d349beea8e3e516c617602c21918b7d64924a019662a89e7d4c36b`  
		Last Modified: Fri, 11 Dec 2020 03:16:46 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:3a8df1a5bbb62756eb7787e19a8bc91603c1c09c93e83a6c37023db7ecad39d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40657636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800c5738cca306f8ee3b656eafa5c35175cca948718b61d12b71ed60f4bb32af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:38:55 GMT
ENV CONSUL_VERSION=1.6.10
# Fri, 11 Dec 2020 03:38:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:39:04 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:39:15 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:39:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:39:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:39:24 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:39:25 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:39:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:39:27 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:39:29 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:39:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:39:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e32a216fda52017d6e8737e8177ec5bb404c7e11bc8303a8090293726ae608`  
		Last Modified: Fri, 11 Dec 2020 03:41:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73c806abc5f5dbdb978860c0c874efac30636f3f1d84374dde7b1ae6fa2d05`  
		Last Modified: Fri, 11 Dec 2020 03:41:24 GMT  
		Size: 37.9 MB (37947721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be564d87fc2f75718e0dfa1d776ef8342e6f7928823d8795876ad04615d57ff`  
		Last Modified: Fri, 11 Dec 2020 03:41:15 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4796e39541c40a09ef84f81f36837a2ed4acace309e55171abe84237d411b45d`  
		Last Modified: Fri, 11 Dec 2020 03:41:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc86a93610092db507491d707cfadcf26b64b6dfd5d2e0d67fb7923d0d4b1e88`  
		Last Modified: Fri, 11 Dec 2020 03:41:15 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; 386

```console
$ docker pull consul@sha256:4e0f5cacbf900e90e3aab47c6dd8f07d057a792e7f45aae0236f27d2fbb33ab4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43952807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:044965116ab4acbbd2bf8bfc28c6b639f9481aad24c9de88722e24bbd3b75b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:39:11 GMT
ENV CONSUL_VERSION=1.6.10
# Sat, 21 Nov 2020 01:39:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:39:12 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:39:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:39:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:39:20 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:39:20 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:39:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:39:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:39:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073955cd82a1400897e9e8c0f871d7b3382f2bd068abd5e4523ff14758e2e908`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3020e8d98304dd9177e08ba742685d53a076f9807fd4ef84a1f3109abaf2e`  
		Last Modified: Sat, 21 Nov 2020 01:40:14 GMT  
		Size: 41.2 MB (41158168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e881d4d393cffbf1679126019e5c1dabe5ed7875a78005f7b2570cce62c46ae`  
		Last Modified: Sat, 21 Nov 2020 01:40:04 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819b2209f9062b82406066a16ac9005018f448a0c1bc06f426c031f864b05ebd`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b2426aa309c8071a39df0069984a071114bb3777032933745d60603f0a5fea`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6.10`

```console
$ docker pull consul@sha256:e2c784c7f9820a3c1ef58e79a58afb08be8111b62a287e576fd1fed4c022163f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6.10` - linux; amd64

```console
$ docker pull consul@sha256:dd84a400239d14d8f1778a2a2a8cacb129382c1527afb6be972eaff722d3ca5e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.8 MB (44791257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f54a78fa9cfb1418f1991fdf3c70b3d43538183d39fb205fad04a48c8dbb2fe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 02:56:33 GMT
ENV CONSUL_VERSION=1.6.10
# Fri, 11 Dec 2020 02:56:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 02:56:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 02:56:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 02:56:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 02:56:45 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:56:45 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 02:56:46 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 02:56:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 02:56:46 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 02:56:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 02:56:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 02:56:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637e1a6d2f2eb8b86a1165b06157992ac04f4f487e63929224ba58831d2f1389`  
		Last Modified: Fri, 11 Dec 2020 02:58:10 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81380126608683d3f3e322217e25bf30a385a0d65377739de011d33578bb05c5`  
		Last Modified: Fri, 11 Dec 2020 02:58:18 GMT  
		Size: 42.0 MB (41991077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6e3a4d48893837760d565dec5302d5439662035f273c6747f288936b81544`  
		Last Modified: Fri, 11 Dec 2020 02:58:10 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8301a486e7cfbb4be1077de6adb467923208f0ee9ac3118e19b0cead9103d2a3`  
		Last Modified: Fri, 11 Dec 2020 02:58:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b0368ea3a8ac9d3a3bca026da11b96f9ec8ce28a1cbd81aaa14606b42f4681`  
		Last Modified: Fri, 11 Dec 2020 02:58:10 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:08144fc23ebb35123bf31b1f4cd9b8480d51edc0428f91af96599733440e13b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40231619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:580318a60f5c5a81c54adf1080cab6b86ad202c6b166efbe11288155faed1d69`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:14:42 GMT
ENV CONSUL_VERSION=1.6.10
# Fri, 11 Dec 2020 03:14:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:14:46 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:14:58 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:15:02 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:15:04 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:15:05 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:15:06 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:15:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:15:08 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:15:09 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:15:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:15:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0718992863a38eff7e646240eba13de8a3fcaa1efdda46b5ddb354e4811fee72`  
		Last Modified: Fri, 11 Dec 2020 03:16:46 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0aba9c95278ad90efba337bb3b2517be6de7c1a562b810c7db8f0c64183da62`  
		Last Modified: Fri, 11 Dec 2020 03:16:54 GMT  
		Size: 37.6 MB (37626335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59197aacf91a6d9a2e9eab91f55748287fff34b5b7815754b261c20e72f9be5e`  
		Last Modified: Fri, 11 Dec 2020 03:16:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10ee0507ad984cd367d13a7777508a41b0077a2714abc2fea8875c11f39d0f`  
		Last Modified: Fri, 11 Dec 2020 03:16:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5c945e42d349beea8e3e516c617602c21918b7d64924a019662a89e7d4c36b`  
		Last Modified: Fri, 11 Dec 2020 03:16:46 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:3a8df1a5bbb62756eb7787e19a8bc91603c1c09c93e83a6c37023db7ecad39d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40657636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800c5738cca306f8ee3b656eafa5c35175cca948718b61d12b71ed60f4bb32af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:38:55 GMT
ENV CONSUL_VERSION=1.6.10
# Fri, 11 Dec 2020 03:38:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:39:04 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:39:15 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:39:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:39:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:39:24 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:39:25 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:39:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:39:27 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:39:29 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:39:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:39:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e32a216fda52017d6e8737e8177ec5bb404c7e11bc8303a8090293726ae608`  
		Last Modified: Fri, 11 Dec 2020 03:41:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e73c806abc5f5dbdb978860c0c874efac30636f3f1d84374dde7b1ae6fa2d05`  
		Last Modified: Fri, 11 Dec 2020 03:41:24 GMT  
		Size: 37.9 MB (37947721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be564d87fc2f75718e0dfa1d776ef8342e6f7928823d8795876ad04615d57ff`  
		Last Modified: Fri, 11 Dec 2020 03:41:15 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4796e39541c40a09ef84f81f36837a2ed4acace309e55171abe84237d411b45d`  
		Last Modified: Fri, 11 Dec 2020 03:41:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc86a93610092db507491d707cfadcf26b64b6dfd5d2e0d67fb7923d0d4b1e88`  
		Last Modified: Fri, 11 Dec 2020 03:41:15 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.10` - linux; 386

```console
$ docker pull consul@sha256:4e0f5cacbf900e90e3aab47c6dd8f07d057a792e7f45aae0236f27d2fbb33ab4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43952807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:044965116ab4acbbd2bf8bfc28c6b639f9481aad24c9de88722e24bbd3b75b35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:39:11 GMT
ENV CONSUL_VERSION=1.6.10
# Sat, 21 Nov 2020 01:39:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:39:12 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:39:19 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     apk -X https://dl-cdn.alpinelinux.org/alpine/v3.8/main add tzdata=2020a-r0 &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:39:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:39:20 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:39:20 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:39:21 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:39:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:39:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:39:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073955cd82a1400897e9e8c0f871d7b3382f2bd068abd5e4523ff14758e2e908`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c3020e8d98304dd9177e08ba742685d53a076f9807fd4ef84a1f3109abaf2e`  
		Last Modified: Sat, 21 Nov 2020 01:40:14 GMT  
		Size: 41.2 MB (41158168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e881d4d393cffbf1679126019e5c1dabe5ed7875a78005f7b2570cce62c46ae`  
		Last Modified: Sat, 21 Nov 2020 01:40:04 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819b2209f9062b82406066a16ac9005018f448a0c1bc06f426c031f864b05ebd`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b2426aa309c8071a39df0069984a071114bb3777032933745d60603f0a5fea`  
		Last Modified: Sat, 21 Nov 2020 01:40:05 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7`

```console
$ docker pull consul@sha256:631063933e4960c45c9cb007ca5b7e0b1e8dad961f27697f9308dab94931646b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:bc16b5304bdcc40a3cea9f6c106363434717586467744d1ce78b2e63a1e5dc6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43093842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60bd34dbc3c3f1f7f4b43cd12ed01b4015baa93ac1392d2b07a12689c6254721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 02:56:13 GMT
ENV CONSUL_VERSION=1.7.10
# Fri, 11 Dec 2020 02:56:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 02:56:15 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 02:56:22 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 02:56:24 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 02:56:25 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:56:25 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 02:56:25 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 02:56:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 02:56:26 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 02:56:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 02:56:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 02:56:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574c36a12202c0f0e34f4b8bf84ddde9f9a0924c19895a461058527f3a0a2cdd`  
		Last Modified: Fri, 11 Dec 2020 02:57:55 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855f7e506d7ddff6882d7974e8eb68c3505d7c723ad5698323743bd64fcd902`  
		Last Modified: Fri, 11 Dec 2020 02:58:04 GMT  
		Size: 40.3 MB (40293661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1238aa95aaba6e5cdc6775497bf004a2e4228df6c8da4e7b2bfa7ef9c4f794`  
		Last Modified: Fri, 11 Dec 2020 02:57:55 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b6c78cc972e1067d1fd8489942639d41f191f3905fc0ce3a2e7130aac3d1be`  
		Last Modified: Fri, 11 Dec 2020 02:57:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02172411f977cfe47523404a06fd5b7b3d3cda3780e621ca6740a4431d8e236`  
		Last Modified: Fri, 11 Dec 2020 02:57:54 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:022280ea5f9d5ab7bc43441c003a7f9eeeb47ec39dfb81d281047139b3b138cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38808868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514032a7eb0f6c19309d94691b68f6d41e135f5c6c86cbd789219bc24ca7f0c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:14:03 GMT
ENV CONSUL_VERSION=1.7.10
# Fri, 11 Dec 2020 03:14:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:14:07 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:14:20 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:14:23 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:14:26 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:14:28 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:14:29 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:14:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:14:31 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:14:31 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:14:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:14:33 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51852c5441a1739bfd2fd44d72a137049d91ef2f49859b5fccc8759ba0cb1bf2`  
		Last Modified: Fri, 11 Dec 2020 03:16:28 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa8f2bb5e3abfd423e07b0274446bad10a00fb8fd9b8320a51453de05ca4b29`  
		Last Modified: Fri, 11 Dec 2020 03:16:36 GMT  
		Size: 36.2 MB (36203579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed119e91f77258272fcc9f00e6ee4a59d027f2f488222190b9e7ee746b7363ad`  
		Last Modified: Fri, 11 Dec 2020 03:16:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0e736e249123fde558821ed3d7ef19280c9f09a9c7b74fd2fc820443aecb8b`  
		Last Modified: Fri, 11 Dec 2020 03:16:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ce1b2809985eaa734d3cec1c396b39161405e05ff4c03bc841d28c82ea1829`  
		Last Modified: Fri, 11 Dec 2020 03:16:27 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:d19d2d22f75ba5599004ee57264cf9a4e071be9ab1f851af21481f08a34c3b3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39022273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d05b0d436c2b47ec1af64dc47df0586bbda55bfecd4b6837abbf39805b7ff3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:38:12 GMT
ENV CONSUL_VERSION=1.7.10
# Fri, 11 Dec 2020 03:38:13 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:38:18 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:38:27 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:38:32 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:38:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:38:38 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:38:39 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:38:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:38:43 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:38:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:38:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:38:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa364485c4dcfa8c805b53954ed13ed2bb898bd74c46ab466b19390625e5558a`  
		Last Modified: Fri, 11 Dec 2020 03:40:58 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0402de5324fafc277321623fb0c59a46777b22c85b4bfc0450ae9addeda26bae`  
		Last Modified: Fri, 11 Dec 2020 03:41:06 GMT  
		Size: 36.3 MB (36312361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789221dee44f58800ceb933315f12ef86eba5cc319892c5946452f14de5b9d52`  
		Last Modified: Fri, 11 Dec 2020 03:40:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e5f481fcc0adfae657dd6760bcb27bbff836c1a2303ccaa0c97052d2d5b05e`  
		Last Modified: Fri, 11 Dec 2020 03:40:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d525323bafec8cd9371bb3c74361299642ca0eb785c395f66d689b9b3b123059`  
		Last Modified: Fri, 11 Dec 2020 03:40:58 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:9060331ac68bc5b49ca118d89b3de037f26d930318384931d8ddae9fdac3689a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42273476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5388bbbe3074d5368f55e8be06633a0207adc15d8b1ed956b25f4932e74d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:38:55 GMT
ENV CONSUL_VERSION=1.7.10
# Sat, 21 Nov 2020 01:38:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:38:56 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:39:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:39:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:39:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:39:05 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:39:05 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:39:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:39:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:39:06 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:39:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9d9e88674a9ee11182151110497f18d229130a39fa8c6afa877d3f68d7211`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c3807ca6a52a3d92cceb7f8c1c3ecd3a0e3bebfcf603fc0e1f18ab493350b3`  
		Last Modified: Sat, 21 Nov 2020 01:40:00 GMT  
		Size: 39.5 MB (39478832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f655fb0d3f657436baef11ac6955a8e4d91c3f95bc563042c8e3ee4a83dca2f`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8581f6b37196be59e34bc65d25f14344d505b62347fd78de5598bffac35f0c0`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b6f208b77ae07b8b434483ec34c407e10c1b89b132f816cae1a8d498c9fb92`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.10`

```console
$ docker pull consul@sha256:631063933e4960c45c9cb007ca5b7e0b1e8dad961f27697f9308dab94931646b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.10` - linux; amd64

```console
$ docker pull consul@sha256:bc16b5304bdcc40a3cea9f6c106363434717586467744d1ce78b2e63a1e5dc6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43093842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60bd34dbc3c3f1f7f4b43cd12ed01b4015baa93ac1392d2b07a12689c6254721`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 02:56:13 GMT
ENV CONSUL_VERSION=1.7.10
# Fri, 11 Dec 2020 02:56:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 02:56:15 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 02:56:22 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 02:56:24 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 02:56:25 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:56:25 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 02:56:25 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 02:56:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 02:56:26 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 02:56:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 02:56:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 02:56:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574c36a12202c0f0e34f4b8bf84ddde9f9a0924c19895a461058527f3a0a2cdd`  
		Last Modified: Fri, 11 Dec 2020 02:57:55 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0855f7e506d7ddff6882d7974e8eb68c3505d7c723ad5698323743bd64fcd902`  
		Last Modified: Fri, 11 Dec 2020 02:58:04 GMT  
		Size: 40.3 MB (40293661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1238aa95aaba6e5cdc6775497bf004a2e4228df6c8da4e7b2bfa7ef9c4f794`  
		Last Modified: Fri, 11 Dec 2020 02:57:55 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b6c78cc972e1067d1fd8489942639d41f191f3905fc0ce3a2e7130aac3d1be`  
		Last Modified: Fri, 11 Dec 2020 02:57:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02172411f977cfe47523404a06fd5b7b3d3cda3780e621ca6740a4431d8e236`  
		Last Modified: Fri, 11 Dec 2020 02:57:54 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:022280ea5f9d5ab7bc43441c003a7f9eeeb47ec39dfb81d281047139b3b138cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38808868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:514032a7eb0f6c19309d94691b68f6d41e135f5c6c86cbd789219bc24ca7f0c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:14:03 GMT
ENV CONSUL_VERSION=1.7.10
# Fri, 11 Dec 2020 03:14:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:14:07 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:14:20 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:14:23 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:14:26 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:14:28 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:14:29 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:14:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:14:31 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:14:31 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:14:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:14:33 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51852c5441a1739bfd2fd44d72a137049d91ef2f49859b5fccc8759ba0cb1bf2`  
		Last Modified: Fri, 11 Dec 2020 03:16:28 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa8f2bb5e3abfd423e07b0274446bad10a00fb8fd9b8320a51453de05ca4b29`  
		Last Modified: Fri, 11 Dec 2020 03:16:36 GMT  
		Size: 36.2 MB (36203579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed119e91f77258272fcc9f00e6ee4a59d027f2f488222190b9e7ee746b7363ad`  
		Last Modified: Fri, 11 Dec 2020 03:16:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0e736e249123fde558821ed3d7ef19280c9f09a9c7b74fd2fc820443aecb8b`  
		Last Modified: Fri, 11 Dec 2020 03:16:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ce1b2809985eaa734d3cec1c396b39161405e05ff4c03bc841d28c82ea1829`  
		Last Modified: Fri, 11 Dec 2020 03:16:27 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:d19d2d22f75ba5599004ee57264cf9a4e071be9ab1f851af21481f08a34c3b3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39022273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d05b0d436c2b47ec1af64dc47df0586bbda55bfecd4b6837abbf39805b7ff3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:38:12 GMT
ENV CONSUL_VERSION=1.7.10
# Fri, 11 Dec 2020 03:38:13 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:38:18 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:38:27 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:38:32 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:38:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:38:38 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:38:39 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:38:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:38:43 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:38:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:38:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:38:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa364485c4dcfa8c805b53954ed13ed2bb898bd74c46ab466b19390625e5558a`  
		Last Modified: Fri, 11 Dec 2020 03:40:58 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0402de5324fafc277321623fb0c59a46777b22c85b4bfc0450ae9addeda26bae`  
		Last Modified: Fri, 11 Dec 2020 03:41:06 GMT  
		Size: 36.3 MB (36312361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789221dee44f58800ceb933315f12ef86eba5cc319892c5946452f14de5b9d52`  
		Last Modified: Fri, 11 Dec 2020 03:40:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e5f481fcc0adfae657dd6760bcb27bbff836c1a2303ccaa0c97052d2d5b05e`  
		Last Modified: Fri, 11 Dec 2020 03:40:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d525323bafec8cd9371bb3c74361299642ca0eb785c395f66d689b9b3b123059`  
		Last Modified: Fri, 11 Dec 2020 03:40:58 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.10` - linux; 386

```console
$ docker pull consul@sha256:9060331ac68bc5b49ca118d89b3de037f26d930318384931d8ddae9fdac3689a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42273476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5388bbbe3074d5368f55e8be06633a0207adc15d8b1ed956b25f4932e74d47d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:38:55 GMT
ENV CONSUL_VERSION=1.7.10
# Sat, 21 Nov 2020 01:38:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:38:56 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:39:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:39:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:39:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:39:05 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:39:05 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:39:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:39:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:39:06 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:39:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:39:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad9d9e88674a9ee11182151110497f18d229130a39fa8c6afa877d3f68d7211`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c3807ca6a52a3d92cceb7f8c1c3ecd3a0e3bebfcf603fc0e1f18ab493350b3`  
		Last Modified: Sat, 21 Nov 2020 01:40:00 GMT  
		Size: 39.5 MB (39478832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f655fb0d3f657436baef11ac6955a8e4d91c3f95bc563042c8e3ee4a83dca2f`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8581f6b37196be59e34bc65d25f14344d505b62347fd78de5598bffac35f0c0`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b6f208b77ae07b8b434483ec34c407e10c1b89b132f816cae1a8d498c9fb92`  
		Last Modified: Sat, 21 Nov 2020 01:39:49 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:7ebdaffada0a218c3ce7b048f0f248a323b807851346a891c615c47978be5086
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:3efabf42b246dae092b236df440d95b25cc79f08941128653fbb490d8068f779
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46461787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36094c09e82962f378f08056864385d0ac1a28ef278b9050423de34b6bd2d07d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 02:55:54 GMT
ENV CONSUL_VERSION=1.8.6
# Fri, 11 Dec 2020 02:55:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 02:55:56 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 02:56:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 02:56:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 02:56:06 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:56:06 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 02:56:06 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 02:56:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 02:56:07 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 02:56:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 02:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 02:56:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe56e704066b43589bb857c9465831a2c34bbbef933b423569c4afe1f8511e3`  
		Last Modified: Fri, 11 Dec 2020 02:57:37 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7854da3823fa235c4710a7558b08efd96290dd80cf0c0252c3100b83f264dfc5`  
		Last Modified: Fri, 11 Dec 2020 02:57:47 GMT  
		Size: 43.7 MB (43661611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b68bd84e508f434ab57fdd39663b88c3e9541e86b01051eb13f41e02049edaa`  
		Last Modified: Fri, 11 Dec 2020 02:57:38 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8494b9fb8d1cc1a0ce36ca17d71f50be0eeb0a299ac3fa836fc54beb2a75e4d`  
		Last Modified: Fri, 11 Dec 2020 02:57:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cce9eef4f2ebc00b962a237fa3e9451a52b28d2d744e48f2ee9d751b4c8d2f0`  
		Last Modified: Fri, 11 Dec 2020 02:57:38 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:334c9f2ed9393ebc322ab707ba05cee30bc7a690df78068fd0910dff150a9af7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41725636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d11e41fbb7db9ecd01e17397ecb9a0b54af9d8d3ffd6cbd5d96bf7b6a7523f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:13:28 GMT
ENV CONSUL_VERSION=1.8.6
# Fri, 11 Dec 2020 03:13:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:13:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:13:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:13:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:13:48 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:13:49 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:13:50 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:13:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:13:52 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:13:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:13:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:13:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae25b06630113a08cb483831556b1c93e2e387a7264fd435f74fa915b7a54a`  
		Last Modified: Fri, 11 Dec 2020 03:16:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47dcb10ad021b2d7f6a18a72b36b488fe9c839e87a9060a87491e9488a5202ba`  
		Last Modified: Fri, 11 Dec 2020 03:16:19 GMT  
		Size: 39.1 MB (39120349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fcb09bf0d7f29af2781bd98bfe0129ca27fa185edd8fae7c7eff1ad6387ade9`  
		Last Modified: Fri, 11 Dec 2020 03:16:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553aab41258e4b942d2fce34957758217f83453925a5fc6a7875f979b7be046`  
		Last Modified: Fri, 11 Dec 2020 03:16:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0062f04ae06c86fb1f067e692d3db0ae1dd552a24c8de44815a849651e419f1c`  
		Last Modified: Fri, 11 Dec 2020 03:16:10 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:ef535790a37e1a99a3d4aebf16a4a5de63f0edacfbdfe6e94bc33acabc1f8c6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41889047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b86702540ec5974ba3a9331a3bc43d021879b0e250694befe4620f3a767b8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:37:28 GMT
ENV CONSUL_VERSION=1.8.6
# Fri, 11 Dec 2020 03:37:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:37:33 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:37:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:37:47 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:37:51 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:37:52 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:37:53 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:37:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:37:56 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:37:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:37:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:37:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f305a28acd173642e8f85c5a1d7f56660ecf7ecd7f0fba73c93b92f2795383b2`  
		Last Modified: Fri, 11 Dec 2020 03:40:38 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01430bb70cd5ef6ffe24b0dcf1079161ad1ff97f395db99b7f62af4771a64d74`  
		Last Modified: Fri, 11 Dec 2020 03:40:49 GMT  
		Size: 39.2 MB (39179135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60eb63112da8eabf1e578e9e39df003a047d01916928b6f384e316609a36e9a9`  
		Last Modified: Fri, 11 Dec 2020 03:40:39 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f966963dd48ffa314bbc482ded77806b13d5c2de847e24ca3f0b578ab5cac7b`  
		Last Modified: Fri, 11 Dec 2020 03:40:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42e1fca3eb7b391c4a4384c639cc4213c0dfeb2459db70aa98bfc219cafc78f`  
		Last Modified: Fri, 11 Dec 2020 03:40:39 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:84ae85b48c8d01fce5cc0e9a6e90e9f8afcf43489c397a86af1094e1edcbb979
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46352079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:138cc84a33f3f503a4f09b51b0c3e2ed7fe7f7d6fb2a0a76dc1aed4a30c4c2e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:38:31 GMT
ENV CONSUL_VERSION=1.8.6
# Sat, 21 Nov 2020 01:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:38:33 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:38:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:38:42 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:38:44 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:38:44 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:38:44 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:38:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:38:45 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:38:45 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:38:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:38:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f7ea6bb49fcd83fa1e2532a46fa73673811b4f190eabbeac27b70126e99483`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5b10ad85a8ca78f92681700a4adf4286665337db08649aade4832e289c1b1`  
		Last Modified: Sat, 21 Nov 2020 01:39:42 GMT  
		Size: 43.6 MB (43557436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc233fbc0a691dfc0d0d6632924d73a80241aace4095d2562084aada2f889003`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b2f813151022af8a8d729fd038d6d97deeb7edf8cda7cd53b6d584074f09d`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fb85334aeb38ba47abe71d6bafa659b496f04bb6b2195305ef4dcafbe7929e`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.6`

```console
$ docker pull consul@sha256:7ebdaffada0a218c3ce7b048f0f248a323b807851346a891c615c47978be5086
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.6` - linux; amd64

```console
$ docker pull consul@sha256:3efabf42b246dae092b236df440d95b25cc79f08941128653fbb490d8068f779
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46461787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36094c09e82962f378f08056864385d0ac1a28ef278b9050423de34b6bd2d07d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 02:55:54 GMT
ENV CONSUL_VERSION=1.8.6
# Fri, 11 Dec 2020 02:55:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 02:55:56 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 02:56:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 02:56:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 02:56:06 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:56:06 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 02:56:06 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 02:56:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 02:56:07 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 02:56:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 02:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 02:56:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe56e704066b43589bb857c9465831a2c34bbbef933b423569c4afe1f8511e3`  
		Last Modified: Fri, 11 Dec 2020 02:57:37 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7854da3823fa235c4710a7558b08efd96290dd80cf0c0252c3100b83f264dfc5`  
		Last Modified: Fri, 11 Dec 2020 02:57:47 GMT  
		Size: 43.7 MB (43661611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b68bd84e508f434ab57fdd39663b88c3e9541e86b01051eb13f41e02049edaa`  
		Last Modified: Fri, 11 Dec 2020 02:57:38 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8494b9fb8d1cc1a0ce36ca17d71f50be0eeb0a299ac3fa836fc54beb2a75e4d`  
		Last Modified: Fri, 11 Dec 2020 02:57:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cce9eef4f2ebc00b962a237fa3e9451a52b28d2d744e48f2ee9d751b4c8d2f0`  
		Last Modified: Fri, 11 Dec 2020 02:57:38 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:334c9f2ed9393ebc322ab707ba05cee30bc7a690df78068fd0910dff150a9af7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41725636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09d11e41fbb7db9ecd01e17397ecb9a0b54af9d8d3ffd6cbd5d96bf7b6a7523f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:13:28 GMT
ENV CONSUL_VERSION=1.8.6
# Fri, 11 Dec 2020 03:13:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:13:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:13:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:13:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:13:48 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:13:49 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:13:50 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:13:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:13:52 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:13:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:13:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:13:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3ae25b06630113a08cb483831556b1c93e2e387a7264fd435f74fa915b7a54a`  
		Last Modified: Fri, 11 Dec 2020 03:16:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47dcb10ad021b2d7f6a18a72b36b488fe9c839e87a9060a87491e9488a5202ba`  
		Last Modified: Fri, 11 Dec 2020 03:16:19 GMT  
		Size: 39.1 MB (39120349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fcb09bf0d7f29af2781bd98bfe0129ca27fa185edd8fae7c7eff1ad6387ade9`  
		Last Modified: Fri, 11 Dec 2020 03:16:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5553aab41258e4b942d2fce34957758217f83453925a5fc6a7875f979b7be046`  
		Last Modified: Fri, 11 Dec 2020 03:16:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0062f04ae06c86fb1f067e692d3db0ae1dd552a24c8de44815a849651e419f1c`  
		Last Modified: Fri, 11 Dec 2020 03:16:10 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:ef535790a37e1a99a3d4aebf16a4a5de63f0edacfbdfe6e94bc33acabc1f8c6f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41889047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74b86702540ec5974ba3a9331a3bc43d021879b0e250694befe4620f3a767b8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:37:28 GMT
ENV CONSUL_VERSION=1.8.6
# Fri, 11 Dec 2020 03:37:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:37:33 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:37:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:37:47 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:37:51 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:37:52 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:37:53 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:37:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:37:56 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:37:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:37:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:37:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f305a28acd173642e8f85c5a1d7f56660ecf7ecd7f0fba73c93b92f2795383b2`  
		Last Modified: Fri, 11 Dec 2020 03:40:38 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01430bb70cd5ef6ffe24b0dcf1079161ad1ff97f395db99b7f62af4771a64d74`  
		Last Modified: Fri, 11 Dec 2020 03:40:49 GMT  
		Size: 39.2 MB (39179135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60eb63112da8eabf1e578e9e39df003a047d01916928b6f384e316609a36e9a9`  
		Last Modified: Fri, 11 Dec 2020 03:40:39 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f966963dd48ffa314bbc482ded77806b13d5c2de847e24ca3f0b578ab5cac7b`  
		Last Modified: Fri, 11 Dec 2020 03:40:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42e1fca3eb7b391c4a4384c639cc4213c0dfeb2459db70aa98bfc219cafc78f`  
		Last Modified: Fri, 11 Dec 2020 03:40:39 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.6` - linux; 386

```console
$ docker pull consul@sha256:84ae85b48c8d01fce5cc0e9a6e90e9f8afcf43489c397a86af1094e1edcbb979
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46352079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:138cc84a33f3f503a4f09b51b0c3e2ed7fe7f7d6fb2a0a76dc1aed4a30c4c2e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 21 Nov 2020 01:38:31 GMT
ENV CONSUL_VERSION=1.8.6
# Sat, 21 Nov 2020 01:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 21 Nov 2020 01:38:33 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 21 Nov 2020 01:38:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 21 Nov 2020 01:38:42 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 21 Nov 2020 01:38:44 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 21 Nov 2020 01:38:44 GMT
VOLUME [/consul/data]
# Sat, 21 Nov 2020 01:38:44 GMT
EXPOSE 8300
# Sat, 21 Nov 2020 01:38:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 21 Nov 2020 01:38:45 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 21 Nov 2020 01:38:45 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 21 Nov 2020 01:38:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 21 Nov 2020 01:38:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f7ea6bb49fcd83fa1e2532a46fa73673811b4f190eabbeac27b70126e99483`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f5b10ad85a8ca78f92681700a4adf4286665337db08649aade4832e289c1b1`  
		Last Modified: Sat, 21 Nov 2020 01:39:42 GMT  
		Size: 43.6 MB (43557436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc233fbc0a691dfc0d0d6632924d73a80241aace4095d2562084aada2f889003`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803b2f813151022af8a8d729fd038d6d97deeb7edf8cda7cd53b6d584074f09d`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4fb85334aeb38ba47abe71d6bafa659b496f04bb6b2195305ef4dcafbe7929e`  
		Last Modified: Sat, 21 Nov 2020 01:39:33 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.7-beta1`

```console
$ docker pull consul@sha256:01327c1298c1e00ee716501e5a72611282a2eccc7aa9d675d5733e38f5f815ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.7-beta1` - linux; amd64

```console
$ docker pull consul@sha256:452254bbabf95081f81104cbff556ad545f1d3cc92035975b04f7fb2e38d2dcc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46491832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f951f2e924c9281ed7a899fade78dabdf91f67af08b5927059f2a6a1dbb9a5d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 02:55:34 GMT
ENV CONSUL_VERSION=1.8.7-beta1
# Fri, 11 Dec 2020 02:55:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 02:55:36 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 02:55:43 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 02:55:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 02:55:45 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:55:46 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 02:55:46 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 02:55:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 02:55:46 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 02:55:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 02:55:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 02:55:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a66b9ce7b221ab146c84eb25a277e06a0826b99714e7eeb6ca8c40b6b66a787`  
		Last Modified: Fri, 11 Dec 2020 02:57:24 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cea40e081f3be1faad62cc0af4827326a61331123e121af23383402571e7e9`  
		Last Modified: Fri, 11 Dec 2020 02:57:33 GMT  
		Size: 43.7 MB (43691656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9334338c9897f03737e2af9b77f01c9cf2ac2a502bdd374bdd680bb5b1bcac6`  
		Last Modified: Fri, 11 Dec 2020 02:57:24 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd80cf0e6584242464edce17d4d1bd4ec3440846670e94ae28b71d548e775026`  
		Last Modified: Fri, 11 Dec 2020 02:57:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc69d15a5375864740337be4930e5922f7bf471c0705072381e4664bab65be81`  
		Last Modified: Fri, 11 Dec 2020 02:57:24 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.7-beta1` - linux; arm variant v6

```console
$ docker pull consul@sha256:6f89e0ac5bd6e1da320a9a7ba905c143a47cc8e7d08b8acdb22da4a82d633ae5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41750472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3794e81845c550ed7932b4bb9f0f4155546d1ac583d97f9acb3d3cd1fcb96b90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:12:50 GMT
ENV CONSUL_VERSION=1.8.7-beta1
# Fri, 11 Dec 2020 03:12:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:12:54 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:13:05 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:13:07 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:13:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:13:12 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:13:13 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:13:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:13:15 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:13:16 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:13:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:13:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335c560a580f06b06f67c2bdfeba13666872484f11c7ab02ebdaa33957d8ec44`  
		Last Modified: Fri, 11 Dec 2020 03:15:51 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b947aeb96ebc7d87db8f1a7520d58195d39710b43f3567b80266087da5b43a0b`  
		Last Modified: Fri, 11 Dec 2020 03:16:02 GMT  
		Size: 39.1 MB (39145184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb854f61fefba4c4d9db80b6536505205de56c6bbffb2f2623d9977bd2a4607`  
		Last Modified: Fri, 11 Dec 2020 03:15:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe6d76761c7c2316935399492b5d70492bd3bf74f239d43ed25c9efdf0db5d57`  
		Last Modified: Fri, 11 Dec 2020 03:15:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf4067909751af352adf482d93191bf5728ac138a290e94293d6028b319ca95`  
		Last Modified: Fri, 11 Dec 2020 03:15:51 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.7-beta1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1788a03ef00de43f7b8de11cf4f9145931c0bccf76b39e550f0da5940762a503
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41921536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf7de691e0e76a94897653aca76dd946f76f3771edce856133893f0b02a934dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:36:39 GMT
ENV CONSUL_VERSION=1.8.7-beta1
# Fri, 11 Dec 2020 03:36:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:36:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:36:51 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:36:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:37:04 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:37:07 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:37:09 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:37:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:37:15 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:37:16 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:37:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:37:20 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143f2407a6188758bd2837c48a8221c63df562124050a5610c44613f2fd9dc6b`  
		Last Modified: Fri, 11 Dec 2020 03:40:20 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4e74b34941fd6053ed184baaff2fefc8050d15c2e62f8143c27731dfc26c79`  
		Last Modified: Fri, 11 Dec 2020 03:40:31 GMT  
		Size: 39.2 MB (39211628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496e8a99c70fd013a21d561991674c578375caf20cbfe8e3abc75b8ed549285b`  
		Last Modified: Fri, 11 Dec 2020 03:40:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8020348695f9d21624ae5a46045177bcb07005b730527abf1a071208b45cd890`  
		Last Modified: Fri, 11 Dec 2020 03:40:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f83f506da8f5fa2e62ec0fd6ff64141b305288d47239c1438440d3bd9c744f8`  
		Last Modified: Fri, 11 Dec 2020 03:40:20 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.7-beta1` - linux; 386

```console
$ docker pull consul@sha256:430eb1c9a4629c9df39cc4e11b03cdd4621435054416b7ffc97d246479cc730f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.4 MB (46375562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6dee82c387312983169c74fcb38bc412cb73a5f6ec48e58a5644568a9570c77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 03 Dec 2020 22:40:05 GMT
ENV CONSUL_VERSION=1.8.7-beta1
# Thu, 03 Dec 2020 22:40:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 03 Dec 2020 22:40:06 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 03 Dec 2020 22:40:12 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 03 Dec 2020 22:40:13 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 03 Dec 2020 22:40:14 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 03 Dec 2020 22:40:14 GMT
VOLUME [/consul/data]
# Thu, 03 Dec 2020 22:40:14 GMT
EXPOSE 8300
# Thu, 03 Dec 2020 22:40:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 03 Dec 2020 22:40:14 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 03 Dec 2020 22:40:15 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 03 Dec 2020 22:40:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Dec 2020 22:40:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66da464d16ffb961dc677b6a098d9b882abdf5e13fc48e2eb7328b0613fffcdb`  
		Last Modified: Thu, 03 Dec 2020 22:40:40 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542fe049b69d9d812b17c8f5fabf2a54e9d238ba8082e93f9a25d96a7c675cde`  
		Last Modified: Thu, 03 Dec 2020 22:40:48 GMT  
		Size: 43.6 MB (43580920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7918d136acf07af5f2dd94795f491dba2e90c52c6a23c05a1082bab54fd25863`  
		Last Modified: Thu, 03 Dec 2020 22:40:40 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8bf6b229e96c0f834f0fd4135d5e3755f79dad031a8150f7e79f7fe76b6963`  
		Last Modified: Thu, 03 Dec 2020 22:40:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d6b49718a62a616e193eb296177e636a6fd9d0c6aca0972283fc440478632a`  
		Last Modified: Thu, 03 Dec 2020 22:40:40 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:2d0929de7e38cc2b62ee2e100c3a565acbb56d264cbfca40ea4b92620931b8cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:3aeb5ab2d0fa9189ed99692f8cce218d1c5eb591255ac38c389b680aad3bd5bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45520428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8429e82f47dd20c7833966453d571fc43ece763fa5cadec460390351f99d839`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 02:55:15 GMT
ENV CONSUL_VERSION=1.9.0
# Fri, 11 Dec 2020 02:55:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 02:55:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 02:55:24 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 02:55:26 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 02:55:27 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:55:28 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 02:55:28 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 02:55:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 02:55:28 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 02:55:29 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 02:55:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 02:55:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0dc5b4d599656ad90b0d9809894af2414f9ffadb68145140f4038ecac2eb174`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07ae847c23d3422b795a3bdf170616176238924d44bb8b99503f34b86222246`  
		Last Modified: Fri, 11 Dec 2020 02:57:17 GMT  
		Size: 42.7 MB (42720248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f01f506e7a1412784c106cd451bf530c4e2fa89b82da5494eb7fcee179ee04`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54d30ff31eeef79e6a8ecf14d92c4324b82f4be1176b8a22b89172bdbb1e535`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0811e7d6f99e0f9f0104dbcbb3682d6b9da402b2d9993c9ba173c6c014904e3`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:ea57f6e8a3ac35a8d762d5efc0255be5ff6f343e7f42da89f9cf5f35269d8460
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40798326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c287fbf4311372e3435b6ca8a04dbe0e562c7d63771ba584499ce679b76d95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:12:14 GMT
ENV CONSUL_VERSION=1.9.0
# Fri, 11 Dec 2020 03:12:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:12:18 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:12:27 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:12:31 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:12:35 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:12:36 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:12:37 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:12:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:12:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:12:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:12:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:12:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8283f855d02b9925e08d773e17c594b6fab1103cd5a38180770ad785e5133257`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511d3f0ca831f083e1ea3506ba1dda3d750e633c4692380f322f4d283ed7ba2e`  
		Last Modified: Fri, 11 Dec 2020 03:15:41 GMT  
		Size: 38.2 MB (38193039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4881e90e27a62c4d13595fc04a5d52732daf830d336c9b126820f257f9fbc115`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c59a7a7c5e1ca0d9ad62d618bb3be147339f3f54a956a913f454d687930dd0`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03202c39a02367e52e75468a4b0db5ff8829e5c614c4f26cb24263971b21a92c`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2f7f2f48062c6f2c626d180d7bbe189a228ece877c67467497f599463e568abb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41004660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf783fef2553f04076b300b3cc699e3cf3c7c01a537d0a2964b4520862e9445`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:36:07 GMT
ENV CONSUL_VERSION=1.9.0
# Fri, 11 Dec 2020 03:36:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:36:10 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:36:18 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:36:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:36:24 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:36:25 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:36:26 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:36:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:36:28 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:36:29 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:36:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:36:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9646958c33e98d576e6fb8e6af71e6669d27599d4e856b994c2745e2b28dc6`  
		Last Modified: Fri, 11 Dec 2020 03:40:00 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fda4034b47493ffa2bdc2fc00e1f1737c1316e7bcf20b7e67594f267441744`  
		Last Modified: Fri, 11 Dec 2020 03:40:09 GMT  
		Size: 38.3 MB (38294743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196b47efdb30abfc356adaa8a9a46ad212262e86bb9c841645a7f563b716c330`  
		Last Modified: Fri, 11 Dec 2020 03:39:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f9f95e7f2fc8ddf2d990b63395688513dd0ddcfa97f5551009374cfb1392d1`  
		Last Modified: Fri, 11 Dec 2020 03:40:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aebe0597c9546716c89ee816495ecd422c9b9669988e72e84b7076376631ab`  
		Last Modified: Fri, 11 Dec 2020 03:40:00 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:3ad6148e3cdb242420b209f4d1fe73da7c23f2c78598dbb3df16f6538d5a013a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45231403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:addffb46e74179410991b94d4784f09f5e804e3345dea67754c93b743b861fbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:38:31 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:38:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:38:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:38:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:38:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:38:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:38:40 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:38:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:38:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b670227cf5b0369dec1890afd49daa761d5219f770e6e1717eeb94aa0d30d795`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886f4ead96bdf58722ac9a1bb62e065252db84d364caac2f2f162484607b9679`  
		Last Modified: Wed, 25 Nov 2020 00:39:12 GMT  
		Size: 42.4 MB (42436764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099eaffdcf30a6fc42310fad858f1210dc9a72b912f3867f84114f14283e4b1`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60de6fed51016b0bc661d53792674a602f12405b5ee4fa32ff4760a2c97fd0a`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1722523c085b312cc345217410e18206bcf15369b2bb5c423315508580a7e0`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.0`

```console
$ docker pull consul@sha256:2d0929de7e38cc2b62ee2e100c3a565acbb56d264cbfca40ea4b92620931b8cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.0` - linux; amd64

```console
$ docker pull consul@sha256:3aeb5ab2d0fa9189ed99692f8cce218d1c5eb591255ac38c389b680aad3bd5bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45520428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8429e82f47dd20c7833966453d571fc43ece763fa5cadec460390351f99d839`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 02:55:15 GMT
ENV CONSUL_VERSION=1.9.0
# Fri, 11 Dec 2020 02:55:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 02:55:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 02:55:24 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 02:55:26 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 02:55:27 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:55:28 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 02:55:28 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 02:55:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 02:55:28 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 02:55:29 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 02:55:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 02:55:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0dc5b4d599656ad90b0d9809894af2414f9ffadb68145140f4038ecac2eb174`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07ae847c23d3422b795a3bdf170616176238924d44bb8b99503f34b86222246`  
		Last Modified: Fri, 11 Dec 2020 02:57:17 GMT  
		Size: 42.7 MB (42720248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f01f506e7a1412784c106cd451bf530c4e2fa89b82da5494eb7fcee179ee04`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54d30ff31eeef79e6a8ecf14d92c4324b82f4be1176b8a22b89172bdbb1e535`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0811e7d6f99e0f9f0104dbcbb3682d6b9da402b2d9993c9ba173c6c014904e3`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0` - linux; arm variant v6

```console
$ docker pull consul@sha256:ea57f6e8a3ac35a8d762d5efc0255be5ff6f343e7f42da89f9cf5f35269d8460
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40798326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c287fbf4311372e3435b6ca8a04dbe0e562c7d63771ba584499ce679b76d95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:12:14 GMT
ENV CONSUL_VERSION=1.9.0
# Fri, 11 Dec 2020 03:12:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:12:18 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:12:27 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:12:31 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:12:35 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:12:36 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:12:37 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:12:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:12:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:12:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:12:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:12:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8283f855d02b9925e08d773e17c594b6fab1103cd5a38180770ad785e5133257`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511d3f0ca831f083e1ea3506ba1dda3d750e633c4692380f322f4d283ed7ba2e`  
		Last Modified: Fri, 11 Dec 2020 03:15:41 GMT  
		Size: 38.2 MB (38193039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4881e90e27a62c4d13595fc04a5d52732daf830d336c9b126820f257f9fbc115`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c59a7a7c5e1ca0d9ad62d618bb3be147339f3f54a956a913f454d687930dd0`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03202c39a02367e52e75468a4b0db5ff8829e5c614c4f26cb24263971b21a92c`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2f7f2f48062c6f2c626d180d7bbe189a228ece877c67467497f599463e568abb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41004660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf783fef2553f04076b300b3cc699e3cf3c7c01a537d0a2964b4520862e9445`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:36:07 GMT
ENV CONSUL_VERSION=1.9.0
# Fri, 11 Dec 2020 03:36:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:36:10 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:36:18 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:36:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:36:24 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:36:25 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:36:26 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:36:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:36:28 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:36:29 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:36:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:36:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9646958c33e98d576e6fb8e6af71e6669d27599d4e856b994c2745e2b28dc6`  
		Last Modified: Fri, 11 Dec 2020 03:40:00 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fda4034b47493ffa2bdc2fc00e1f1737c1316e7bcf20b7e67594f267441744`  
		Last Modified: Fri, 11 Dec 2020 03:40:09 GMT  
		Size: 38.3 MB (38294743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196b47efdb30abfc356adaa8a9a46ad212262e86bb9c841645a7f563b716c330`  
		Last Modified: Fri, 11 Dec 2020 03:39:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f9f95e7f2fc8ddf2d990b63395688513dd0ddcfa97f5551009374cfb1392d1`  
		Last Modified: Fri, 11 Dec 2020 03:40:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aebe0597c9546716c89ee816495ecd422c9b9669988e72e84b7076376631ab`  
		Last Modified: Fri, 11 Dec 2020 03:40:00 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0` - linux; 386

```console
$ docker pull consul@sha256:3ad6148e3cdb242420b209f4d1fe73da7c23f2c78598dbb3df16f6538d5a013a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45231403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:addffb46e74179410991b94d4784f09f5e804e3345dea67754c93b743b861fbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:38:31 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:38:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:38:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:38:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:38:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:38:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:38:40 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:38:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:38:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b670227cf5b0369dec1890afd49daa761d5219f770e6e1717eeb94aa0d30d795`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886f4ead96bdf58722ac9a1bb62e065252db84d364caac2f2f162484607b9679`  
		Last Modified: Wed, 25 Nov 2020 00:39:12 GMT  
		Size: 42.4 MB (42436764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099eaffdcf30a6fc42310fad858f1210dc9a72b912f3867f84114f14283e4b1`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60de6fed51016b0bc661d53792674a602f12405b5ee4fa32ff4760a2c97fd0a`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1722523c085b312cc345217410e18206bcf15369b2bb5c423315508580a7e0`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:2d0929de7e38cc2b62ee2e100c3a565acbb56d264cbfca40ea4b92620931b8cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:3aeb5ab2d0fa9189ed99692f8cce218d1c5eb591255ac38c389b680aad3bd5bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45520428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8429e82f47dd20c7833966453d571fc43ece763fa5cadec460390351f99d839`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 02:55:15 GMT
ENV CONSUL_VERSION=1.9.0
# Fri, 11 Dec 2020 02:55:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 02:55:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 02:55:24 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 02:55:26 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 02:55:27 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 02:55:28 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 02:55:28 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 02:55:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 02:55:28 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 02:55:29 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 02:55:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 02:55:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0dc5b4d599656ad90b0d9809894af2414f9ffadb68145140f4038ecac2eb174`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07ae847c23d3422b795a3bdf170616176238924d44bb8b99503f34b86222246`  
		Last Modified: Fri, 11 Dec 2020 02:57:17 GMT  
		Size: 42.7 MB (42720248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f01f506e7a1412784c106cd451bf530c4e2fa89b82da5494eb7fcee179ee04`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54d30ff31eeef79e6a8ecf14d92c4324b82f4be1176b8a22b89172bdbb1e535`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0811e7d6f99e0f9f0104dbcbb3682d6b9da402b2d9993c9ba173c6c014904e3`  
		Last Modified: Fri, 11 Dec 2020 02:57:08 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:ea57f6e8a3ac35a8d762d5efc0255be5ff6f343e7f42da89f9cf5f35269d8460
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40798326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5c287fbf4311372e3435b6ca8a04dbe0e562c7d63771ba584499ce679b76d95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:12:14 GMT
ENV CONSUL_VERSION=1.9.0
# Fri, 11 Dec 2020 03:12:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:12:18 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:12:27 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:12:31 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:12:35 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:12:36 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:12:37 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:12:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:12:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:12:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:12:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:12:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8283f855d02b9925e08d773e17c594b6fab1103cd5a38180770ad785e5133257`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:511d3f0ca831f083e1ea3506ba1dda3d750e633c4692380f322f4d283ed7ba2e`  
		Last Modified: Fri, 11 Dec 2020 03:15:41 GMT  
		Size: 38.2 MB (38193039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4881e90e27a62c4d13595fc04a5d52732daf830d336c9b126820f257f9fbc115`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c59a7a7c5e1ca0d9ad62d618bb3be147339f3f54a956a913f454d687930dd0`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03202c39a02367e52e75468a4b0db5ff8829e5c614c4f26cb24263971b21a92c`  
		Last Modified: Fri, 11 Dec 2020 03:15:30 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2f7f2f48062c6f2c626d180d7bbe189a228ece877c67467497f599463e568abb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41004660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf783fef2553f04076b300b3cc699e3cf3c7c01a537d0a2964b4520862e9445`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Dec 2020 03:36:07 GMT
ENV CONSUL_VERSION=1.9.0
# Fri, 11 Dec 2020 03:36:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Dec 2020 03:36:10 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Dec 2020 03:36:18 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Dec 2020 03:36:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Dec 2020 03:36:24 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Dec 2020 03:36:25 GMT
VOLUME [/consul/data]
# Fri, 11 Dec 2020 03:36:26 GMT
EXPOSE 8300
# Fri, 11 Dec 2020 03:36:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Dec 2020 03:36:28 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Dec 2020 03:36:29 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Dec 2020 03:36:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Dec 2020 03:36:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9646958c33e98d576e6fb8e6af71e6669d27599d4e856b994c2745e2b28dc6`  
		Last Modified: Fri, 11 Dec 2020 03:40:00 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fda4034b47493ffa2bdc2fc00e1f1737c1316e7bcf20b7e67594f267441744`  
		Last Modified: Fri, 11 Dec 2020 03:40:09 GMT  
		Size: 38.3 MB (38294743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196b47efdb30abfc356adaa8a9a46ad212262e86bb9c841645a7f563b716c330`  
		Last Modified: Fri, 11 Dec 2020 03:39:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f9f95e7f2fc8ddf2d990b63395688513dd0ddcfa97f5551009374cfb1392d1`  
		Last Modified: Fri, 11 Dec 2020 03:40:00 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8aebe0597c9546716c89ee816495ecd422c9b9669988e72e84b7076376631ab`  
		Last Modified: Fri, 11 Dec 2020 03:40:00 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:3ad6148e3cdb242420b209f4d1fe73da7c23f2c78598dbb3df16f6538d5a013a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45231403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:addffb46e74179410991b94d4784f09f5e804e3345dea67754c93b743b861fbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 25 Nov 2020 00:38:31 GMT
ENV CONSUL_VERSION=1.9.0
# Wed, 25 Nov 2020 00:38:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 25 Nov 2020 00:38:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 25 Nov 2020 00:38:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 25 Nov 2020 00:38:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 25 Nov 2020 00:38:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 25 Nov 2020 00:38:40 GMT
VOLUME [/consul/data]
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8300
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 25 Nov 2020 00:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 25 Nov 2020 00:38:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 25 Nov 2020 00:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 25 Nov 2020 00:38:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b670227cf5b0369dec1890afd49daa761d5219f770e6e1717eeb94aa0d30d795`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886f4ead96bdf58722ac9a1bb62e065252db84d364caac2f2f162484607b9679`  
		Last Modified: Wed, 25 Nov 2020 00:39:12 GMT  
		Size: 42.4 MB (42436764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9099eaffdcf30a6fc42310fad858f1210dc9a72b912f3867f84114f14283e4b1`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60de6fed51016b0bc661d53792674a602f12405b5ee4fa32ff4760a2c97fd0a`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1722523c085b312cc345217410e18206bcf15369b2bb5c423315508580a7e0`  
		Last Modified: Wed, 25 Nov 2020 00:39:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
