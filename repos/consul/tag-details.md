<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.6`](#consul16)
-	[`consul:1.6.9`](#consul169)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.9`](#consul179)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.5`](#consul185)
-	[`consul:1.9.0-beta`](#consul190-beta)
-	[`consul:1.9.0-beta2`](#consul190-beta2)
-	[`consul:latest`](#consullatest)

## `consul:1.6`

```console
$ docker pull consul@sha256:cb126a8ba3b1e9338d836344d7b348022561910b2b4b9c01e37ef1d75149e306
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6` - linux; amd64

```console
$ docker pull consul@sha256:5b5f1b3ba3465882a2aebcaaea977ae4f34f0737419a20a54f5e25c81c2f99af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41876435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5207934c0f7102ad1f56bc59d0463fa4b0db22f914e3579663e2eaf74c2a2863`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 03:18:33 GMT
ENV CONSUL_VERSION=1.6.9
# Thu, 22 Oct 2020 03:18:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 03:18:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 03:18:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 03:18:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 03:18:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:18:40 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 03:18:40 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 03:18:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 03:18:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 03:18:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 03:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:18:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cc3f32f0e27d7fac726129817fae6878496c1b4c62b4a7325c2ea7e697e66c`  
		Last Modified: Thu, 22 Oct 2020 03:19:35 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c6fad90b4c6d56b701482b4e231fffd52a9c134d5a41575debf9efcf273231`  
		Last Modified: Thu, 22 Oct 2020 03:19:41 GMT  
		Size: 39.1 MB (39076342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dbf5206913830fa67c472f42d776334ef4e10fa30e51abe9078545998faaf4`  
		Last Modified: Thu, 22 Oct 2020 03:19:35 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d53a2aaf01b1ef3df39ff27cc598238d76da9262f38dd741df52f9144961a14`  
		Last Modified: Thu, 22 Oct 2020 03:19:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c47673cd83f6bc5efeb05cb3df7cfc82bae8018ee2885afb14965e55612088`  
		Last Modified: Thu, 22 Oct 2020 03:19:35 GMT  
		Size: 1.7 KB (1705 bytes)  
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
$ docker pull consul@sha256:cb126a8ba3b1e9338d836344d7b348022561910b2b4b9c01e37ef1d75149e306
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6.9` - linux; amd64

```console
$ docker pull consul@sha256:5b5f1b3ba3465882a2aebcaaea977ae4f34f0737419a20a54f5e25c81c2f99af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41876435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5207934c0f7102ad1f56bc59d0463fa4b0db22f914e3579663e2eaf74c2a2863`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 22 Oct 2020 03:18:33 GMT
ENV CONSUL_VERSION=1.6.9
# Thu, 22 Oct 2020 03:18:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 22 Oct 2020 03:18:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 22 Oct 2020 03:18:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 22 Oct 2020 03:18:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 22 Oct 2020 03:18:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 22 Oct 2020 03:18:40 GMT
VOLUME [/consul/data]
# Thu, 22 Oct 2020 03:18:40 GMT
EXPOSE 8300
# Thu, 22 Oct 2020 03:18:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 22 Oct 2020 03:18:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 22 Oct 2020 03:18:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 22 Oct 2020 03:18:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 22 Oct 2020 03:18:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cc3f32f0e27d7fac726129817fae6878496c1b4c62b4a7325c2ea7e697e66c`  
		Last Modified: Thu, 22 Oct 2020 03:19:35 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c6fad90b4c6d56b701482b4e231fffd52a9c134d5a41575debf9efcf273231`  
		Last Modified: Thu, 22 Oct 2020 03:19:41 GMT  
		Size: 39.1 MB (39076342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dbf5206913830fa67c472f42d776334ef4e10fa30e51abe9078545998faaf4`  
		Last Modified: Thu, 22 Oct 2020 03:19:35 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d53a2aaf01b1ef3df39ff27cc598238d76da9262f38dd741df52f9144961a14`  
		Last Modified: Thu, 22 Oct 2020 03:19:35 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c47673cd83f6bc5efeb05cb3df7cfc82bae8018ee2885afb14965e55612088`  
		Last Modified: Thu, 22 Oct 2020 03:19:35 GMT  
		Size: 1.7 KB (1705 bytes)  
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
$ docker pull consul@sha256:7b954dd6711f97152351d96165ac2befb331f2445f0f70fffa9e3540d61902a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:c26aa3600b67e72524aea18743d106b910e04a469b90d4fa588a06547173f3d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43103077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45d8ac75f45916816c893d4b3a03c70332c51d8daddf6c65e55a8d52459d6f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:19:54 GMT
ENV CONSUL_VERSION=1.7.9
# Tue, 10 Nov 2020 00:19:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:19:55 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:20:00 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:20:01 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:20:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:20:02 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:20:02 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:20:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:20:03 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:20:03 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:20:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:20:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c30a83d82862c73e8fe68dbf7bd156a449aa462e8c9684d9454e26bc7c420af`  
		Last Modified: Tue, 10 Nov 2020 00:20:30 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f5b0a0c0cc0c39ac944fa27f36515aefa4f60364898612be92aefdfc5f893`  
		Last Modified: Tue, 10 Nov 2020 00:20:37 GMT  
		Size: 40.3 MB (40302979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471876f84ad3000f8ce1ef977d818bcf829f6579fb60def6d0b338d47afa09b2`  
		Last Modified: Tue, 10 Nov 2020 00:20:31 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5e8019c869e9ba65bdbee66368d9d074435f9c9ef30121d102f12f7af9d459`  
		Last Modified: Tue, 10 Nov 2020 00:20:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dd8d1d934b1851da00d69396daf0bf2907e34219f37ddb26a91cad89e86166`  
		Last Modified: Tue, 10 Nov 2020 00:20:30 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:0812f853781b95843fae738052b046648e687ad7cfd66d468d88a00624151421
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38804219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e2c1cda44431b50a9a9cef062aa9eb3e1bc45b9edd0fbeadee9afbf7ea352d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:50:32 GMT
ENV CONSUL_VERSION=1.7.9
# Tue, 10 Nov 2020 00:50:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:50:39 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:50:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:50:51 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:50:54 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:50:55 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:50:55 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:50:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:50:57 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:50:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:50:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaf5206b49f57822c76d1196c30037ec5794766205996725fc16dd7f23a9ce4`  
		Last Modified: Tue, 10 Nov 2020 00:51:40 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f88f8cb22e73c8f79c4ab555433ccb485182c21aaada1b4e6ecdd8ac4ddfeb`  
		Last Modified: Tue, 10 Nov 2020 00:51:50 GMT  
		Size: 36.2 MB (36199008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65715849e83e86ef849415dc8127771083c391ebae001f5b7a206e727ca14084`  
		Last Modified: Tue, 10 Nov 2020 00:51:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfe6a69cd7e4d4db731839077c2350f5a408bada1b969ba26027247317dbc6c`  
		Last Modified: Tue, 10 Nov 2020 00:51:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b2902dd09e8a53cc72c43235ca8184807d3fe57cae3421a11c710d91386b9c`  
		Last Modified: Tue, 10 Nov 2020 00:51:41 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:158473f170531ae1a59d241874f74c7046653847f80c5b1c9e89cd29e807cc33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39016197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f666704300617b79bbf2880f42ec82491eb7121429a88c6cc783e087a5b1269d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:40:23 GMT
ENV CONSUL_VERSION=1.7.9
# Tue, 10 Nov 2020 00:40:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:40:28 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:40:37 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:40:40 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:40:46 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:40:49 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:40:53 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:40:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:41:05 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:41:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:41:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:41:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8738962314ae1bee76797d9701d864854fd9506b718b0777cdd3a409dc448b8d`  
		Last Modified: Tue, 10 Nov 2020 00:41:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0951496aa41ad5410b3073e1ebcdb0f85797e6d6cd0669d87215422e95671924`  
		Last Modified: Tue, 10 Nov 2020 00:42:01 GMT  
		Size: 36.3 MB (36306342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23578ed1d93e7bc57564db4d8896aad1913d72cc549b8be8d9fdfd11b5ab5206`  
		Last Modified: Tue, 10 Nov 2020 00:41:52 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968b142dbe05e055a57622dc33d128b1cc49332cb48a147dc01c1668bc2eae4b`  
		Last Modified: Tue, 10 Nov 2020 00:41:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea9b551827e061d641afbd06c20f166f115f3871a36fb47a1b5264d6b77c5b4`  
		Last Modified: Tue, 10 Nov 2020 00:41:52 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:58f5af98f07040c72a0a54231077a92210c5628dbb11cb605ac13ea6e278d1ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41897054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41699beae2fc1248f1a8752d340ed90c6db8d91c71742159a1a25a58bbd50f38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:38:45 GMT
ENV CONSUL_VERSION=1.7.9
# Tue, 10 Nov 2020 00:38:46 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:38:46 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:38:51 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:38:52 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:38:53 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:38:53 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:38:53 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:38:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:38:54 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:38:54 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:38:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:38:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f7f961bf531deb5ce8efc65c416413aeb8ba0246c803ab33fce867057df76d`  
		Last Modified: Tue, 10 Nov 2020 00:39:27 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067308e3322d9d6f07a75512e30c8f8bdae23e15560457b3671a48e3b86940b3`  
		Last Modified: Tue, 10 Nov 2020 00:39:34 GMT  
		Size: 39.1 MB (39102414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed90c091a175fc0a9ed1b51e23ca7e3227c05f99ccf6460237def400256d92b3`  
		Last Modified: Tue, 10 Nov 2020 00:39:26 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637dcae92e8bcf912819529f5b70722b43984f43e361b47ff9cbb1e8262aeb0e`  
		Last Modified: Tue, 10 Nov 2020 00:39:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf1e63633861c8f3a7d9b33c908ecf0c67a7965efab414ae1569f9510a45694`  
		Last Modified: Tue, 10 Nov 2020 00:39:26 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.9`

```console
$ docker pull consul@sha256:7b954dd6711f97152351d96165ac2befb331f2445f0f70fffa9e3540d61902a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.9` - linux; amd64

```console
$ docker pull consul@sha256:c26aa3600b67e72524aea18743d106b910e04a469b90d4fa588a06547173f3d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43103077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45d8ac75f45916816c893d4b3a03c70332c51d8daddf6c65e55a8d52459d6f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:19:54 GMT
ENV CONSUL_VERSION=1.7.9
# Tue, 10 Nov 2020 00:19:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:19:55 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:20:00 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:20:01 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:20:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:20:02 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:20:02 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:20:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:20:03 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:20:03 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:20:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:20:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c30a83d82862c73e8fe68dbf7bd156a449aa462e8c9684d9454e26bc7c420af`  
		Last Modified: Tue, 10 Nov 2020 00:20:30 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6f5b0a0c0cc0c39ac944fa27f36515aefa4f60364898612be92aefdfc5f893`  
		Last Modified: Tue, 10 Nov 2020 00:20:37 GMT  
		Size: 40.3 MB (40302979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471876f84ad3000f8ce1ef977d818bcf829f6579fb60def6d0b338d47afa09b2`  
		Last Modified: Tue, 10 Nov 2020 00:20:31 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5e8019c869e9ba65bdbee66368d9d074435f9c9ef30121d102f12f7af9d459`  
		Last Modified: Tue, 10 Nov 2020 00:20:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dd8d1d934b1851da00d69396daf0bf2907e34219f37ddb26a91cad89e86166`  
		Last Modified: Tue, 10 Nov 2020 00:20:30 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:0812f853781b95843fae738052b046648e687ad7cfd66d468d88a00624151421
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38804219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35e2c1cda44431b50a9a9cef062aa9eb3e1bc45b9edd0fbeadee9afbf7ea352d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:50:32 GMT
ENV CONSUL_VERSION=1.7.9
# Tue, 10 Nov 2020 00:50:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:50:39 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:50:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:50:51 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:50:54 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:50:55 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:50:55 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:50:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:50:57 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:50:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:50:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:50:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaf5206b49f57822c76d1196c30037ec5794766205996725fc16dd7f23a9ce4`  
		Last Modified: Tue, 10 Nov 2020 00:51:40 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f88f8cb22e73c8f79c4ab555433ccb485182c21aaada1b4e6ecdd8ac4ddfeb`  
		Last Modified: Tue, 10 Nov 2020 00:51:50 GMT  
		Size: 36.2 MB (36199008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65715849e83e86ef849415dc8127771083c391ebae001f5b7a206e727ca14084`  
		Last Modified: Tue, 10 Nov 2020 00:51:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cfe6a69cd7e4d4db731839077c2350f5a408bada1b969ba26027247317dbc6c`  
		Last Modified: Tue, 10 Nov 2020 00:51:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b2902dd09e8a53cc72c43235ca8184807d3fe57cae3421a11c710d91386b9c`  
		Last Modified: Tue, 10 Nov 2020 00:51:41 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:158473f170531ae1a59d241874f74c7046653847f80c5b1c9e89cd29e807cc33
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39016197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f666704300617b79bbf2880f42ec82491eb7121429a88c6cc783e087a5b1269d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:40:23 GMT
ENV CONSUL_VERSION=1.7.9
# Tue, 10 Nov 2020 00:40:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:40:28 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:40:37 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:40:40 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:40:46 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:40:49 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:40:53 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:40:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:41:05 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:41:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:41:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:41:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8738962314ae1bee76797d9701d864854fd9506b718b0777cdd3a409dc448b8d`  
		Last Modified: Tue, 10 Nov 2020 00:41:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0951496aa41ad5410b3073e1ebcdb0f85797e6d6cd0669d87215422e95671924`  
		Last Modified: Tue, 10 Nov 2020 00:42:01 GMT  
		Size: 36.3 MB (36306342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23578ed1d93e7bc57564db4d8896aad1913d72cc549b8be8d9fdfd11b5ab5206`  
		Last Modified: Tue, 10 Nov 2020 00:41:52 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968b142dbe05e055a57622dc33d128b1cc49332cb48a147dc01c1668bc2eae4b`  
		Last Modified: Tue, 10 Nov 2020 00:41:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea9b551827e061d641afbd06c20f166f115f3871a36fb47a1b5264d6b77c5b4`  
		Last Modified: Tue, 10 Nov 2020 00:41:52 GMT  
		Size: 1.7 KB (1711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.9` - linux; 386

```console
$ docker pull consul@sha256:58f5af98f07040c72a0a54231077a92210c5628dbb11cb605ac13ea6e278d1ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41897054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41699beae2fc1248f1a8752d340ed90c6db8d91c71742159a1a25a58bbd50f38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:38:45 GMT
ENV CONSUL_VERSION=1.7.9
# Tue, 10 Nov 2020 00:38:46 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:38:46 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:38:51 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:38:52 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:38:53 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:38:53 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:38:53 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:38:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:38:54 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:38:54 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:38:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:38:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f7f961bf531deb5ce8efc65c416413aeb8ba0246c803ab33fce867057df76d`  
		Last Modified: Tue, 10 Nov 2020 00:39:27 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067308e3322d9d6f07a75512e30c8f8bdae23e15560457b3671a48e3b86940b3`  
		Last Modified: Tue, 10 Nov 2020 00:39:34 GMT  
		Size: 39.1 MB (39102414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed90c091a175fc0a9ed1b51e23ca7e3227c05f99ccf6460237def400256d92b3`  
		Last Modified: Tue, 10 Nov 2020 00:39:26 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637dcae92e8bcf912819529f5b70722b43984f43e361b47ff9cbb1e8262aeb0e`  
		Last Modified: Tue, 10 Nov 2020 00:39:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bf1e63633861c8f3a7d9b33c908ecf0c67a7965efab414ae1569f9510a45694`  
		Last Modified: Tue, 10 Nov 2020 00:39:26 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:b85322aa8c65355341dd81b5e95d5c0e8468e6419724d4e8a125198d40426a30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:43eb37c372432743a4a7334f41dfde3aeac2e08ec6698c79cb23a6550898bff3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46463818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f7b214361a700e6ca4a014ff49035be3678c9375ba478a7b20bd0859bdcd9a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:19:39 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:19:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:19:40 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:19:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:19:45 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:19:46 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:19:46 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:19:46 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:19:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:19:47 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:19:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:19:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd0ad15d15483ddb156f9f3f293505ab3d80dd4f0298f988e53879107c17045`  
		Last Modified: Sat, 24 Oct 2020 00:20:05 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30a01add5552182d8cf627fb6bfafb1bd6404bd9e8964d0f318e75ac909292`  
		Last Modified: Sat, 24 Oct 2020 00:20:11 GMT  
		Size: 43.7 MB (43663725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f3ae3ba267f18945e80a9a9d9b1aa4e960addad7330381e1eebeb178e893c1`  
		Last Modified: Sat, 24 Oct 2020 00:20:06 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de0e80834954020a245984ab98e3a34b047ac702b81eb4674171d53caf4c95b`  
		Last Modified: Sat, 24 Oct 2020 00:20:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f607b07c9f2cfc208634b1170ebbfa675e6de56058826fec0ede6e593289b`  
		Last Modified: Sat, 24 Oct 2020 00:20:05 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:9cba8ea4acf03eec79ac41b0b0e86ef5d23819bcfaab38ad7d12aa4af5e3f86d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41724116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e7e84124bc9a52ebf375f54aa75182a64a07c13a9941e005da0cf936bcfb94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:50:53 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:50:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:50:55 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:51:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:51:06 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:51:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:51:10 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:51:11 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:51:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:51:13 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:51:13 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:51:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab63e1d933b90542c55c0589580d0ae8a9e2158b1a513a3f48ad426b6b19dc5`  
		Last Modified: Sat, 24 Oct 2020 00:51:36 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadae91cd7b954aab20e1a7852252f1d899656643f5a93419082e227368c1ba9`  
		Last Modified: Sat, 24 Oct 2020 00:51:48 GMT  
		Size: 39.1 MB (39118908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4aefd409dfcff320e4f4abc93acd6b79c75be32a4f8e945a7973b16e906f371`  
		Last Modified: Sat, 24 Oct 2020 00:51:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee425345016882213d153f7d97b63547b624b495d324a12f56499a64ec4bff4`  
		Last Modified: Sat, 24 Oct 2020 00:51:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2fb9fc2e5b60fa972411f03c730ae9062ba8f15afb38eb1bdda9787ec92001`  
		Last Modified: Sat, 24 Oct 2020 00:51:37 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b000c9a1b959e6e0f6a44e692719b859bbcf0a1dfce1457923223ad813de00ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41902164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbca14e16df0a545915052fd53f21614a74fc15be4d8f29f8c0b3778726f9feb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:39:48 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:39:49 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:39:51 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:39:58 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:40:00 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:40:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:40:02 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:40:03 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:40:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:40:04 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:40:04 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:40:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b6d3b9131728e261c4c4fc3af4cdd89e6dcba8ab1ab38c3c0f914e2eb39560`  
		Last Modified: Sat, 24 Oct 2020 00:40:31 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea498f059520372848099a86a79729c7818c4aebc0f8a0fe20587c848e59f415`  
		Last Modified: Sat, 24 Oct 2020 00:40:39 GMT  
		Size: 39.2 MB (39192313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9301e6a3342587e952ba4823d9d46356ef7f784b57e2e9fd46f14bfe405a08b6`  
		Last Modified: Sat, 24 Oct 2020 00:40:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d987f7d735d43368f22b2d5f0382da052100071025a829c766e8cc328f30f0`  
		Last Modified: Sat, 24 Oct 2020 00:40:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8904802b6e26f57003d8bce038eca94dc3b115a409726918967d41a91ab1a1`  
		Last Modified: Sat, 24 Oct 2020 00:40:31 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:b2b1abf3a45a2d4aab2e52e4211de930519d7602b448cd4ff1497c4783f2b59e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45976028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c8c5f30e70866e42e6cd1d5fca57611f44e3806485c2834b90d0a279e121cd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:38:28 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:38:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:38:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:38:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:38:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:38:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:38:36 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:38:36 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:38:37 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50575978b96251e969c7433bf747ff9948c7569cdba08b82642c9ff28dc3dad8`  
		Last Modified: Sat, 24 Oct 2020 00:38:57 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0bd61c7abe46d0a8800e07b99771a4a177768e7951b6e4bc406ef8c1ba5672`  
		Last Modified: Sat, 24 Oct 2020 00:39:04 GMT  
		Size: 43.2 MB (43181392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df109c109076c96fc724f585f9e9b2decc3c9c96a51c0a26891089492f2a793b`  
		Last Modified: Sat, 24 Oct 2020 00:38:57 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c51e22ab172236135e965946eaf3a7a7a54768ec71cf853a1a6b18c4326df4`  
		Last Modified: Sat, 24 Oct 2020 00:38:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf571036f9872b050d07d5272ddeebf9629fa2af03e0dac3456433ac857abca`  
		Last Modified: Sat, 24 Oct 2020 00:38:56 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.5`

```console
$ docker pull consul@sha256:b85322aa8c65355341dd81b5e95d5c0e8468e6419724d4e8a125198d40426a30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.5` - linux; amd64

```console
$ docker pull consul@sha256:43eb37c372432743a4a7334f41dfde3aeac2e08ec6698c79cb23a6550898bff3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46463818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f7b214361a700e6ca4a014ff49035be3678c9375ba478a7b20bd0859bdcd9a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:19:39 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:19:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:19:40 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:19:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:19:45 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:19:46 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:19:46 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:19:46 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:19:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:19:47 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:19:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:19:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd0ad15d15483ddb156f9f3f293505ab3d80dd4f0298f988e53879107c17045`  
		Last Modified: Sat, 24 Oct 2020 00:20:05 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30a01add5552182d8cf627fb6bfafb1bd6404bd9e8964d0f318e75ac909292`  
		Last Modified: Sat, 24 Oct 2020 00:20:11 GMT  
		Size: 43.7 MB (43663725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f3ae3ba267f18945e80a9a9d9b1aa4e960addad7330381e1eebeb178e893c1`  
		Last Modified: Sat, 24 Oct 2020 00:20:06 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de0e80834954020a245984ab98e3a34b047ac702b81eb4674171d53caf4c95b`  
		Last Modified: Sat, 24 Oct 2020 00:20:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f607b07c9f2cfc208634b1170ebbfa675e6de56058826fec0ede6e593289b`  
		Last Modified: Sat, 24 Oct 2020 00:20:05 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.5` - linux; arm variant v6

```console
$ docker pull consul@sha256:9cba8ea4acf03eec79ac41b0b0e86ef5d23819bcfaab38ad7d12aa4af5e3f86d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41724116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e7e84124bc9a52ebf375f54aa75182a64a07c13a9941e005da0cf936bcfb94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:50:53 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:50:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:50:55 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:51:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:51:06 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:51:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:51:10 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:51:11 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:51:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:51:13 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:51:13 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:51:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab63e1d933b90542c55c0589580d0ae8a9e2158b1a513a3f48ad426b6b19dc5`  
		Last Modified: Sat, 24 Oct 2020 00:51:36 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadae91cd7b954aab20e1a7852252f1d899656643f5a93419082e227368c1ba9`  
		Last Modified: Sat, 24 Oct 2020 00:51:48 GMT  
		Size: 39.1 MB (39118908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4aefd409dfcff320e4f4abc93acd6b79c75be32a4f8e945a7973b16e906f371`  
		Last Modified: Sat, 24 Oct 2020 00:51:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee425345016882213d153f7d97b63547b624b495d324a12f56499a64ec4bff4`  
		Last Modified: Sat, 24 Oct 2020 00:51:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2fb9fc2e5b60fa972411f03c730ae9062ba8f15afb38eb1bdda9787ec92001`  
		Last Modified: Sat, 24 Oct 2020 00:51:37 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.5` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b000c9a1b959e6e0f6a44e692719b859bbcf0a1dfce1457923223ad813de00ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41902164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbca14e16df0a545915052fd53f21614a74fc15be4d8f29f8c0b3778726f9feb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:39:48 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:39:49 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:39:51 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:39:58 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:40:00 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:40:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:40:02 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:40:03 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:40:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:40:04 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:40:04 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:40:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b6d3b9131728e261c4c4fc3af4cdd89e6dcba8ab1ab38c3c0f914e2eb39560`  
		Last Modified: Sat, 24 Oct 2020 00:40:31 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea498f059520372848099a86a79729c7818c4aebc0f8a0fe20587c848e59f415`  
		Last Modified: Sat, 24 Oct 2020 00:40:39 GMT  
		Size: 39.2 MB (39192313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9301e6a3342587e952ba4823d9d46356ef7f784b57e2e9fd46f14bfe405a08b6`  
		Last Modified: Sat, 24 Oct 2020 00:40:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d987f7d735d43368f22b2d5f0382da052100071025a829c766e8cc328f30f0`  
		Last Modified: Sat, 24 Oct 2020 00:40:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8904802b6e26f57003d8bce038eca94dc3b115a409726918967d41a91ab1a1`  
		Last Modified: Sat, 24 Oct 2020 00:40:31 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.5` - linux; 386

```console
$ docker pull consul@sha256:b2b1abf3a45a2d4aab2e52e4211de930519d7602b448cd4ff1497c4783f2b59e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45976028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c8c5f30e70866e42e6cd1d5fca57611f44e3806485c2834b90d0a279e121cd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:38:28 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:38:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:38:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:38:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:38:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:38:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:38:36 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:38:36 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:38:37 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50575978b96251e969c7433bf747ff9948c7569cdba08b82642c9ff28dc3dad8`  
		Last Modified: Sat, 24 Oct 2020 00:38:57 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0bd61c7abe46d0a8800e07b99771a4a177768e7951b6e4bc406ef8c1ba5672`  
		Last Modified: Sat, 24 Oct 2020 00:39:04 GMT  
		Size: 43.2 MB (43181392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df109c109076c96fc724f585f9e9b2decc3c9c96a51c0a26891089492f2a793b`  
		Last Modified: Sat, 24 Oct 2020 00:38:57 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c51e22ab172236135e965946eaf3a7a7a54768ec71cf853a1a6b18c4326df4`  
		Last Modified: Sat, 24 Oct 2020 00:38:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf571036f9872b050d07d5272ddeebf9629fa2af03e0dac3456433ac857abca`  
		Last Modified: Sat, 24 Oct 2020 00:38:56 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.0-beta`

```console
$ docker pull consul@sha256:9cd5e3ad48fd9677cdbc6ed57824d4ba2528bcf7884757e8d39720f30e8bc072
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.0-beta` - linux; amd64

```console
$ docker pull consul@sha256:2897fdd00e856fc1645d1af65e4ff410ed76afd2b0080eae37d7259a84be73e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47613032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d27404aaf8003ee5c2c6d5eabba784a80458542cc3253367eb08ebffcfe2365`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:19:37 GMT
ENV CONSUL_VERSION=1.9.0-beta2
# Tue, 10 Nov 2020 00:19:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:19:38 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:19:43 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:19:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:19:45 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:19:45 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:19:45 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:19:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:19:45 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:19:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:19:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223da4bd7281cd2ef68d023b276dfed6867aa1ca3e8f7a4bc65cc7a8ec5ade30`  
		Last Modified: Tue, 10 Nov 2020 00:20:19 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e39b318901911e0c27a5b3fa40c461da6f5a967c535b168ba149c9ff24ae28`  
		Last Modified: Tue, 10 Nov 2020 00:20:25 GMT  
		Size: 44.8 MB (44812934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c421e84c97e65083cbce0cd833d4c84686ec6ee61836a9314b2e3a422363c611`  
		Last Modified: Tue, 10 Nov 2020 00:20:19 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964ca9b2d56c363928b1adefd9fa6ab932b0664e0a391e9e981f8a804be99c31`  
		Last Modified: Tue, 10 Nov 2020 00:20:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582415e604e8debaf22db05eb6101d0b6553ee8ecb5a5b806af85dbff0f4d481`  
		Last Modified: Tue, 10 Nov 2020 00:20:19 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta` - linux; arm variant v6

```console
$ docker pull consul@sha256:ff8d3a5138c26b87f23d19cc660fdba93ddc80fa0f4c9b59b05b3fb640b28ead
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42753228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4585257c32a497765a97852393e654be8bdc55ff68026e38e7365bb3143b3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:49:45 GMT
ENV CONSUL_VERSION=1.9.0-beta2
# Tue, 10 Nov 2020 00:49:46 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:49:51 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:50:00 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:50:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:50:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:50:09 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:50:10 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:50:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:50:14 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:50:16 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:50:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e131a5df145f881404fc0abe80afe7455b2568951b0551a0817d6a8d5baf716c`  
		Last Modified: Tue, 10 Nov 2020 00:51:19 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375e7de02144ac5cac3e38da0a5d885a104a043943a8584ac2077a66cd9dd901`  
		Last Modified: Tue, 10 Nov 2020 00:51:29 GMT  
		Size: 40.1 MB (40148014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f959500cb16977f084c383b5f50c34113ad41e134893eea43cb16463d0c2d1a7`  
		Last Modified: Tue, 10 Nov 2020 00:51:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840d5a58ef3842ba935459a18cd3459b388cb1699a96aad18677fd0957aa7f2c`  
		Last Modified: Tue, 10 Nov 2020 00:51:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7087c272b0d4e98e1a9264a988090a2254b774df4ac3b921b415c0c455e2a029`  
		Last Modified: Tue, 10 Nov 2020 00:51:19 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:aea9366ca108201e5890dbe13c9cb111f3bfe2ba14845aba5bb863241718df36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42929266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeeeaf7eb6f16764562bac6cac7049577144557a1ace183f79a2c1111e598f18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:39:41 GMT
ENV CONSUL_VERSION=1.9.0-beta2
# Tue, 10 Nov 2020 00:39:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:39:45 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:39:51 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:39:54 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:39:56 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:39:59 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:40:01 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:40:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:40:06 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:40:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:40:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf41dd54644063fdcebf45fc3cc2027f2fb16293f1b385d0b9a5b45169fb031`  
		Last Modified: Tue, 10 Nov 2020 00:41:33 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45cd727b67bdea06ee2570dbe2de062f76b53fb4caceaf27ff48b0646b739f5`  
		Last Modified: Tue, 10 Nov 2020 00:41:43 GMT  
		Size: 40.2 MB (40219416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ead836df91ce8f402f8b2a3772043586e362d1034c3b4840d5972a25bf2f8d`  
		Last Modified: Tue, 10 Nov 2020 00:41:33 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9876995714e1816ef92fe8c36cd09ae5cbf89a7a0565d59d68b3b208c8cfec5f`  
		Last Modified: Tue, 10 Nov 2020 00:41:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9beb9d8d025e105e891ff0d238e25a8d69dce0d53d7fa1b9173414e91320d11d`  
		Last Modified: Tue, 10 Nov 2020 00:41:33 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta` - linux; 386

```console
$ docker pull consul@sha256:2f56896038022a6cac8863a243c2fbb90c6bc91d8bbfe914821369cb05b906c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47124361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c743767eea6fede292d808f11438eb85045796c9ac7c29c08c820cbecd2a279`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:38:28 GMT
ENV CONSUL_VERSION=1.9.0-beta2
# Tue, 10 Nov 2020 00:38:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:38:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:38:35 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:38:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:38:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:38:36 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:38:36 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:38:37 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:38:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1639f104c4cbd743f8afd60edfc2a3655d4c6215d544394c02c029c227e530a7`  
		Last Modified: Tue, 10 Nov 2020 00:39:10 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3db6d7198ad0b8dc982b51e2f2a02cf78411c235db15e0ef8f75b71393dc45`  
		Last Modified: Tue, 10 Nov 2020 00:39:17 GMT  
		Size: 44.3 MB (44329718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b339fdf401a8f6a80559a34ea1dff7809225a0560630bc21245e81f18fb8da`  
		Last Modified: Tue, 10 Nov 2020 00:39:11 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89a1ab42fadff3e21014b873b2d63e291b6270e05ca61be946b37d765bece5f`  
		Last Modified: Tue, 10 Nov 2020 00:39:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c86e68114e8882a4985d51c5411b6fe606d0375b923cab7169f01c67a9d3f3`  
		Last Modified: Tue, 10 Nov 2020 00:39:10 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.0-beta2`

```console
$ docker pull consul@sha256:9cd5e3ad48fd9677cdbc6ed57824d4ba2528bcf7884757e8d39720f30e8bc072
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.0-beta2` - linux; amd64

```console
$ docker pull consul@sha256:2897fdd00e856fc1645d1af65e4ff410ed76afd2b0080eae37d7259a84be73e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47613032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d27404aaf8003ee5c2c6d5eabba784a80458542cc3253367eb08ebffcfe2365`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:19:37 GMT
ENV CONSUL_VERSION=1.9.0-beta2
# Tue, 10 Nov 2020 00:19:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:19:38 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:19:43 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:19:44 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:19:45 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:19:45 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:19:45 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:19:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:19:45 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:19:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:19:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223da4bd7281cd2ef68d023b276dfed6867aa1ca3e8f7a4bc65cc7a8ec5ade30`  
		Last Modified: Tue, 10 Nov 2020 00:20:19 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e39b318901911e0c27a5b3fa40c461da6f5a967c535b168ba149c9ff24ae28`  
		Last Modified: Tue, 10 Nov 2020 00:20:25 GMT  
		Size: 44.8 MB (44812934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c421e84c97e65083cbce0cd833d4c84686ec6ee61836a9314b2e3a422363c611`  
		Last Modified: Tue, 10 Nov 2020 00:20:19 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964ca9b2d56c363928b1adefd9fa6ab932b0664e0a391e9e981f8a804be99c31`  
		Last Modified: Tue, 10 Nov 2020 00:20:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582415e604e8debaf22db05eb6101d0b6553ee8ecb5a5b806af85dbff0f4d481`  
		Last Modified: Tue, 10 Nov 2020 00:20:19 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta2` - linux; arm variant v6

```console
$ docker pull consul@sha256:ff8d3a5138c26b87f23d19cc660fdba93ddc80fa0f4c9b59b05b3fb640b28ead
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42753228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4585257c32a497765a97852393e654be8bdc55ff68026e38e7365bb3143b3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:49:45 GMT
ENV CONSUL_VERSION=1.9.0-beta2
# Tue, 10 Nov 2020 00:49:46 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:49:51 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:50:00 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:50:04 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:50:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:50:09 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:50:10 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:50:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:50:14 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:50:16 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:50:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e131a5df145f881404fc0abe80afe7455b2568951b0551a0817d6a8d5baf716c`  
		Last Modified: Tue, 10 Nov 2020 00:51:19 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375e7de02144ac5cac3e38da0a5d885a104a043943a8584ac2077a66cd9dd901`  
		Last Modified: Tue, 10 Nov 2020 00:51:29 GMT  
		Size: 40.1 MB (40148014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f959500cb16977f084c383b5f50c34113ad41e134893eea43cb16463d0c2d1a7`  
		Last Modified: Tue, 10 Nov 2020 00:51:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840d5a58ef3842ba935459a18cd3459b388cb1699a96aad18677fd0957aa7f2c`  
		Last Modified: Tue, 10 Nov 2020 00:51:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7087c272b0d4e98e1a9264a988090a2254b774df4ac3b921b415c0c455e2a029`  
		Last Modified: Tue, 10 Nov 2020 00:51:19 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:aea9366ca108201e5890dbe13c9cb111f3bfe2ba14845aba5bb863241718df36
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42929266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeeeaf7eb6f16764562bac6cac7049577144557a1ace183f79a2c1111e598f18`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:39:41 GMT
ENV CONSUL_VERSION=1.9.0-beta2
# Tue, 10 Nov 2020 00:39:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:39:45 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:39:51 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:39:54 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:39:56 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:39:59 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:40:01 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:40:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:40:06 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:40:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:40:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf41dd54644063fdcebf45fc3cc2027f2fb16293f1b385d0b9a5b45169fb031`  
		Last Modified: Tue, 10 Nov 2020 00:41:33 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45cd727b67bdea06ee2570dbe2de062f76b53fb4caceaf27ff48b0646b739f5`  
		Last Modified: Tue, 10 Nov 2020 00:41:43 GMT  
		Size: 40.2 MB (40219416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ead836df91ce8f402f8b2a3772043586e362d1034c3b4840d5972a25bf2f8d`  
		Last Modified: Tue, 10 Nov 2020 00:41:33 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9876995714e1816ef92fe8c36cd09ae5cbf89a7a0565d59d68b3b208c8cfec5f`  
		Last Modified: Tue, 10 Nov 2020 00:41:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9beb9d8d025e105e891ff0d238e25a8d69dce0d53d7fa1b9173414e91320d11d`  
		Last Modified: Tue, 10 Nov 2020 00:41:33 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.0-beta2` - linux; 386

```console
$ docker pull consul@sha256:2f56896038022a6cac8863a243c2fbb90c6bc91d8bbfe914821369cb05b906c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47124361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c743767eea6fede292d808f11438eb85045796c9ac7c29c08c820cbecd2a279`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 10 Nov 2020 00:38:28 GMT
ENV CONSUL_VERSION=1.9.0-beta2
# Tue, 10 Nov 2020 00:38:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 10 Nov 2020 00:38:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 10 Nov 2020 00:38:35 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 10 Nov 2020 00:38:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 10 Nov 2020 00:38:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 10 Nov 2020 00:38:36 GMT
VOLUME [/consul/data]
# Tue, 10 Nov 2020 00:38:36 GMT
EXPOSE 8300
# Tue, 10 Nov 2020 00:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 10 Nov 2020 00:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 10 Nov 2020 00:38:37 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 10 Nov 2020 00:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 10 Nov 2020 00:38:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1639f104c4cbd743f8afd60edfc2a3655d4c6215d544394c02c029c227e530a7`  
		Last Modified: Tue, 10 Nov 2020 00:39:10 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3db6d7198ad0b8dc982b51e2f2a02cf78411c235db15e0ef8f75b71393dc45`  
		Last Modified: Tue, 10 Nov 2020 00:39:17 GMT  
		Size: 44.3 MB (44329718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b339fdf401a8f6a80559a34ea1dff7809225a0560630bc21245e81f18fb8da`  
		Last Modified: Tue, 10 Nov 2020 00:39:11 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89a1ab42fadff3e21014b873b2d63e291b6270e05ca61be946b37d765bece5f`  
		Last Modified: Tue, 10 Nov 2020 00:39:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c86e68114e8882a4985d51c5411b6fe606d0375b923cab7169f01c67a9d3f3`  
		Last Modified: Tue, 10 Nov 2020 00:39:10 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:b85322aa8c65355341dd81b5e95d5c0e8468e6419724d4e8a125198d40426a30
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:43eb37c372432743a4a7334f41dfde3aeac2e08ec6698c79cb23a6550898bff3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46463818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f7b214361a700e6ca4a014ff49035be3678c9375ba478a7b20bd0859bdcd9a9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:17:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:19:39 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:19:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:19:40 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:19:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:19:45 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:19:46 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:19:46 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:19:46 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:19:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:19:47 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:19:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:19:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd0ad15d15483ddb156f9f3f293505ab3d80dd4f0298f988e53879107c17045`  
		Last Modified: Sat, 24 Oct 2020 00:20:05 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d30a01add5552182d8cf627fb6bfafb1bd6404bd9e8964d0f318e75ac909292`  
		Last Modified: Sat, 24 Oct 2020 00:20:11 GMT  
		Size: 43.7 MB (43663725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f3ae3ba267f18945e80a9a9d9b1aa4e960addad7330381e1eebeb178e893c1`  
		Last Modified: Sat, 24 Oct 2020 00:20:06 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de0e80834954020a245984ab98e3a34b047ac702b81eb4674171d53caf4c95b`  
		Last Modified: Sat, 24 Oct 2020 00:20:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000f607b07c9f2cfc208634b1170ebbfa675e6de56058826fec0ede6e593289b`  
		Last Modified: Sat, 24 Oct 2020 00:20:05 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:9cba8ea4acf03eec79ac41b0b0e86ef5d23819bcfaab38ad7d12aa4af5e3f86d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41724116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28e7e84124bc9a52ebf375f54aa75182a64a07c13a9941e005da0cf936bcfb94`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:17:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:50:53 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:50:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:50:55 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:51:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:51:06 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:51:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:51:10 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:51:11 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:51:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:51:13 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:51:13 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:51:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:51:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab63e1d933b90542c55c0589580d0ae8a9e2158b1a513a3f48ad426b6b19dc5`  
		Last Modified: Sat, 24 Oct 2020 00:51:36 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadae91cd7b954aab20e1a7852252f1d899656643f5a93419082e227368c1ba9`  
		Last Modified: Sat, 24 Oct 2020 00:51:48 GMT  
		Size: 39.1 MB (39118908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4aefd409dfcff320e4f4abc93acd6b79c75be32a4f8e945a7973b16e906f371`  
		Last Modified: Sat, 24 Oct 2020 00:51:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee425345016882213d153f7d97b63547b624b495d324a12f56499a64ec4bff4`  
		Last Modified: Sat, 24 Oct 2020 00:51:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2fb9fc2e5b60fa972411f03c730ae9062ba8f15afb38eb1bdda9787ec92001`  
		Last Modified: Sat, 24 Oct 2020 00:51:37 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b000c9a1b959e6e0f6a44e692719b859bbcf0a1dfce1457923223ad813de00ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41902164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbca14e16df0a545915052fd53f21614a74fc15be4d8f29f8c0b3778726f9feb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:42:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:39:48 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:39:49 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:39:51 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:39:58 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:40:00 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:40:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:40:02 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:40:03 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:40:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:40:04 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:40:04 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:40:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3b6d3b9131728e261c4c4fc3af4cdd89e6dcba8ab1ab38c3c0f914e2eb39560`  
		Last Modified: Sat, 24 Oct 2020 00:40:31 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea498f059520372848099a86a79729c7818c4aebc0f8a0fe20587c848e59f415`  
		Last Modified: Sat, 24 Oct 2020 00:40:39 GMT  
		Size: 39.2 MB (39192313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9301e6a3342587e952ba4823d9d46356ef7f784b57e2e9fd46f14bfe405a08b6`  
		Last Modified: Sat, 24 Oct 2020 00:40:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d987f7d735d43368f22b2d5f0382da052100071025a829c766e8cc328f30f0`  
		Last Modified: Sat, 24 Oct 2020 00:40:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc8904802b6e26f57003d8bce038eca94dc3b115a409726918967d41a91ab1a1`  
		Last Modified: Sat, 24 Oct 2020 00:40:31 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:b2b1abf3a45a2d4aab2e52e4211de930519d7602b448cd4ff1497c4783f2b59e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45976028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c8c5f30e70866e42e6cd1d5fca57611f44e3806485c2834b90d0a279e121cd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 02:32:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 24 Oct 2020 00:38:28 GMT
ENV CONSUL_VERSION=1.8.5
# Sat, 24 Oct 2020 00:38:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 24 Oct 2020 00:38:29 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 24 Oct 2020 00:38:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 24 Oct 2020 00:38:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 24 Oct 2020 00:38:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 24 Oct 2020 00:38:36 GMT
VOLUME [/consul/data]
# Sat, 24 Oct 2020 00:38:36 GMT
EXPOSE 8300
# Sat, 24 Oct 2020 00:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 24 Oct 2020 00:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 24 Oct 2020 00:38:37 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 24 Oct 2020 00:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 24 Oct 2020 00:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50575978b96251e969c7433bf747ff9948c7569cdba08b82642c9ff28dc3dad8`  
		Last Modified: Sat, 24 Oct 2020 00:38:57 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0bd61c7abe46d0a8800e07b99771a4a177768e7951b6e4bc406ef8c1ba5672`  
		Last Modified: Sat, 24 Oct 2020 00:39:04 GMT  
		Size: 43.2 MB (43181392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df109c109076c96fc724f585f9e9b2decc3c9c96a51c0a26891089492f2a793b`  
		Last Modified: Sat, 24 Oct 2020 00:38:57 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c51e22ab172236135e965946eaf3a7a7a54768ec71cf853a1a6b18c4326df4`  
		Last Modified: Sat, 24 Oct 2020 00:38:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf571036f9872b050d07d5272ddeebf9629fa2af03e0dac3456433ac857abca`  
		Last Modified: Sat, 24 Oct 2020 00:38:56 GMT  
		Size: 1.7 KB (1701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
