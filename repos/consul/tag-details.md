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
$ docker pull consul@sha256:f38830adbdeb98ae091077bd01a2c7ce2522dafa9baff247afb11726f5d1b23a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:73d7837259fe925e083bc5c4299377409df977ab1e4a3f7cf6d12f7dedb51c92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43109497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540024263411f620aa8a17c93efaa51bd9eca28dde5c8661ce2f921728f1d181`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 24 Feb 2021 21:19:57 GMT
ARG CONSUL_VERSION=1.7.12
# Wed, 24 Feb 2021 21:19:57 GMT
LABEL org.opencontainers.image.version=1.7.12
# Wed, 24 Feb 2021 21:19:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 24 Feb 2021 21:19:59 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 24 Feb 2021 21:20:08 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 24 Feb 2021 21:20:09 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 24 Feb 2021 21:20:10 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:20:10 GMT
VOLUME [/consul/data]
# Wed, 24 Feb 2021 21:20:10 GMT
EXPOSE 8300
# Wed, 24 Feb 2021 21:20:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 24 Feb 2021 21:20:11 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 24 Feb 2021 21:20:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 21:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:20:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2785cec4ba498fcba748252781799fc4f401dec767f24a4af3be0ecf2fbec00f`  
		Last Modified: Wed, 24 Feb 2021 21:21:01 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de04a3634d5da9ea8428384d03ba055e1224c525dcfc701b229e330574eddb0`  
		Last Modified: Wed, 24 Feb 2021 21:21:08 GMT  
		Size: 40.3 MB (40306774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ca2e0f91f93554273dff9d4632eb9474975b9c41b5e804a85f9ec93fb149ec`  
		Last Modified: Wed, 24 Feb 2021 21:21:02 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc98d1bf879ed15433b27102ab01a64d0a28be1e85cfe7730dddf7ea77184d0`  
		Last Modified: Wed, 24 Feb 2021 21:21:01 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbfa6885d14da90f8a2159d7971593d7e96c079930a47092b1108d6576a07e83`  
		Last Modified: Wed, 24 Feb 2021 21:21:01 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:c179ecdef358f351fac3afb04321654c1554930aa3b793fcc246a333d8e33f23
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38829572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1920af3658a3b67f2c693ff2a985d9de8f969dcd22990bcbc52115be74dd1a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:08:49 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:52:34 GMT
ARG CONSUL_VERSION=1.7.13
# Sat, 06 Mar 2021 01:52:35 GMT
LABEL org.opencontainers.image.version=1.7.13
# Sat, 06 Mar 2021 01:52:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:52:39 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:54:59 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:55:02 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:55:05 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:55:07 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:55:07 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:55:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:55:10 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:55:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:55:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:55:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cebd1781d5b4951d886c6746e6b830685b1e87ec26729af74c0a86d95ee908f`  
		Last Modified: Sat, 06 Mar 2021 01:56:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e283df1e8b789fa3a672b80c98dfa22e0556ca3965a9353095395133bb33d9`  
		Last Modified: Sat, 06 Mar 2021 01:56:20 GMT  
		Size: 36.2 MB (36221758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d13e1b4827cc2d8b7acd8e175b5516fa38f00a6e57702d6fab62165ddba5dd8`  
		Last Modified: Sat, 06 Mar 2021 01:56:10 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562a8fa2ad347311ad633f140f35008e54a7c3a85903c116bca8e7ea15dfe5b5`  
		Last Modified: Sat, 06 Mar 2021 01:56:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a06bfb9187e803e0f2c6a638d31cd2292a22fd549f70e79638a81b29093291`  
		Last Modified: Sat, 06 Mar 2021 01:56:09 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:c9a722f04f4fcf962bf06b863a512755d14c3400797810ea45beb6f91a52a662
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39044384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e227efaffabb4e733d987843f78cd69fb80a2018ff8623c2f0cef160243fafcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:29:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:40:44 GMT
ARG CONSUL_VERSION=1.7.13
# Sat, 06 Mar 2021 01:40:45 GMT
LABEL org.opencontainers.image.version=1.7.13
# Sat, 06 Mar 2021 01:40:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:40:47 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:40:53 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:40:56 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:40:58 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:40:58 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:40:59 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:41:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:41:00 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:41:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:41:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:41:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e98ab9c36bed7cd96968272d16b684cbbd5af80baa9fddda75d15e0fdae6ba`  
		Last Modified: Sat, 06 Mar 2021 01:41:51 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9def8db5e7928046613750b833584ef616255b98faccec9bfd510ec07608c910`  
		Last Modified: Sat, 06 Mar 2021 01:42:01 GMT  
		Size: 36.3 MB (36331208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ad2eed92c922e45efa44587c6db5a6ae6ea78336467a4452cb8d170af69eae`  
		Last Modified: Sat, 06 Mar 2021 01:41:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f698cd341e7540b08e5d098b728da61cf2db7867a3e0a92c9ac97ca259f009`  
		Last Modified: Sat, 06 Mar 2021 01:41:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ac6e6070dfe0456106a6a9664205d6b8edc4d30e33af93d7b02e0cd22afbb5`  
		Last Modified: Sat, 06 Mar 2021 01:41:52 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:815a213b1201ea1e86b5fa5a27722916ea4c6a1e3e247463acfb4d04215f92c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41906837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:789515f75590466ba33f0adad049207cd0d99a1b56438833f1a6f6d31b0f309f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 20:55:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 24 Feb 2021 20:55:38 GMT
