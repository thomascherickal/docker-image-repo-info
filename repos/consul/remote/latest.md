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
