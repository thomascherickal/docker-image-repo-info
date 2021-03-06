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
$ docker pull consul@sha256:e729ce514e2c069bd28759a4fcbbcaba53499656e33436a55fd57451232d8ff7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:9c4f7b7cd4446f3490ef0d7be548a7ae40b7fe9331d95a9b19aca8677ee8a7f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43132577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896e230f7eb6200bdf87cb91fdd6bf5db015c1a50d3fa8d260aa97fb20c10578`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:27:46 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 07:28:50 GMT
ARG CONSUL_VERSION=1.7.13
# Sat, 06 Mar 2021 07:28:51 GMT
LABEL org.opencontainers.image.version=1.7.13
# Sat, 06 Mar 2021 07:28:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 07:28:52 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 07:28:57 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 07:28:58 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 07:28:59 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 07:28:59 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 07:28:59 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 07:29:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 07:29:00 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 07:29:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 07:29:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:29:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92b2997ba2254dafae368f67cf53bd0a7aeb49d9eaf3a65d0456485a2768f05`  
		Last Modified: Sat, 06 Mar 2021 07:29:57 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a5959af88c55ad0a54e88ae1258295174bf32ecbb08a5d6ce989016947a9a7`  
		Last Modified: Sat, 06 Mar 2021 07:30:04 GMT  
		Size: 40.3 MB (40329788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd8fcf2c29ecdc16d38a99bafc17d1d6b946537f3ec240dfacaa97805762dff`  
		Last Modified: Sat, 06 Mar 2021 07:29:57 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03deb0f53e5cc5aae8b1c55de87eabf50f001d04a0d146aea7b6f9de3ff25ad`  
		Last Modified: Sat, 06 Mar 2021 07:29:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ba163d06f48a4f1e98086bc28cdbe65e75b08ea4287c726524ae4e1a5a9bf8`  
		Last Modified: Sat, 06 Mar 2021 07:29:57 GMT  
		Size: 1.7 KB (1708 bytes)  
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
$ docker pull consul@sha256:22317e75e8a10d01ae23f77e6f800558cedf76247de3a63bb00d0ee13faa1889
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41938750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06bc285bebb45ce4facbdd56a00dadb646d0bb534d74e7536da5c78a54b4ca38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 06:53:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 06:53:54 GMT
ARG CONSUL_VERSION=1.7.13
# Sat, 06 Mar 2021 06:53:54 GMT
LABEL org.opencontainers.image.version=1.7.13
# Sat, 06 Mar 2021 06:53:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 06:53:55 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 06:54:00 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 06:54:02 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 06:54:03 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 06:54:03 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 06:54:04 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 06:54:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 06:54:04 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 06:54:05 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 06:54:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 06:54:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570358da82359003032b987373e1ce0ffe1a2487a1a10c3fb0f86e9d1a8ab311`  
		Last Modified: Sat, 06 Mar 2021 06:55:19 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c60241c6c4b0e82f7691250f0040c03a765c47d563591eed9d366d02ed227c`  
		Last Modified: Sat, 06 Mar 2021 06:55:26 GMT  
		Size: 39.1 MB (39140703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667c23c807c21c5a414164d938ae5542c0b1d9851b97f4ff53147fa0562a6669`  
		Last Modified: Sat, 06 Mar 2021 06:55:19 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaddb714f3957534160c57613769bf116de4046db6dc7f3452bdee1a9e2c27c`  
		Last Modified: Sat, 06 Mar 2021 06:55:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd810e47e010cf181de20dad838cda305e28fd3aecd3296965d50105c3604cd5`  
		Last Modified: Sat, 06 Mar 2021 06:55:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.13`

```console
$ docker pull consul@sha256:e729ce514e2c069bd28759a4fcbbcaba53499656e33436a55fd57451232d8ff7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.13` - linux; amd64

```console
$ docker pull consul@sha256:9c4f7b7cd4446f3490ef0d7be548a7ae40b7fe9331d95a9b19aca8677ee8a7f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43132577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896e230f7eb6200bdf87cb91fdd6bf5db015c1a50d3fa8d260aa97fb20c10578`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:27:46 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 07:28:50 GMT
ARG CONSUL_VERSION=1.7.13
# Sat, 06 Mar 2021 07:28:51 GMT
LABEL org.opencontainers.image.version=1.7.13
# Sat, 06 Mar 2021 07:28:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 07:28:52 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 07:28:57 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 07:28:58 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 07:28:59 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 07:28:59 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 07:28:59 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 07:29:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 07:29:00 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 07:29:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 07:29:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:29:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92b2997ba2254dafae368f67cf53bd0a7aeb49d9eaf3a65d0456485a2768f05`  
		Last Modified: Sat, 06 Mar 2021 07:29:57 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a5959af88c55ad0a54e88ae1258295174bf32ecbb08a5d6ce989016947a9a7`  
		Last Modified: Sat, 06 Mar 2021 07:30:04 GMT  
		Size: 40.3 MB (40329788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd8fcf2c29ecdc16d38a99bafc17d1d6b946537f3ec240dfacaa97805762dff`  
		Last Modified: Sat, 06 Mar 2021 07:29:57 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03deb0f53e5cc5aae8b1c55de87eabf50f001d04a0d146aea7b6f9de3ff25ad`  
		Last Modified: Sat, 06 Mar 2021 07:29:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ba163d06f48a4f1e98086bc28cdbe65e75b08ea4287c726524ae4e1a5a9bf8`  
		Last Modified: Sat, 06 Mar 2021 07:29:57 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `consul:1.7.13` - linux; 386