ARG CONSUL_VERSION=1.7.12
# Wed, 24 Feb 2021 20:55:38 GMT
LABEL org.opencontainers.image.version=1.7.12
# Wed, 24 Feb 2021 20:55:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 24 Feb 2021 20:55:39 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 24 Feb 2021 20:55:45 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 24 Feb 2021 20:55:45 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 24 Feb 2021 20:55:46 GMT
# ARGS: CONSUL_VERSION=1.7.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 20:55:46 GMT
VOLUME [/consul/data]
# Wed, 24 Feb 2021 20:55:47 GMT
EXPOSE 8300
# Wed, 24 Feb 2021 20:55:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 24 Feb 2021 20:55:47 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 24 Feb 2021 20:55:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 20:55:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 20:55:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea8f950aeecbcc7d559863b8a06226a5594acefed366f1da98bb69137cd8c4e`  
		Last Modified: Wed, 24 Feb 2021 20:56:29 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86e71274113ef1614b90fdee71ad0ec2ab1c3faee59924aa45099d56c1f71a`  
		Last Modified: Wed, 24 Feb 2021 20:56:37 GMT  
		Size: 39.1 MB (39108856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd4f863928d80df77b389bea2ba52577d3be9ee13c4ecfcbbe8454948060965`  
		Last Modified: Wed, 24 Feb 2021 20:56:29 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a473c6fbbc3f4b1499570ea27d3bc9c12fa1ee368b544f99cf80929f2afcc3`  
		Last Modified: Wed, 24 Feb 2021 20:56:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38901b4c81ccc34f16b011871ef0c5192180dc38bd532770a8dc4b3cdcd63ba9`  
		Last Modified: Wed, 24 Feb 2021 20:56:29 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.13`

```console
$ docker pull consul@sha256:684f562f15d889c6c40591243c39d0bf214e3f5b6cc6a30c4a038d67ad6b73c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `consul:1.7.13` - linux; arm variant v6

