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
$ docker pull consul@sha256:6ed45c51448faf0bccd93678bc47003c9090eeb4785059baf777db92d5828188
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:99ce7f93fa338b174b41e4232ab629ce04a36d4a89eba5d8a253d867f45d4f08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43132781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea0d70916c0f52a063e51028a42816593e4f3e61c54115efe6ffa51900d3d7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:55:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:58:27 GMT
ARG CONSUL_VERSION=1.7.13
# Thu, 01 Apr 2021 13:58:27 GMT
LABEL org.opencontainers.image.version=1.7.13
# Thu, 01 Apr 2021 13:58:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:58:28 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:58:33 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:58:34 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:58:35 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:58:36 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:58:36 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:58:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:58:36 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:58:36 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:58:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d76bfb1d9f848c669287051235329a8f47f5263bbf6e01baf0e6a9d750b13a`  
		Last Modified: Thu, 01 Apr 2021 13:59:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff4edafd1eaccf1815c24781c204035dca6796707a5b16ab4867f69408b65f`  
		Last Modified: Thu, 01 Apr 2021 13:59:44 GMT  
		Size: 40.3 MB (40329779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e31edf64debe816fbd0b0a0c559284d9d7d558fe17fd050dc6494791351e1c`  
		Last Modified: Thu, 01 Apr 2021 13:59:38 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae22bedb3935281cb594a2eaf0f0d232c9a2360bb309dbe35165b8a4db93de6`  
		Last Modified: Thu, 01 Apr 2021 13:59:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a41c1db4f3ee381cd5f185723ec27c880de5a81f45e6df153f9ecc10312dd47`  
		Last Modified: Thu, 01 Apr 2021 13:59:37 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:56d4778b8542176ab9f9787f283c11a51db09ae620e335210acfe30b5264df86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38829684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff0c663b94bafa65171effcad2ce02299d760c2abf094c491344bfb2780cbc1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:17:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 31 Mar 2021 18:19:48 GMT
ARG CONSUL_VERSION=1.7.13
# Wed, 31 Mar 2021 18:19:50 GMT
LABEL org.opencontainers.image.version=1.7.13
# Wed, 31 Mar 2021 18:19:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 31 Mar 2021 18:19:54 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 31 Mar 2021 18:20:05 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 31 Mar 2021 18:20:09 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 31 Mar 2021 18:20:11 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:20:12 GMT
VOLUME [/consul/data]
# Wed, 31 Mar 2021 18:20:13 GMT
EXPOSE 8300
# Wed, 31 Mar 2021 18:20:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 31 Mar 2021 18:20:15 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 31 Mar 2021 18:20:16 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Mar 2021 18:20:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 18:20:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0529e7baba67302a45e39b19648a7a5087420bd12e6c5e7edd264de9bf0c5246`  
		Last Modified: Wed, 31 Mar 2021 18:21:19 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe80981258c00e5deeae7d6a7bd7c31df363947dfc611fc8f63f58c0da83539c`  
		Last Modified: Wed, 31 Mar 2021 18:21:29 GMT  
		Size: 36.2 MB (36221735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a12e832dc4bf86a46031d49fdf7baec415ef626977c66eb162dd10bc0991259`  
		Last Modified: Wed, 31 Mar 2021 18:21:19 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2575599c9a8e8beba97f517f4a60988ab6436cbc40263726f09e72b20799ce06`  
		Last Modified: Wed, 31 Mar 2021 18:21:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65db31c460e548d6b2581483491186419b784f36355111139539d912f60190dc`  
		Last Modified: Wed, 31 Mar 2021 18:21:19 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:8968c269311883718bad6baa0bc9f3598398fb9ba64332b5e8fd36651fa3727e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39044354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:727a3b1133355abecc34c8038176c9a76bcc6811d43e4b59f42e727d35939fa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:15:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:16:32 GMT
ARG CONSUL_VERSION=1.7.13
# Thu, 01 Apr 2021 13:16:33 GMT
LABEL org.opencontainers.image.version=1.7.13
# Thu, 01 Apr 2021 13:16:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:16:37 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:16:44 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:16:46 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:16:49 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:16:49 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:16:50 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:16:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:16:52 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:16:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:16:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:16:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e5c1aefa210ae3dfecac0ec872610e683f104f805a547562211705ce103d98`  
		Last Modified: Thu, 01 Apr 2021 13:17:50 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c6d5db760cb467f096f671cbe5e4d0536e60d2407e8b55a45d5256bbc929fa`  
		Last Modified: Thu, 01 Apr 2021 13:18:02 GMT  
		Size: 36.3 MB (36331208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dbae4541b4e4e62e9ffbf1e5339a2d74dc196d0507520bcf608570d760976a`  
		Last Modified: Thu, 01 Apr 2021 13:17:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5110b4103739ee727ff2078d70e9aed949d2423720fb887cb2ec21cd55d28934`  
		Last Modified: Thu, 01 Apr 2021 13:17:50 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fda23495846065e1d5e97c572e365dbaac409a8d282967a2fa660f46c0b831`  
		Last Modified: Thu, 01 Apr 2021 13:17:50 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:1cfda55781340c835db6260551947813b1459e0b905f2046b59aff0ca9bddad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41938947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58104fb1f88b8045824c49cc20ffb9b198b8f9161b549e393fbc28ea35d21d77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:08 GMT