```console
$ docker pull consul@sha256:22317e75e8a10d01ae23f77e6f800558cedf76247de3a63bb00d0ee13faa1889
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41938750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06bc285bebb45ce4facbdd56a00dadb646d0bb534d74e7536da5c78a54b4ca38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 06:53:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 06:53:54 GMT
ARG CONSUL_VERSION=1.7.13
# Sat, 06 Mar 2021 06:53:54 GMT
LABEL org.opencontainers.image.version=1.7.13
# Sat, 06 Mar 2021 06:53:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 06:53:55 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 06:54:00 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 06:54:02 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 06:54:03 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 06:54:03 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 06:54:04 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 06:54:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 06:54:04 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 06:54:05 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 06:54:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 06:54:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570358da82359003032b987373e1ce0ffe1a2487a1a10c3fb0f86e9d1a8ab311`  
		Last Modified: Sat, 06 Mar 2021 06:55:19 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04c60241c6c4b0e82f7691250f0040c03a765c47d563591eed9d366d02ed227c`  
		Last Modified: Sat, 06 Mar 2021 06:55:26 GMT  
		Size: 39.1 MB (39140703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667c23c807c21c5a414164d938ae5542c0b1d9851b97f4ff53147fa0562a6669`  
		Last Modified: Sat, 06 Mar 2021 06:55:19 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaddb714f3957534160c57613769bf116de4046db6dc7f3452bdee1a9e2c27c`  
		Last Modified: Sat, 06 Mar 2021 06:55:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd810e47e010cf181de20dad838cda305e28fd3aecd3296965d50105c3604cd5`  
		Last Modified: Sat, 06 Mar 2021 06:55:20 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:b6e283cd4abcab21362e5669d378fb062a068ed7903ca5891a7de6060d3035d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:6d182801688a07d9f7b44f19f9658bf184d18abfbfe4bc5f4065ef2646f92324
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46518990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d526b5d080875ab30992b3ff166734e037248aaa1c0a45cb4d231d6574460cc9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:27:46 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 07:28:37 GMT
ARG CONSUL_VERSION=1.8.9
# Sat, 06 Mar 2021 07:28:37 GMT
LABEL org.opencontainers.image.version=1.8.9
# Sat, 06 Mar 2021 07:28:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 07:28:38 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 07:28:44 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 07:28:45 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 07:28:46 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 07:28:46 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 07:28:46 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 07:28:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 07:28:47 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 07:28:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 07:28:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:28:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1eb75caf6e0d2890960532799f074c5365160538eec08d8c7114a600f93734`  
		Last Modified: Sat, 06 Mar 2021 07:29:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d80d7ffdf95e9ebd0fde83c90b7a3376c272ad1703071d1d45babbe605c1fa8`  
		Last Modified: Sat, 06 Mar 2021 07:29:46 GMT  
		Size: 43.7 MB (43716200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03b37de62baf80205ef8100e09928d6748cbdacaca97d7a5f2f91b708640171`  
		Last Modified: Sat, 06 Mar 2021 07:29:40 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d095e808f2c029e9fc8a1e5c50c8695ad64a63709138505b2e97e5839827b43f`  
		Last Modified: Sat, 06 Mar 2021 07:29:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00216b803b00d7f28b6f35dd6d3bd8faa3fbd12680e4eba20c02f11ccf9c623`  
		Last Modified: Sat, 06 Mar 2021 07:29:40 GMT  
		Size: 1.7 KB (1708 bytes)  
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
$ docker pull consul@sha256:1260a98e3fecf88dec9302492c4b8ad0774c9b61deb1c655501ad17173defb71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46043394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ac05d684f3c4142e1a0235edf2124f5505b1c93ac542931d45612614e938e86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 06:53:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 06:53:37 GMT
ARG CONSUL_VERSION=1.8.9
# Sat, 06 Mar 2021 06:53:37 GMT
LABEL org.opencontainers.image.version=1.8.9
# Sat, 06 Mar 2021 06:53:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 06:53:38 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 06:53:44 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 06:53:46 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 06:53:47 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 06:53:47 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 06:53:47 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 06:53:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 06:53:47 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 06:53:48 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 06:53:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 06:53:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7913042344ef9ecb2a8c31d2d2417022ca5334c371026fdd0e1b6af99e7c3e40`  
		Last Modified: Sat, 06 Mar 2021 06:54:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22014404920b99b8062ab12ecbcf0df85bccacb8597f347f72cf225e6a45f704`  
		Last Modified: Sat, 06 Mar 2021 06:55:07 GMT  
		Size: 43.2 MB (43245351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a86eb5f9e632a9d68bef6cbd21eecbb565c437c6a3b8fc6589c8effdacf80c`  
		Last Modified: Sat, 06 Mar 2021 06:54:59 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c53c9010dfd656861899214ad1536b123114e5552d1d281542e225adbf41ad`  
		Last Modified: Sat, 06 Mar 2021 06:54:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef8cafe28da00b8a6c7d80ab0c8e288eb50d39994758f84120f802756230648`  
		Last Modified: Sat, 06 Mar 2021 06:54:59 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.9`

```console
$ docker pull consul@sha256:b6e283cd4abcab21362e5669d378fb062a068ed7903ca5891a7de6060d3035d5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.9` - linux; amd64

```console
$ docker pull consul@sha256:6d182801688a07d9f7b44f19f9658bf184d18abfbfe4bc5f4065ef2646f92324
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46518990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d526b5d080875ab30992b3ff166734e037248aaa1c0a45cb4d231d6574460cc9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:27:46 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 07:28:37 GMT
ARG CONSUL_VERSION=1.8.9
# Sat, 06 Mar 2021 07:28:37 GMT
LABEL org.opencontainers.image.version=1.8.9
# Sat, 06 Mar 2021 07:28:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 07:28:38 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 07:28:44 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 07:28:45 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 07:28:46 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 07:28:46 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 07:28:46 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 07:28:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 07:28:47 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 07:28:47 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 07:28:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:28:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1eb75caf6e0d2890960532799f074c5365160538eec08d8c7114a600f93734`  
		Last Modified: Sat, 06 Mar 2021 07:29:40 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d80d7ffdf95e9ebd0fde83c90b7a3376c272ad1703071d1d45babbe605c1fa8`  
		Last Modified: Sat, 06 Mar 2021 07:29:46 GMT  
		Size: 43.7 MB (43716200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b03b37de62baf80205ef8100e09928d6748cbdacaca97d7a5f2f91b708640171`  
		Last Modified: Sat, 06 Mar 2021 07:29:40 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d095e808f2c029e9fc8a1e5c50c8695ad64a63709138505b2e97e5839827b43f`  
		Last Modified: Sat, 06 Mar 2021 07:29:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00216b803b00d7f28b6f35dd6d3bd8faa3fbd12680e4eba20c02f11ccf9c623`  
		Last Modified: Sat, 06 Mar 2021 07:29:40 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `consul:1.8.9` - linux; 386