```console
$ docker pull consul@sha256:c179ecdef358f351fac3afb04321654c1554930aa3b793fcc246a333d8e33f23
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38829572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1920af3658a3b67f2c693ff2a985d9de8f969dcd22990bcbc52115be74dd1a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:08:49 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:52:34 GMT
ARG CONSUL_VERSION=1.7.13
# Sat, 06 Mar 2021 01:52:35 GMT
LABEL org.opencontainers.image.version=1.7.13
# Sat, 06 Mar 2021 01:52:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:52:39 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:54:59 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:55:02 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:55:05 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:55:07 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:55:07 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:55:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:55:10 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:55:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:55:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:55:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cebd1781d5b4951d886c6746e6b830685b1e87ec26729af74c0a86d95ee908f`  
		Last Modified: Sat, 06 Mar 2021 01:56:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e283df1e8b789fa3a672b80c98dfa22e0556ca3965a9353095395133bb33d9`  
		Last Modified: Sat, 06 Mar 2021 01:56:20 GMT  
		Size: 36.2 MB (36221758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d13e1b4827cc2d8b7acd8e175b5516fa38f00a6e57702d6fab62165ddba5dd8`  
		Last Modified: Sat, 06 Mar 2021 01:56:10 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:562a8fa2ad347311ad633f140f35008e54a7c3a85903c116bca8e7ea15dfe5b5`  
		Last Modified: Sat, 06 Mar 2021 01:56:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a06bfb9187e803e0f2c6a638d31cd2292a22fd549f70e79638a81b29093291`  
		Last Modified: Sat, 06 Mar 2021 01:56:09 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.13` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:c9a722f04f4fcf962bf06b863a512755d14c3400797810ea45beb6f91a52a662
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39044384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e227efaffabb4e733d987843f78cd69fb80a2018ff8623c2f0cef160243fafcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:29:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:40:44 GMT
ARG CONSUL_VERSION=1.7.13
# Sat, 06 Mar 2021 01:40:45 GMT
LABEL org.opencontainers.image.version=1.7.13
# Sat, 06 Mar 2021 01:40:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:40:47 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:40:53 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:40:56 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:40:58 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:40:58 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:40:59 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:41:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:41:00 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:41:01 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:41:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:41:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e98ab9c36bed7cd96968272d16b684cbbd5af80baa9fddda75d15e0fdae6ba`  
		Last Modified: Sat, 06 Mar 2021 01:41:51 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9def8db5e7928046613750b833584ef616255b98faccec9bfd510ec07608c910`  
		Last Modified: Sat, 06 Mar 2021 01:42:01 GMT  
		Size: 36.3 MB (36331208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ad2eed92c922e45efa44587c6db5a6ae6ea78336467a4452cb8d170af69eae`  
		Last Modified: Sat, 06 Mar 2021 01:41:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f698cd341e7540b08e5d098b728da61cf2db7867a3e0a92c9ac97ca259f009`  
		Last Modified: Sat, 06 Mar 2021 01:41:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ac6e6070dfe0456106a6a9664205d6b8edc4d30e33af93d7b02e0cd22afbb5`  
		Last Modified: Sat, 06 Mar 2021 01:41:52 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:4f0f6170d84b647dba1470638add3c092e04589ff6ef46ed996301cec7015141
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:2eebae1a25cfb180a454335d3574fb8d234b97300ec73a648b6380642a2b7cb0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46506320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a612af4eda80843e370c1bdc92c8e10a5d7a9674e536586f7c2f09d57df9fb6b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 24 Feb 2021 21:19:43 GMT
ARG CONSUL_VERSION=1.8.8
# Wed, 24 Feb 2021 21:19:43 GMT
LABEL org.opencontainers.image.version=1.8.8
# Wed, 24 Feb 2021 21:19:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 24 Feb 2021 21:19:44 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 24 Feb 2021 21:19:49 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 24 Feb 2021 21:19:50 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 24 Feb 2021 21:19:51 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:19:51 GMT
VOLUME [/consul/data]
# Wed, 24 Feb 2021 21:19:52 GMT
EXPOSE 8300
# Wed, 24 Feb 2021 21:19:52 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 24 Feb 2021 21:19:52 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 24 Feb 2021 21:19:52 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 21:19:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:19:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ee609be1391429b3766e6ac4288a5f3d309438ad51d9e9025ed047858574e2`  
		Last Modified: Wed, 24 Feb 2021 21:20:48 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b951ddc6c7a6aa3278bc0cdd01b56e438bb2a0109bfdbd75b6ebeb2acbb2b9df`  
		Last Modified: Wed, 24 Feb 2021 21:20:54 GMT  
		Size: 43.7 MB (43703595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a042aef537b5d5dc1e80dc21a4c5afc925583db3ba63dea0bee61afd96695a9`  
		Last Modified: Wed, 24 Feb 2021 21:20:47 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ac6df9e8395ca5777cc0faedd032cf9abe70cc8cca5bdd89a39942decd05f7`  
		Last Modified: Wed, 24 Feb 2021 21:20:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a80219dd727c080fc4d07e0dccf78cecbaca68d08db0e62c8d7121c34e35a81`  
		Last Modified: Wed, 24 Feb 2021 21:20:47 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:063481f25cd9af8cbaa22aca770e5987e4fec4ad41dd4b8910a9d874c6a6c8dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41786797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9eef936adc7afa3f05e0afad9f049776027d0f41f65b8f121045c2b90339e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:08:49 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:52:02 GMT
