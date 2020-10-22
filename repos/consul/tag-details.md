<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.6`](#consul16)
-	[`consul:1.6.9`](#consul169)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.8`](#consul178)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.4`](#consul184)
-	[`consul:1.9.0-beta`](#consul190-beta)
-	[`consul:1.9.0-beta1`](#consul190-beta1)
-	[`consul:latest`](#consullatest)

## `consul:1.6`

```console
$ docker pull consul@sha256:5f8a0bd95ba809f3f34a4d3e5f3fe9ebd0da81fdde8b0c93521f20de669da957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6` - linux; amd64

```console
$ docker pull consul@sha256:eddec9d26473fe2e94f4e3bd1b881af9f873dce17f441feaabef2dc531b1b09d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42259611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e74740b420e54b5fabfa7de9085e3f9a92284a068f07e2b2d1ff51da47e8d752`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:35:16 GMT
ENV CONSUL_VERSION=1.6.9
# Fri, 11 Sep 2020 21:35:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:35:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:35:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:35:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:35:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:35:23 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:35:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:35:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:35:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42497aee15ea85ada3648423d8d60d805b4046840e36e2592010f03b46b5c3`  
		Last Modified: Fri, 11 Sep 2020 21:35:56 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb172b87dfe72a49c6f089cf7da7c050b7da582882d8acf632f5f7912bf3ffa7`  
		Last Modified: Fri, 11 Sep 2020 21:36:01 GMT  
		Size: 39.5 MB (39458832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f80f502d16c7f8614e287d6b921d01d7e0dbd9eb57e6aedaf04567acc00f07`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05694da12802199551dded466f04e09ea60449649d97d73f9845a24753edb98d`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013954d81caeedbfde4d469f884e6ec28c3fc8b608b467cd4e34104b573ed6a`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:11402265c959324ae00a4be3e13c6b163fa028bdac6c516286cdcb602c7295ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37557209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6c2989bc3346a2aec8227ad0d910bff035ff464b4c5eaff3075c05d7c1afd8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:19:05 GMT
ENV CONSUL_VERSION=1.6.9
# Thu, 22 Oct 2020 02:19:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:19:09 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:19:18 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:19:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:19:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:19:24 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:19:25 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:19:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:19:26 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:19:27 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:19:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:19:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd239832650b55fa048bc70f1d78fc8bbbd2c747915b960be35ea5d4b5eda01`  
		Last Modified: Thu, 22 Oct 2020 02:20:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9877f1a374dcd23efcd28ce516c7bdef47a2b906e6f0273844e30e0110c34e78`  
		Last Modified: Thu, 22 Oct 2020 02:20:53 GMT  
		Size: 35.0 MB (34952002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccb722985e3f755b5e11b4aa4934954ed81c6c29b7f514f54a8d5318f737b97`  
		Last Modified: Thu, 22 Oct 2020 02:20:43 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f37034126eb607ef4651ab1d37dd11ab119260e9e97c1456f8dde11568f22e`  
		Last Modified: Thu, 22 Oct 2020 02:20:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a159cc9bb0a9562a3f9a71eb14e64499ac3ca631199b8ae25fcb0190fecbed13`  
		Last Modified: Thu, 22 Oct 2020 02:20:44 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:651562ab568f0e5f048ff79fb85571a96020002a7303bdc4c38434b0d726ee2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37770578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e4b0254d660feff03752cb9e82c296b041c1c345cc3b784a0fe2196fa28c70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:44:25 GMT
ENV CONSUL_VERSION=1.6.9
# Thu, 22 Oct 2020 02:44:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:44:28 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:44:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:44:38 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:44:43 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:44:44 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:44:46 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:44:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:44:47 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:44:48 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:44:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:44:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16997447fe87a1e8bbe78be659c82a0468ebd3c2da305fd40d5591a03dccb4a`  
		Last Modified: Thu, 22 Oct 2020 02:46:11 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d61c64ebeecfcbdcbb6fc2fce1e4ef538a936b94bca26de6e9ff54e0284731`  
		Last Modified: Thu, 22 Oct 2020 02:46:18 GMT  
		Size: 35.1 MB (35060733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616c87b38760da24b59bdbe435c945322b008564896a31be07d0a3c45d2053b9`  
		Last Modified: Thu, 22 Oct 2020 02:46:11 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed7362120f6af6391c8c69787dc5231391109ce44cce78be039956d3b5fe483`  
		Last Modified: Thu, 22 Oct 2020 02:46:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f83e82bb9fffaf33d87091dde5f758127f0a62a7bfd235ca3a727c8f919fe7`  
		Last Modified: Thu, 22 Oct 2020 02:46:11 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; 386

```console
$ docker pull consul@sha256:c0ccc0d7d9d39b0b590ab7e7600d9a60622efedd792f4e29a1face7cb54fcef2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40711205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b939eaa71dd621532345005883735117cc2d10081e9f46c8e9a943f55c4b92c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:33:30 GMT
ENV CONSUL_VERSION=1.6.9
# Thu, 22 Oct 2020 02:33:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:33:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:33:35 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:33:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:33:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:33:37 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:33:37 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:33:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:33:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:33:38 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:33:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:33:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f593edb3ca181cedb465d47bc8d5f95fb0fbb2fd684196c9e5a9dcbaa452e2c`  
		Last Modified: Thu, 22 Oct 2020 02:34:34 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9045232253bcf9de8195d1df7cd598411be6b6a40b0e89818bb6befb51420643`  
		Last Modified: Thu, 22 Oct 2020 02:34:41 GMT  
		Size: 37.9 MB (37916567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87d11b33cb71552cd11e3aa1d36d118f3cf0e57d128f8857fd1af558334756b`  
		Last Modified: Thu, 22 Oct 2020 02:34:33 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7eaac794af9076db31f291ace339f2c6b5efb18de116ea29e2560eaab353628`  
		Last Modified: Thu, 22 Oct 2020 02:34:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2163c1d05156ee0574c9979e9426c9a6078d4b23ce7c23badf94a57e42f16fe2`  
		Last Modified: Thu, 22 Oct 2020 02:34:33 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6.9`

```console
$ docker pull consul@sha256:5f8a0bd95ba809f3f34a4d3e5f3fe9ebd0da81fdde8b0c93521f20de669da957
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6.9` - linux; amd64

```console
$ docker pull consul@sha256:eddec9d26473fe2e94f4e3bd1b881af9f873dce17f441feaabef2dc531b1b09d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42259611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e74740b420e54b5fabfa7de9085e3f9a92284a068f07e2b2d1ff51da47e8d752`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:35:16 GMT
ENV CONSUL_VERSION=1.6.9
# Fri, 11 Sep 2020 21:35:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:35:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:35:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:35:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:35:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:35:23 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:35:23 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:35:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:35:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:35:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c42497aee15ea85ada3648423d8d60d805b4046840e36e2592010f03b46b5c3`  
		Last Modified: Fri, 11 Sep 2020 21:35:56 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb172b87dfe72a49c6f089cf7da7c050b7da582882d8acf632f5f7912bf3ffa7`  
		Last Modified: Fri, 11 Sep 2020 21:36:01 GMT  
		Size: 39.5 MB (39458832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f80f502d16c7f8614e287d6b921d01d7e0dbd9eb57e6aedaf04567acc00f07`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05694da12802199551dded466f04e09ea60449649d97d73f9845a24753edb98d`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5013954d81caeedbfde4d469f884e6ec28c3fc8b608b467cd4e34104b573ed6a`  
		Last Modified: Fri, 11 Sep 2020 21:35:55 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:11402265c959324ae00a4be3e13c6b163fa028bdac6c516286cdcb602c7295ed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37557209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6c2989bc3346a2aec8227ad0d910bff035ff464b4c5eaff3075c05d7c1afd8e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:19:05 GMT
ENV CONSUL_VERSION=1.6.9
# Thu, 22 Oct 2020 02:19:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:19:09 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:19:18 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:19:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:19:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:19:24 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:19:25 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:19:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:19:26 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:19:27 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:19:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:19:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd239832650b55fa048bc70f1d78fc8bbbd2c747915b960be35ea5d4b5eda01`  
		Last Modified: Thu, 22 Oct 2020 02:20:45 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9877f1a374dcd23efcd28ce516c7bdef47a2b906e6f0273844e30e0110c34e78`  
		Last Modified: Thu, 22 Oct 2020 02:20:53 GMT  
		Size: 35.0 MB (34952002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ccb722985e3f755b5e11b4aa4934954ed81c6c29b7f514f54a8d5318f737b97`  
		Last Modified: Thu, 22 Oct 2020 02:20:43 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f37034126eb607ef4651ab1d37dd11ab119260e9e97c1456f8dde11568f22e`  
		Last Modified: Thu, 22 Oct 2020 02:20:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a159cc9bb0a9562a3f9a71eb14e64499ac3ca631199b8ae25fcb0190fecbed13`  
		Last Modified: Thu, 22 Oct 2020 02:20:44 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:651562ab568f0e5f048ff79fb85571a96020002a7303bdc4c38434b0d726ee2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37770578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e4b0254d660feff03752cb9e82c296b041c1c345cc3b784a0fe2196fa28c70`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:44:25 GMT
ENV CONSUL_VERSION=1.6.9
# Thu, 22 Oct 2020 02:44:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:44:28 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:44:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:44:38 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:44:43 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:44:44 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:44:46 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:44:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:44:47 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:44:48 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:44:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:44:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16997447fe87a1e8bbe78be659c82a0468ebd3c2da305fd40d5591a03dccb4a`  
		Last Modified: Thu, 22 Oct 2020 02:46:11 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d61c64ebeecfcbdcbb6fc2fce1e4ef538a936b94bca26de6e9ff54e0284731`  
		Last Modified: Thu, 22 Oct 2020 02:46:18 GMT  
		Size: 35.1 MB (35060733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616c87b38760da24b59bdbe435c945322b008564896a31be07d0a3c45d2053b9`  
		Last Modified: Thu, 22 Oct 2020 02:46:11 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed7362120f6af6391c8c69787dc5231391109ce44cce78be039956d3b5fe483`  
		Last Modified: Thu, 22 Oct 2020 02:46:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f83e82bb9fffaf33d87091dde5f758127f0a62a7bfd235ca3a727c8f919fe7`  
		Last Modified: Thu, 22 Oct 2020 02:46:11 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.9` - linux; 386

```console
$ docker pull consul@sha256:c0ccc0d7d9d39b0b590ab7e7600d9a60622efedd792f4e29a1face7cb54fcef2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40711205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b939eaa71dd621532345005883735117cc2d10081e9f46c8e9a943f55c4b92c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:33:30 GMT
ENV CONSUL_VERSION=1.6.9
# Thu, 22 Oct 2020 02:33:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:33:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:33:35 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:33:36 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:33:37 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:33:37 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:33:37 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:33:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:33:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:33:38 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:33:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:33:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f593edb3ca181cedb465d47bc8d5f95fb0fbb2fd684196c9e5a9dcbaa452e2c`  
		Last Modified: Thu, 22 Oct 2020 02:34:34 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9045232253bcf9de8195d1df7cd598411be6b6a40b0e89818bb6befb51420643`  
		Last Modified: Thu, 22 Oct 2020 02:34:41 GMT  
		Size: 37.9 MB (37916567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87d11b33cb71552cd11e3aa1d36d118f3cf0e57d128f8857fd1af558334756b`  
		Last Modified: Thu, 22 Oct 2020 02:34:33 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7eaac794af9076db31f291ace339f2c6b5efb18de116ea29e2560eaab353628`  
		Last Modified: Thu, 22 Oct 2020 02:34:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2163c1d05156ee0574c9979e9426c9a6078d4b23ce7c23badf94a57e42f16fe2`  
		Last Modified: Thu, 22 Oct 2020 02:34:33 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7`

```console
$ docker pull consul@sha256:e86ac5dbf6087690a2357ef9fefa6efdac82c10c0ad97418dc99a5b3ba13c381
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:fd06290ad67183ed4f65c35e05efe269dec80b9c665a301ab4e45336dd9b7bf8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43633264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6869b20c1bf31d78cd2525d9607eccb6643ba8ff5aa6ecc5d12fece9e60d5455`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:35:04 GMT
ENV CONSUL_VERSION=1.7.8
# Fri, 11 Sep 2020 21:35:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:35:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:35:09 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:35:10 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:35:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:35:10 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:35:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:35:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:35:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa86cffd3d009f7a9062b7c62420ed125fec80d5c3ab5c9432246d6b3d7ce11`  
		Last Modified: Fri, 11 Sep 2020 21:35:45 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e25af134fa51e8e53d03ff4baf1e6b48909de064e5ce2fe617ed73586b48b4`  
		Last Modified: Fri, 11 Sep 2020 21:35:52 GMT  
		Size: 40.8 MB (40832486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8188b0a8b6262076f7dcced96696a6a9f50a6bc10f74abb2dd990a5b9b648e0`  
		Last Modified: Fri, 11 Sep 2020 21:35:46 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c6376cdcf722e41d109f488d4ae9df81f05a1a8fd276f2aa68e2e745048e4f`  
		Last Modified: Fri, 11 Sep 2020 21:35:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b0f8bcd6a04a40bfd629b41a694d2adac2f09fda47e1b93f01f53d8434e3e1`  
		Last Modified: Fri, 11 Sep 2020 21:35:46 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:2db40f6ad0da60a8bd9f7f00f71c56115f039cbf0316885c2cb20e23f0931dd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.9 MB (38924120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e8680f4300a83e027a835b43674073a118375528edcc4d4d10d18e0f4e4d13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:18:28 GMT
ENV CONSUL_VERSION=1.7.8
# Thu, 22 Oct 2020 02:18:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:18:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:18:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:18:43 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:18:46 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:18:48 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:18:50 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:18:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:18:54 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:18:54 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:18:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362d7bc1ef4aabc8f77c9ee4075120e73c1713da1a068e507628e93cfd70b9d5`  
		Last Modified: Thu, 22 Oct 2020 02:20:26 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0f913815265503adbe9d2795af3f68f558bedee744c1f2db9b2331181a5835`  
		Last Modified: Thu, 22 Oct 2020 02:20:36 GMT  
		Size: 36.3 MB (36318909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebc63ea7d35f00edbfbf244ab241567f12332a2dfb14366c2c45d8887315729`  
		Last Modified: Thu, 22 Oct 2020 02:20:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bbabb0d9883ceaafbb96aa45f4af26028284490ca6aa9b998982fffbd0de8d`  
		Last Modified: Thu, 22 Oct 2020 02:20:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b8b0280c0c57750295448b33f5585177c360ba3331fab6ce2209bebeb750b5`  
		Last Modified: Thu, 22 Oct 2020 02:20:27 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b8ae68f21657f99a78c35accfa81b273d4fb54394f37a427e98336aed2d536fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39103791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf49477b99c8feb367ad880b495034920d284e1cc73e7a0ed4b9df8a207352e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:43:44 GMT
ENV CONSUL_VERSION=1.7.8
# Thu, 22 Oct 2020 02:43:46 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:43:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:44:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:44:05 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:44:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:44:08 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:44:09 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:44:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:44:11 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:44:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:44:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:44:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968982c6d6074d48939087574059ff72725e2958974fb5b80436f49161fdd115`  
		Last Modified: Thu, 22 Oct 2020 02:45:37 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5702da4067070094b526298b3a05abf0d2a9a8e0c60201bc7f1a6fc744d9d80`  
		Last Modified: Thu, 22 Oct 2020 02:46:03 GMT  
		Size: 36.4 MB (36393942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ccf2eb561e86187b01dfab1a20f1cf597967516917c1589489bd5e09c638b2`  
		Last Modified: Thu, 22 Oct 2020 02:45:37 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2ba40bff249761f03bb4f4a5100e72cd0cf928ee37ef07015edcdbcf26153`  
		Last Modified: Thu, 22 Oct 2020 02:45:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04029515034058419f2d60d6c2dd1a06a6d10105a522f6d5575dd9c907249557`  
		Last Modified: Thu, 22 Oct 2020 02:45:37 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:3926844f90e94a6f3be5bdbc889769528541d1e0be8b17c074b8073f922a36f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (42034053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3df2eac77c1efad58c3951fa319b458d1b7da01915f8a14a926a613f41d8873e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:33:16 GMT
ENV CONSUL_VERSION=1.7.8
# Thu, 22 Oct 2020 02:33:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:33:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:33:22 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:33:23 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:33:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:33:24 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:33:24 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:33:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:33:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:33:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:33:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846db40e649b58b8967aacf1f6f7a7d8627f1ffd6f918f6cb4367370d86f720e`  
		Last Modified: Thu, 22 Oct 2020 02:34:16 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731e87c48127e5fea1a2158e52aef1babde7f5bdc5f3fac254f813e8ac5871ab`  
		Last Modified: Thu, 22 Oct 2020 02:34:27 GMT  
		Size: 39.2 MB (39239414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef242b5bc816d7b2d2bc0a9a840fcc4a88c262936c3672739b5a2d91f32f711`  
		Last Modified: Thu, 22 Oct 2020 02:34:16 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e02e9eed1127a82a8898fea88eb8eb225449f970a78099c8fc7ac8348c9ab3`  
		Last Modified: Thu, 22 Oct 2020 02:34:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e0f6a184523db8b8a646ce977a666df54ba7508f2021b178f413a2823a020e`  
		Last Modified: Thu, 22 Oct 2020 02:34:16 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.8`

```console
$ docker pull consul@sha256:e86ac5dbf6087690a2357ef9fefa6efdac82c10c0ad97418dc99a5b3ba13c381
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.8` - linux; amd64

```console
$ docker pull consul@sha256:fd06290ad67183ed4f65c35e05efe269dec80b9c665a301ab4e45336dd9b7bf8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43633264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6869b20c1bf31d78cd2525d9607eccb6643ba8ff5aa6ecc5d12fece9e60d5455`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:35:04 GMT
ENV CONSUL_VERSION=1.7.8
# Fri, 11 Sep 2020 21:35:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:35:05 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:35:09 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:35:10 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:35:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:35:10 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:35:11 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:35:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:35:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:35:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa86cffd3d009f7a9062b7c62420ed125fec80d5c3ab5c9432246d6b3d7ce11`  
		Last Modified: Fri, 11 Sep 2020 21:35:45 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e25af134fa51e8e53d03ff4baf1e6b48909de064e5ce2fe617ed73586b48b4`  
		Last Modified: Fri, 11 Sep 2020 21:35:52 GMT  
		Size: 40.8 MB (40832486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8188b0a8b6262076f7dcced96696a6a9f50a6bc10f74abb2dd990a5b9b648e0`  
		Last Modified: Fri, 11 Sep 2020 21:35:46 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c6376cdcf722e41d109f488d4ae9df81f05a1a8fd276f2aa68e2e745048e4f`  
		Last Modified: Fri, 11 Sep 2020 21:35:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b0f8bcd6a04a40bfd629b41a694d2adac2f09fda47e1b93f01f53d8434e3e1`  
		Last Modified: Fri, 11 Sep 2020 21:35:46 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:2db40f6ad0da60a8bd9f7f00f71c56115f039cbf0316885c2cb20e23f0931dd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.9 MB (38924120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e8680f4300a83e027a835b43674073a118375528edcc4d4d10d18e0f4e4d13f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:18:28 GMT
ENV CONSUL_VERSION=1.7.8
# Thu, 22 Oct 2020 02:18:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:18:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:18:40 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:18:43 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:18:46 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:18:48 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:18:50 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:18:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:18:54 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:18:54 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:18:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:18:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362d7bc1ef4aabc8f77c9ee4075120e73c1713da1a068e507628e93cfd70b9d5`  
		Last Modified: Thu, 22 Oct 2020 02:20:26 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0f913815265503adbe9d2795af3f68f558bedee744c1f2db9b2331181a5835`  
		Last Modified: Thu, 22 Oct 2020 02:20:36 GMT  
		Size: 36.3 MB (36318909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebc63ea7d35f00edbfbf244ab241567f12332a2dfb14366c2c45d8887315729`  
		Last Modified: Thu, 22 Oct 2020 02:20:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bbabb0d9883ceaafbb96aa45f4af26028284490ca6aa9b998982fffbd0de8d`  
		Last Modified: Thu, 22 Oct 2020 02:20:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b8b0280c0c57750295448b33f5585177c360ba3331fab6ce2209bebeb750b5`  
		Last Modified: Thu, 22 Oct 2020 02:20:27 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b8ae68f21657f99a78c35accfa81b273d4fb54394f37a427e98336aed2d536fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39103791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bf49477b99c8feb367ad880b495034920d284e1cc73e7a0ed4b9df8a207352e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:43:44 GMT
ENV CONSUL_VERSION=1.7.8
# Thu, 22 Oct 2020 02:43:46 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:43:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:44:02 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:44:05 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:44:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:44:08 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:44:09 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:44:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:44:11 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:44:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:44:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:44:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968982c6d6074d48939087574059ff72725e2958974fb5b80436f49161fdd115`  
		Last Modified: Thu, 22 Oct 2020 02:45:37 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5702da4067070094b526298b3a05abf0d2a9a8e0c60201bc7f1a6fc744d9d80`  
		Last Modified: Thu, 22 Oct 2020 02:46:03 GMT  
		Size: 36.4 MB (36393942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ccf2eb561e86187b01dfab1a20f1cf597967516917c1589489bd5e09c638b2`  
		Last Modified: Thu, 22 Oct 2020 02:45:37 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c2ba40bff249761f03bb4f4a5100e72cd0cf928ee37ef07015edcdbcf26153`  
		Last Modified: Thu, 22 Oct 2020 02:45:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04029515034058419f2d60d6c2dd1a06a6d10105a522f6d5575dd9c907249557`  
		Last Modified: Thu, 22 Oct 2020 02:45:37 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.8` - linux; 386

```console
$ docker pull consul@sha256:3926844f90e94a6f3be5bdbc889769528541d1e0be8b17c074b8073f922a36f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (42034053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3df2eac77c1efad58c3951fa319b458d1b7da01915f8a14a926a613f41d8873e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:33:16 GMT
ENV CONSUL_VERSION=1.7.8
# Thu, 22 Oct 2020 02:33:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:33:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:33:22 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:33:23 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:33:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:33:24 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:33:24 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:33:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:33:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:33:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:33:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846db40e649b58b8967aacf1f6f7a7d8627f1ffd6f918f6cb4367370d86f720e`  
		Last Modified: Thu, 22 Oct 2020 02:34:16 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731e87c48127e5fea1a2158e52aef1babde7f5bdc5f3fac254f813e8ac5871ab`  
		Last Modified: Thu, 22 Oct 2020 02:34:27 GMT  
		Size: 39.2 MB (39239414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef242b5bc816d7b2d2bc0a9a840fcc4a88c262936c3672739b5a2d91f32f711`  
		Last Modified: Thu, 22 Oct 2020 02:34:16 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e02e9eed1127a82a8898fea88eb8eb225449f970a78099c8fc7ac8348c9ab3`  
		Last Modified: Thu, 22 Oct 2020 02:34:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77e0f6a184523db8b8a646ce977a666df54ba7508f2021b178f413a2823a020e`  
		Last Modified: Thu, 22 Oct 2020 02:34:16 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:54f477fb5c9123db824e5392f948853512db018f512b1e87386c021a69089971
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:e9b4eca3141960e18f2c09d1dcc5e1232ddc8d3bc077b5577460b4d3ee96a7ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46719494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3945f796958277e335d0fc06f16ccf59b2ffe67b1550e820bfae255cd0e02362`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:34:51 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 21:34:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:34:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:34:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:34:57 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:34:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:34:58 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:34:58 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:34:59 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:34:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:34:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f53b97be57a8b151b90aec8c0bae62ff8fdc031c1f1e6b4aa5b2f89fbde0b0`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc3ccb924c034d384494391649d39785a32803293fa81ab720bcea287a190ec`  
		Last Modified: Fri, 11 Sep 2020 21:35:40 GMT  
		Size: 43.9 MB (43918715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16d05c330fa3bcea904ee0349c9181bc61c774f7cd5f9e5b2f2c09f36c7c5e`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed495875d84a63a5b86b2b9bb50739a6f2c4c2847882bfc7b39fc40171f2f3`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c418676c3be3c8a9a79211b1318c090eab2b0ff1bbc0cff682107f32b4c85f96`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:c28a31c07f5cca9c4a185fb2ca70c7422f43d625039a430e511b9a79645848e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41608414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:180e309df45a05a41c5ebd73534c7f90837ca0591c1f379779ceb95229fefc9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:17:57 GMT
ENV CONSUL_VERSION=1.8.4
# Thu, 22 Oct 2020 02:17:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:18:00 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:18:09 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:18:12 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:18:14 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:18:15 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:18:15 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:18:16 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:18:17 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:18:18 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:18:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:18:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fb392a1ca3d94269069b4b4620cd0e02511b701eda1fac1e5b79136a7b803e`  
		Last Modified: Thu, 22 Oct 2020 02:20:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca620e4d0315454f52e9fefcbda0aa131157295e1a9b4e365921516303ad9e25`  
		Last Modified: Thu, 22 Oct 2020 02:20:18 GMT  
		Size: 39.0 MB (39003207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1a80f56a15c383ce153047e4244c6edb01e6789086bdff9fd7407b830c50`  
		Last Modified: Thu, 22 Oct 2020 02:20:05 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a708821617e1abac3edc7141a16ffce71d9c15c2c7a3f524b3c18cc26f9ae`  
		Last Modified: Thu, 22 Oct 2020 02:20:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8faed379f80af1b8cf37981cbb17a094425fb99b6a80a8cb3ef951205981e2e`  
		Last Modified: Thu, 22 Oct 2020 02:20:05 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:0292ae2f7a1edb9c24ceb163993b00d7b01dba24747057b977b05365e3e8d28b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41774548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2672d707b0b94603b44b70d450ef7e4f3c15e1df6eeda8c876c6e251e6eee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:43:16 GMT
ENV CONSUL_VERSION=1.8.4
# Thu, 22 Oct 2020 02:43:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:43:19 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:43:26 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:43:30 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:43:32 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:43:32 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:43:33 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:43:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:43:35 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:43:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:43:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60bd458a3d5e9f7d484bad277af5c4e3d1e7a0eb0b395536a70fbc00fa06c31`  
		Last Modified: Thu, 22 Oct 2020 02:45:20 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee48b0248366fb18feaded9bd9a8132de87824ea5530fe9242feb0aa889d8ad5`  
		Last Modified: Thu, 22 Oct 2020 02:45:28 GMT  
		Size: 39.1 MB (39064701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd562b87edc6235d798834cdec6a75c12c6a22b2659f92749b6fdb279df735`  
		Last Modified: Thu, 22 Oct 2020 02:45:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b431a09a2983c07657b122847b5e570da613f365250cbdaf567a5a1de3836`  
		Last Modified: Thu, 22 Oct 2020 02:45:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03401417cf601f8a36d24c9cf06d66cf20df323068ead7818d5463071ae4b545`  
		Last Modified: Thu, 22 Oct 2020 02:45:19 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:ef0a03aa2f620b58fdf7a7ae000aa69c8503f115dfc597918722d324f3f04095
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45856870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8945eb2aa40bf7444d94339498292d5b4741f7f7e6eb717f2d23afe2ffcbcd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:33:02 GMT
ENV CONSUL_VERSION=1.8.4
# Thu, 22 Oct 2020 02:33:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:33:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:33:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:33:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:33:09 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:33:09 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:33:10 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:33:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:33:10 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:33:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:33:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:33:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267bda11844908ebac12317a001e99ba60b99692cf1c734fe1cddff7aeed7e5`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83774b722875108bfe40a515a84a5793493650c6ba335c2e9e33b9b1b25127f`  
		Last Modified: Thu, 22 Oct 2020 02:34:10 GMT  
		Size: 43.1 MB (43062231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ec319fd425602cfc76f78e677d068113f6e4d6f9c263a135c1c8b01f253af7`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76249c1f1f8d1620e917c66a5db5ce55fec2cf218aef466bb09fa66b55b3dcf`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001ad7f4b499c0bc2cccb20038a656a90920073a25919808b6594c1c02b9580d`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.4`

```console
$ docker pull consul@sha256:54f477fb5c9123db824e5392f948853512db018f512b1e87386c021a69089971
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.4` - linux; amd64

```console
$ docker pull consul@sha256:e9b4eca3141960e18f2c09d1dcc5e1232ddc8d3bc077b5577460b4d3ee96a7ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46719494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3945f796958277e335d0fc06f16ccf59b2ffe67b1550e820bfae255cd0e02362`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:34:51 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 21:34:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:34:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:34:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:34:57 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:34:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:34:58 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:34:58 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:34:59 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:34:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:34:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f53b97be57a8b151b90aec8c0bae62ff8fdc031c1f1e6b4aa5b2f89fbde0b0`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc3ccb924c034d384494391649d39785a32803293fa81ab720bcea287a190ec`  
		Last Modified: Fri, 11 Sep 2020 21:35:40 GMT  
		Size: 43.9 MB (43918715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16d05c330fa3bcea904ee0349c9181bc61c774f7cd5f9e5b2f2c09f36c7c5e`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed495875d84a63a5b86b2b9bb50739a6f2c4c2847882bfc7b39fc40171f2f3`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c418676c3be3c8a9a79211b1318c090eab2b0ff1bbc0cff682107f32b4c85f96`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:c28a31c07f5cca9c4a185fb2ca70c7422f43d625039a430e511b9a79645848e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41608414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:180e309df45a05a41c5ebd73534c7f90837ca0591c1f379779ceb95229fefc9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:17:57 GMT
ENV CONSUL_VERSION=1.8.4
# Thu, 22 Oct 2020 02:17:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:18:00 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:18:09 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:18:12 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:18:14 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:18:15 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:18:15 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:18:16 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:18:17 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:18:18 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:18:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:18:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fb392a1ca3d94269069b4b4620cd0e02511b701eda1fac1e5b79136a7b803e`  
		Last Modified: Thu, 22 Oct 2020 02:20:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca620e4d0315454f52e9fefcbda0aa131157295e1a9b4e365921516303ad9e25`  
		Last Modified: Thu, 22 Oct 2020 02:20:18 GMT  
		Size: 39.0 MB (39003207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1a80f56a15c383ce153047e4244c6edb01e6789086bdff9fd7407b830c50`  
		Last Modified: Thu, 22 Oct 2020 02:20:05 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a708821617e1abac3edc7141a16ffce71d9c15c2c7a3f524b3c18cc26f9ae`  
		Last Modified: Thu, 22 Oct 2020 02:20:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8faed379f80af1b8cf37981cbb17a094425fb99b6a80a8cb3ef951205981e2e`  
		Last Modified: Thu, 22 Oct 2020 02:20:05 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:0292ae2f7a1edb9c24ceb163993b00d7b01dba24747057b977b05365e3e8d28b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41774548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2672d707b0b94603b44b70d450ef7e4f3c15e1df6eeda8c876c6e251e6eee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:43:16 GMT
ENV CONSUL_VERSION=1.8.4
# Thu, 22 Oct 2020 02:43:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:43:19 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:43:26 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:43:30 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:43:32 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:43:32 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:43:33 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:43:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:43:35 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:43:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:43:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60bd458a3d5e9f7d484bad277af5c4e3d1e7a0eb0b395536a70fbc00fa06c31`  
		Last Modified: Thu, 22 Oct 2020 02:45:20 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee48b0248366fb18feaded9bd9a8132de87824ea5530fe9242feb0aa889d8ad5`  
		Last Modified: Thu, 22 Oct 2020 02:45:28 GMT  
		Size: 39.1 MB (39064701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd562b87edc6235d798834cdec6a75c12c6a22b2659f92749b6fdb279df735`  
		Last Modified: Thu, 22 Oct 2020 02:45:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b431a09a2983c07657b122847b5e570da613f365250cbdaf567a5a1de3836`  
		Last Modified: Thu, 22 Oct 2020 02:45:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03401417cf601f8a36d24c9cf06d66cf20df323068ead7818d5463071ae4b545`  
		Last Modified: Thu, 22 Oct 2020 02:45:19 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.4` - linux; 386

```console
$ docker pull consul@sha256:ef0a03aa2f620b58fdf7a7ae000aa69c8503f115dfc597918722d324f3f04095
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45856870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8945eb2aa40bf7444d94339498292d5b4741f7f7e6eb717f2d23afe2ffcbcd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:33:02 GMT
ENV CONSUL_VERSION=1.8.4
# Thu, 22 Oct 2020 02:33:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:33:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:33:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:33:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:33:09 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:33:09 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:33:10 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:33:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:33:10 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:33:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:33:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:33:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267bda11844908ebac12317a001e99ba60b99692cf1c734fe1cddff7aeed7e5`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83774b722875108bfe40a515a84a5793493650c6ba335c2e9e33b9b1b25127f`  
		Last Modified: Thu, 22 Oct 2020 02:34:10 GMT  
		Size: 43.1 MB (43062231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ec319fd425602cfc76f78e677d068113f6e4d6f9c263a135c1c8b01f253af7`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76249c1f1f8d1620e917c66a5db5ce55fec2cf218aef466bb09fa66b55b3dcf`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001ad7f4b499c0bc2cccb20038a656a90920073a25919808b6594c1c02b9580d`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.0-beta`

```console
$ docker pull consul@sha256:4efbaaafd1930f92adc7b05017c8f23b501c109130c89cbd02fecd9ef21eff7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.0-beta` - linux; amd64

```console
$ docker pull consul@sha256:93beed4c1164b3ea24799046c4be26d3e8bf4e5ff727fb3fde974c149824265a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47994383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:964d692fbce612e9e67a567be57bcb9859d0a0278375e93dfb4da70147842801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 12 Oct 2020 22:22:15 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Mon, 12 Oct 2020 22:22:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 12 Oct 2020 22:22:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 12 Oct 2020 22:22:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 12 Oct 2020 22:22:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 12 Oct 2020 22:22:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Oct 2020 22:22:22 GMT
VOLUME [/consul/data]
# Mon, 12 Oct 2020 22:22:22 GMT
EXPOSE 8300
# Mon, 12 Oct 2020 22:22:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 12 Oct 2020 22:22:23 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 12 Oct 2020 22:22:23 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 12 Oct 2020 22:22:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 22:22:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3017652a3d3658694bb2a2bb454b5fa6455549d6453beced201949d72a23bfe5`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b151ef90caabd14c7236bbf180a8b6df6df9487d87d10affbd8a9972e63db96`  
		Last Modified: Mon, 12 Oct 2020 22:23:14 GMT  
		Size: 45.2 MB (45193611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc5f1955835928aa40afef11414617267f87fd99dcef5b556f6160eab495728`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d067c492a0b8f26e8ff71a3ff2398c713059def8fac5358e58a858bacaaa88d`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee1fc1229b9953b6020dfaac75a9d3cfb4520118149eae1b273d9af6c8038dd`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta` - linux; arm variant v6

```console
$ docker pull consul@sha256:e7fc72551958e03470b8c03c19d09000a61b034832fbb55f0f4d738cd85de8b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42755955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb59ad52e173656e0d37e52ad3a2a4ec4a2f0ebf6c9c7afdd0fd0f5da58ca2cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:17:16 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Thu, 22 Oct 2020 02:17:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:17:19 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:17:29 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:17:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:17:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:17:37 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:17:38 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:17:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:17:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:17:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:17:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8eb599ef0b38d2b800e58e74a80f31d7487a726532c8f254d0e05bba6603385`  
		Last Modified: Thu, 22 Oct 2020 02:19:43 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4cec6230bd53ded39135fc8034bcce62320e90a5797428e5163be7b779ea92`  
		Last Modified: Thu, 22 Oct 2020 02:19:55 GMT  
		Size: 40.2 MB (40150746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab0596547824bed8f0b17196a88ba2af9967fc517221e8ea516753a1fe52335`  
		Last Modified: Thu, 22 Oct 2020 02:19:43 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b977009089ae5433276df5b2f18bc23cb00a63e99d941e5326a26944d85ac313`  
		Last Modified: Thu, 22 Oct 2020 02:19:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b252efd0fcdd733a2d9795e6c91ce4a9a45787ae12a9ad939cdc040486ffe812`  
		Last Modified: Thu, 22 Oct 2020 02:19:43 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:40546a0a57a5bca1e7df9b3fc2106ad962bd6784307ca5b374e57959608560d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42928725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d678b6b66c8d7e73effed28b73932b1f8f169b35235b3c8fd618bc3b9cd9e35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:42:39 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Thu, 22 Oct 2020 02:42:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:42:41 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:42:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:42:52 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:42:54 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:42:57 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:42:58 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:43:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:43:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:43:03 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:43:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:43:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7da2a8d23de5894604ad32a80a1f2d126d574b4a8c7cdf045a22fa0e4474b2`  
		Last Modified: Thu, 22 Oct 2020 02:45:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf97b02f0060a7ef5f6a44e897d20fe50b1820572e1d57f2d0a4c90399adaf3a`  
		Last Modified: Thu, 22 Oct 2020 02:45:12 GMT  
		Size: 40.2 MB (40218875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90f956b556e062ccf5b00512e74ad487505409e0c8c739a20c34b0b5be959a9`  
		Last Modified: Thu, 22 Oct 2020 02:45:04 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562e039c4c33e7fdffb4a8f85e7fda3c3ed3eff4261ee20608c3d144d0512afc`  
		Last Modified: Thu, 22 Oct 2020 02:45:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb23a4d41b227257d9c4d1c9452f49b5125ed9e4851f0690f88f3123ef661066`  
		Last Modified: Thu, 22 Oct 2020 02:45:04 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta` - linux; 386

```console
$ docker pull consul@sha256:5e065d9760024fe3580a52b9f063732fa986b52c91ff878399640bbd16faf894
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47138871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c68f91828b5d862325406a94f6ba7867a7c5cc90a4bdca28944e1b750ecc1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:32:48 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Thu, 22 Oct 2020 02:32:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:32:49 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:32:54 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:32:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:32:56 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:32:56 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:32:56 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:32:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:32:56 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:32:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:32:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:32:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9938449d4230918267ff788aabd4f1fb43fee53ade28166cba4854e13ee7d7e7`  
		Last Modified: Thu, 22 Oct 2020 02:33:50 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3248c43e54d8a39258c71eccacf966b1f371f15cb7de1c3b6104d9100ea8a5f1`  
		Last Modified: Thu, 22 Oct 2020 02:33:57 GMT  
		Size: 44.3 MB (44344230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0a0b3ecd556a5deda07794e649446be448e4f6347991a01e1c26bf6cf6b574`  
		Last Modified: Thu, 22 Oct 2020 02:33:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0dd6a9d0f77164977ec00259936c24a979ee022a753a7c9d72744a13359565`  
		Last Modified: Thu, 22 Oct 2020 02:33:50 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883cb925e3f5da96924b31152da91c1b2a599d78c0e77bc426b1cc1d1d610c6d`  
		Last Modified: Thu, 22 Oct 2020 02:33:49 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.0-beta1`

```console
$ docker pull consul@sha256:4efbaaafd1930f92adc7b05017c8f23b501c109130c89cbd02fecd9ef21eff7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.0-beta1` - linux; amd64

```console
$ docker pull consul@sha256:93beed4c1164b3ea24799046c4be26d3e8bf4e5ff727fb3fde974c149824265a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47994383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:964d692fbce612e9e67a567be57bcb9859d0a0278375e93dfb4da70147842801`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 12 Oct 2020 22:22:15 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Mon, 12 Oct 2020 22:22:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 12 Oct 2020 22:22:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 12 Oct 2020 22:22:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 12 Oct 2020 22:22:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 12 Oct 2020 22:22:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 12 Oct 2020 22:22:22 GMT
VOLUME [/consul/data]
# Mon, 12 Oct 2020 22:22:22 GMT
EXPOSE 8300
# Mon, 12 Oct 2020 22:22:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 12 Oct 2020 22:22:23 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 12 Oct 2020 22:22:23 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 12 Oct 2020 22:22:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 12 Oct 2020 22:22:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3017652a3d3658694bb2a2bb454b5fa6455549d6453beced201949d72a23bfe5`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b151ef90caabd14c7236bbf180a8b6df6df9487d87d10affbd8a9972e63db96`  
		Last Modified: Mon, 12 Oct 2020 22:23:14 GMT  
		Size: 45.2 MB (45193611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc5f1955835928aa40afef11414617267f87fd99dcef5b556f6160eab495728`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d067c492a0b8f26e8ff71a3ff2398c713059def8fac5358e58a858bacaaa88d`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee1fc1229b9953b6020dfaac75a9d3cfb4520118149eae1b273d9af6c8038dd`  
		Last Modified: Mon, 12 Oct 2020 22:22:42 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta1` - linux; arm variant v6

```console
$ docker pull consul@sha256:e7fc72551958e03470b8c03c19d09000a61b034832fbb55f0f4d738cd85de8b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42755955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb59ad52e173656e0d37e52ad3a2a4ec4a2f0ebf6c9c7afdd0fd0f5da58ca2cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:17:16 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Thu, 22 Oct 2020 02:17:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:17:19 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:17:29 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:17:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:17:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:17:37 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:17:38 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:17:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:17:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:17:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:17:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:17:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8eb599ef0b38d2b800e58e74a80f31d7487a726532c8f254d0e05bba6603385`  
		Last Modified: Thu, 22 Oct 2020 02:19:43 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4cec6230bd53ded39135fc8034bcce62320e90a5797428e5163be7b779ea92`  
		Last Modified: Thu, 22 Oct 2020 02:19:55 GMT  
		Size: 40.2 MB (40150746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ab0596547824bed8f0b17196a88ba2af9967fc517221e8ea516753a1fe52335`  
		Last Modified: Thu, 22 Oct 2020 02:19:43 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b977009089ae5433276df5b2f18bc23cb00a63e99d941e5326a26944d85ac313`  
		Last Modified: Thu, 22 Oct 2020 02:19:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b252efd0fcdd733a2d9795e6c91ce4a9a45787ae12a9ad939cdc040486ffe812`  
		Last Modified: Thu, 22 Oct 2020 02:19:43 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:40546a0a57a5bca1e7df9b3fc2106ad962bd6784307ca5b374e57959608560d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42928725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d678b6b66c8d7e73effed28b73932b1f8f169b35235b3c8fd618bc3b9cd9e35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:42:39 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Thu, 22 Oct 2020 02:42:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:42:41 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:42:49 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:42:52 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:42:54 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:42:57 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:42:58 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:43:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:43:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:43:03 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:43:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:43:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7da2a8d23de5894604ad32a80a1f2d126d574b4a8c7cdf045a22fa0e4474b2`  
		Last Modified: Thu, 22 Oct 2020 02:45:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf97b02f0060a7ef5f6a44e897d20fe50b1820572e1d57f2d0a4c90399adaf3a`  
		Last Modified: Thu, 22 Oct 2020 02:45:12 GMT  
		Size: 40.2 MB (40218875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90f956b556e062ccf5b00512e74ad487505409e0c8c739a20c34b0b5be959a9`  
		Last Modified: Thu, 22 Oct 2020 02:45:04 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562e039c4c33e7fdffb4a8f85e7fda3c3ed3eff4261ee20608c3d144d0512afc`  
		Last Modified: Thu, 22 Oct 2020 02:45:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb23a4d41b227257d9c4d1c9452f49b5125ed9e4851f0690f88f3123ef661066`  
		Last Modified: Thu, 22 Oct 2020 02:45:04 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta1` - linux; 386

```console
$ docker pull consul@sha256:5e065d9760024fe3580a52b9f063732fa986b52c91ff878399640bbd16faf894
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47138871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54c68f91828b5d862325406a94f6ba7867a7c5cc90a4bdca28944e1b750ecc1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:32:48 GMT
ENV CONSUL_VERSION=1.9.0-beta1
# Thu, 22 Oct 2020 02:32:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:32:49 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:32:54 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:32:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:32:56 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:32:56 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:32:56 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:32:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:32:56 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:32:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:32:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:32:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9938449d4230918267ff788aabd4f1fb43fee53ade28166cba4854e13ee7d7e7`  
		Last Modified: Thu, 22 Oct 2020 02:33:50 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3248c43e54d8a39258c71eccacf966b1f371f15cb7de1c3b6104d9100ea8a5f1`  
		Last Modified: Thu, 22 Oct 2020 02:33:57 GMT  
		Size: 44.3 MB (44344230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0a0b3ecd556a5deda07794e649446be448e4f6347991a01e1c26bf6cf6b574`  
		Last Modified: Thu, 22 Oct 2020 02:33:49 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0dd6a9d0f77164977ec00259936c24a979ee022a753a7c9d72744a13359565`  
		Last Modified: Thu, 22 Oct 2020 02:33:50 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883cb925e3f5da96924b31152da91c1b2a599d78c0e77bc426b1cc1d1d610c6d`  
		Last Modified: Thu, 22 Oct 2020 02:33:49 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:54f477fb5c9123db824e5392f948853512db018f512b1e87386c021a69089971
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:e9b4eca3141960e18f2c09d1dcc5e1232ddc8d3bc077b5577460b4d3ee96a7ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46719494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3945f796958277e335d0fc06f16ccf59b2ffe67b1550e820bfae255cd0e02362`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 11 Sep 2020 21:34:51 GMT
ENV CONSUL_VERSION=1.8.4
# Fri, 11 Sep 2020 21:34:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 11 Sep 2020 21:34:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 11 Sep 2020 21:34:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 11 Sep 2020 21:34:57 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 11 Sep 2020 21:34:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 11 Sep 2020 21:34:58 GMT
VOLUME [/consul/data]
# Fri, 11 Sep 2020 21:34:58 GMT
EXPOSE 8300
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 11 Sep 2020 21:34:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 11 Sep 2020 21:34:59 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 11 Sep 2020 21:34:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 11 Sep 2020 21:34:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f53b97be57a8b151b90aec8c0bae62ff8fdc031c1f1e6b4aa5b2f89fbde0b0`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc3ccb924c034d384494391649d39785a32803293fa81ab720bcea287a190ec`  
		Last Modified: Fri, 11 Sep 2020 21:35:40 GMT  
		Size: 43.9 MB (43918715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d16d05c330fa3bcea904ee0349c9181bc61c774f7cd5f9e5b2f2c09f36c7c5e`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ed495875d84a63a5b86b2b9bb50739a6f2c4c2847882bfc7b39fc40171f2f3`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c418676c3be3c8a9a79211b1318c090eab2b0ff1bbc0cff682107f32b4c85f96`  
		Last Modified: Fri, 11 Sep 2020 21:35:32 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:c28a31c07f5cca9c4a185fb2ca70c7422f43d625039a430e511b9a79645848e0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41608414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:180e309df45a05a41c5ebd73534c7f90837ca0591c1f379779ceb95229fefc9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:17:57 GMT
ENV CONSUL_VERSION=1.8.4
# Thu, 22 Oct 2020 02:17:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:18:00 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:18:09 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:18:12 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:18:14 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:18:15 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:18:15 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:18:16 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:18:17 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:18:18 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:18:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:18:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fb392a1ca3d94269069b4b4620cd0e02511b701eda1fac1e5b79136a7b803e`  
		Last Modified: Thu, 22 Oct 2020 02:20:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca620e4d0315454f52e9fefcbda0aa131157295e1a9b4e365921516303ad9e25`  
		Last Modified: Thu, 22 Oct 2020 02:20:18 GMT  
		Size: 39.0 MB (39003207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74c1a80f56a15c383ce153047e4244c6edb01e6789086bdff9fd7407b830c50`  
		Last Modified: Thu, 22 Oct 2020 02:20:05 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3a708821617e1abac3edc7141a16ffce71d9c15c2c7a3f524b3c18cc26f9ae`  
		Last Modified: Thu, 22 Oct 2020 02:20:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8faed379f80af1b8cf37981cbb17a094425fb99b6a80a8cb3ef951205981e2e`  
		Last Modified: Thu, 22 Oct 2020 02:20:05 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:0292ae2f7a1edb9c24ceb163993b00d7b01dba24747057b977b05365e3e8d28b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41774548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f2672d707b0b94603b44b70d450ef7e4f3c15e1df6eeda8c876c6e251e6eee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:43:16 GMT
ENV CONSUL_VERSION=1.8.4
# Thu, 22 Oct 2020 02:43:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:43:19 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:43:26 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:43:30 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:43:32 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:43:32 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:43:33 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:43:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:43:35 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:43:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:43:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:43:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60bd458a3d5e9f7d484bad277af5c4e3d1e7a0eb0b395536a70fbc00fa06c31`  
		Last Modified: Thu, 22 Oct 2020 02:45:20 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee48b0248366fb18feaded9bd9a8132de87824ea5530fe9242feb0aa889d8ad5`  
		Last Modified: Thu, 22 Oct 2020 02:45:28 GMT  
		Size: 39.1 MB (39064701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd562b87edc6235d798834cdec6a75c12c6a22b2659f92749b6fdb279df735`  
		Last Modified: Thu, 22 Oct 2020 02:45:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72b431a09a2983c07657b122847b5e570da613f365250cbdaf567a5a1de3836`  
		Last Modified: Thu, 22 Oct 2020 02:45:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03401417cf601f8a36d24c9cf06d66cf20df323068ead7818d5463071ae4b545`  
		Last Modified: Thu, 22 Oct 2020 02:45:19 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:ef0a03aa2f620b58fdf7a7ae000aa69c8503f115dfc597918722d324f3f04095
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45856870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd8945eb2aa40bf7444d94339498292d5b4741f7f7e6eb717f2d23afe2ffcbcd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 02:33:02 GMT
ENV CONSUL_VERSION=1.8.4
# Thu, 22 Oct 2020 02:33:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 02:33:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 02:33:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 02:33:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 02:33:09 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 02:33:09 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 02:33:10 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 02:33:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 02:33:10 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 02:33:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 02:33:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 02:33:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267bda11844908ebac12317a001e99ba60b99692cf1c734fe1cddff7aeed7e5`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83774b722875108bfe40a515a84a5793493650c6ba335c2e9e33b9b1b25127f`  
		Last Modified: Thu, 22 Oct 2020 02:34:10 GMT  
		Size: 43.1 MB (43062231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ec319fd425602cfc76f78e677d068113f6e4d6f9c263a135c1c8b01f253af7`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76249c1f1f8d1620e917c66a5db5ce55fec2cf218aef466bb09fa66b55b3dcf`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001ad7f4b499c0bc2cccb20038a656a90920073a25919808b6594c1c02b9580d`  
		Last Modified: Thu, 22 Oct 2020 02:34:02 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