ADD file:053c3a6154e80758106cbf0fec936c3b41dabf24a9f5eda36416caa90556810c in / 
# Wed, 31 Mar 2021 17:43:09 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:21:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 01:22:32 GMT
ARG CONSUL_VERSION=1.7.13
# Thu, 01 Apr 2021 01:22:32 GMT
LABEL org.opencontainers.image.version=1.7.13
# Thu, 01 Apr 2021 01:22:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 01:22:33 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 01:22:38 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 01:22:39 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 01:22:40 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 01:22:40 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 01:22:41 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 01:22:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 01:22:41 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 01:22:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 01:22:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 01:22:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8eca83e4805e4c5e7b071425a4603bc4b02885b817aa7c1bba9605bd2cb9125a`  
		Last Modified: Wed, 31 Mar 2021 17:44:26 GMT  
		Size: 2.8 MB (2794977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893ce3db6debc969dedbf90babb2c4f7f699f290229304eb62073d129908bdd5`  
		Last Modified: Thu, 01 Apr 2021 01:23:53 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f3307521d89857d4a61746c0acbd35571281218a1a8052c016ad66eefb9600`  
		Last Modified: Thu, 01 Apr 2021 01:24:00 GMT  
		Size: 39.1 MB (39140678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767934d01d9396ad8790e5d2437107e3150c474916e2d07ca60cb854be82945`  
		Last Modified: Thu, 01 Apr 2021 01:23:53 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0a4538b413e1c29dceac731f5ce84b6c869fe10ebee8534102241ffaeb503d`  
		Last Modified: Thu, 01 Apr 2021 01:23:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357d41df9e29d8c63d89e757c7660ee4be8b02fc9d661bc6a2f4c8511e4364c9`  
		Last Modified: Thu, 01 Apr 2021 01:23:53 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.13`

```console
$ docker pull consul@sha256:6ed45c51448faf0bccd93678bc47003c9090eeb4785059baf777db92d5828188
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.13` - linux; amd64

```console
$ docker pull consul@sha256:99ce7f93fa338b174b41e4232ab629ce04a36d4a89eba5d8a253d867f45d4f08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43132781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ea0d70916c0f52a063e51028a42816593e4f3e61c54115efe6ffa51900d3d7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:55:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:58:27 GMT
ARG CONSUL_VERSION=1.7.13
# Thu, 01 Apr 2021 13:58:27 GMT
LABEL org.opencontainers.image.version=1.7.13
# Thu, 01 Apr 2021 13:58:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:58:28 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:58:33 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:58:34 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:58:35 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:58:36 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:58:36 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:58:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:58:36 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:58:36 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:58:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:58:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d76bfb1d9f848c669287051235329a8f47f5263bbf6e01baf0e6a9d750b13a`  
		Last Modified: Thu, 01 Apr 2021 13:59:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dff4edafd1eaccf1815c24781c204035dca6796707a5b16ab4867f69408b65f`  
		Last Modified: Thu, 01 Apr 2021 13:59:44 GMT  
		Size: 40.3 MB (40329779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e31edf64debe816fbd0b0a0c559284d9d7d558fe17fd050dc6494791351e1c`  
		Last Modified: Thu, 01 Apr 2021 13:59:38 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae22bedb3935281cb594a2eaf0f0d232c9a2360bb309dbe35165b8a4db93de6`  
		Last Modified: Thu, 01 Apr 2021 13:59:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a41c1db4f3ee381cd5f185723ec27c880de5a81f45e6df153f9ecc10312dd47`  
		Last Modified: Thu, 01 Apr 2021 13:59:37 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.13` - linux; arm variant v6

```console
$ docker pull consul@sha256:56d4778b8542176ab9f9787f283c11a51db09ae620e335210acfe30b5264df86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38829684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff0c663b94bafa65171effcad2ce02299d760c2abf094c491344bfb2780cbc1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:17:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 31 Mar 2021 18:19:48 GMT
ARG CONSUL_VERSION=1.7.13
# Wed, 31 Mar 2021 18:19:50 GMT
LABEL org.opencontainers.image.version=1.7.13
# Wed, 31 Mar 2021 18:19:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 31 Mar 2021 18:19:54 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 31 Mar 2021 18:20:05 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 31 Mar 2021 18:20:09 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 31 Mar 2021 18:20:11 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:20:12 GMT
VOLUME [/consul/data]
# Wed, 31 Mar 2021 18:20:13 GMT
EXPOSE 8300
# Wed, 31 Mar 2021 18:20:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 31 Mar 2021 18:20:15 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 31 Mar 2021 18:20:16 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Mar 2021 18:20:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 18:20:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0529e7baba67302a45e39b19648a7a5087420bd12e6c5e7edd264de9bf0c5246`  
		Last Modified: Wed, 31 Mar 2021 18:21:19 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe80981258c00e5deeae7d6a7bd7c31df363947dfc611fc8f63f58c0da83539c`  
		Last Modified: Wed, 31 Mar 2021 18:21:29 GMT  
		Size: 36.2 MB (36221735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a12e832dc4bf86a46031d49fdf7baec415ef626977c66eb162dd10bc0991259`  
		Last Modified: Wed, 31 Mar 2021 18:21:19 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2575599c9a8e8beba97f517f4a60988ab6436cbc40263726f09e72b20799ce06`  
		Last Modified: Wed, 31 Mar 2021 18:21:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65db31c460e548d6b2581483491186419b784f36355111139539d912f60190dc`  
		Last Modified: Wed, 31 Mar 2021 18:21:19 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.13` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:8968c269311883718bad6baa0bc9f3598398fb9ba64332b5e8fd36651fa3727e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39044354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:727a3b1133355abecc34c8038176c9a76bcc6811d43e4b59f42e727d35939fa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:15:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:16:32 GMT
ARG CONSUL_VERSION=1.7.13
# Thu, 01 Apr 2021 13:16:33 GMT
LABEL org.opencontainers.image.version=1.7.13
# Thu, 01 Apr 2021 13:16:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:16:37 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:16:44 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:16:46 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:16:49 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:16:49 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:16:50 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:16:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:16:52 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:16:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:16:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:16:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e5c1aefa210ae3dfecac0ec872610e683f104f805a547562211705ce103d98`  
		Last Modified: Thu, 01 Apr 2021 13:17:50 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c6d5db760cb467f096f671cbe5e4d0536e60d2407e8b55a45d5256bbc929fa`  
		Last Modified: Thu, 01 Apr 2021 13:18:02 GMT  
		Size: 36.3 MB (36331208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dbae4541b4e4e62e9ffbf1e5339a2d74dc196d0507520bcf608570d760976a`  
		Last Modified: Thu, 01 Apr 2021 13:17:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5110b4103739ee727ff2078d70e9aed949d2423720fb887cb2ec21cd55d28934`  
		Last Modified: Thu, 01 Apr 2021 13:17:50 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fda23495846065e1d5e97c572e365dbaac409a8d282967a2fa660f46c0b831`  
		Last Modified: Thu, 01 Apr 2021 13:17:50 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.13` - linux; 386

```console
$ docker pull consul@sha256:1cfda55781340c835db6260551947813b1459e0b905f2046b59aff0ca9bddad0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41938947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58104fb1f88b8045824c49cc20ffb9b198b8f9161b549e393fbc28ea35d21d77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:08 GMT
ADD file:053c3a6154e80758106cbf0fec936c3b41dabf24a9f5eda36416caa90556810c in / 
# Wed, 31 Mar 2021 17:43:09 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:21:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 01:22:32 GMT
ARG CONSUL_VERSION=1.7.13
# Thu, 01 Apr 2021 01:22:32 GMT
LABEL org.opencontainers.image.version=1.7.13
# Thu, 01 Apr 2021 01:22:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 01:22:33 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 01:22:38 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 01:22:39 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 01:22:40 GMT
# ARGS: CONSUL_VERSION=1.7.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 01:22:40 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 01:22:41 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 01:22:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 01:22:41 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 01:22:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 01:22:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 01:22:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8eca83e4805e4c5e7b071425a4603bc4b02885b817aa7c1bba9605bd2cb9125a`  
		Last Modified: Wed, 31 Mar 2021 17:44:26 GMT  
		Size: 2.8 MB (2794977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893ce3db6debc969dedbf90babb2c4f7f699f290229304eb62073d129908bdd5`  
		Last Modified: Thu, 01 Apr 2021 01:23:53 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f3307521d89857d4a61746c0acbd35571281218a1a8052c016ad66eefb9600`  
		Last Modified: Thu, 01 Apr 2021 01:24:00 GMT  
		Size: 39.1 MB (39140678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b767934d01d9396ad8790e5d2437107e3150c474916e2d07ca60cb854be82945`  
		Last Modified: Thu, 01 Apr 2021 01:23:53 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0a4538b413e1c29dceac731f5ce84b6c869fe10ebee8534102241ffaeb503d`  
		Last Modified: Thu, 01 Apr 2021 01:23:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357d41df9e29d8c63d89e757c7660ee4be8b02fc9d661bc6a2f4c8511e4364c9`  
		Last Modified: Thu, 01 Apr 2021 01:23:53 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:fa6dd7b43c414091379595769d015a8838974f49abb8bd06e6e0e2b5b38cdda7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:1c85a1abf85528c0b96c75c783db902f5c5d9f0204af066a241661765d5afef5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46519178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebb5800a09fb0ad08ed9b9f34ac56a367aed36dc31b09fb0e862e443888a1dec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:55:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:58:14 GMT
ARG CONSUL_VERSION=1.8.9
# Thu, 01 Apr 2021 13:58:14 GMT
LABEL org.opencontainers.image.version=1.8.9
# Thu, 01 Apr 2021 13:58:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:58:15 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:58:20 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:58:22 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:58:23 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:58:23 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:58:23 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:58:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:58:23 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:58:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:58:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:58:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9b771409f4f3f2f129221ce337f2081dd152cce17c174a9fac5c12459293f1`  
		Last Modified: Thu, 01 Apr 2021 13:59:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf511b0af74102bdd5dc799e059f0babaaa036a3e2aa77ec680dca6b0bcb181`  
		Last Modified: Thu, 01 Apr 2021 13:59:27 GMT  
		Size: 43.7 MB (43716176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26be0088f3fb542426f3b16b714a6e2c6bb96c3cb271c8a3be4357659b2708ca`  
		Last Modified: Thu, 01 Apr 2021 13:59:19 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404a0ea273d8d2a6357df52a8febc721807149a5dfdf98a3ba72a7a8e4c1d77f`  
		Last Modified: Thu, 01 Apr 2021 13:59:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e18aef70ec04c786d67ed4f9edc24be85880db30dcd107c010de51044f86a96`  
		Last Modified: Thu, 01 Apr 2021 13:59:20 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:3ce0aaf87899af79726707ca5f6cce3aa05c0e09e60f744238f6c10ff02b379e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41786936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13df4b2e9e8f5beee9f678fb146d62f8f893031e03ca8d415e89ff6eba77f3e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:17:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 31 Mar 2021 18:18:52 GMT
ARG CONSUL_VERSION=1.8.9
# Wed, 31 Mar 2021 18:18:55 GMT
LABEL org.opencontainers.image.version=1.8.9
# Wed, 31 Mar 2021 18:18:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 31 Mar 2021 18:19:00 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 31 Mar 2021 18:19:12 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 31 Mar 2021 18:19:16 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 31 Mar 2021 18:19:19 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:19:21 GMT
VOLUME [/consul/data]
# Wed, 31 Mar 2021 18:19:22 GMT
EXPOSE 8300
# Wed, 31 Mar 2021 18:19:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 31 Mar 2021 18:19:24 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 31 Mar 2021 18:19:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Mar 2021 18:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 18:19:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6361f4b4701b9c8dd7e21881c0145615ccb6a248aa8747974b044ce2c13c79bd`  
		Last Modified: Wed, 31 Mar 2021 18:20:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf5025eb71243b618ec0eb15217a060db83fe892c2df7c8dd7d7141a7b985d3`  
		Last Modified: Wed, 31 Mar 2021 18:21:10 GMT  
		Size: 39.2 MB (39178987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0009e1bfe638c28c30aad9b1b37a68410e1b5781cc64f528cd63f10e765c92`  
		Last Modified: Wed, 31 Mar 2021 18:20:56 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bcca113639fa0e6481b1d4bc011c7302a4cca8a97f2dabe9f8445ae6dec5a1`  
		Last Modified: Wed, 31 Mar 2021 18:20:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4819c38721e3cda06e2ad730593405bc4f0fd135ef6f6c9f75cf720ffa2896d`  
		Last Modified: Wed, 31 Mar 2021 18:20:56 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:393ca7381fa3a7a774d954f1f123fa8df85f2c341f3ba7ea7629436e6ba89d1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41954214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ca529af1c326d195168cf9dbd749bddff8ea8aea644b2909873291bb937e9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:15:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:16:00 GMT
ARG CONSUL_VERSION=1.8.9
# Thu, 01 Apr 2021 13:16:01 GMT
LABEL org.opencontainers.image.version=1.8.9
# Thu, 01 Apr 2021 13:16:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:16:04 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:16:11 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:16:14 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:16:16 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:16:17 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:16:18 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:16:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:16:20 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:16:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:16:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:16:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729ff08fc13fc203134530b00fd498bd90e3bad896803701db94204c5d8f6087`  
		Last Modified: Thu, 01 Apr 2021 13:17:36 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a787ddfa393fe9dc5e2b2d889aaea5167a8ccdc153deae8c7581121873ad0820`  
		Last Modified: Thu, 01 Apr 2021 13:17:41 GMT  
		Size: 39.2 MB (39241071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c6130bf3d46130456927fd9f697e732de3b6e9b06f9993aa8dab1657d6ac13`  
		Last Modified: Thu, 01 Apr 2021 13:17:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3561239980e6da442481bb041933e0344b9e3b5272de41638a389888d88767`  
		Last Modified: Thu, 01 Apr 2021 13:17:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aaa6391fde8aa3720ae3ffd7d3e12784127262d8f6a8333426a407cac5ad977`  
		Last Modified: Thu, 01 Apr 2021 13:17:35 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:80689474c180d96ec715197a5eae3b79935d1d31aeffb185a647996784198618
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46043596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e4c7219543fc09b86be4abfc02929e2a4ba272259f34e273c875a055d1f84f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:08 GMT
ADD file:053c3a6154e80758106cbf0fec936c3b41dabf24a9f5eda36416caa90556810c in / 
# Wed, 31 Mar 2021 17:43:09 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:21:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 01:22:17 GMT
ARG CONSUL_VERSION=1.8.9
# Thu, 01 Apr 2021 01:22:17 GMT
LABEL org.opencontainers.image.version=1.8.9
# Thu, 01 Apr 2021 01:22:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 01:22:18 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 01:22:23 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 01:22:24 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 01:22:25 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 01:22:25 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 01:22:25 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 01:22:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 01:22:26 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 01:22:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 01:22:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 01:22:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8eca83e4805e4c5e7b071425a4603bc4b02885b817aa7c1bba9605bd2cb9125a`  
		Last Modified: Wed, 31 Mar 2021 17:44:26 GMT  
		Size: 2.8 MB (2794977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1067568206d0e1fc99eeb01ebbd742ad9b38910eafe59484d06639b554982e`  
		Last Modified: Thu, 01 Apr 2021 01:23:33 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78872870eba6d6ecb8cc6dbafdd66d99e088102e7ad3e0e334e60c1ea77424`  
		Last Modified: Thu, 01 Apr 2021 01:23:40 GMT  
		Size: 43.2 MB (43245329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b0186af352bfd50f344400a3e1db73797bd6ffebfbebca9c8cb16c1ad56007`  
		Last Modified: Thu, 01 Apr 2021 01:23:33 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1802628957717a3a1c183b80b640bd500e212741a70cc8046772fdd26a85a4a9`  
		Last Modified: Thu, 01 Apr 2021 01:23:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f145654d1fa11a0f6e1d697ce6f8e48f1cafbaab5ac1274ea32ffd84a4436d`  
		Last Modified: Thu, 01 Apr 2021 01:23:33 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.9`

```console
$ docker pull consul@sha256:fa6dd7b43c414091379595769d015a8838974f49abb8bd06e6e0e2b5b38cdda7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.9` - linux; amd64

```console
$ docker pull consul@sha256:1c85a1abf85528c0b96c75c783db902f5c5d9f0204af066a241661765d5afef5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46519178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebb5800a09fb0ad08ed9b9f34ac56a367aed36dc31b09fb0e862e443888a1dec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:55:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:58:14 GMT
ARG CONSUL_VERSION=1.8.9
# Thu, 01 Apr 2021 13:58:14 GMT
LABEL org.opencontainers.image.version=1.8.9
# Thu, 01 Apr 2021 13:58:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:58:15 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:58:20 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:58:22 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:58:23 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:58:23 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:58:23 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:58:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:58:23 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:58:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:58:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:58:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9b771409f4f3f2f129221ce337f2081dd152cce17c174a9fac5c12459293f1`  
		Last Modified: Thu, 01 Apr 2021 13:59:20 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf511b0af74102bdd5dc799e059f0babaaa036a3e2aa77ec680dca6b0bcb181`  
		Last Modified: Thu, 01 Apr 2021 13:59:27 GMT  
		Size: 43.7 MB (43716176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26be0088f3fb542426f3b16b714a6e2c6bb96c3cb271c8a3be4357659b2708ca`  
		Last Modified: Thu, 01 Apr 2021 13:59:19 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:404a0ea273d8d2a6357df52a8febc721807149a5dfdf98a3ba72a7a8e4c1d77f`  
		Last Modified: Thu, 01 Apr 2021 13:59:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e18aef70ec04c786d67ed4f9edc24be85880db30dcd107c010de51044f86a96`  
		Last Modified: Thu, 01 Apr 2021 13:59:20 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:3ce0aaf87899af79726707ca5f6cce3aa05c0e09e60f744238f6c10ff02b379e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41786936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13df4b2e9e8f5beee9f678fb146d62f8f893031e03ca8d415e89ff6eba77f3e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:17:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 31 Mar 2021 18:18:52 GMT
ARG CONSUL_VERSION=1.8.9
# Wed, 31 Mar 2021 18:18:55 GMT
LABEL org.opencontainers.image.version=1.8.9
# Wed, 31 Mar 2021 18:18:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 31 Mar 2021 18:19:00 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 31 Mar 2021 18:19:12 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 31 Mar 2021 18:19:16 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 31 Mar 2021 18:19:19 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:19:21 GMT
VOLUME [/consul/data]
# Wed, 31 Mar 2021 18:19:22 GMT
EXPOSE 8300
# Wed, 31 Mar 2021 18:19:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 31 Mar 2021 18:19:24 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 31 Mar 2021 18:19:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Mar 2021 18:19:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 18:19:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6361f4b4701b9c8dd7e21881c0145615ccb6a248aa8747974b044ce2c13c79bd`  
		Last Modified: Wed, 31 Mar 2021 18:20:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf5025eb71243b618ec0eb15217a060db83fe892c2df7c8dd7d7141a7b985d3`  
		Last Modified: Wed, 31 Mar 2021 18:21:10 GMT  
		Size: 39.2 MB (39178987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d0009e1bfe638c28c30aad9b1b37a68410e1b5781cc64f528cd63f10e765c92`  
		Last Modified: Wed, 31 Mar 2021 18:20:56 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bcca113639fa0e6481b1d4bc011c7302a4cca8a97f2dabe9f8445ae6dec5a1`  
		Last Modified: Wed, 31 Mar 2021 18:20:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4819c38721e3cda06e2ad730593405bc4f0fd135ef6f6c9f75cf720ffa2896d`  
		Last Modified: Wed, 31 Mar 2021 18:20:56 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:393ca7381fa3a7a774d954f1f123fa8df85f2c341f3ba7ea7629436e6ba89d1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41954214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22ca529af1c326d195168cf9dbd749bddff8ea8aea644b2909873291bb937e9e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:15:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:16:00 GMT
ARG CONSUL_VERSION=1.8.9
# Thu, 01 Apr 2021 13:16:01 GMT
LABEL org.opencontainers.image.version=1.8.9
# Thu, 01 Apr 2021 13:16:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:16:04 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:16:11 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:16:14 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:16:16 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:16:17 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:16:18 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:16:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:16:20 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:16:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:16:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:16:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:729ff08fc13fc203134530b00fd498bd90e3bad896803701db94204c5d8f6087`  
		Last Modified: Thu, 01 Apr 2021 13:17:36 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a787ddfa393fe9dc5e2b2d889aaea5167a8ccdc153deae8c7581121873ad0820`  
		Last Modified: Thu, 01 Apr 2021 13:17:41 GMT  
		Size: 39.2 MB (39241071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c6130bf3d46130456927fd9f697e732de3b6e9b06f9993aa8dab1657d6ac13`  
		Last Modified: Thu, 01 Apr 2021 13:17:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3561239980e6da442481bb041933e0344b9e3b5272de41638a389888d88767`  
		Last Modified: Thu, 01 Apr 2021 13:17:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aaa6391fde8aa3720ae3ffd7d3e12784127262d8f6a8333426a407cac5ad977`  
		Last Modified: Thu, 01 Apr 2021 13:17:35 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.9` - linux; 386

```console
$ docker pull consul@sha256:80689474c180d96ec715197a5eae3b79935d1d31aeffb185a647996784198618
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46043596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8e4c7219543fc09b86be4abfc02929e2a4ba272259f34e273c875a055d1f84f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:08 GMT
ADD file:053c3a6154e80758106cbf0fec936c3b41dabf24a9f5eda36416caa90556810c in / 
# Wed, 31 Mar 2021 17:43:09 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:21:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 01:22:17 GMT
ARG CONSUL_VERSION=1.8.9
# Thu, 01 Apr 2021 01:22:17 GMT
LABEL org.opencontainers.image.version=1.8.9
# Thu, 01 Apr 2021 01:22:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 01:22:18 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 01:22:23 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 01:22:24 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 01:22:25 GMT
# ARGS: CONSUL_VERSION=1.8.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 01:22:25 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 01:22:25 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 01:22:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 01:22:26 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 01:22:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 01:22:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 01:22:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8eca83e4805e4c5e7b071425a4603bc4b02885b817aa7c1bba9605bd2cb9125a`  
		Last Modified: Wed, 31 Mar 2021 17:44:26 GMT  
		Size: 2.8 MB (2794977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1067568206d0e1fc99eeb01ebbd742ad9b38910eafe59484d06639b554982e`  
		Last Modified: Thu, 01 Apr 2021 01:23:33 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc78872870eba6d6ecb8cc6dbafdd66d99e088102e7ad3e0e334e60c1ea77424`  
		Last Modified: Thu, 01 Apr 2021 01:23:40 GMT  
		Size: 43.2 MB (43245329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b0186af352bfd50f344400a3e1db73797bd6ffebfbebca9c8cb16c1ad56007`  
		Last Modified: Thu, 01 Apr 2021 01:23:33 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1802628957717a3a1c183b80b640bd500e212741a70cc8046772fdd26a85a4a9`  
		Last Modified: Thu, 01 Apr 2021 01:23:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f145654d1fa11a0f6e1d697ce6f8e48f1cafbaab5ac1274ea32ffd84a4436d`  
		Last Modified: Thu, 01 Apr 2021 01:23:33 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:57f6d77e07b0bfdf4ced6f6fff7cd095658afb1ccc586558d24f8b3562e9e374
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:c28c1495e8b6ab3dc8b80585b9eb269c3a8ce70d534fc141936ca5e62a425c8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45630924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb701064c41aef58ca3504b14eed918eaba77f3d21967694a08329d64272e321`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:55:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:55:33 GMT
ARG CONSUL_VERSION=1.9.4
# Thu, 01 Apr 2021 13:55:33 GMT
LABEL org.opencontainers.image.version=1.9.4
# Thu, 01 Apr 2021 13:55:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:55:35 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:57:57 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:57:58 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:57:59 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:57:59 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:57:59 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:57:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:57:59 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:58:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:58:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:58:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258501eb950bc3320ca3f00551a08bc5c4ff077f4a74028afb9226581d3c5c75`  
		Last Modified: Thu, 01 Apr 2021 13:58:54 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786844d2dd3a2bdedd54c5517778e834b06533b35cf74ff910a1fdccfd2f27ea`  
		Last Modified: Thu, 01 Apr 2021 13:59:03 GMT  
		Size: 42.8 MB (42827918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb33e490aaf4758702ef5641b86b2ff5c8ce2d2bb002b4a07c61c9e6630710e`  
		Last Modified: Thu, 01 Apr 2021 13:58:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2060c3060ba858186857225b4e10fe20cf36750d7539b2745bc75711efe93c`  
		Last Modified: Thu, 01 Apr 2021 13:58:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b0c7e5b1257c37ec8c067350b190446fa79363350c5b36f52b92cc8856a38`  
		Last Modified: Thu, 01 Apr 2021 13:58:54 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:5e95979eb0f587bdaa6bc9a907dec906caa691feea0879993f6238add7761df5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40887286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bac78aa811340290f5bcdb4fd6b795832d86439728d4d3c1ce82cf33fe83d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:17:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 31 Mar 2021 18:17:52 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 31 Mar 2021 18:17:53 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 31 Mar 2021 18:17:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 31 Mar 2021 18:18:00 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 31 Mar 2021 18:18:16 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 31 Mar 2021 18:18:19 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 31 Mar 2021 18:18:22 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:18:24 GMT
VOLUME [/consul/data]
# Wed, 31 Mar 2021 18:18:26 GMT
EXPOSE 8300
# Wed, 31 Mar 2021 18:18:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 31 Mar 2021 18:18:28 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 31 Mar 2021 18:18:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Mar 2021 18:18:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 18:18:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecf3f2720c2819a62021fa2ddd31406cc9d809b36c240babf654d9aecfa175c`  
		Last Modified: Wed, 31 Mar 2021 18:20:38 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc3089d78358b4878644e925bcb5bf9fe5926d68382f50983cf64d3e0f99234`  
		Last Modified: Wed, 31 Mar 2021 18:20:47 GMT  
		Size: 38.3 MB (38279335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feb7541c18a5da452edc3d87e11122fb8274645e3b87f560526c1237d4e9607`  
		Last Modified: Wed, 31 Mar 2021 18:20:38 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634a695f91bd002196d854b0c991c3a73216c4777a448f289abba30876e00903`  
		Last Modified: Wed, 31 Mar 2021 18:20:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656c5b4d5174cceb4408fd595d02246961ef3dca2a97e9ba6933b79b23b16830`  
		Last Modified: Wed, 31 Mar 2021 18:20:37 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:17e6ca9bba3f0fc0eadaa2c709949c70ca9f3d8f7257746f487fcd8e8044b213
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41098536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1bca6e20f940e411617a50daf2bdce2bb8f7564c1b0469c6eacf944fa99acf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:15:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:15:30 GMT
ARG CONSUL_VERSION=1.9.4
# Thu, 01 Apr 2021 13:15:31 GMT
LABEL org.opencontainers.image.version=1.9.4
# Thu, 01 Apr 2021 13:15:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:15:34 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:15:41 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:15:44 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:15:46 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:15:47 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:15:48 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:15:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:15:50 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:15:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:15:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:15:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0270c495653787dc761bcfe234e38b84c63a061bb65e717be6c2f5b2b429df`  
		Last Modified: Thu, 01 Apr 2021 13:17:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84350bd82fabce9206e69dff6551597826a43e4a583e3a625f09fed46a09eab0`  
		Last Modified: Thu, 01 Apr 2021 13:17:23 GMT  
		Size: 38.4 MB (38385391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7db23543df741db1bb8308cd955a8d563f924f5706fab4e327cc02c9bc819c`  
		Last Modified: Thu, 01 Apr 2021 13:17:14 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea9c2c2ad85406bb999aa39267b62bc5f3a1503982b18f975de47c8df91531f`  
		Last Modified: Thu, 01 Apr 2021 13:17:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e059f907f36358631e2b3818dd86392efc8b13cb164671ae33383812abfbe1`  
		Last Modified: Thu, 01 Apr 2021 13:17:17 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:23686a1dd3bdd3397129a652df5c3a20f2dbad52a9d788ee3f5817be8e5e776e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44977544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23acd3d24399e73e50541d91e938b76557481edaf1bd77430ed2c3cdcbfd2a4b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:08 GMT
ADD file:053c3a6154e80758106cbf0fec936c3b41dabf24a9f5eda36416caa90556810c in / 
# Wed, 31 Mar 2021 17:43:09 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:21:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 01:21:56 GMT
ARG CONSUL_VERSION=1.9.4
# Thu, 01 Apr 2021 01:21:57 GMT
LABEL org.opencontainers.image.version=1.9.4
# Thu, 01 Apr 2021 01:21:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 01:21:58 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 01:22:07 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 01:22:08 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 01:22:09 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 01:22:09 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 01:22:09 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 01:22:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 01:22:10 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 01:22:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 01:22:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 01:22:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8eca83e4805e4c5e7b071425a4603bc4b02885b817aa7c1bba9605bd2cb9125a`  
		Last Modified: Wed, 31 Mar 2021 17:44:26 GMT  
		Size: 2.8 MB (2794977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7342c69e19efac9391e075228f97883422e2ead6bacdaa2395c2f0e542d679e6`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319f6347360fb8e0afb9de289600ba4195b16af160154d83a8cb54b4700073b`  
		Last Modified: Thu, 01 Apr 2021 01:23:15 GMT  
		Size: 42.2 MB (42179275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4c83cec42bd7e817ed5295dd37c6bb5edd795f737d6dcaebe7bc0efc2a42e`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004e28eb9a622391f62ded8507411a3e48da8b561b7409087c1b939af1ac557`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df52be9f1d02c84167a282cb7aa9b2c4faf018338bde09132d55442dc0aa200`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.4`

```console
$ docker pull consul@sha256:57f6d77e07b0bfdf4ced6f6fff7cd095658afb1ccc586558d24f8b3562e9e374
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.4` - linux; amd64

```console
$ docker pull consul@sha256:c28c1495e8b6ab3dc8b80585b9eb269c3a8ce70d534fc141936ca5e62a425c8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45630924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb701064c41aef58ca3504b14eed918eaba77f3d21967694a08329d64272e321`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:55:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:55:33 GMT
ARG CONSUL_VERSION=1.9.4
# Thu, 01 Apr 2021 13:55:33 GMT
LABEL org.opencontainers.image.version=1.9.4
# Thu, 01 Apr 2021 13:55:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:55:35 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:57:57 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:57:58 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:57:59 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:57:59 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:57:59 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:57:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:57:59 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:58:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:58:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:58:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258501eb950bc3320ca3f00551a08bc5c4ff077f4a74028afb9226581d3c5c75`  
		Last Modified: Thu, 01 Apr 2021 13:58:54 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786844d2dd3a2bdedd54c5517778e834b06533b35cf74ff910a1fdccfd2f27ea`  
		Last Modified: Thu, 01 Apr 2021 13:59:03 GMT  
		Size: 42.8 MB (42827918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb33e490aaf4758702ef5641b86b2ff5c8ce2d2bb002b4a07c61c9e6630710e`  
		Last Modified: Thu, 01 Apr 2021 13:58:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2060c3060ba858186857225b4e10fe20cf36750d7539b2745bc75711efe93c`  
		Last Modified: Thu, 01 Apr 2021 13:58:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b0c7e5b1257c37ec8c067350b190446fa79363350c5b36f52b92cc8856a38`  
		Last Modified: Thu, 01 Apr 2021 13:58:54 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:5e95979eb0f587bdaa6bc9a907dec906caa691feea0879993f6238add7761df5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40887286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bac78aa811340290f5bcdb4fd6b795832d86439728d4d3c1ce82cf33fe83d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:17:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 31 Mar 2021 18:17:52 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 31 Mar 2021 18:17:53 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 31 Mar 2021 18:17:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 31 Mar 2021 18:18:00 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 31 Mar 2021 18:18:16 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 31 Mar 2021 18:18:19 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 31 Mar 2021 18:18:22 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:18:24 GMT
VOLUME [/consul/data]
# Wed, 31 Mar 2021 18:18:26 GMT
EXPOSE 8300
# Wed, 31 Mar 2021 18:18:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 31 Mar 2021 18:18:28 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 31 Mar 2021 18:18:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Mar 2021 18:18:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 18:18:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecf3f2720c2819a62021fa2ddd31406cc9d809b36c240babf654d9aecfa175c`  
		Last Modified: Wed, 31 Mar 2021 18:20:38 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc3089d78358b4878644e925bcb5bf9fe5926d68382f50983cf64d3e0f99234`  
		Last Modified: Wed, 31 Mar 2021 18:20:47 GMT  
		Size: 38.3 MB (38279335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feb7541c18a5da452edc3d87e11122fb8274645e3b87f560526c1237d4e9607`  
		Last Modified: Wed, 31 Mar 2021 18:20:38 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634a695f91bd002196d854b0c991c3a73216c4777a448f289abba30876e00903`  
		Last Modified: Wed, 31 Mar 2021 18:20:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656c5b4d5174cceb4408fd595d02246961ef3dca2a97e9ba6933b79b23b16830`  
		Last Modified: Wed, 31 Mar 2021 18:20:37 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:17e6ca9bba3f0fc0eadaa2c709949c70ca9f3d8f7257746f487fcd8e8044b213
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41098536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1bca6e20f940e411617a50daf2bdce2bb8f7564c1b0469c6eacf944fa99acf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:15:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:15:30 GMT
ARG CONSUL_VERSION=1.9.4
# Thu, 01 Apr 2021 13:15:31 GMT
LABEL org.opencontainers.image.version=1.9.4
# Thu, 01 Apr 2021 13:15:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:15:34 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:15:41 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:15:44 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:15:46 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:15:47 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:15:48 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:15:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:15:50 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:15:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:15:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:15:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0270c495653787dc761bcfe234e38b84c63a061bb65e717be6c2f5b2b429df`  
		Last Modified: Thu, 01 Apr 2021 13:17:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84350bd82fabce9206e69dff6551597826a43e4a583e3a625f09fed46a09eab0`  
		Last Modified: Thu, 01 Apr 2021 13:17:23 GMT  
		Size: 38.4 MB (38385391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7db23543df741db1bb8308cd955a8d563f924f5706fab4e327cc02c9bc819c`  
		Last Modified: Thu, 01 Apr 2021 13:17:14 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea9c2c2ad85406bb999aa39267b62bc5f3a1503982b18f975de47c8df91531f`  
		Last Modified: Thu, 01 Apr 2021 13:17:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e059f907f36358631e2b3818dd86392efc8b13cb164671ae33383812abfbe1`  
		Last Modified: Thu, 01 Apr 2021 13:17:17 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.4` - linux; 386

```console
$ docker pull consul@sha256:23686a1dd3bdd3397129a652df5c3a20f2dbad52a9d788ee3f5817be8e5e776e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44977544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23acd3d24399e73e50541d91e938b76557481edaf1bd77430ed2c3cdcbfd2a4b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:08 GMT
ADD file:053c3a6154e80758106cbf0fec936c3b41dabf24a9f5eda36416caa90556810c in / 
# Wed, 31 Mar 2021 17:43:09 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:21:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 01:21:56 GMT
ARG CONSUL_VERSION=1.9.4
# Thu, 01 Apr 2021 01:21:57 GMT
LABEL org.opencontainers.image.version=1.9.4
# Thu, 01 Apr 2021 01:21:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 01:21:58 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 01:22:07 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 01:22:08 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 01:22:09 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 01:22:09 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 01:22:09 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 01:22:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 01:22:10 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 01:22:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 01:22:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 01:22:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8eca83e4805e4c5e7b071425a4603bc4b02885b817aa7c1bba9605bd2cb9125a`  
		Last Modified: Wed, 31 Mar 2021 17:44:26 GMT  
		Size: 2.8 MB (2794977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7342c69e19efac9391e075228f97883422e2ead6bacdaa2395c2f0e542d679e6`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319f6347360fb8e0afb9de289600ba4195b16af160154d83a8cb54b4700073b`  
		Last Modified: Thu, 01 Apr 2021 01:23:15 GMT  
		Size: 42.2 MB (42179275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4c83cec42bd7e817ed5295dd37c6bb5edd795f737d6dcaebe7bc0efc2a42e`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004e28eb9a622391f62ded8507411a3e48da8b561b7409087c1b939af1ac557`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df52be9f1d02c84167a282cb7aa9b2c4faf018338bde09132d55442dc0aa200`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:57f6d77e07b0bfdf4ced6f6fff7cd095658afb1ccc586558d24f8b3562e9e374
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:c28c1495e8b6ab3dc8b80585b9eb269c3a8ce70d534fc141936ca5e62a425c8e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45630924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb701064c41aef58ca3504b14eed918eaba77f3d21967694a08329d64272e321`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:55:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:55:33 GMT
ARG CONSUL_VERSION=1.9.4
# Thu, 01 Apr 2021 13:55:33 GMT
LABEL org.opencontainers.image.version=1.9.4
# Thu, 01 Apr 2021 13:55:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:55:35 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:57:57 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:57:58 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:57:59 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:57:59 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:57:59 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:57:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:57:59 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:58:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:58:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:58:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258501eb950bc3320ca3f00551a08bc5c4ff077f4a74028afb9226581d3c5c75`  
		Last Modified: Thu, 01 Apr 2021 13:58:54 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786844d2dd3a2bdedd54c5517778e834b06533b35cf74ff910a1fdccfd2f27ea`  
		Last Modified: Thu, 01 Apr 2021 13:59:03 GMT  
		Size: 42.8 MB (42827918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb33e490aaf4758702ef5641b86b2ff5c8ce2d2bb002b4a07c61c9e6630710e`  
		Last Modified: Thu, 01 Apr 2021 13:58:54 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2060c3060ba858186857225b4e10fe20cf36750d7539b2745bc75711efe93c`  
		Last Modified: Thu, 01 Apr 2021 13:58:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b0c7e5b1257c37ec8c067350b190446fa79363350c5b36f52b92cc8856a38`  
		Last Modified: Thu, 01 Apr 2021 13:58:54 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:5e95979eb0f587bdaa6bc9a907dec906caa691feea0879993f6238add7761df5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40887286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bac78aa811340290f5bcdb4fd6b795832d86439728d4d3c1ce82cf33fe83d45`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 18:17:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 31 Mar 2021 18:17:52 GMT
ARG CONSUL_VERSION=1.9.4
# Wed, 31 Mar 2021 18:17:53 GMT
LABEL org.opencontainers.image.version=1.9.4
# Wed, 31 Mar 2021 18:17:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 31 Mar 2021 18:18:00 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 31 Mar 2021 18:18:16 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 31 Mar 2021 18:18:19 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 31 Mar 2021 18:18:22 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 31 Mar 2021 18:18:24 GMT
VOLUME [/consul/data]
# Wed, 31 Mar 2021 18:18:26 GMT
EXPOSE 8300
# Wed, 31 Mar 2021 18:18:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 31 Mar 2021 18:18:28 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 31 Mar 2021 18:18:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 31 Mar 2021 18:18:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 31 Mar 2021 18:18:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecf3f2720c2819a62021fa2ddd31406cc9d809b36c240babf654d9aecfa175c`  
		Last Modified: Wed, 31 Mar 2021 18:20:38 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc3089d78358b4878644e925bcb5bf9fe5926d68382f50983cf64d3e0f99234`  
		Last Modified: Wed, 31 Mar 2021 18:20:47 GMT  
		Size: 38.3 MB (38279335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feb7541c18a5da452edc3d87e11122fb8274645e3b87f560526c1237d4e9607`  
		Last Modified: Wed, 31 Mar 2021 18:20:38 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634a695f91bd002196d854b0c991c3a73216c4777a448f289abba30876e00903`  
		Last Modified: Wed, 31 Mar 2021 18:20:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656c5b4d5174cceb4408fd595d02246961ef3dca2a97e9ba6933b79b23b16830`  
		Last Modified: Wed, 31 Mar 2021 18:20:37 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:17e6ca9bba3f0fc0eadaa2c709949c70ca9f3d8f7257746f487fcd8e8044b213
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41098536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef1bca6e20f940e411617a50daf2bdce2bb8f7564c1b0469c6eacf944fa99acf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:15:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 13:15:30 GMT
ARG CONSUL_VERSION=1.9.4
# Thu, 01 Apr 2021 13:15:31 GMT
LABEL org.opencontainers.image.version=1.9.4
# Thu, 01 Apr 2021 13:15:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 13:15:34 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 13:15:41 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 13:15:44 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 13:15:46 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 13:15:47 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 13:15:48 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 13:15:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 13:15:50 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 13:15:51 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 13:15:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 13:15:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0270c495653787dc761bcfe234e38b84c63a061bb65e717be6c2f5b2b429df`  
		Last Modified: Thu, 01 Apr 2021 13:17:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84350bd82fabce9206e69dff6551597826a43e4a583e3a625f09fed46a09eab0`  
		Last Modified: Thu, 01 Apr 2021 13:17:23 GMT  
		Size: 38.4 MB (38385391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7db23543df741db1bb8308cd955a8d563f924f5706fab4e327cc02c9bc819c`  
		Last Modified: Thu, 01 Apr 2021 13:17:14 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea9c2c2ad85406bb999aa39267b62bc5f3a1503982b18f975de47c8df91531f`  
		Last Modified: Thu, 01 Apr 2021 13:17:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e059f907f36358631e2b3818dd86392efc8b13cb164671ae33383812abfbe1`  
		Last Modified: Thu, 01 Apr 2021 13:17:17 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:23686a1dd3bdd3397129a652df5c3a20f2dbad52a9d788ee3f5817be8e5e776e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44977544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23acd3d24399e73e50541d91e938b76557481edaf1bd77430ed2c3cdcbfd2a4b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:08 GMT
ADD file:053c3a6154e80758106cbf0fec936c3b41dabf24a9f5eda36416caa90556810c in / 
# Wed, 31 Mar 2021 17:43:09 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:21:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 01 Apr 2021 01:21:56 GMT
ARG CONSUL_VERSION=1.9.4
# Thu, 01 Apr 2021 01:21:57 GMT
LABEL org.opencontainers.image.version=1.9.4
# Thu, 01 Apr 2021 01:21:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Apr 2021 01:21:58 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Apr 2021 01:22:07 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pool.sks-keyservers.net --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Apr 2021 01:22:08 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Apr 2021 01:22:09 GMT
# ARGS: CONSUL_VERSION=1.9.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Apr 2021 01:22:09 GMT
VOLUME [/consul/data]
# Thu, 01 Apr 2021 01:22:09 GMT
EXPOSE 8300
# Thu, 01 Apr 2021 01:22:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Apr 2021 01:22:10 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Apr 2021 01:22:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 01:22:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 01:22:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8eca83e4805e4c5e7b071425a4603bc4b02885b817aa7c1bba9605bd2cb9125a`  
		Last Modified: Wed, 31 Mar 2021 17:44:26 GMT  
		Size: 2.8 MB (2794977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7342c69e19efac9391e075228f97883422e2ead6bacdaa2395c2f0e542d679e6`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1319f6347360fb8e0afb9de289600ba4195b16af160154d83a8cb54b4700073b`  
		Last Modified: Thu, 01 Apr 2021 01:23:15 GMT  
		Size: 42.2 MB (42179275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f4c83cec42bd7e817ed5295dd37c6bb5edd795f737d6dcaebe7bc0efc2a42e`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1004e28eb9a622391f62ded8507411a3e48da8b561b7409087c1b939af1ac557`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df52be9f1d02c84167a282cb7aa9b2c4faf018338bde09132d55442dc0aa200`  
		Last Modified: Thu, 01 Apr 2021 01:23:08 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