ARG CONSUL_VERSION=1.8.9
# Sat, 06 Mar 2021 01:52:03 GMT
LABEL org.opencontainers.image.version=1.8.9
# Sat, 06 Mar 2021 01:52:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:52:07 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:52:16 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:52:18 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:52:20 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:52:21 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:52:22 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:52:22 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:52:23 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:52:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:52:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24277549321b59b3f0478097be319b2bfdef5bb067c652bc89c5f03881a2854`  
		Last Modified: Sat, 06 Mar 2021 01:55:51 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf052660b95a8db1b1ba4326350473f1e1fb34ea78a373a4871e96ef5699f4f`  
		Last Modified: Sat, 06 Mar 2021 01:56:01 GMT  
		Size: 39.2 MB (39178987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beadb945879e66936cb9642c9a3630b264ade60d53f7648bc559fe8b2f139533`  
		Last Modified: Sat, 06 Mar 2021 01:55:51 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4c53b10d6a2696762cdc0f535fe573f771d3333dd7ca5af6ef3b90945f28d3`  
		Last Modified: Sat, 06 Mar 2021 01:55:50 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbb7ddd57a3b8bc8f273017e9ada43a9790b8b479aae5c378dfac4a3050af7c`  
		Last Modified: Sat, 06 Mar 2021 01:55:50 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:64505afd8214bad2f88c9b387ba2ac0776cad02ef64bdedd54fffe35a1c0bff3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41954275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2e52d02c3713651dc7e30ebc9e05e1b3f2c87058b63b78291ce7044a00b2f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:29:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:40:16 GMT
ARG CONSUL_VERSION=1.8.9
# Sat, 06 Mar 2021 01:40:17 GMT
LABEL org.opencontainers.image.version=1.8.9
# Sat, 06 Mar 2021 01:40:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:40:20 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:40:26 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:40:28 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:40:30 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:40:31 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:40:32 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:40:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:40:33 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:40:34 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:40:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:40:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49118f7327ac707f4143297de7ac045ec8c753e74809ae7534de42be82682500`  
		Last Modified: Sat, 06 Mar 2021 01:41:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d44069345c849c39fe962d2f55dc7f7b3adb784c7a5ac0c8a829661e1636efa`  
		Last Modified: Sat, 06 Mar 2021 01:41:44 GMT  
		Size: 39.2 MB (39241098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7f76aa2289746c0525dad0941bb579ed5cb67e4cbf2d3c05f7776838feec88`  
		Last Modified: Sat, 06 Mar 2021 01:41:34 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bf8691e049d2fd912bed04170b056a8573c39feb632d27a1e21f7443728d8c`  
		Last Modified: Sat, 06 Mar 2021 01:41:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deea873381a2808abfe7ba9393eb855cc8a2ae9f5247196b8f45da6bd3a5cfc2`  
		Last Modified: Sat, 06 Mar 2021 01:41:35 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:545df4dfc31f93f06e557a8620b5c6101bb57525719f48ca3ccc63a494100c7e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46005161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85a2629fc939833aec7de29e23d0cae93467093afc2de7af97fb9eac28597307`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 20:55:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 24 Feb 2021 20:55:18 GMT
ARG CONSUL_VERSION=1.8.8
# Wed, 24 Feb 2021 20:55:19 GMT
LABEL org.opencontainers.image.version=1.8.8
# Wed, 24 Feb 2021 20:55:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 24 Feb 2021 20:55:20 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 24 Feb 2021 20:55:30 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 24 Feb 2021 20:55:31 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 24 Feb 2021 20:55:32 GMT
# ARGS: CONSUL_VERSION=1.8.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 20:55:32 GMT
VOLUME [/consul/data]
# Wed, 24 Feb 2021 20:55:32 GMT
EXPOSE 8300
# Wed, 24 Feb 2021 20:55:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 24 Feb 2021 20:55:33 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 24 Feb 2021 20:55:33 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 20:55:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 20:55:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53618af4970523c2bca671a34cd38b368cf818b1400f18722b45bfd6b6df6b1c`  
		Last Modified: Wed, 24 Feb 2021 20:56:15 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a3f61853569fc014b13fcba9e37275765b2196d3c5bdf29f995c151e53ffb46`  
		Last Modified: Wed, 24 Feb 2021 20:56:24 GMT  
		Size: 43.2 MB (43207179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd836d41cf73d3f346500e9acab45d986e33334fab498cf6488eaf64ed4bba6`  
		Last Modified: Wed, 24 Feb 2021 20:56:15 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e07c782896de40fd9b34cff71aa41ff5970981581ff7391af04514011c3270`  
		Last Modified: Wed, 24 Feb 2021 20:56:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5200aff1394c7ee8ba0b78e139075a200b6b2c21d453864f01e9c278c68c62b5`  
		Last Modified: Wed, 24 Feb 2021 20:56:15 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.9`

```console
$ docker pull consul@sha256:bec124fad818d13ab242dda8e99a02c20f9dce2cc06d81d275d47e6861a008e8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `consul:1.8.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:063481f25cd9af8cbaa22aca770e5987e4fec4ad41dd4b8910a9d874c6a6c8dc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41786797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9eef936adc7afa3f05e0afad9f049776027d0f41f65b8f121045c2b90339e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:08:49 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:52:02 GMT
ARG CONSUL_VERSION=1.8.9
# Sat, 06 Mar 2021 01:52:03 GMT
LABEL org.opencontainers.image.version=1.8.9
# Sat, 06 Mar 2021 01:52:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:52:07 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:52:16 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:52:18 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:52:20 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:52:21 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:52:22 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:52:22 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:52:23 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:52:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:52:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:52:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24277549321b59b3f0478097be319b2bfdef5bb067c652bc89c5f03881a2854`  
		Last Modified: Sat, 06 Mar 2021 01:55:51 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf052660b95a8db1b1ba4326350473f1e1fb34ea78a373a4871e96ef5699f4f`  
		Last Modified: Sat, 06 Mar 2021 01:56:01 GMT  
		Size: 39.2 MB (39178987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beadb945879e66936cb9642c9a3630b264ade60d53f7648bc559fe8b2f139533`  
		Last Modified: Sat, 06 Mar 2021 01:55:51 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4c53b10d6a2696762cdc0f535fe573f771d3333dd7ca5af6ef3b90945f28d3`  
		Last Modified: Sat, 06 Mar 2021 01:55:50 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbb7ddd57a3b8bc8f273017e9ada43a9790b8b479aae5c378dfac4a3050af7c`  
		Last Modified: Sat, 06 Mar 2021 01:55:50 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:64505afd8214bad2f88c9b387ba2ac0776cad02ef64bdedd54fffe35a1c0bff3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41954275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2e52d02c3713651dc7e30ebc9e05e1b3f2c87058b63b78291ce7044a00b2f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:29:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:40:16 GMT
