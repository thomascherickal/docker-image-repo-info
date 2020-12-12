<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.7`](#consul17)
-	[`consul:1.7.11`](#consul1711)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.7`](#consul187)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.1`](#consul191)
-	[`consul:latest`](#consullatest)

## `consul:1.7`

```console
$ docker pull consul@sha256:dd2853ee83e12f7991391fd3521ddede867787cccc55f257e8ea6bc4cc0d5828
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:f5ba1c10ede8ea46bb02c6a19c70b82ad0ac638119bb63c83640d3aa4714dc7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43109963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff8cca0998622aa819606b6ff094462ac4cbef1d430d1a79393425e708e3484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 18:11:03 GMT
ENV CONSUL_VERSION=1.7.11
# Sat, 12 Dec 2020 18:11:03 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 18:11:04 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 18:11:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 18:11:09 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 18:11:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 18:11:10 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 18:11:11 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 18:11:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 18:11:11 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 18:11:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 18:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 18:11:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5c69d0ff3e52886ce3d4059d5891a2d768719aa984dcba7913772ea0b731c7`  
		Last Modified: Sat, 12 Dec 2020 18:11:59 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d265686f6dd56faa1a3f6fe33d5f797823ba814ac40f59bc4efc60625ba541e`  
		Last Modified: Sat, 12 Dec 2020 18:12:06 GMT  
		Size: 40.3 MB (40309785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486c10f69ace72305dea706e9cf682df431bda05d661e14feb527e760748f208`  
		Last Modified: Sat, 12 Dec 2020 18:12:00 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3fb3e64da9394bb2e9f734c704ea0dbfc6e9fd11793c1954066fc81d127ec1`  
		Last Modified: Sat, 12 Dec 2020 18:12:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d05d68b95eea15dc959736eea9fc4d86cfd7788a4edff455b4e9108b0456c7`  
		Last Modified: Sat, 12 Dec 2020 18:12:00 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:f2dce1c8bfcf33d175732fe0ef56342674735edb3be2224f65a341cbec18b3c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38812406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f691a1d42bb1229ec76bd15c35360f0584fa52ad6f32c6d1581c35753a197d88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 00:55:24 GMT
ENV CONSUL_VERSION=1.7.11
# Sat, 12 Dec 2020 00:55:25 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 00:55:30 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 00:55:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 00:55:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 00:55:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 00:55:50 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 00:55:55 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 00:55:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 00:55:58 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 00:55:59 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 00:56:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 00:56:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c131071c301e2d6e6f5d5a5eefb8d6932e5a4f4077ffd76525ebe1553258ab3f`  
		Last Modified: Sat, 12 Dec 2020 00:57:08 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad9bae7fe82dcc03de361eae7942072cb328d4470ad1f235f375e8d20b0eec6`  
		Last Modified: Sat, 12 Dec 2020 00:57:18 GMT  
		Size: 36.2 MB (36207123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371c83906741a4af030f924c9adaae9d4f7a6383f8a400ace5baf03163eabaf1`  
		Last Modified: Sat, 12 Dec 2020 00:57:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860a4026e11b38efec011508b265799304407bed92877804317bbd3828455152`  
		Last Modified: Sat, 12 Dec 2020 00:57:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b5950edec2988c46cc03ca2a8562adfae3399761b2aa13145cf97b96958433`  
		Last Modified: Sat, 12 Dec 2020 00:57:09 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:5741d7cbcdbcdee8df6fd569dd0a1821026610ffad717deb8b0d7447078b46c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39020690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d84b92201c235c95047f58df92783a12f112e6201855e360450c0fcc3f9ef16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 14:08:32 GMT
ENV CONSUL_VERSION=1.7.11
# Sat, 12 Dec 2020 14:08:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 14:08:35 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 14:08:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 14:08:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 14:08:48 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 14:08:49 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 14:08:49 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 14:08:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 14:08:51 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 14:08:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 14:08:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 14:08:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2013218a4de91072d128f42f581a286f763ca311ba03a40919119c685eac0f41`  
		Last Modified: Sat, 12 Dec 2020 14:09:46 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358f4028c41610ee96392fb6837b2c2060e820f9cae0e700541965028084ad22`  
		Last Modified: Sat, 12 Dec 2020 14:09:54 GMT  
		Size: 36.3 MB (36310779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5349efa350c0ffd84c5fc595d20cb1bc02ac5dcd8d3cc454cc42d97247ec774`  
		Last Modified: Sat, 12 Dec 2020 14:09:46 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf3ea6c2326d360c03390f51b0ecbf53ca155f3b4d9315a0c40289c041edbd7`  
		Last Modified: Sat, 12 Dec 2020 14:09:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c0f0523202f2ac153b3cddf46ef3f6fb4d15972464c94a8cd03910ecac4486`  
		Last Modified: Sat, 12 Dec 2020 14:09:46 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:86be8bf0b121140e143600433e39e5853e8ba1141b79aab1beecdbb092160161
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41898134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c96f81d08a1705d786920d5f9b9181cea456bd7a6307c32b74a7ca56919915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:57:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 16:22:16 GMT
ENV CONSUL_VERSION=1.7.11
# Sat, 12 Dec 2020 16:22:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 16:22:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 16:22:24 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 16:22:25 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 16:22:26 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 16:22:27 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 16:22:27 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 16:22:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 16:22:27 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 16:22:28 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 16:22:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 16:22:28 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b80dc7aaa4032eba286f81c64b7e4f7a026f052e95e48008409919338a6946b`  
		Last Modified: Sat, 12 Dec 2020 16:23:24 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572ea19941ac071160e89a9d591683a40ae269e7fda7e07b127fc8353aaaa9d5`  
		Last Modified: Sat, 12 Dec 2020 16:23:36 GMT  
		Size: 39.1 MB (39103396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e54683c743ce4d88e5a45255b6fc28bfe32240c5917584cfbb435d8f77c21c`  
		Last Modified: Sat, 12 Dec 2020 16:23:25 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656b8ee2dc85087436651e34980d2f7c28ae9ee982b331d04793055222ae3b65`  
		Last Modified: Sat, 12 Dec 2020 16:23:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cc56fabbdb730edd86088a0650e7f83f977f8225520af9afd0c8fcec54e738`  
		Last Modified: Sat, 12 Dec 2020 16:23:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.11`

```console
$ docker pull consul@sha256:dd2853ee83e12f7991391fd3521ddede867787cccc55f257e8ea6bc4cc0d5828
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.11` - linux; amd64

```console
$ docker pull consul@sha256:f5ba1c10ede8ea46bb02c6a19c70b82ad0ac638119bb63c83640d3aa4714dc7a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43109963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ff8cca0998622aa819606b6ff094462ac4cbef1d430d1a79393425e708e3484`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 18:11:03 GMT
ENV CONSUL_VERSION=1.7.11
# Sat, 12 Dec 2020 18:11:03 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 18:11:04 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 18:11:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 18:11:09 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 18:11:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 18:11:10 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 18:11:11 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 18:11:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 18:11:11 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 18:11:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 18:11:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 18:11:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da5c69d0ff3e52886ce3d4059d5891a2d768719aa984dcba7913772ea0b731c7`  
		Last Modified: Sat, 12 Dec 2020 18:11:59 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d265686f6dd56faa1a3f6fe33d5f797823ba814ac40f59bc4efc60625ba541e`  
		Last Modified: Sat, 12 Dec 2020 18:12:06 GMT  
		Size: 40.3 MB (40309785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:486c10f69ace72305dea706e9cf682df431bda05d661e14feb527e760748f208`  
		Last Modified: Sat, 12 Dec 2020 18:12:00 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3fb3e64da9394bb2e9f734c704ea0dbfc6e9fd11793c1954066fc81d127ec1`  
		Last Modified: Sat, 12 Dec 2020 18:12:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d05d68b95eea15dc959736eea9fc4d86cfd7788a4edff455b4e9108b0456c7`  
		Last Modified: Sat, 12 Dec 2020 18:12:00 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:f2dce1c8bfcf33d175732fe0ef56342674735edb3be2224f65a341cbec18b3c5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38812406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f691a1d42bb1229ec76bd15c35360f0584fa52ad6f32c6d1581c35753a197d88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 00:55:24 GMT
ENV CONSUL_VERSION=1.7.11
# Sat, 12 Dec 2020 00:55:25 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 00:55:30 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 00:55:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 00:55:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 00:55:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 00:55:50 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 00:55:55 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 00:55:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 00:55:58 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 00:55:59 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 00:56:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 00:56:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c131071c301e2d6e6f5d5a5eefb8d6932e5a4f4077ffd76525ebe1553258ab3f`  
		Last Modified: Sat, 12 Dec 2020 00:57:08 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad9bae7fe82dcc03de361eae7942072cb328d4470ad1f235f375e8d20b0eec6`  
		Last Modified: Sat, 12 Dec 2020 00:57:18 GMT  
		Size: 36.2 MB (36207123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371c83906741a4af030f924c9adaae9d4f7a6383f8a400ace5baf03163eabaf1`  
		Last Modified: Sat, 12 Dec 2020 00:57:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860a4026e11b38efec011508b265799304407bed92877804317bbd3828455152`  
		Last Modified: Sat, 12 Dec 2020 00:57:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b5950edec2988c46cc03ca2a8562adfae3399761b2aa13145cf97b96958433`  
		Last Modified: Sat, 12 Dec 2020 00:57:09 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:5741d7cbcdbcdee8df6fd569dd0a1821026610ffad717deb8b0d7447078b46c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39020690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d84b92201c235c95047f58df92783a12f112e6201855e360450c0fcc3f9ef16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 14:08:32 GMT
ENV CONSUL_VERSION=1.7.11
# Sat, 12 Dec 2020 14:08:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 14:08:35 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 14:08:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 14:08:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 14:08:48 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 14:08:49 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 14:08:49 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 14:08:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 14:08:51 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 14:08:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 14:08:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 14:08:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2013218a4de91072d128f42f581a286f763ca311ba03a40919119c685eac0f41`  
		Last Modified: Sat, 12 Dec 2020 14:09:46 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:358f4028c41610ee96392fb6837b2c2060e820f9cae0e700541965028084ad22`  
		Last Modified: Sat, 12 Dec 2020 14:09:54 GMT  
		Size: 36.3 MB (36310779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5349efa350c0ffd84c5fc595d20cb1bc02ac5dcd8d3cc454cc42d97247ec774`  
		Last Modified: Sat, 12 Dec 2020 14:09:46 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf3ea6c2326d360c03390f51b0ecbf53ca155f3b4d9315a0c40289c041edbd7`  
		Last Modified: Sat, 12 Dec 2020 14:09:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c0f0523202f2ac153b3cddf46ef3f6fb4d15972464c94a8cd03910ecac4486`  
		Last Modified: Sat, 12 Dec 2020 14:09:46 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.11` - linux; 386

```console
$ docker pull consul@sha256:86be8bf0b121140e143600433e39e5853e8ba1141b79aab1beecdbb092160161
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41898134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04c96f81d08a1705d786920d5f9b9181cea456bd7a6307c32b74a7ca56919915`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:57:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 16:22:16 GMT
ENV CONSUL_VERSION=1.7.11
# Sat, 12 Dec 2020 16:22:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 16:22:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 16:22:24 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 16:22:25 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 16:22:26 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 16:22:27 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 16:22:27 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 16:22:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 16:22:27 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 16:22:28 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 16:22:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 16:22:28 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b80dc7aaa4032eba286f81c64b7e4f7a026f052e95e48008409919338a6946b`  
		Last Modified: Sat, 12 Dec 2020 16:23:24 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572ea19941ac071160e89a9d591683a40ae269e7fda7e07b127fc8353aaaa9d5`  
		Last Modified: Sat, 12 Dec 2020 16:23:36 GMT  
		Size: 39.1 MB (39103396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e54683c743ce4d88e5a45255b6fc28bfe32240c5917584cfbb435d8f77c21c`  
		Last Modified: Sat, 12 Dec 2020 16:23:25 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656b8ee2dc85087436651e34980d2f7c28ae9ee982b331d04793055222ae3b65`  
		Last Modified: Sat, 12 Dec 2020 16:23:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cc56fabbdb730edd86088a0650e7f83f977f8225520af9afd0c8fcec54e738`  
		Last Modified: Sat, 12 Dec 2020 16:23:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:764e86d2b5deb2abf01d523fd85981e8039a226ad4984edb2f7ccc14cf2cbc49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:9160035c831a0e976acfdd6f2a40af5db7bb646adbd74fb832c0d7bd7efcbb06
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46490386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b404af955f9a59e02d0b99fd3d318d0130e2c1a1051ae9668e304fade204c53d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 18:10:49 GMT
ENV CONSUL_VERSION=1.8.7
# Sat, 12 Dec 2020 18:10:49 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 18:10:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 18:10:54 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 18:10:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 18:10:56 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 18:10:57 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 18:10:57 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 18:10:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 18:10:57 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 18:10:58 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 18:10:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 18:10:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e57714d98115cef3592709bbdccf649f3c8bfa4381aee05b86fd7c93a881d`  
		Last Modified: Sat, 12 Dec 2020 18:11:38 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9106f38e55f03273066533b61332ca498e63bacb91839b5559ce4599ed864cf0`  
		Last Modified: Sat, 12 Dec 2020 18:11:44 GMT  
		Size: 43.7 MB (43690210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73c267ce2f07457ee99cb1e4ee8cf91ee4db80db062781db61b58043e6630ef`  
		Last Modified: Sat, 12 Dec 2020 18:11:38 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828a9641b3ab6a9523840af6981d3d3ecfc00afbce4c4e31fc39930542fccddf`  
		Last Modified: Sat, 12 Dec 2020 18:11:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b563f0db78dd870850899b7fffaeedf9fd9cc882315196b79ad1837676946f5`  
		Last Modified: Sat, 12 Dec 2020 18:11:38 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:d78749199ec26b1313131548f125f1595bcaba8f19fa40eff30a6eb6d05b2f62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41749676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a4486a0b825fa5403d9d2449076e560f2b30976a4ae39ecd82fd97f222007be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 00:54:32 GMT
ENV CONSUL_VERSION=1.8.7
# Sat, 12 Dec 2020 00:54:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 00:54:44 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 00:54:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 00:55:01 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 00:55:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 00:55:06 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 00:55:08 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 00:55:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 00:55:11 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 00:55:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 00:55:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 00:55:17 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f867519477f47aa70333212857fd1ddb46b69bf4b98f518e1bbe496438bef1e`  
		Last Modified: Sat, 12 Dec 2020 00:56:44 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac0e237f16c96907f707d86f37dda73ac40da0793884c2bb4fa1e67fbccbc04`  
		Last Modified: Sat, 12 Dec 2020 00:56:54 GMT  
		Size: 39.1 MB (39144390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74c932c87fa8ab2b3cd86e4bf0aef7aa6adc3ed9fa50da38be177307f3c563c`  
		Last Modified: Sat, 12 Dec 2020 00:56:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccf3c7a7aa5c54f02663b1de91e984939c9f1354c58aee6a6a3aa3c8d27ba2b`  
		Last Modified: Sat, 12 Dec 2020 00:56:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab18aa67b4fa150d63f8e9e8a82430c854fcf2e0de132e88d335c1bec6cea07`  
		Last Modified: Sat, 12 Dec 2020 00:56:43 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1a35f1ef79f8c8485f695a16385f32aa161c7d72e54fc7533bfdbb1b512bc99d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41922422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2302ba2caae5a6a35ad9f35271c7684c2d15befe556695f5367ba1f143731340`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 14:08:04 GMT
ENV CONSUL_VERSION=1.8.7
# Sat, 12 Dec 2020 14:08:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 14:08:08 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 14:08:14 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 14:08:17 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 14:08:18 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 14:08:19 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 14:08:20 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 14:08:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 14:08:21 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 14:08:22 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 14:08:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 14:08:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebd7aff50e3b65b8c18402716fd1ce5d2d97de2bf856953410d51b1082b1b7f`  
		Last Modified: Sat, 12 Dec 2020 14:09:27 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c0d7faf267bf65aba7a1d0e9f8562170e12c03e7bbf12260d44fcefeab243a`  
		Last Modified: Sat, 12 Dec 2020 14:09:36 GMT  
		Size: 39.2 MB (39212510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c39d9c93d21f37cd1d1003d0912ffa8c5560292d3206e39318bb7588d820fa`  
		Last Modified: Sat, 12 Dec 2020 14:09:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3a1facbf5164132306c810a5016c33aea489b57da3975ac0face40c38c4c70`  
		Last Modified: Sat, 12 Dec 2020 14:09:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fda8a31b605c2fe24343e315f58d5cf3ec4d8b50aa97fa26d3c71de60c24b4`  
		Last Modified: Sat, 12 Dec 2020 14:09:27 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:b0af803e62b91e0722e8134424a18df9aaff32259de97c1119fec8cd79cc3587
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46007452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e73b950ce7b31842d5256385cfc2ed3f15ab37f14705304e251d70c8ef8cdfb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:57:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 16:21:57 GMT
ENV CONSUL_VERSION=1.8.7
# Sat, 12 Dec 2020 16:21:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 16:21:58 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 16:22:06 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 16:22:07 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 16:22:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 16:22:09 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 16:22:09 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 16:22:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 16:22:09 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 16:22:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 16:22:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 16:22:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf00cc0ce55903c54b90dbfba43fbca4c38a0d2334075b03814a2204873b5bd`  
		Last Modified: Sat, 12 Dec 2020 16:23:05 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7c00be4b9f44436d687aef80f5b3089db6f90ce291548ed5c104bd05aad77`  
		Last Modified: Sat, 12 Dec 2020 16:23:19 GMT  
		Size: 43.2 MB (43212717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3f88b2f4add19ec60ce6f97221041ed65ff3747828bdeae4eac00946b7707d`  
		Last Modified: Sat, 12 Dec 2020 16:23:05 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43c4bbfc828ecfafee606ef32344424dfbd9cdebaf73369c65e6a4a71d6c3b4`  
		Last Modified: Sat, 12 Dec 2020 16:23:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a93c872f6731243f74b1bef918a4421e3999d7132325e0e77653252233882d4`  
		Last Modified: Sat, 12 Dec 2020 16:23:05 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.7`

```console
$ docker pull consul@sha256:764e86d2b5deb2abf01d523fd85981e8039a226ad4984edb2f7ccc14cf2cbc49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.7` - linux; amd64

```console
$ docker pull consul@sha256:9160035c831a0e976acfdd6f2a40af5db7bb646adbd74fb832c0d7bd7efcbb06
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46490386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b404af955f9a59e02d0b99fd3d318d0130e2c1a1051ae9668e304fade204c53d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 18:10:49 GMT
ENV CONSUL_VERSION=1.8.7
# Sat, 12 Dec 2020 18:10:49 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 18:10:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 18:10:54 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 18:10:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 18:10:56 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 18:10:57 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 18:10:57 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 18:10:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 18:10:57 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 18:10:58 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 18:10:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 18:10:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c6e57714d98115cef3592709bbdccf649f3c8bfa4381aee05b86fd7c93a881d`  
		Last Modified: Sat, 12 Dec 2020 18:11:38 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9106f38e55f03273066533b61332ca498e63bacb91839b5559ce4599ed864cf0`  
		Last Modified: Sat, 12 Dec 2020 18:11:44 GMT  
		Size: 43.7 MB (43690210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73c267ce2f07457ee99cb1e4ee8cf91ee4db80db062781db61b58043e6630ef`  
		Last Modified: Sat, 12 Dec 2020 18:11:38 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828a9641b3ab6a9523840af6981d3d3ecfc00afbce4c4e31fc39930542fccddf`  
		Last Modified: Sat, 12 Dec 2020 18:11:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b563f0db78dd870850899b7fffaeedf9fd9cc882315196b79ad1837676946f5`  
		Last Modified: Sat, 12 Dec 2020 18:11:38 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:d78749199ec26b1313131548f125f1595bcaba8f19fa40eff30a6eb6d05b2f62
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41749676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a4486a0b825fa5403d9d2449076e560f2b30976a4ae39ecd82fd97f222007be`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 00:54:32 GMT
ENV CONSUL_VERSION=1.8.7
# Sat, 12 Dec 2020 00:54:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 00:54:44 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 00:54:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 00:55:01 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 00:55:05 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 00:55:06 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 00:55:08 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 00:55:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 00:55:11 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 00:55:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 00:55:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 00:55:17 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f867519477f47aa70333212857fd1ddb46b69bf4b98f518e1bbe496438bef1e`  
		Last Modified: Sat, 12 Dec 2020 00:56:44 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac0e237f16c96907f707d86f37dda73ac40da0793884c2bb4fa1e67fbccbc04`  
		Last Modified: Sat, 12 Dec 2020 00:56:54 GMT  
		Size: 39.1 MB (39144390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74c932c87fa8ab2b3cd86e4bf0aef7aa6adc3ed9fa50da38be177307f3c563c`  
		Last Modified: Sat, 12 Dec 2020 00:56:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccf3c7a7aa5c54f02663b1de91e984939c9f1354c58aee6a6a3aa3c8d27ba2b`  
		Last Modified: Sat, 12 Dec 2020 00:56:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab18aa67b4fa150d63f8e9e8a82430c854fcf2e0de132e88d335c1bec6cea07`  
		Last Modified: Sat, 12 Dec 2020 00:56:43 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1a35f1ef79f8c8485f695a16385f32aa161c7d72e54fc7533bfdbb1b512bc99d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41922422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2302ba2caae5a6a35ad9f35271c7684c2d15befe556695f5367ba1f143731340`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 14:08:04 GMT
ENV CONSUL_VERSION=1.8.7
# Sat, 12 Dec 2020 14:08:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 14:08:08 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 14:08:14 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 14:08:17 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 14:08:18 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 14:08:19 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 14:08:20 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 14:08:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 14:08:21 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 14:08:22 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 14:08:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 14:08:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebd7aff50e3b65b8c18402716fd1ce5d2d97de2bf856953410d51b1082b1b7f`  
		Last Modified: Sat, 12 Dec 2020 14:09:27 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c0d7faf267bf65aba7a1d0e9f8562170e12c03e7bbf12260d44fcefeab243a`  
		Last Modified: Sat, 12 Dec 2020 14:09:36 GMT  
		Size: 39.2 MB (39212510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c39d9c93d21f37cd1d1003d0912ffa8c5560292d3206e39318bb7588d820fa`  
		Last Modified: Sat, 12 Dec 2020 14:09:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3a1facbf5164132306c810a5016c33aea489b57da3975ac0face40c38c4c70`  
		Last Modified: Sat, 12 Dec 2020 14:09:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fda8a31b605c2fe24343e315f58d5cf3ec4d8b50aa97fa26d3c71de60c24b4`  
		Last Modified: Sat, 12 Dec 2020 14:09:27 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.7` - linux; 386

```console
$ docker pull consul@sha256:b0af803e62b91e0722e8134424a18df9aaff32259de97c1119fec8cd79cc3587
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46007452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e73b950ce7b31842d5256385cfc2ed3f15ab37f14705304e251d70c8ef8cdfb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:57:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 16:21:57 GMT
ENV CONSUL_VERSION=1.8.7
# Sat, 12 Dec 2020 16:21:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 16:21:58 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 16:22:06 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 16:22:07 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 16:22:08 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 16:22:09 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 16:22:09 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 16:22:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 16:22:09 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 16:22:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 16:22:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 16:22:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcf00cc0ce55903c54b90dbfba43fbca4c38a0d2334075b03814a2204873b5bd`  
		Last Modified: Sat, 12 Dec 2020 16:23:05 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a7c00be4b9f44436d687aef80f5b3089db6f90ce291548ed5c104bd05aad77`  
		Last Modified: Sat, 12 Dec 2020 16:23:19 GMT  
		Size: 43.2 MB (43212717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3f88b2f4add19ec60ce6f97221041ed65ff3747828bdeae4eac00946b7707d`  
		Last Modified: Sat, 12 Dec 2020 16:23:05 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43c4bbfc828ecfafee606ef32344424dfbd9cdebaf73369c65e6a4a71d6c3b4`  
		Last Modified: Sat, 12 Dec 2020 16:23:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a93c872f6731243f74b1bef918a4421e3999d7132325e0e77653252233882d4`  
		Last Modified: Sat, 12 Dec 2020 16:23:05 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:cc7b4d6ab8f9566698d427a0bf15a5131841b02d7288588b71e5854c37bd98ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:ee35e3fd2b35d790a533464e50f6fe43aafa0e3806354cc0265d95b35f7400e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45570396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958f2bba75997fafbccecdfb4b4300dfc99c64fd56d2833f840768f730b1052e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 18:10:35 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 18:10:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 18:10:36 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 18:10:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 18:10:42 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 18:10:43 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 18:10:43 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 18:10:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 18:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 18:10:44 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a3cabec490762fe7c1682455f9a2b2e320ceae8da91eb35b37c39b5783e403`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0538a1f915b778b756a74592840a68bf5b6a5bc60ab99f8f856079acf8c21c`  
		Last Modified: Sat, 12 Dec 2020 18:11:32 GMT  
		Size: 42.8 MB (42770214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f6bd70bdf9ab843e9922f4b141362c6f21dd373b57f1e0d9e05be832275994`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7e79697988f100cf30f3f1e08e02fc6c521d767147c9d4df66e349147dddba`  
		Last Modified: Sat, 12 Dec 2020 18:11:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce30221736f3aa7199e6ed008bd3220f589bce402fdf97dabc10bf0f59fef5c3`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:ba2cf92ad7a299b67b0836ec07dc80362f4e4983ef588cf78778a5c8b1453a55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40832579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41486a63c4ded8d1f8cac34fd763459ae65be3c5802bef1fed8232cc2f8336d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 00:53:40 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 00:53:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 00:53:46 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 00:53:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 00:53:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 00:54:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 00:54:03 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 00:54:04 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 00:54:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 00:54:08 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 00:54:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 00:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 00:54:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f07005897aa5ca7dc61824b38a71822bf3c41d8ee1381f410f3cec7e71295e`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0abaf0b0db4322f0c362e05a8f33b4bd9459c9e5b10d7fb9460d51bd0aec91`  
		Last Modified: Sat, 12 Dec 2020 00:56:33 GMT  
		Size: 38.2 MB (38227295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd18ac82951699c3cf6a5d413f6934917c183b4e08716016d14566525a71bcd0`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326c928d9eb761f450fad803c5bc4643fa105e666092783558b85557c8b3bc0`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48742b61655f27ca3ed3c85be1b091efb7b1e1024749a53d4984a4c1e178bf8d`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:01d2cef184a6ff688693974cfcc36c5d92f9a37832381b2a008e460b26d358f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41052267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e983dda7fd04f095f885f204ae5c644845ca023ce29555418af478cf5d046c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 14:07:35 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 14:07:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 14:07:37 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 14:07:44 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 14:07:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 14:07:50 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 14:07:51 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 14:07:52 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 14:07:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 14:07:55 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 14:07:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 14:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 14:07:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c8060704c53f3ff052629f979f702282b4cdedc728a02c83ddfcb511067de2`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fc274a81c60ca4deddc3eb2021465a3cacb68e5c35024212cf02fa2a3055da`  
		Last Modified: Sat, 12 Dec 2020 14:09:16 GMT  
		Size: 38.3 MB (38342356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421085bf757533067046c72d4f76aa17383fe82a1c5a709df6015e5f3f7a3af3`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92d7c3c09e2f09ab13919755506eb2699a0dbcf2b107a570e6bc9ca536be912`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa6ebe29a594ab16a614fc400231c0e5d0b79f316e51ebf17b0ebcdd0db9875`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:06faa80f0bfba7962ff496d09fb892760439823eabe40c6915f3a32cce950018
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44903544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3a426b880d0017fa66288c3a1f92a89a9a425e86cbcda5d66762a0fec10258`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:57:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 16:21:38 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 16:21:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 16:21:39 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 16:21:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 16:21:48 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 16:21:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 16:21:50 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 16:21:50 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 16:21:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 16:21:51 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 16:21:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 16:21:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 16:21:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d44decd170c537cbf0169cb6157dbce3addc3082d52007a874f5f02f907ec3`  
		Last Modified: Sat, 12 Dec 2020 16:22:45 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b95d7a59da7c28695c7b52be91ec48f2abeaf8a7772b472d3422d1c0e7bfbb4`  
		Last Modified: Sat, 12 Dec 2020 16:22:57 GMT  
		Size: 42.1 MB (42108808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e398434dc9091267104c4cc6271516cdff49e87102373432f2294ffa99b3dc2`  
		Last Modified: Sat, 12 Dec 2020 16:22:44 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c6b429057f7e0f03ee300f359dc209beedaae65ad4733c1006a2552f98ea6`  
		Last Modified: Sat, 12 Dec 2020 16:22:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1977bb69b681a65c762e379e90c09ff9913147a1c76be17b8338df50330aaf2a`  
		Last Modified: Sat, 12 Dec 2020 16:22:45 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.1`

```console
$ docker pull consul@sha256:cc7b4d6ab8f9566698d427a0bf15a5131841b02d7288588b71e5854c37bd98ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.1` - linux; amd64

```console
$ docker pull consul@sha256:ee35e3fd2b35d790a533464e50f6fe43aafa0e3806354cc0265d95b35f7400e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45570396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958f2bba75997fafbccecdfb4b4300dfc99c64fd56d2833f840768f730b1052e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 18:10:35 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 18:10:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 18:10:36 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 18:10:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 18:10:42 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 18:10:43 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 18:10:43 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 18:10:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 18:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 18:10:44 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a3cabec490762fe7c1682455f9a2b2e320ceae8da91eb35b37c39b5783e403`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0538a1f915b778b756a74592840a68bf5b6a5bc60ab99f8f856079acf8c21c`  
		Last Modified: Sat, 12 Dec 2020 18:11:32 GMT  
		Size: 42.8 MB (42770214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f6bd70bdf9ab843e9922f4b141362c6f21dd373b57f1e0d9e05be832275994`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7e79697988f100cf30f3f1e08e02fc6c521d767147c9d4df66e349147dddba`  
		Last Modified: Sat, 12 Dec 2020 18:11:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce30221736f3aa7199e6ed008bd3220f589bce402fdf97dabc10bf0f59fef5c3`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:ba2cf92ad7a299b67b0836ec07dc80362f4e4983ef588cf78778a5c8b1453a55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40832579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41486a63c4ded8d1f8cac34fd763459ae65be3c5802bef1fed8232cc2f8336d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 00:53:40 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 00:53:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 00:53:46 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 00:53:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 00:53:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 00:54:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 00:54:03 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 00:54:04 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 00:54:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 00:54:08 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 00:54:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 00:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 00:54:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f07005897aa5ca7dc61824b38a71822bf3c41d8ee1381f410f3cec7e71295e`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0abaf0b0db4322f0c362e05a8f33b4bd9459c9e5b10d7fb9460d51bd0aec91`  
		Last Modified: Sat, 12 Dec 2020 00:56:33 GMT  
		Size: 38.2 MB (38227295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd18ac82951699c3cf6a5d413f6934917c183b4e08716016d14566525a71bcd0`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326c928d9eb761f450fad803c5bc4643fa105e666092783558b85557c8b3bc0`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48742b61655f27ca3ed3c85be1b091efb7b1e1024749a53d4984a4c1e178bf8d`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:01d2cef184a6ff688693974cfcc36c5d92f9a37832381b2a008e460b26d358f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41052267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e983dda7fd04f095f885f204ae5c644845ca023ce29555418af478cf5d046c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 14:07:35 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 14:07:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 14:07:37 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 14:07:44 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 14:07:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 14:07:50 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 14:07:51 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 14:07:52 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 14:07:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 14:07:55 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 14:07:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 14:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 14:07:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c8060704c53f3ff052629f979f702282b4cdedc728a02c83ddfcb511067de2`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fc274a81c60ca4deddc3eb2021465a3cacb68e5c35024212cf02fa2a3055da`  
		Last Modified: Sat, 12 Dec 2020 14:09:16 GMT  
		Size: 38.3 MB (38342356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421085bf757533067046c72d4f76aa17383fe82a1c5a709df6015e5f3f7a3af3`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92d7c3c09e2f09ab13919755506eb2699a0dbcf2b107a570e6bc9ca536be912`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa6ebe29a594ab16a614fc400231c0e5d0b79f316e51ebf17b0ebcdd0db9875`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.1` - linux; 386

```console
$ docker pull consul@sha256:06faa80f0bfba7962ff496d09fb892760439823eabe40c6915f3a32cce950018
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44903544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3a426b880d0017fa66288c3a1f92a89a9a425e86cbcda5d66762a0fec10258`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:57:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 16:21:38 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 16:21:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 16:21:39 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 16:21:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 16:21:48 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 16:21:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 16:21:50 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 16:21:50 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 16:21:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 16:21:51 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 16:21:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 16:21:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 16:21:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d44decd170c537cbf0169cb6157dbce3addc3082d52007a874f5f02f907ec3`  
		Last Modified: Sat, 12 Dec 2020 16:22:45 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b95d7a59da7c28695c7b52be91ec48f2abeaf8a7772b472d3422d1c0e7bfbb4`  
		Last Modified: Sat, 12 Dec 2020 16:22:57 GMT  
		Size: 42.1 MB (42108808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e398434dc9091267104c4cc6271516cdff49e87102373432f2294ffa99b3dc2`  
		Last Modified: Sat, 12 Dec 2020 16:22:44 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c6b429057f7e0f03ee300f359dc209beedaae65ad4733c1006a2552f98ea6`  
		Last Modified: Sat, 12 Dec 2020 16:22:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1977bb69b681a65c762e379e90c09ff9913147a1c76be17b8338df50330aaf2a`  
		Last Modified: Sat, 12 Dec 2020 16:22:45 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:cc7b4d6ab8f9566698d427a0bf15a5131841b02d7288588b71e5854c37bd98ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:ee35e3fd2b35d790a533464e50f6fe43aafa0e3806354cc0265d95b35f7400e1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45570396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:958f2bba75997fafbccecdfb4b4300dfc99c64fd56d2833f840768f730b1052e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 02:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 18:10:35 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 18:10:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 18:10:36 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 18:10:41 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 18:10:42 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 18:10:43 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 18:10:43 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 18:10:43 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 18:10:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 18:10:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 18:10:44 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a3cabec490762fe7c1682455f9a2b2e320ceae8da91eb35b37c39b5783e403`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0538a1f915b778b756a74592840a68bf5b6a5bc60ab99f8f856079acf8c21c`  
		Last Modified: Sat, 12 Dec 2020 18:11:32 GMT  
		Size: 42.8 MB (42770214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f6bd70bdf9ab843e9922f4b141362c6f21dd373b57f1e0d9e05be832275994`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc7e79697988f100cf30f3f1e08e02fc6c521d767147c9d4df66e349147dddba`  
		Last Modified: Sat, 12 Dec 2020 18:11:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce30221736f3aa7199e6ed008bd3220f589bce402fdf97dabc10bf0f59fef5c3`  
		Last Modified: Sat, 12 Dec 2020 18:11:25 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:ba2cf92ad7a299b67b0836ec07dc80362f4e4983ef588cf78778a5c8b1453a55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40832579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41486a63c4ded8d1f8cac34fd763459ae65be3c5802bef1fed8232cc2f8336d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:12:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 00:53:40 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 00:53:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 00:53:46 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 00:53:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 00:53:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 00:54:02 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 00:54:03 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 00:54:04 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 00:54:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 00:54:08 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 00:54:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 00:54:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 00:54:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f07005897aa5ca7dc61824b38a71822bf3c41d8ee1381f410f3cec7e71295e`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0abaf0b0db4322f0c362e05a8f33b4bd9459c9e5b10d7fb9460d51bd0aec91`  
		Last Modified: Sat, 12 Dec 2020 00:56:33 GMT  
		Size: 38.2 MB (38227295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd18ac82951699c3cf6a5d413f6934917c183b4e08716016d14566525a71bcd0`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5326c928d9eb761f450fad803c5bc4643fa105e666092783558b85557c8b3bc0`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48742b61655f27ca3ed3c85be1b091efb7b1e1024749a53d4984a4c1e178bf8d`  
		Last Modified: Sat, 12 Dec 2020 00:56:24 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:01d2cef184a6ff688693974cfcc36c5d92f9a37832381b2a008e460b26d358f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41052267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e983dda7fd04f095f885f204ae5c644845ca023ce29555418af478cf5d046c7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:42:58 GMT
ADD file:a1a6d0f8dffb9bc75438921cdb5c04d2f2f49400a7526dcf3d8dff9238e3235a in / 
# Fri, 11 Dec 2020 02:43:00 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 03:36:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 14:07:35 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 14:07:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 14:07:37 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 14:07:44 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 14:07:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 14:07:50 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 14:07:51 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 14:07:52 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 14:07:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 14:07:55 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 14:07:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 14:07:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 14:07:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a3cc7d3b244e0bac4f32b7529f804d1ab735b088ea432061c3949b2a890b919f`  
		Last Modified: Fri, 11 Dec 2020 02:43:46 GMT  
		Size: 2.7 MB (2706619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c8060704c53f3ff052629f979f702282b4cdedc728a02c83ddfcb511067de2`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fc274a81c60ca4deddc3eb2021465a3cacb68e5c35024212cf02fa2a3055da`  
		Last Modified: Sat, 12 Dec 2020 14:09:16 GMT  
		Size: 38.3 MB (38342356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421085bf757533067046c72d4f76aa17383fe82a1c5a709df6015e5f3f7a3af3`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f92d7c3c09e2f09ab13919755506eb2699a0dbcf2b107a570e6bc9ca536be912`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa6ebe29a594ab16a614fc400231c0e5d0b79f316e51ebf17b0ebcdd0db9875`  
		Last Modified: Sat, 12 Dec 2020 14:09:08 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:06faa80f0bfba7962ff496d09fb892760439823eabe40c6915f3a32cce950018
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44903544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3a426b880d0017fa66288c3a1f92a89a9a425e86cbcda5d66762a0fec10258`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:01:14 GMT
ADD file:8812e502f26af2dc4efdfb7387f8bf99f2a098b6c95b9f6abf900df2ce74e3da in / 
# Fri, 11 Dec 2020 02:01:14 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 05:57:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Sat, 12 Dec 2020 16:21:38 GMT
ENV CONSUL_VERSION=1.9.1
# Sat, 12 Dec 2020 16:21:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Dec 2020 16:21:39 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Dec 2020 16:21:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Dec 2020 16:21:48 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Dec 2020 16:21:49 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Dec 2020 16:21:50 GMT
VOLUME [/consul/data]
# Sat, 12 Dec 2020 16:21:50 GMT
EXPOSE 8300
# Sat, 12 Dec 2020 16:21:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Dec 2020 16:21:51 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Dec 2020 16:21:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Dec 2020 16:21:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Dec 2020 16:21:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b62269920a7a62a905817c7c1b33f33b6e658121e9a054715ff052a23f7de3a0`  
		Last Modified: Fri, 11 Dec 2020 02:01:43 GMT  
		Size: 2.8 MB (2791504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d44decd170c537cbf0169cb6157dbce3addc3082d52007a874f5f02f907ec3`  
		Last Modified: Sat, 12 Dec 2020 16:22:45 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b95d7a59da7c28695c7b52be91ec48f2abeaf8a7772b472d3422d1c0e7bfbb4`  
		Last Modified: Sat, 12 Dec 2020 16:22:57 GMT  
		Size: 42.1 MB (42108808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e398434dc9091267104c4cc6271516cdff49e87102373432f2294ffa99b3dc2`  
		Last Modified: Sat, 12 Dec 2020 16:22:44 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09c6b429057f7e0f03ee300f359dc209beedaae65ad4733c1006a2552f98ea6`  
		Last Modified: Sat, 12 Dec 2020 16:22:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1977bb69b681a65c762e379e90c09ff9913147a1c76be17b8338df50330aaf2a`  
		Last Modified: Sat, 12 Dec 2020 16:22:45 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