```console
$ docker pull consul@sha256:1260a98e3fecf88dec9302492c4b8ad0774c9b61deb1c655501ad17173defb71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46043394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ac05d684f3c4142e1a0235edf2124f5505b1c93ac542931d45612614e938e86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 06:53:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 06:53:37 GMT
ARG CONSUL_VERSION=1.8.9
# Sat, 06 Mar 2021 06:53:37 GMT
LABEL org.opencontainers.image.version=1.8.9
# Sat, 06 Mar 2021 06:53:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 06:53:38 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 06:53:44 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 06:53:46 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 06:53:47 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 06:53:47 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 06:53:47 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 06:53:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 06:53:47 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 06:53:48 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 06:53:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 06:53:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7913042344ef9ecb2a8c31d2d2417022ca5334c371026fdd0e1b6af99e7c3e40`  
		Last Modified: Sat, 06 Mar 2021 06:54:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22014404920b99b8062ab12ecbcf0df85bccacb8597f347f72cf225e6a45f704`  
		Last Modified: Sat, 06 Mar 2021 06:55:07 GMT  
		Size: 43.2 MB (43245351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a86eb5f9e632a9d68bef6cbd21eecbb565c437c6a3b8fc6589c8effdacf80c`  
		Last Modified: Sat, 06 Mar 2021 06:54:59 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c53c9010dfd656861899214ad1536b123114e5552d1d281542e225adbf41ad`  
		Last Modified: Sat, 06 Mar 2021 06:54:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef8cafe28da00b8a6c7d80ab0c8e288eb50d39994758f84120f802756230648`  
		Last Modified: Sat, 06 Mar 2021 06:54:59 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:6476d32fd71d3d740593068bc950672fe6835f462500cf4d01ccadaf42c8788c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:750ef49168ba503a114c1f90378030678f2c4d17679d795e7e980d20bd43c268
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45630722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d544f4c4e87c388d3535d758860bbc15cc6369ed977d6d8d361936e79e913576`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:27:46 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 07:27:47 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 07:27:47 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 07:27:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 07:27:48 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 07:28:27 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 07:28:28 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 07:28:29 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 07:28:29 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 07:28:29 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 07:28:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 07:28:30 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 07:28:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 07:28:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:28:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bef71355ee6be6a9717bfd4443d6642fab9f51a1e5dc9a489d8fa8f9aeaf11`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eee5cf2b9dea04246397a00b4fe776b9fd45973810fc60d5cb93ba0c7487cfb`  
		Last Modified: Sat, 06 Mar 2021 07:29:23 GMT  
		Size: 42.8 MB (42827933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e442decf40c9d24a8411723aacd309788a63a8108796e7795da4129c549791`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e14956c1141d0d457b3cc8915ef2a5d8df261769f936b6c10b31d79077a042`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c58c08140c5ffee239eb9f3d9c813e0062de37e75dada055cafc0900a2626`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
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
$ docker pull consul@sha256:4d1ae4b655c00f006df070f699685bcc6dae791833a05fb45270963673f703a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44977337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc7b22fad055bdea30205eabb344370b620be78d0723cd0fef2a7f4952739128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 06:53:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 06:53:18 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 06:53:18 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 06:53:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 06:53:19 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 06:53:27 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 06:53:28 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 06:53:29 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 06:53:29 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 06:53:29 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 06:53:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 06:53:30 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 06:53:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 06:53:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 06:53:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fa07be517920a3bb1d548c208b00436c2fabff225e33d8be0fe04fc73c0300`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0cfa198eed101b51acb5450643ff946992f8ee1425a692d43810492e3d4cbd`  
		Last Modified: Sat, 06 Mar 2021 06:54:42 GMT  
		Size: 42.2 MB (42179293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb7e0d70cec51498e895112e500b72371259a9befd07649226b617331676986`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d614aa518e3249cb6d61ba6f2857bae9e7d71258b7d7582f74d79baf820a6e`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bccb2df305ef9dc0ffe686cae8c3123fdd23b2220e186436a42eecf759d774`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.4`

```console
$ docker pull consul@sha256:6476d32fd71d3d740593068bc950672fe6835f462500cf4d01ccadaf42c8788c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.4` - linux; amd64

```console
$ docker pull consul@sha256:750ef49168ba503a114c1f90378030678f2c4d17679d795e7e980d20bd43c268
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45630722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d544f4c4e87c388d3535d758860bbc15cc6369ed977d6d8d361936e79e913576`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:27:46 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 07:27:47 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 07:27:47 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 07:27:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 07:27:48 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 07:28:27 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 07:28:28 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 07:28:29 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 07:28:29 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 07:28:29 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 07:28:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 07:28:30 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 07:28:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 07:28:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:28:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bef71355ee6be6a9717bfd4443d6642fab9f51a1e5dc9a489d8fa8f9aeaf11`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eee5cf2b9dea04246397a00b4fe776b9fd45973810fc60d5cb93ba0c7487cfb`  
		Last Modified: Sat, 06 Mar 2021 07:29:23 GMT  
		Size: 42.8 MB (42827933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e442decf40c9d24a8411723aacd309788a63a8108796e7795da4129c549791`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e14956c1141d0d457b3cc8915ef2a5d8df261769f936b6c10b31d79077a042`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c58c08140c5ffee239eb9f3d9c813e0062de37e75dada055cafc0900a2626`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `consul:1.9.4` - linux; 386

```console
$ docker pull consul@sha256:4d1ae4b655c00f006df070f699685bcc6dae791833a05fb45270963673f703a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44977337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc7b22fad055bdea30205eabb344370b620be78d0723cd0fef2a7f4952739128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 06:53:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 06:53:18 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 06:53:18 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 06:53:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 06:53:19 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 06:53:27 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 06:53:28 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 06:53:29 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 06:53:29 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 06:53:29 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 06:53:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 06:53:30 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 06:53:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 06:53:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 06:53:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fa07be517920a3bb1d548c208b00436c2fabff225e33d8be0fe04fc73c0300`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0cfa198eed101b51acb5450643ff946992f8ee1425a692d43810492e3d4cbd`  
		Last Modified: Sat, 06 Mar 2021 06:54:42 GMT  
		Size: 42.2 MB (42179293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb7e0d70cec51498e895112e500b72371259a9befd07649226b617331676986`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d614aa518e3249cb6d61ba6f2857bae9e7d71258b7d7582f74d79baf820a6e`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bccb2df305ef9dc0ffe686cae8c3123fdd23b2220e186436a42eecf759d774`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:6476d32fd71d3d740593068bc950672fe6835f462500cf4d01ccadaf42c8788c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:750ef49168ba503a114c1f90378030678f2c4d17679d795e7e980d20bd43c268
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45630722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d544f4c4e87c388d3535d758860bbc15cc6369ed977d6d8d361936e79e913576`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 07:27:46 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 07:27:47 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 07:27:47 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 07:27:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 07:27:48 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 07:28:27 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 07:28:28 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 07:28:29 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 07:28:29 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 07:28:29 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 07:28:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 07:28:30 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 07:28:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 07:28:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 07:28:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22bef71355ee6be6a9717bfd4443d6642fab9f51a1e5dc9a489d8fa8f9aeaf11`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eee5cf2b9dea04246397a00b4fe776b9fd45973810fc60d5cb93ba0c7487cfb`  
		Last Modified: Sat, 06 Mar 2021 07:29:23 GMT  
		Size: 42.8 MB (42827933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e442decf40c9d24a8411723aacd309788a63a8108796e7795da4129c549791`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e14956c1141d0d457b3cc8915ef2a5d8df261769f936b6c10b31d79077a042`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61c58c08140c5ffee239eb9f3d9c813e0062de37e75dada055cafc0900a2626`  
		Last Modified: Sat, 06 Mar 2021 07:29:16 GMT  
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
$ docker pull consul@sha256:4d1ae4b655c00f006df070f699685bcc6dae791833a05fb45270963673f703a3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44977337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc7b22fad055bdea30205eabb344370b620be78d0723cd0fef2a7f4952739128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:41 GMT
ADD file:1f1a1b55522505e78fcc069edb6c793371f78991e90dcb464e4ddac7efd6588c in / 
# Wed, 24 Feb 2021 20:38:41 GMT
CMD ["/bin/sh"]
# Sat, 06 Mar 2021 06:53:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 06 Mar 2021 06:53:18 GMT
ARG CONSUL_VERSION=1.9.4
# Sat, 06 Mar 2021 06:53:18 GMT
LABEL org.opencontainers.image.version=1.9.4
# Sat, 06 Mar 2021 06:53:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 06 Mar 2021 06:53:19 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 06 Mar 2021 06:53:27 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 06 Mar 2021 06:53:28 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 06 Mar 2021 06:53:29 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 06 Mar 2021 06:53:29 GMT
VOLUME [/consul/data]
# Sat, 06 Mar 2021 06:53:29 GMT
EXPOSE 8300
# Sat, 06 Mar 2021 06:53:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 06 Mar 2021 06:53:30 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 06 Mar 2021 06:53:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 06 Mar 2021 06:53:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 06 Mar 2021 06:53:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:045e8056601208133bee5c98e76028f9b97e055c738892f8d6283205e1006173`  
		Last Modified: Wed, 24 Feb 2021 20:39:27 GMT  
		Size: 2.8 MB (2794750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fa07be517920a3bb1d548c208b00436c2fabff225e33d8be0fe04fc73c0300`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0cfa198eed101b51acb5450643ff946992f8ee1425a692d43810492e3d4cbd`  
		Last Modified: Sat, 06 Mar 2021 06:54:42 GMT  
		Size: 42.2 MB (42179293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb7e0d70cec51498e895112e500b72371259a9befd07649226b617331676986`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d614aa518e3249cb6d61ba6f2857bae9e7d71258b7d7582f74d79baf820a6e`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bccb2df305ef9dc0ffe686cae8c3123fdd23b2220e186436a42eecf759d774`  
		Last Modified: Sat, 06 Mar 2021 06:54:34 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