ARG CONSUL_VERSION=1.8.9
# Sat, 06 Mar 2021 01:40:17 GMT
LABEL org.opencontainers.image.version=1.8.9
# Sat, 06 Mar 2021 01:40:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:40:20 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:40:26 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:40:28 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:40:30 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:40:31 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:40:32 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:40:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:40:33 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:40:34 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:40:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:40:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49118f7327ac707f4143297de7ac045ec8c753e74809ae7534de42be82682500`  
		Last Modified: Sat, 06 Mar 2021 01:41:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d44069345c849c39fe962d2f55dc7f7b3adb784c7a5ac0c8a829661e1636efa`  
		Last Modified: Sat, 06 Mar 2021 01:41:44 GMT  
		Size: 39.2 MB (39241098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7f76aa2289746c0525dad0941bb579ed5cb67e4cbf2d3c05f7776838feec88`  
		Last Modified: Sat, 06 Mar 2021 01:41:34 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bf8691e049d2fd912bed04170b056a8573c39feb632d27a1e21f7443728d8c`  
		Last Modified: Sat, 06 Mar 2021 01:41:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deea873381a2808abfe7ba9393eb855cc8a2ae9f5247196b8f45da6bd3a5cfc2`  
		Last Modified: Sat, 06 Mar 2021 01:41:35 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:77802993c000b9e21100c94e7ab80c5c54eed9487328071da526430d57948c6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:adbf5269451afbfdc6fc5119fe4edf01b530f443969cb3cff0a00109613db349
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45605807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:881134d490742be947022560fe1dc94f58a6d4de2cc356e00a9aac59392538f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 24 Feb 2021 21:19:29 GMT
ARG CONSUL_VERSION=1.9.3
# Wed, 24 Feb 2021 21:19:29 GMT
LABEL org.opencontainers.image.version=1.9.3
# Wed, 24 Feb 2021 21:19:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 24 Feb 2021 21:19:31 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 24 Feb 2021 21:19:35 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 24 Feb 2021 21:19:36 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 24 Feb 2021 21:19:37 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:19:38 GMT
VOLUME [/consul/data]
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 8300
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 24 Feb 2021 21:19:38 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 21:19:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:19:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea52006ac511368e3c6bcb4a73d30678c542c0c3fb8a37d65f827068653579f6`  
		Last Modified: Wed, 24 Feb 2021 21:20:31 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e14090bc9d8bfe39c13dfb297d4bcf1538266cec537752e4ad6efabd891756`  
		Last Modified: Wed, 24 Feb 2021 21:20:40 GMT  
		Size: 42.8 MB (42803082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592cff81a0c3344b1ac69a78209a4d49549b47f75103613029c2b371ec7db7c9`  
		Last Modified: Wed, 24 Feb 2021 21:20:30 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9aa5162537717ccc5634c8a34f89e58b1c4731856fee3c87fc09a800bd54898`  
		Last Modified: Wed, 24 Feb 2021 21:20:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8e3c9e516b9424db7cd5c9c8f4f6f2ceae55ed0afaad8cecd7abedc5975740`  
		Last Modified: Wed, 24 Feb 2021 21:20:29 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:6646a089116e4403b19979d956f0346b7e77842fe862a460db93b4fbdfa162c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40887150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df2967ad14eb3d8f8df4dbf80b9f3ee6cdd32b38d18df6518bf4b4fa6523cd1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:08:49 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:51:33 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 01:51:34 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 01:51:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:51:36 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:51:46 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:51:49 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:51:51 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:51:52 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:51:52 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:51:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:51:54 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:51:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:51:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:51:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfdd160f84f7e3aedd41dd69efe406b991b0f3a8c0e1f8e221930e167c0af7e`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28af0ed6a4dee0bc6db150c621e961dd9065b76b5235b9f3b617d69eb28edf7`  
		Last Modified: Sat, 06 Mar 2021 01:55:43 GMT  
		Size: 38.3 MB (38279340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8b744b1e0dfbbd4631239671ad6a97c7910505c868cd0a25b0150e8a991b92`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881bf8e77ec3abe2587c2703e56dfac2ae17c312e755d778f046a45a683e5d45`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95249e42a7e6928f1a5d3efffb9559cf92d5cad9ba3cf481092a325da5bad36c`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:f3bdbe6cc8319c82d2772697aa2abde415cf67123e6aae858aa1d2161fb7d3f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41098571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0e18aa0bc27fe443dd5f7d8c2294ff284cd3454d5263c8c6ceef3874e872ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:29:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:39:49 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 01:39:50 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 01:39:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:39:53 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:40:00 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:40:02 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:40:04 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:40:04 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:40:05 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:40:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:40:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:40:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:40:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b66eb7b864cdce497d20bac9846c1a36d34fdcd8730976613687a89ccda47f`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe120a4c70e82662ef00cbe9a6935c4c2d36fd9750f55d39c977f3504a57eb9d`  
		Last Modified: Sat, 06 Mar 2021 01:41:27 GMT  
		Size: 38.4 MB (38385398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3efa590bb6dd06ff2ddaa79afbeccbe24072a5f6285fcae317525ba7ca1d8a`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441bb269f2e353b50bb1f4497aea940e38fab20e18ecdd4aa30812034c6de63f`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b58b49ea0374313420b69ff3a40f9154191a1d8c740b6eb8204a398c8f7aa6`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:035c25bb69369d460af645c9b0c7054d1f7898b0c6846dc79c29153a76af41f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44931903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9278ff98c7391c7667b2aa6b4fa34542b6789fc023bcbfaf8c3e46a4aa60727`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 20:55:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 24 Feb 2021 20:55:02 GMT
ARG CONSUL_VERSION=1.9.3
# Wed, 24 Feb 2021 20:55:02 GMT
LABEL org.opencontainers.image.version=1.9.3
# Wed, 24 Feb 2021 20:55:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 24 Feb 2021 20:55:03 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 24 Feb 2021 20:55:09 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 24 Feb 2021 20:55:10 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 24 Feb 2021 20:55:11 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 20:55:12 GMT
VOLUME [/consul/data]
# Wed, 24 Feb 2021 20:55:12 GMT
EXPOSE 8300
# Wed, 24 Feb 2021 20:55:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 24 Feb 2021 20:55:12 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 24 Feb 2021 20:55:13 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 20:55:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 20:55:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb2681bebeadff1ca0914e09619d419e7d4e39d6bec343d93e66fcede66d82e`  
		Last Modified: Wed, 24 Feb 2021 20:56:02 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100266ffa9756a72fe161c8439fb8111b7db8c074946f18e76824e6cfd9a79e8`  
		Last Modified: Wed, 24 Feb 2021 20:56:10 GMT  
		Size: 42.1 MB (42133919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73ff495a1d55d7f730f76ec25ae78705097b748f948b8297a401704f8a5c5d9`  
		Last Modified: Wed, 24 Feb 2021 20:56:05 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3087a92a4fe968273b0a7c2f115e35fb4a583a69c1263ee803510c407823241`  
		Last Modified: Wed, 24 Feb 2021 20:56:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f513b227a70e0d8ddefaa0a1a53aeb0c26f4ef3e0644adeaf2156636c002b9`  
		Last Modified: Wed, 24 Feb 2021 20:56:01 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.4`

```console
$ docker pull consul@sha256:f4ed36dd451f8706921ab1c762de17d34ab5c87a74a5528939e72668d09b794a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `consul:1.9.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:6646a089116e4403b19979d956f0346b7e77842fe862a460db93b4fbdfa162c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40887150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df2967ad14eb3d8f8df4dbf80b9f3ee6cdd32b38d18df6518bf4b4fa6523cd1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:08:49 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:51:33 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 01:51:34 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 01:51:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:51:36 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:51:46 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:51:49 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:51:51 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:51:52 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:51:52 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:51:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:51:54 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:51:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:51:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:51:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfdd160f84f7e3aedd41dd69efe406b991b0f3a8c0e1f8e221930e167c0af7e`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28af0ed6a4dee0bc6db150c621e961dd9065b76b5235b9f3b617d69eb28edf7`  
		Last Modified: Sat, 06 Mar 2021 01:55:43 GMT  
		Size: 38.3 MB (38279340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8b744b1e0dfbbd4631239671ad6a97c7910505c868cd0a25b0150e8a991b92`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881bf8e77ec3abe2587c2703e56dfac2ae17c312e755d778f046a45a683e5d45`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95249e42a7e6928f1a5d3efffb9559cf92d5cad9ba3cf481092a325da5bad36c`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:f3bdbe6cc8319c82d2772697aa2abde415cf67123e6aae858aa1d2161fb7d3f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41098571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0e18aa0bc27fe443dd5f7d8c2294ff284cd3454d5263c8c6ceef3874e872ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:29:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:39:49 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 01:39:50 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 01:39:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:39:53 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:40:00 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:40:02 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:40:04 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:40:04 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:40:05 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:40:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:40:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:40:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:40:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b66eb7b864cdce497d20bac9846c1a36d34fdcd8730976613687a89ccda47f`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe120a4c70e82662ef00cbe9a6935c4c2d36fd9750f55d39c977f3504a57eb9d`  
		Last Modified: Sat, 06 Mar 2021 01:41:27 GMT  
		Size: 38.4 MB (38385398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3efa590bb6dd06ff2ddaa79afbeccbe24072a5f6285fcae317525ba7ca1d8a`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441bb269f2e353b50bb1f4497aea940e38fab20e18ecdd4aa30812034c6de63f`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b58b49ea0374313420b69ff3a40f9154191a1d8c740b6eb8204a398c8f7aa6`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:77802993c000b9e21100c94e7ab80c5c54eed9487328071da526430d57948c6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:adbf5269451afbfdc6fc5119fe4edf01b530f443969cb3cff0a00109613db349
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45605807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:881134d490742be947022560fe1dc94f58a6d4de2cc356e00a9aac59392538f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 24 Feb 2021 21:19:29 GMT
ARG CONSUL_VERSION=1.9.3
# Wed, 24 Feb 2021 21:19:29 GMT
LABEL org.opencontainers.image.version=1.9.3
# Wed, 24 Feb 2021 21:19:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 24 Feb 2021 21:19:31 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 24 Feb 2021 21:19:35 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 24 Feb 2021 21:19:36 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 24 Feb 2021 21:19:37 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 21:19:38 GMT
VOLUME [/consul/data]
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 8300
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 24 Feb 2021 21:19:38 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 24 Feb 2021 21:19:38 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 21:19:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 21:19:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea52006ac511368e3c6bcb4a73d30678c542c0c3fb8a37d65f827068653579f6`  
		Last Modified: Wed, 24 Feb 2021 21:20:31 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e14090bc9d8bfe39c13dfb297d4bcf1538266cec537752e4ad6efabd891756`  
		Last Modified: Wed, 24 Feb 2021 21:20:40 GMT  
		Size: 42.8 MB (42803082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:592cff81a0c3344b1ac69a78209a4d49549b47f75103613029c2b371ec7db7c9`  
		Last Modified: Wed, 24 Feb 2021 21:20:30 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9aa5162537717ccc5634c8a34f89e58b1c4731856fee3c87fc09a800bd54898`  
		Last Modified: Wed, 24 Feb 2021 21:20:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b8e3c9e516b9424db7cd5c9c8f4f6f2ceae55ed0afaad8cecd7abedc5975740`  
		Last Modified: Wed, 24 Feb 2021 21:20:29 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:6646a089116e4403b19979d956f0346b7e77842fe862a460db93b4fbdfa162c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40887150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df2967ad14eb3d8f8df4dbf80b9f3ee6cdd32b38d18df6518bf4b4fa6523cd1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:34 GMT
ADD file:8bbb59eeaad0cbcf11559bc6e2b4492aadf6822d1935ed50c710f8bed858b7b5 in / 
# Wed, 24 Feb 2021 20:50:35 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:08:49 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:51:33 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 01:51:34 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 01:51:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:51:36 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:51:46 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:51:49 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:51:51 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:51:52 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:51:52 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:51:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:51:54 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:51:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:51:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:51:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:55242616b0494f68f44470d864da746cd2a8f8f2d1ffca698114de64032247ef`  
		Last Modified: Wed, 24 Feb 2021 20:51:17 GMT  
		Size: 2.6 MB (2604518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfdd160f84f7e3aedd41dd69efe406b991b0f3a8c0e1f8e221930e167c0af7e`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e28af0ed6a4dee0bc6db150c621e961dd9065b76b5235b9f3b617d69eb28edf7`  
		Last Modified: Sat, 06 Mar 2021 01:55:43 GMT  
		Size: 38.3 MB (38279340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8b744b1e0dfbbd4631239671ad6a97c7910505c868cd0a25b0150e8a991b92`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881bf8e77ec3abe2587c2703e56dfac2ae17c312e755d778f046a45a683e5d45`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95249e42a7e6928f1a5d3efffb9559cf92d5cad9ba3cf481092a325da5bad36c`  
		Last Modified: Sat, 06 Mar 2021 01:55:32 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:f3bdbe6cc8319c82d2772697aa2abde415cf67123e6aae858aa1d2161fb7d3f1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41098571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0e18aa0bc27fe443dd5f7d8c2294ff284cd3454d5263c8c6ceef3874e872ae`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 21:29:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 01:39:49 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 01:39:50 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 01:39:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 01:39:53 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 01:40:00 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 01:40:02 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 01:40:04 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 01:40:04 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 01:40:05 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 01:40:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 01:40:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 01:40:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 01:40:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 01:40:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b66eb7b864cdce497d20bac9846c1a36d34fdcd8730976613687a89ccda47f`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe120a4c70e82662ef00cbe9a6935c4c2d36fd9750f55d39c977f3504a57eb9d`  
		Last Modified: Sat, 06 Mar 2021 01:41:27 GMT  
		Size: 38.4 MB (38385398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3efa590bb6dd06ff2ddaa79afbeccbe24072a5f6285fcae317525ba7ca1d8a`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441bb269f2e353b50bb1f4497aea940e38fab20e18ecdd4aa30812034c6de63f`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b58b49ea0374313420b69ff3a40f9154191a1d8c740b6eb8204a398c8f7aa6`  
		Last Modified: Sat, 06 Mar 2021 01:41:17 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:035c25bb69369d460af645c9b0c7054d1f7898b0c6846dc79c29153a76af41f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44931903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9278ff98c7391c7667b2aa6b4fa34542b6789fc023bcbfaf8c3e46a4aa60727`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 20:55:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 24 Feb 2021 20:55:02 GMT
ARG CONSUL_VERSION=1.9.3
# Wed, 24 Feb 2021 20:55:02 GMT
LABEL org.opencontainers.image.version=1.9.3
# Wed, 24 Feb 2021 20:55:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 24 Feb 2021 20:55:03 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 24 Feb 2021 20:55:09 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 24 Feb 2021 20:55:10 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 24 Feb 2021 20:55:11 GMT
# ARGS: CONSUL_VERSION=1.9.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 24 Feb 2021 20:55:12 GMT
VOLUME [/consul/data]
# Wed, 24 Feb 2021 20:55:12 GMT
EXPOSE 8300
# Wed, 24 Feb 2021 20:55:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 24 Feb 2021 20:55:12 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 24 Feb 2021 20:55:13 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 20:55:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 20:55:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb2681bebeadff1ca0914e09619d419e7d4e39d6bec343d93e66fcede66d82e`  
		Last Modified: Wed, 24 Feb 2021 20:56:02 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100266ffa9756a72fe161c8439fb8111b7db8c074946f18e76824e6cfd9a79e8`  
		Last Modified: Wed, 24 Feb 2021 20:56:10 GMT  
		Size: 42.1 MB (42133919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73ff495a1d55d7f730f76ec25ae78705097b748f948b8297a401704f8a5c5d9`  
		Last Modified: Wed, 24 Feb 2021 20:56:05 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3087a92a4fe968273b0a7c2f115e35fb4a583a69c1263ee803510c407823241`  
		Last Modified: Wed, 24 Feb 2021 20:56:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f513b227a70e0d8ddefaa0a1a53aeb0c26f4ef3e0644adeaf2156636c002b9`  
		Last Modified: Wed, 24 Feb 2021 20:56:01 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
