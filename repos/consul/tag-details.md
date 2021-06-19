<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10.0-beta`](#consul1100-beta)
-	[`consul:1.10.0-rc2`](#consul1100-rc2)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.14`](#consul1714)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.12`](#consul1812)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.6`](#consul196)
-	[`consul:latest`](#consullatest)

## `consul:1.10.0-beta`

```console
$ docker pull consul@sha256:a3a7e4fca544b3d64a36a361e3bfe814eb052df2cd76f5dd48c5005124850338
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.0-beta` - linux; amd64

```console
$ docker pull consul@sha256:709e5586649cb21b1aa202e1188d0c6d780667f53fb553d181e51302158a4a14
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43620369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fa6cd196c94ab25eeec6f69190f17b12366e664cf39ba29720712c8deb9d3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 18 Jun 2021 18:19:34 GMT
ARG CONSUL_VERSION=1.10.0-rc2
# Fri, 18 Jun 2021 18:19:34 GMT
LABEL org.opencontainers.image.version=1.10.0-rc2
# Fri, 18 Jun 2021 18:19:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Jun 2021 18:19:35 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Jun 2021 18:19:41 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Jun 2021 18:19:42 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Jun 2021 18:19:43 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Jun 2021 18:19:44 GMT
VOLUME [/consul/data]
# Fri, 18 Jun 2021 18:19:44 GMT
EXPOSE 8300
# Fri, 18 Jun 2021 18:19:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Jun 2021 18:19:44 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Jun 2021 18:19:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Jun 2021 18:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 18:19:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4aedf7cf3f49237410eb5a424fec6e00897388f97ceb8af2029a3c738ab6b0`  
		Last Modified: Fri, 18 Jun 2021 18:20:10 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661ea24a48f4fc1b4fdb34d9b97ff7b59e74ae58dabd46a56d5d405628e380a5`  
		Last Modified: Fri, 18 Jun 2021 18:20:16 GMT  
		Size: 40.8 MB (40805105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da8f8e86a06aa9e972e8131a66983076972278bdf2a8bea4f5da4a4d54456d2`  
		Last Modified: Fri, 18 Jun 2021 18:20:10 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ad24e5fc350b2707ebee21c659f11b18cebe566279e71e541812e5db785405`  
		Last Modified: Fri, 18 Jun 2021 18:20:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed2a32074f86033817e9d718522ced57c9101c07bbbe212b9db390b222398ef`  
		Last Modified: Fri, 18 Jun 2021 18:20:10 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-beta` - linux; arm variant v6

```console
$ docker pull consul@sha256:aa74889833c4ad56a631cb60cb89064b75f3eedfbf90e507cfc6ad822c0b2445
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39628492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f51926d210cb87ab4a5435b68d1ee03b64a4b2f1a25985aa476f2299588d80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 10:07:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 18 Jun 2021 17:50:29 GMT
ARG CONSUL_VERSION=1.10.0-rc2
# Fri, 18 Jun 2021 17:50:29 GMT
LABEL org.opencontainers.image.version=1.10.0-rc2
# Fri, 18 Jun 2021 17:50:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Jun 2021 17:50:30 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Jun 2021 17:50:37 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Jun 2021 17:50:38 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Jun 2021 17:50:39 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Jun 2021 17:50:39 GMT
VOLUME [/consul/data]
# Fri, 18 Jun 2021 17:50:39 GMT
EXPOSE 8300
# Fri, 18 Jun 2021 17:50:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Jun 2021 17:50:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Jun 2021 17:50:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Jun 2021 17:50:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 17:50:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f4f8c02a711bb80da0a62984efc9b02211a17db613092c8b8a518f550e2f24`  
		Last Modified: Fri, 18 Jun 2021 17:51:36 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88abb4bac49e366e00b7b7e671ad7ec824af715cd487ad5fe5cc7dacd837140`  
		Last Modified: Fri, 18 Jun 2021 17:51:43 GMT  
		Size: 37.0 MB (37003064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bda94d4c8b6944047036378dd709163d0788ec42349e0fd3e826ae85cdbd0a5`  
		Last Modified: Fri, 18 Jun 2021 17:51:36 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840224b05afc9c829cb45736172752658e1dcc73d1bed94171a6314a31987d2`  
		Last Modified: Fri, 18 Jun 2021 17:51:36 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fdf58dcb7510da107a0c587a67312ed209ab5b467c5ad19f9ae82ba88d80ff`  
		Last Modified: Fri, 18 Jun 2021 17:51:36 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-beta` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1398dcf1d01a08d0dcf9ea850371d8a2dbac498b162f255fab39666ab3ac335e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39574468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2379f8f81be936fbc565f44a19acab75ceab5ba57777d0e9b7101552da65107`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:25:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 18 Jun 2021 18:39:32 GMT
ARG CONSUL_VERSION=1.10.0-rc2
# Fri, 18 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.version=1.10.0-rc2
# Fri, 18 Jun 2021 18:39:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Jun 2021 18:39:33 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Jun 2021 18:39:39 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Jun 2021 18:39:39 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Jun 2021 18:39:40 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Jun 2021 18:39:40 GMT
VOLUME [/consul/data]
# Fri, 18 Jun 2021 18:39:41 GMT
EXPOSE 8300
# Fri, 18 Jun 2021 18:39:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Jun 2021 18:39:41 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Jun 2021 18:39:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Jun 2021 18:39:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 18:39:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9464111124b54380ef73fd90f7d60bfbdb462dd090ce8fd52d9b7e408caf6627`  
		Last Modified: Fri, 18 Jun 2021 18:40:19 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e40d41e38da7417b7a101c96d248a88a0ca2680bb952ee28dbde100854cb97c`  
		Last Modified: Fri, 18 Jun 2021 18:40:25 GMT  
		Size: 36.9 MB (36859146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8058b6b598b51f3d10e7f03b17c91219528b019d83006d35abf117885efa973`  
		Last Modified: Fri, 18 Jun 2021 18:40:19 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e7ce63a4c561cffc60d9502b8629b0d50cc77dac91e6c49f5cdc959488bf46`  
		Last Modified: Fri, 18 Jun 2021 18:40:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bb770b5deb150d8d0f18442083c5094522b481ad4092f9fdb7b71278211b5`  
		Last Modified: Fri, 18 Jun 2021 18:40:19 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-beta` - linux; 386

```console
$ docker pull consul@sha256:ae3e86ac2de4922bd289f0a04d23bfbdab0f6ddfe829113b558ecee2ca5f24d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (42984503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc6e1dc82c25abaa1480124c93204dd2f120445f6ecd1da6ed6988620603099f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 18 Jun 2021 18:38:26 GMT
ARG CONSUL_VERSION=1.10.0-rc2
# Fri, 18 Jun 2021 18:38:26 GMT
LABEL org.opencontainers.image.version=1.10.0-rc2
# Fri, 18 Jun 2021 18:38:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Jun 2021 18:38:27 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Jun 2021 18:38:34 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Jun 2021 18:38:35 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Jun 2021 18:38:36 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Jun 2021 18:38:36 GMT
VOLUME [/consul/data]
# Fri, 18 Jun 2021 18:38:36 GMT
EXPOSE 8300
# Fri, 18 Jun 2021 18:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Jun 2021 18:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Jun 2021 18:38:37 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Jun 2021 18:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 18:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f21716c250dfdf254a1e0daf168cfaf795e5ffccf31c464a35eba6fd2d2ec80`  
		Last Modified: Fri, 18 Jun 2021 18:39:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd8f33b2524c5211c5f610ea7bc4fda361ef38bf808f5814b8d1f660be11fa`  
		Last Modified: Fri, 18 Jun 2021 18:39:23 GMT  
		Size: 40.2 MB (40162315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba393690b2abd4f31e3c953dddda5952e7dfeb7ecebad0af6bc80cfb16b8da6`  
		Last Modified: Fri, 18 Jun 2021 18:39:16 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546efe37d36f08ebdf85d4fa61782ab72617ac2cb424cbae35debba1741ad3f2`  
		Last Modified: Fri, 18 Jun 2021 18:39:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0564f5ad66c6d933ad154dbde76e077de671f2f293f868b099a5084ad82358`  
		Last Modified: Fri, 18 Jun 2021 18:39:16 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.0-rc2`

```console
$ docker pull consul@sha256:a3a7e4fca544b3d64a36a361e3bfe814eb052df2cd76f5dd48c5005124850338
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.0-rc2` - linux; amd64

```console
$ docker pull consul@sha256:709e5586649cb21b1aa202e1188d0c6d780667f53fb553d181e51302158a4a14
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43620369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74fa6cd196c94ab25eeec6f69190f17b12366e664cf39ba29720712c8deb9d3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 18 Jun 2021 18:19:34 GMT
ARG CONSUL_VERSION=1.10.0-rc2
# Fri, 18 Jun 2021 18:19:34 GMT
LABEL org.opencontainers.image.version=1.10.0-rc2
# Fri, 18 Jun 2021 18:19:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Jun 2021 18:19:35 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Jun 2021 18:19:41 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Jun 2021 18:19:42 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Jun 2021 18:19:43 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Jun 2021 18:19:44 GMT
VOLUME [/consul/data]
# Fri, 18 Jun 2021 18:19:44 GMT
EXPOSE 8300
# Fri, 18 Jun 2021 18:19:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Jun 2021 18:19:44 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Jun 2021 18:19:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Jun 2021 18:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 18:19:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4aedf7cf3f49237410eb5a424fec6e00897388f97ceb8af2029a3c738ab6b0`  
		Last Modified: Fri, 18 Jun 2021 18:20:10 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661ea24a48f4fc1b4fdb34d9b97ff7b59e74ae58dabd46a56d5d405628e380a5`  
		Last Modified: Fri, 18 Jun 2021 18:20:16 GMT  
		Size: 40.8 MB (40805105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8da8f8e86a06aa9e972e8131a66983076972278bdf2a8bea4f5da4a4d54456d2`  
		Last Modified: Fri, 18 Jun 2021 18:20:10 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ad24e5fc350b2707ebee21c659f11b18cebe566279e71e541812e5db785405`  
		Last Modified: Fri, 18 Jun 2021 18:20:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eed2a32074f86033817e9d718522ced57c9101c07bbbe212b9db390b222398ef`  
		Last Modified: Fri, 18 Jun 2021 18:20:10 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-rc2` - linux; arm variant v6

```console
$ docker pull consul@sha256:aa74889833c4ad56a631cb60cb89064b75f3eedfbf90e507cfc6ad822c0b2445
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39628492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f51926d210cb87ab4a5435b68d1ee03b64a4b2f1a25985aa476f2299588d80e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 10:07:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 18 Jun 2021 17:50:29 GMT
ARG CONSUL_VERSION=1.10.0-rc2
# Fri, 18 Jun 2021 17:50:29 GMT
LABEL org.opencontainers.image.version=1.10.0-rc2
# Fri, 18 Jun 2021 17:50:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Jun 2021 17:50:30 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Jun 2021 17:50:37 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Jun 2021 17:50:38 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Jun 2021 17:50:39 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Jun 2021 17:50:39 GMT
VOLUME [/consul/data]
# Fri, 18 Jun 2021 17:50:39 GMT
EXPOSE 8300
# Fri, 18 Jun 2021 17:50:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Jun 2021 17:50:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Jun 2021 17:50:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Jun 2021 17:50:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 17:50:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f4f8c02a711bb80da0a62984efc9b02211a17db613092c8b8a518f550e2f24`  
		Last Modified: Fri, 18 Jun 2021 17:51:36 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88abb4bac49e366e00b7b7e671ad7ec824af715cd487ad5fe5cc7dacd837140`  
		Last Modified: Fri, 18 Jun 2021 17:51:43 GMT  
		Size: 37.0 MB (37003064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bda94d4c8b6944047036378dd709163d0788ec42349e0fd3e826ae85cdbd0a5`  
		Last Modified: Fri, 18 Jun 2021 17:51:36 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1840224b05afc9c829cb45736172752658e1dcc73d1bed94171a6314a31987d2`  
		Last Modified: Fri, 18 Jun 2021 17:51:36 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1fdf58dcb7510da107a0c587a67312ed209ab5b467c5ad19f9ae82ba88d80ff`  
		Last Modified: Fri, 18 Jun 2021 17:51:36 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-rc2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1398dcf1d01a08d0dcf9ea850371d8a2dbac498b162f255fab39666ab3ac335e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39574468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2379f8f81be936fbc565f44a19acab75ceab5ba57777d0e9b7101552da65107`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:25:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 18 Jun 2021 18:39:32 GMT
ARG CONSUL_VERSION=1.10.0-rc2
# Fri, 18 Jun 2021 18:39:32 GMT
LABEL org.opencontainers.image.version=1.10.0-rc2
# Fri, 18 Jun 2021 18:39:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Jun 2021 18:39:33 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Jun 2021 18:39:39 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Jun 2021 18:39:39 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Jun 2021 18:39:40 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Jun 2021 18:39:40 GMT
VOLUME [/consul/data]
# Fri, 18 Jun 2021 18:39:41 GMT
EXPOSE 8300
# Fri, 18 Jun 2021 18:39:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Jun 2021 18:39:41 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Jun 2021 18:39:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Jun 2021 18:39:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 18:39:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9464111124b54380ef73fd90f7d60bfbdb462dd090ce8fd52d9b7e408caf6627`  
		Last Modified: Fri, 18 Jun 2021 18:40:19 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e40d41e38da7417b7a101c96d248a88a0ca2680bb952ee28dbde100854cb97c`  
		Last Modified: Fri, 18 Jun 2021 18:40:25 GMT  
		Size: 36.9 MB (36859146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8058b6b598b51f3d10e7f03b17c91219528b019d83006d35abf117885efa973`  
		Last Modified: Fri, 18 Jun 2021 18:40:19 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e7ce63a4c561cffc60d9502b8629b0d50cc77dac91e6c49f5cdc959488bf46`  
		Last Modified: Fri, 18 Jun 2021 18:40:19 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bb770b5deb150d8d0f18442083c5094522b481ad4092f9fdb7b71278211b5`  
		Last Modified: Fri, 18 Jun 2021 18:40:19 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-rc2` - linux; 386

```console
$ docker pull consul@sha256:ae3e86ac2de4922bd289f0a04d23bfbdab0f6ddfe829113b558ecee2ca5f24d6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (42984503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc6e1dc82c25abaa1480124c93204dd2f120445f6ecd1da6ed6988620603099f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 18 Jun 2021 18:38:26 GMT
ARG CONSUL_VERSION=1.10.0-rc2
# Fri, 18 Jun 2021 18:38:26 GMT
LABEL org.opencontainers.image.version=1.10.0-rc2
# Fri, 18 Jun 2021 18:38:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Jun 2021 18:38:27 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Jun 2021 18:38:34 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Jun 2021 18:38:35 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Jun 2021 18:38:36 GMT
# ARGS: CONSUL_VERSION=1.10.0-rc2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Jun 2021 18:38:36 GMT
VOLUME [/consul/data]
# Fri, 18 Jun 2021 18:38:36 GMT
EXPOSE 8300
# Fri, 18 Jun 2021 18:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Jun 2021 18:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Jun 2021 18:38:37 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Jun 2021 18:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Jun 2021 18:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f21716c250dfdf254a1e0daf168cfaf795e5ffccf31c464a35eba6fd2d2ec80`  
		Last Modified: Fri, 18 Jun 2021 18:39:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd8f33b2524c5211c5f610ea7bc4fda361ef38bf808f5814b8d1f660be11fa`  
		Last Modified: Fri, 18 Jun 2021 18:39:23 GMT  
		Size: 40.2 MB (40162315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba393690b2abd4f31e3c953dddda5952e7dfeb7ecebad0af6bc80cfb16b8da6`  
		Last Modified: Fri, 18 Jun 2021 18:39:16 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546efe37d36f08ebdf85d4fa61782ab72617ac2cb424cbae35debba1741ad3f2`  
		Last Modified: Fri, 18 Jun 2021 18:39:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0564f5ad66c6d933ad154dbde76e077de671f2f293f868b099a5084ad82358`  
		Last Modified: Fri, 18 Jun 2021 18:39:16 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7`

```console
$ docker pull consul@sha256:fce4d3cbf7d610394f5c862356f0bddc652c0062c6fb078bc7a67a8831d55d97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:39b85f0bf0d4bfbea54c408d8acbf9de1d8ebb40a700df01a5ffcf25819b3c26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43631510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5cc4b8af79ec6f3f0ccced9e875518bd83b0054f5836f43965c3e79f78826e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:14:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 16 Apr 2021 21:20:22 GMT
ARG CONSUL_VERSION=1.7.14
# Fri, 16 Apr 2021 21:20:22 GMT
LABEL org.opencontainers.image.version=1.7.14
# Fri, 16 Apr 2021 21:20:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 16 Apr 2021 21:20:23 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 May 2021 20:20:27 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 May 2021 20:20:29 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 May 2021 20:20:30 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 May 2021 20:20:30 GMT
VOLUME [/consul/data]
# Fri, 07 May 2021 20:20:30 GMT
EXPOSE 8300
# Fri, 07 May 2021 20:20:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 May 2021 20:20:30 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 May 2021 20:20:31 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 May 2021 20:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 20:20:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3500336ca0dccc760254ac4274787d6035ad80339bac4345fd22ebc79a955bac`  
		Last Modified: Fri, 16 Apr 2021 21:21:52 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63681fede5b4b7f696729a820ab2ad2c5e48760a332774a9e84c64b37c23d8fc`  
		Last Modified: Fri, 07 May 2021 20:21:47 GMT  
		Size: 40.8 MB (40827649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4198aca0a6cd7a3a0fe81e2462199c5647ae6ba55badb513146893949a73c333`  
		Last Modified: Fri, 07 May 2021 20:21:40 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb16e29a2099e26e72a04c6e26a3a084c27004458bc660d1ba32e55a61cbc858`  
		Last Modified: Fri, 07 May 2021 20:21:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba0dc0e74e18c969fbd07578ef486f86bb211c4d37ba907eb4b6046046c8bcf`  
		Last Modified: Fri, 07 May 2021 20:21:40 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:b2f7da00d818c6ed3efa15662c1fc880cfe2a9004a9e1828e662b4707da7c796
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39269598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e2be20ca5daeff74371bce1ca0c00ab8dd48e1f98ef5d7272cd88e0661f3b22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 10:08:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 16 Jun 2021 10:08:18 GMT
ARG CONSUL_VERSION=1.7.14
# Wed, 16 Jun 2021 10:08:18 GMT
LABEL org.opencontainers.image.version=1.7.14
# Wed, 16 Jun 2021 10:08:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 16 Jun 2021 10:08:19 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 16 Jun 2021 10:08:25 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 16 Jun 2021 10:08:26 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 16 Jun 2021 10:08:27 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 10:08:27 GMT
VOLUME [/consul/data]
# Wed, 16 Jun 2021 10:08:27 GMT
EXPOSE 8300
# Wed, 16 Jun 2021 10:08:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 16 Jun 2021 10:08:28 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 16 Jun 2021 10:08:28 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 10:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 10:08:28 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf984c23ca0398e412fc2758d580a76b253efbeaca778f12b0d4b23569040db0`  
		Last Modified: Wed, 16 Jun 2021 10:10:13 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12a6c1dcfc53ebb5335e7904706b6a6dfc4792f43c1081212fccaca032e5f1b`  
		Last Modified: Wed, 16 Jun 2021 10:10:20 GMT  
		Size: 36.7 MB (36661047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d515149ccaacbb82af63169169af612ebe4a8b9a44cdd963722c026dcfbaad7`  
		Last Modified: Wed, 16 Jun 2021 10:10:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68f0dcd0d26c1588d1fbc71710484609132bd6144384babffe0222e0b6931bd`  
		Last Modified: Wed, 16 Jun 2021 10:10:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45faf4bb8010ff1d038d66da5b29aff8ed78129c0dfe3416052bb63ce5f5c7b`  
		Last Modified: Wed, 16 Jun 2021 10:10:13 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:698851681f678b6f99419251ea4aaf39f934df5b5eeaa1e909232fd2070a254f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39546854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfa5383ad17598ac072a8d0d84deaa8d36a3a61ba46b51989b459e273e0c969`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:26:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 15 Jun 2021 23:26:48 GMT
ARG CONSUL_VERSION=1.7.14
# Tue, 15 Jun 2021 23:26:48 GMT
LABEL org.opencontainers.image.version=1.7.14
# Tue, 15 Jun 2021 23:26:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Jun 2021 23:26:49 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Jun 2021 23:26:54 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Jun 2021 23:26:55 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Jun 2021 23:26:56 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 23:26:56 GMT
VOLUME [/consul/data]
# Tue, 15 Jun 2021 23:26:57 GMT
EXPOSE 8300
# Tue, 15 Jun 2021 23:26:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Jun 2021 23:26:57 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Jun 2021 23:26:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Jun 2021 23:26:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 23:26:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef042bfe14abb40e56c56d41810a8317fd516b9e1054cf869d8608ef54afc15d`  
		Last Modified: Tue, 15 Jun 2021 23:28:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e27ebc0a80971c0617f728456c5c2d40c84d3e3c3de672272c37f0f5030a4a`  
		Last Modified: Tue, 15 Jun 2021 23:28:29 GMT  
		Size: 36.8 MB (36832863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bf7da665fa8e1e3c787482088a26e6cbff0ce2090f00f8086c3f4048ceb708`  
		Last Modified: Tue, 15 Jun 2021 23:28:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce165eed71e8b7145990f835cce0f93421f8e7c254763fe719aa7750afe727ce`  
		Last Modified: Tue, 15 Jun 2021 23:28:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25733ddb9891f9b4a4dac51710afa4339303f6e67b660ae3941e946d01263373`  
		Last Modified: Tue, 15 Jun 2021 23:28:23 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:7b956c6c7002df613b9047a28ea2d9f48b2f31a0ac67dfc6210bd7686b0689ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42471287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c74ab999f2de49db2fbe107bbac2cb1591a6991e3a7cf06a5dfe921853780608`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 16 Apr 2021 21:39:14 GMT
ARG CONSUL_VERSION=1.7.14
# Fri, 16 Apr 2021 21:39:15 GMT
LABEL org.opencontainers.image.version=1.7.14
# Fri, 16 Apr 2021 21:39:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 16 Apr 2021 21:39:16 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 May 2021 19:39:23 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 May 2021 19:39:24 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 May 2021 19:39:24 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 May 2021 19:39:25 GMT
VOLUME [/consul/data]
# Fri, 07 May 2021 19:39:25 GMT
EXPOSE 8300
# Fri, 07 May 2021 19:39:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 May 2021 19:39:25 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 May 2021 19:39:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 May 2021 19:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 19:39:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d96f33ee206c0fa6e89a9f3e4b285df1c6822e288430f9c70ed09432729bd45`  
		Last Modified: Fri, 16 Apr 2021 21:40:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a23461d0229b5c1339761cacfbd26a338c41fc79c6f51de82b6bf8c7b764c9`  
		Last Modified: Fri, 07 May 2021 19:40:57 GMT  
		Size: 39.7 MB (39672201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef49ca8fc04c808e705b9c507e88b2238d55c1b78e631d6bd4cb42809ebb0eda`  
		Last Modified: Fri, 07 May 2021 19:40:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d85d0d31d42c7160ba7fb07a4b2c3ca0c4cdd1cf45e2891f8e476dcfc7f834e`  
		Last Modified: Fri, 07 May 2021 19:40:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1e2eb3a58069876aa038b93b775e13649d7fffa4febc4c029b006529e4306e`  
		Last Modified: Fri, 07 May 2021 19:40:51 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.14`

```console
$ docker pull consul@sha256:fce4d3cbf7d610394f5c862356f0bddc652c0062c6fb078bc7a67a8831d55d97
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.14` - linux; amd64

```console
$ docker pull consul@sha256:39b85f0bf0d4bfbea54c408d8acbf9de1d8ebb40a700df01a5ffcf25819b3c26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43631510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5cc4b8af79ec6f3f0ccced9e875518bd83b0054f5836f43965c3e79f78826e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:14:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 16 Apr 2021 21:20:22 GMT
ARG CONSUL_VERSION=1.7.14
# Fri, 16 Apr 2021 21:20:22 GMT
LABEL org.opencontainers.image.version=1.7.14
# Fri, 16 Apr 2021 21:20:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 16 Apr 2021 21:20:23 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 May 2021 20:20:27 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 May 2021 20:20:29 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 May 2021 20:20:30 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 May 2021 20:20:30 GMT
VOLUME [/consul/data]
# Fri, 07 May 2021 20:20:30 GMT
EXPOSE 8300
# Fri, 07 May 2021 20:20:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 May 2021 20:20:30 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 May 2021 20:20:31 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 May 2021 20:20:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 20:20:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3500336ca0dccc760254ac4274787d6035ad80339bac4345fd22ebc79a955bac`  
		Last Modified: Fri, 16 Apr 2021 21:21:52 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63681fede5b4b7f696729a820ab2ad2c5e48760a332774a9e84c64b37c23d8fc`  
		Last Modified: Fri, 07 May 2021 20:21:47 GMT  
		Size: 40.8 MB (40827649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4198aca0a6cd7a3a0fe81e2462199c5647ae6ba55badb513146893949a73c333`  
		Last Modified: Fri, 07 May 2021 20:21:40 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb16e29a2099e26e72a04c6e26a3a084c27004458bc660d1ba32e55a61cbc858`  
		Last Modified: Fri, 07 May 2021 20:21:40 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba0dc0e74e18c969fbd07578ef486f86bb211c4d37ba907eb4b6046046c8bcf`  
		Last Modified: Fri, 07 May 2021 20:21:40 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.14` - linux; arm variant v6

```console
$ docker pull consul@sha256:b2f7da00d818c6ed3efa15662c1fc880cfe2a9004a9e1828e662b4707da7c796
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39269598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e2be20ca5daeff74371bce1ca0c00ab8dd48e1f98ef5d7272cd88e0661f3b22`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 10:08:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 16 Jun 2021 10:08:18 GMT
ARG CONSUL_VERSION=1.7.14
# Wed, 16 Jun 2021 10:08:18 GMT
LABEL org.opencontainers.image.version=1.7.14
# Wed, 16 Jun 2021 10:08:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 16 Jun 2021 10:08:19 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 16 Jun 2021 10:08:25 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 16 Jun 2021 10:08:26 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 16 Jun 2021 10:08:27 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 10:08:27 GMT
VOLUME [/consul/data]
# Wed, 16 Jun 2021 10:08:27 GMT
EXPOSE 8300
# Wed, 16 Jun 2021 10:08:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 16 Jun 2021 10:08:28 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 16 Jun 2021 10:08:28 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 10:08:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 10:08:28 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf984c23ca0398e412fc2758d580a76b253efbeaca778f12b0d4b23569040db0`  
		Last Modified: Wed, 16 Jun 2021 10:10:13 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e12a6c1dcfc53ebb5335e7904706b6a6dfc4792f43c1081212fccaca032e5f1b`  
		Last Modified: Wed, 16 Jun 2021 10:10:20 GMT  
		Size: 36.7 MB (36661047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d515149ccaacbb82af63169169af612ebe4a8b9a44cdd963722c026dcfbaad7`  
		Last Modified: Wed, 16 Jun 2021 10:10:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68f0dcd0d26c1588d1fbc71710484609132bd6144384babffe0222e0b6931bd`  
		Last Modified: Wed, 16 Jun 2021 10:10:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45faf4bb8010ff1d038d66da5b29aff8ed78129c0dfe3416052bb63ce5f5c7b`  
		Last Modified: Wed, 16 Jun 2021 10:10:13 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.14` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:698851681f678b6f99419251ea4aaf39f934df5b5eeaa1e909232fd2070a254f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39546854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bfa5383ad17598ac072a8d0d84deaa8d36a3a61ba46b51989b459e273e0c969`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:26:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 15 Jun 2021 23:26:48 GMT
ARG CONSUL_VERSION=1.7.14
# Tue, 15 Jun 2021 23:26:48 GMT
LABEL org.opencontainers.image.version=1.7.14
# Tue, 15 Jun 2021 23:26:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Jun 2021 23:26:49 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Jun 2021 23:26:54 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Jun 2021 23:26:55 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Jun 2021 23:26:56 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 23:26:56 GMT
VOLUME [/consul/data]
# Tue, 15 Jun 2021 23:26:57 GMT
EXPOSE 8300
# Tue, 15 Jun 2021 23:26:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Jun 2021 23:26:57 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Jun 2021 23:26:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Jun 2021 23:26:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 23:26:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef042bfe14abb40e56c56d41810a8317fd516b9e1054cf869d8608ef54afc15d`  
		Last Modified: Tue, 15 Jun 2021 23:28:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e27ebc0a80971c0617f728456c5c2d40c84d3e3c3de672272c37f0f5030a4a`  
		Last Modified: Tue, 15 Jun 2021 23:28:29 GMT  
		Size: 36.8 MB (36832863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bf7da665fa8e1e3c787482088a26e6cbff0ce2090f00f8086c3f4048ceb708`  
		Last Modified: Tue, 15 Jun 2021 23:28:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce165eed71e8b7145990f835cce0f93421f8e7c254763fe719aa7750afe727ce`  
		Last Modified: Tue, 15 Jun 2021 23:28:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25733ddb9891f9b4a4dac51710afa4339303f6e67b660ae3941e946d01263373`  
		Last Modified: Tue, 15 Jun 2021 23:28:23 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.14` - linux; 386

```console
$ docker pull consul@sha256:7b956c6c7002df613b9047a28ea2d9f48b2f31a0ac67dfc6210bd7686b0689ec
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42471287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c74ab999f2de49db2fbe107bbac2cb1591a6991e3a7cf06a5dfe921853780608`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:55:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 16 Apr 2021 21:39:14 GMT
ARG CONSUL_VERSION=1.7.14
# Fri, 16 Apr 2021 21:39:15 GMT
LABEL org.opencontainers.image.version=1.7.14
# Fri, 16 Apr 2021 21:39:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 16 Apr 2021 21:39:16 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 07 May 2021 19:39:23 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 07 May 2021 19:39:24 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 07 May 2021 19:39:24 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 07 May 2021 19:39:25 GMT
VOLUME [/consul/data]
# Fri, 07 May 2021 19:39:25 GMT
EXPOSE 8300
# Fri, 07 May 2021 19:39:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 07 May 2021 19:39:25 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 07 May 2021 19:39:25 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 07 May 2021 19:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 May 2021 19:39:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d96f33ee206c0fa6e89a9f3e4b285df1c6822e288430f9c70ed09432729bd45`  
		Last Modified: Fri, 16 Apr 2021 21:40:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a23461d0229b5c1339761cacfbd26a338c41fc79c6f51de82b6bf8c7b764c9`  
		Last Modified: Fri, 07 May 2021 19:40:57 GMT  
		Size: 39.7 MB (39672201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef49ca8fc04c808e705b9c507e88b2238d55c1b78e631d6bd4cb42809ebb0eda`  
		Last Modified: Fri, 07 May 2021 19:40:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d85d0d31d42c7160ba7fb07a4b2c3ca0c4cdd1cf45e2891f8e476dcfc7f834e`  
		Last Modified: Fri, 07 May 2021 19:40:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1e2eb3a58069876aa038b93b775e13649d7fffa4febc4c029b006529e4306e`  
		Last Modified: Fri, 07 May 2021 19:40:51 GMT  
		Size: 1.7 KB (1703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:7a8e08198392458d96447b105c017879aaf8cfc40653052146865ea0d33342fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:16a579b62911fc315aa3745a7587b830dc3492660707284cad92bd1025d3e926
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47784420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a14d86a5934beabfa80a456cfdb0eb67502c469c091c790d9dad11a816aad806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 21:19:34 GMT
ARG CONSUL_VERSION=1.8.12
# Mon, 14 Jun 2021 21:19:35 GMT
LABEL org.opencontainers.image.version=1.8.12
# Mon, 14 Jun 2021 21:19:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 21:19:36 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 21:19:43 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 21:19:44 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 21:19:45 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 21:19:45 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 21:19:45 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 21:19:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 21:19:45 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 21:19:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 21:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 21:19:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04c7fbae711bd2c2d465d3b7fbda785ff5f8494acb555a79863ea21055c4179`  
		Last Modified: Mon, 14 Jun 2021 21:20:07 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fe4553a3dfa0e9a9602a23559e1b635e5cb83160a78ddb85fb967a5fd0d351`  
		Last Modified: Mon, 14 Jun 2021 21:20:13 GMT  
		Size: 45.0 MB (44969158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b943f75d06255a2f3b92c7756daa5eb8373cef2f62725eae4c1afc4ef2f910d`  
		Last Modified: Mon, 14 Jun 2021 21:20:07 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947a6323cd233cb7ff46a49af822da45b1827d82f9d64adf59d7ebeeeb6017cf`  
		Last Modified: Mon, 14 Jun 2021 21:20:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9a9a8a26baa71d6d61a0771664e8ececb12628dc6453ae88e425e7277f6e7f`  
		Last Modified: Mon, 14 Jun 2021 21:20:07 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:0ee2b4100c5a6ab51947fcccfc485d9afb4bb2f31e9af86cc02098cee5225386
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43013082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30c688174aee0c0f2582d0d7ec7c8960092bcab8b697978db497df0e277ea03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 10:07:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 16 Jun 2021 10:07:49 GMT
ARG CONSUL_VERSION=1.8.12
# Wed, 16 Jun 2021 10:07:50 GMT
LABEL org.opencontainers.image.version=1.8.12
# Wed, 16 Jun 2021 10:07:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 16 Jun 2021 10:07:50 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 16 Jun 2021 10:08:07 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 16 Jun 2021 10:08:08 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 16 Jun 2021 10:08:09 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 10:08:09 GMT
VOLUME [/consul/data]
# Wed, 16 Jun 2021 10:08:09 GMT
EXPOSE 8300
# Wed, 16 Jun 2021 10:08:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 16 Jun 2021 10:08:10 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 16 Jun 2021 10:08:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 10:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 10:08:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c099865187bb396e24462cc214ca0a5e2f6541f5ac49c7543c77c4f3b39cd232`  
		Last Modified: Wed, 16 Jun 2021 10:09:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ace0ab017ba2542ff6fb63b8f5f21f2db481cce555f0a0f64f2dfd534c0e75`  
		Last Modified: Wed, 16 Jun 2021 10:10:00 GMT  
		Size: 40.4 MB (40387654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1540da76e8633df6c20de0314bcf2d5a41a7795e75bfc8f5b6074614a7f2a6`  
		Last Modified: Wed, 16 Jun 2021 10:09:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce52256f8ff85635432d10ba13a9172651a4d68d226630906484c208b4c8587`  
		Last Modified: Wed, 16 Jun 2021 10:09:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ba0829e54d2298982f9b677a29e03ee44874bf853cb0b5eebbf1d4d62c0307`  
		Last Modified: Wed, 16 Jun 2021 10:09:52 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:0bad60159d74bb7e33a0529244a396bd32c55c7dcd018cc5bb000ad581230b35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43214795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e59d9a1710ecda7320608134d03a856244cdca4229e41465ef80edc7af03810`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:25:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 15 Jun 2021 23:26:33 GMT
ARG CONSUL_VERSION=1.8.12
# Tue, 15 Jun 2021 23:26:33 GMT
LABEL org.opencontainers.image.version=1.8.12
# Tue, 15 Jun 2021 23:26:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Jun 2021 23:26:34 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Jun 2021 23:26:39 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Jun 2021 23:26:40 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Jun 2021 23:26:41 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 23:26:41 GMT
VOLUME [/consul/data]
# Tue, 15 Jun 2021 23:26:41 GMT
EXPOSE 8300
# Tue, 15 Jun 2021 23:26:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Jun 2021 23:26:42 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Jun 2021 23:26:42 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Jun 2021 23:26:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 23:26:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe54e333fd380f115727e3666ffae1a9aedd92589a3b8c9dbfc296844434154a`  
		Last Modified: Tue, 15 Jun 2021 23:28:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a844bd3f8a21506c40174db0a3828d37ed514ad8086854d356a7b7fb00ab3636`  
		Last Modified: Tue, 15 Jun 2021 23:28:10 GMT  
		Size: 40.5 MB (40499476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e6cc7e41b21417b117174e9fe0233d5588078ec9cbc3bf50266157be7a3cae`  
		Last Modified: Tue, 15 Jun 2021 23:28:04 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd20c602f030070cbcabb10718e4a21a091755c559fe8841d649347ede36560`  
		Last Modified: Tue, 15 Jun 2021 23:28:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95e5bdbbf526978d9d74b104f3885dd0a8b68ac752dc30362aa99f5774987d0`  
		Last Modified: Tue, 15 Jun 2021 23:28:04 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:760a89adfece3da33413ab9d5f4857ebacb5dee723278587cf56d51b9635a1f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47356376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63985bbb3af3b3d7322f609d9684cd39080ef18c0c21397e131ccc1bab38e6e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 20:38:32 GMT
ARG CONSUL_VERSION=1.8.12
# Mon, 14 Jun 2021 20:38:32 GMT
LABEL org.opencontainers.image.version=1.8.12
# Mon, 14 Jun 2021 20:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 20:38:33 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 20:38:40 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 20:38:41 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 20:38:42 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 20:38:42 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 20:38:42 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 20:38:42 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 20:38:42 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 20:38:43 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 20:38:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 20:38:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256bb6489da66c2aeb1cf25e8adb54c100e2c59e19f477ae8144b31a711f7a4f`  
		Last Modified: Mon, 14 Jun 2021 20:39:17 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6c409fd79006450d0849ed41e2abe5ebc3a509608e25d5576b4896ee3d5dac`  
		Last Modified: Mon, 14 Jun 2021 20:39:24 GMT  
		Size: 44.5 MB (44534182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538ec45504b25d36911500d8f73a4a96df18658f06a45622eb7dcb8f726aeeba`  
		Last Modified: Mon, 14 Jun 2021 20:39:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b1ae7125741f31179f7a6f80b96dc437d3396e5e133d7d2259acc1749addac`  
		Last Modified: Mon, 14 Jun 2021 20:39:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87068562c8d492eadcc7bcfde844a1b7e890e3df49b7ebdb70b76b41608ad1a1`  
		Last Modified: Mon, 14 Jun 2021 20:39:18 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.12`

```console
$ docker pull consul@sha256:7a8e08198392458d96447b105c017879aaf8cfc40653052146865ea0d33342fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.12` - linux; amd64

```console
$ docker pull consul@sha256:16a579b62911fc315aa3745a7587b830dc3492660707284cad92bd1025d3e926
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47784420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a14d86a5934beabfa80a456cfdb0eb67502c469c091c790d9dad11a816aad806`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 21:19:34 GMT
ARG CONSUL_VERSION=1.8.12
# Mon, 14 Jun 2021 21:19:35 GMT
LABEL org.opencontainers.image.version=1.8.12
# Mon, 14 Jun 2021 21:19:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 21:19:36 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 21:19:43 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 21:19:44 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 21:19:45 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 21:19:45 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 21:19:45 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 21:19:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 21:19:45 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 21:19:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 21:19:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 21:19:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04c7fbae711bd2c2d465d3b7fbda785ff5f8494acb555a79863ea21055c4179`  
		Last Modified: Mon, 14 Jun 2021 21:20:07 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95fe4553a3dfa0e9a9602a23559e1b635e5cb83160a78ddb85fb967a5fd0d351`  
		Last Modified: Mon, 14 Jun 2021 21:20:13 GMT  
		Size: 45.0 MB (44969158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b943f75d06255a2f3b92c7756daa5eb8373cef2f62725eae4c1afc4ef2f910d`  
		Last Modified: Mon, 14 Jun 2021 21:20:07 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947a6323cd233cb7ff46a49af822da45b1827d82f9d64adf59d7ebeeeb6017cf`  
		Last Modified: Mon, 14 Jun 2021 21:20:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9a9a8a26baa71d6d61a0771664e8ececb12628dc6453ae88e425e7277f6e7f`  
		Last Modified: Mon, 14 Jun 2021 21:20:07 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.12` - linux; arm variant v6

```console
$ docker pull consul@sha256:0ee2b4100c5a6ab51947fcccfc485d9afb4bb2f31e9af86cc02098cee5225386
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43013082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30c688174aee0c0f2582d0d7ec7c8960092bcab8b697978db497df0e277ea03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 10:07:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 16 Jun 2021 10:07:49 GMT
ARG CONSUL_VERSION=1.8.12
# Wed, 16 Jun 2021 10:07:50 GMT
LABEL org.opencontainers.image.version=1.8.12
# Wed, 16 Jun 2021 10:07:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 16 Jun 2021 10:07:50 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 16 Jun 2021 10:08:07 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 16 Jun 2021 10:08:08 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 16 Jun 2021 10:08:09 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 10:08:09 GMT
VOLUME [/consul/data]
# Wed, 16 Jun 2021 10:08:09 GMT
EXPOSE 8300
# Wed, 16 Jun 2021 10:08:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 16 Jun 2021 10:08:10 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 16 Jun 2021 10:08:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 10:08:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 10:08:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c099865187bb396e24462cc214ca0a5e2f6541f5ac49c7543c77c4f3b39cd232`  
		Last Modified: Wed, 16 Jun 2021 10:09:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ace0ab017ba2542ff6fb63b8f5f21f2db481cce555f0a0f64f2dfd534c0e75`  
		Last Modified: Wed, 16 Jun 2021 10:10:00 GMT  
		Size: 40.4 MB (40387654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1540da76e8633df6c20de0314bcf2d5a41a7795e75bfc8f5b6074614a7f2a6`  
		Last Modified: Wed, 16 Jun 2021 10:09:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce52256f8ff85635432d10ba13a9172651a4d68d226630906484c208b4c8587`  
		Last Modified: Wed, 16 Jun 2021 10:09:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ba0829e54d2298982f9b677a29e03ee44874bf853cb0b5eebbf1d4d62c0307`  
		Last Modified: Wed, 16 Jun 2021 10:09:52 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.12` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:0bad60159d74bb7e33a0529244a396bd32c55c7dcd018cc5bb000ad581230b35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43214795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e59d9a1710ecda7320608134d03a856244cdca4229e41465ef80edc7af03810`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:25:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 15 Jun 2021 23:26:33 GMT
ARG CONSUL_VERSION=1.8.12
# Tue, 15 Jun 2021 23:26:33 GMT
LABEL org.opencontainers.image.version=1.8.12
# Tue, 15 Jun 2021 23:26:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Jun 2021 23:26:34 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Jun 2021 23:26:39 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Jun 2021 23:26:40 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Jun 2021 23:26:41 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 23:26:41 GMT
VOLUME [/consul/data]
# Tue, 15 Jun 2021 23:26:41 GMT
EXPOSE 8300
# Tue, 15 Jun 2021 23:26:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Jun 2021 23:26:42 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Jun 2021 23:26:42 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Jun 2021 23:26:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 23:26:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe54e333fd380f115727e3666ffae1a9aedd92589a3b8c9dbfc296844434154a`  
		Last Modified: Tue, 15 Jun 2021 23:28:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a844bd3f8a21506c40174db0a3828d37ed514ad8086854d356a7b7fb00ab3636`  
		Last Modified: Tue, 15 Jun 2021 23:28:10 GMT  
		Size: 40.5 MB (40499476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e6cc7e41b21417b117174e9fe0233d5588078ec9cbc3bf50266157be7a3cae`  
		Last Modified: Tue, 15 Jun 2021 23:28:04 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd20c602f030070cbcabb10718e4a21a091755c559fe8841d649347ede36560`  
		Last Modified: Tue, 15 Jun 2021 23:28:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d95e5bdbbf526978d9d74b104f3885dd0a8b68ac752dc30362aa99f5774987d0`  
		Last Modified: Tue, 15 Jun 2021 23:28:04 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.12` - linux; 386

```console
$ docker pull consul@sha256:760a89adfece3da33413ab9d5f4857ebacb5dee723278587cf56d51b9635a1f8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47356376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63985bbb3af3b3d7322f609d9684cd39080ef18c0c21397e131ccc1bab38e6e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 20:38:32 GMT
ARG CONSUL_VERSION=1.8.12
# Mon, 14 Jun 2021 20:38:32 GMT
LABEL org.opencontainers.image.version=1.8.12
# Mon, 14 Jun 2021 20:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 20:38:33 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 20:38:40 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 20:38:41 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 20:38:42 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 20:38:42 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 20:38:42 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 20:38:42 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 20:38:42 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 20:38:43 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 20:38:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 20:38:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256bb6489da66c2aeb1cf25e8adb54c100e2c59e19f477ae8144b31a711f7a4f`  
		Last Modified: Mon, 14 Jun 2021 20:39:17 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6c409fd79006450d0849ed41e2abe5ebc3a509608e25d5576b4896ee3d5dac`  
		Last Modified: Mon, 14 Jun 2021 20:39:24 GMT  
		Size: 44.5 MB (44534182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538ec45504b25d36911500d8f73a4a96df18658f06a45622eb7dcb8f726aeeba`  
		Last Modified: Mon, 14 Jun 2021 20:39:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b1ae7125741f31179f7a6f80b96dc437d3396e5e133d7d2259acc1749addac`  
		Last Modified: Mon, 14 Jun 2021 20:39:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87068562c8d492eadcc7bcfde844a1b7e890e3df49b7ebdb70b76b41608ad1a1`  
		Last Modified: Mon, 14 Jun 2021 20:39:18 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:b5858e763b09afc1b52faf1117778cb200749ecc3c20b64e194ab8dbd343ce21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:6e9cd324dc3f526e6a6c403f06bb8d2c973df871c4f97a84682bb0343e7eb686
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46264467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a567dca67fd81811f5b1b033a33b7a9387fc51c10f9c009cb2109651f2723b40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 18:23:41 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 18:23:41 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 18:23:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 18:23:42 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 18:23:52 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 18:23:53 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 18:23:54 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:23:54 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 18:23:54 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 18:23:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 18:23:55 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 18:23:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 18:23:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 18:23:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde40b69059c31854aa6e77d250e2a397755e55db6405a88894d67be03c89cbc`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223081562ed0234de495edff4fff45707cdce8b902099f0f7947fc9422313d81`  
		Last Modified: Mon, 14 Jun 2021 18:24:35 GMT  
		Size: 43.4 MB (43449203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5c8ab26ca1d55cb5e47b60c34d5f1d8f4497a54013a0a6b8c99069de6f4933`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9dedbbe1d0e5c35820ea2c7a756b34541b588f030a40877ab83036b9ff09aa`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14795d064a109c17b145a46d9505a7d5a820f2eadec010513cbd79897b29728`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:b280acdcf1a14d1a265acd1866b8ed2538244f04af804a7a14c51859733a490c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41468455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d3d3f0c577fd404f8680ebee7527ba4682ac3df36cf38f320309528b7bfc5a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 10:07:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 16 Jun 2021 10:07:31 GMT
ARG CONSUL_VERSION=1.9.6
# Wed, 16 Jun 2021 10:07:31 GMT
LABEL org.opencontainers.image.version=1.9.6
# Wed, 16 Jun 2021 10:07:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 16 Jun 2021 10:07:32 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 16 Jun 2021 10:07:38 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 16 Jun 2021 10:07:39 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 16 Jun 2021 10:07:40 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 10:07:40 GMT
VOLUME [/consul/data]
# Wed, 16 Jun 2021 10:07:40 GMT
EXPOSE 8300
# Wed, 16 Jun 2021 10:07:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 16 Jun 2021 10:07:41 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 16 Jun 2021 10:07:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 10:07:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 10:07:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0108bc74874b22bad588476804a5392c12334b7408c3efc9bba24d4f37746e25`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f272638472210f71307e5fd0748e0f8649b847da70f81b1a0e02747c2fac5cb`  
		Last Modified: Wed, 16 Jun 2021 10:09:35 GMT  
		Size: 38.8 MB (38843030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05382787f20dfcc0c82ea28ef6962460fce2cee09634c90353c98790d87b778`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44d0014536e85cb30a2bdec47639a491b42b59920d3c72ac97bb365c6a14717`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e26fc6ee38ef31d867270128d7fec282d844e3cd1aea45d24bd7677c88e0`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a5e069a0b66522342081bfba49efb32664adb20714236d8a192f14be554b270a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41703997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1501e07a79c1edb5402ee22f383b8a66641a2ffdb753526a2072694713f35c10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:25:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 15 Jun 2021 23:26:17 GMT
ARG CONSUL_VERSION=1.9.6
# Tue, 15 Jun 2021 23:26:17 GMT
LABEL org.opencontainers.image.version=1.9.6
# Tue, 15 Jun 2021 23:26:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Jun 2021 23:26:18 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Jun 2021 23:26:24 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Jun 2021 23:26:25 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Jun 2021 23:26:25 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 23:26:26 GMT
VOLUME [/consul/data]
# Tue, 15 Jun 2021 23:26:26 GMT
EXPOSE 8300
# Tue, 15 Jun 2021 23:26:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Jun 2021 23:26:26 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Jun 2021 23:26:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Jun 2021 23:26:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 23:26:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fb07849d5b5c564f3eaffc9d79b9af13b69576177e6c87bfb35eb00f2f55f0`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d3e2322fe476ac4da0701e58800e24278997627030f1daeca29e807670ab8e`  
		Last Modified: Tue, 15 Jun 2021 23:27:48 GMT  
		Size: 39.0 MB (38988674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f6a5bd00aa1c40e2f0d29893ca86c9975bc7fe8e681a6ff0548a0e76bba21b`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01d633c1d168879e677bf4ae1df835f0488183f94adfde92cd71e18907780fe`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d702b2837f77e23e6382aed6cfd7ee2d6c5193b6d7cbca368050ed8f6dd9df59`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:9118e82e2e4a9f473ae4981cdc91f1d50fb881c690d270b72e89a5d029abc2a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45642795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6e5c298ebfeb32f526d360cce957e7c1ee66fa0a136ea745d07c972bd52abb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 18:38:31 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 18:38:31 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 18:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 18:38:32 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 18:38:39 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 18:38:40 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 18:38:41 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:38:41 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 18:38:41 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 18:38:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 18:38:42 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 18:38:42 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 18:38:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 18:38:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67944a51f11e6cfa9950c180de11c215b0c98133e61b48100a4dc594e6ea09`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328187fad7df4b51875cef3c8dd1991dc54ec6fcdfd87c709662bb402a41e64e`  
		Last Modified: Mon, 14 Jun 2021 18:39:37 GMT  
		Size: 42.8 MB (42820607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc84186166a357fb3a53365d8eca62e250858278a931735f55e8dfd36f7730e`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d35d86fa7fdb9f375a93645edb75499a747c4f7d3dde8f3273dfec6edf32ac6`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7be79a2532d4db1e4d47bba89c76a514b3ead9ff66c7f79af558f702e74f46`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.6`

```console
$ docker pull consul@sha256:b5858e763b09afc1b52faf1117778cb200749ecc3c20b64e194ab8dbd343ce21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.6` - linux; amd64

```console
$ docker pull consul@sha256:6e9cd324dc3f526e6a6c403f06bb8d2c973df871c4f97a84682bb0343e7eb686
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46264467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a567dca67fd81811f5b1b033a33b7a9387fc51c10f9c009cb2109651f2723b40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 18:23:41 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 18:23:41 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 18:23:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 18:23:42 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 18:23:52 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 18:23:53 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 18:23:54 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:23:54 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 18:23:54 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 18:23:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 18:23:55 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 18:23:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 18:23:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 18:23:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde40b69059c31854aa6e77d250e2a397755e55db6405a88894d67be03c89cbc`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223081562ed0234de495edff4fff45707cdce8b902099f0f7947fc9422313d81`  
		Last Modified: Mon, 14 Jun 2021 18:24:35 GMT  
		Size: 43.4 MB (43449203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5c8ab26ca1d55cb5e47b60c34d5f1d8f4497a54013a0a6b8c99069de6f4933`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9dedbbe1d0e5c35820ea2c7a756b34541b588f030a40877ab83036b9ff09aa`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14795d064a109c17b145a46d9505a7d5a820f2eadec010513cbd79897b29728`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:b280acdcf1a14d1a265acd1866b8ed2538244f04af804a7a14c51859733a490c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41468455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d3d3f0c577fd404f8680ebee7527ba4682ac3df36cf38f320309528b7bfc5a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 10:07:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 16 Jun 2021 10:07:31 GMT
ARG CONSUL_VERSION=1.9.6
# Wed, 16 Jun 2021 10:07:31 GMT
LABEL org.opencontainers.image.version=1.9.6
# Wed, 16 Jun 2021 10:07:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 16 Jun 2021 10:07:32 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 16 Jun 2021 10:07:38 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 16 Jun 2021 10:07:39 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 16 Jun 2021 10:07:40 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 10:07:40 GMT
VOLUME [/consul/data]
# Wed, 16 Jun 2021 10:07:40 GMT
EXPOSE 8300
# Wed, 16 Jun 2021 10:07:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 16 Jun 2021 10:07:41 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 16 Jun 2021 10:07:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 10:07:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 10:07:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0108bc74874b22bad588476804a5392c12334b7408c3efc9bba24d4f37746e25`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f272638472210f71307e5fd0748e0f8649b847da70f81b1a0e02747c2fac5cb`  
		Last Modified: Wed, 16 Jun 2021 10:09:35 GMT  
		Size: 38.8 MB (38843030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05382787f20dfcc0c82ea28ef6962460fce2cee09634c90353c98790d87b778`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44d0014536e85cb30a2bdec47639a491b42b59920d3c72ac97bb365c6a14717`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e26fc6ee38ef31d867270128d7fec282d844e3cd1aea45d24bd7677c88e0`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a5e069a0b66522342081bfba49efb32664adb20714236d8a192f14be554b270a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41703997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1501e07a79c1edb5402ee22f383b8a66641a2ffdb753526a2072694713f35c10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:25:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 15 Jun 2021 23:26:17 GMT
ARG CONSUL_VERSION=1.9.6
# Tue, 15 Jun 2021 23:26:17 GMT
LABEL org.opencontainers.image.version=1.9.6
# Tue, 15 Jun 2021 23:26:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Jun 2021 23:26:18 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Jun 2021 23:26:24 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Jun 2021 23:26:25 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Jun 2021 23:26:25 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 23:26:26 GMT
VOLUME [/consul/data]
# Tue, 15 Jun 2021 23:26:26 GMT
EXPOSE 8300
# Tue, 15 Jun 2021 23:26:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Jun 2021 23:26:26 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Jun 2021 23:26:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Jun 2021 23:26:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 23:26:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fb07849d5b5c564f3eaffc9d79b9af13b69576177e6c87bfb35eb00f2f55f0`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d3e2322fe476ac4da0701e58800e24278997627030f1daeca29e807670ab8e`  
		Last Modified: Tue, 15 Jun 2021 23:27:48 GMT  
		Size: 39.0 MB (38988674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f6a5bd00aa1c40e2f0d29893ca86c9975bc7fe8e681a6ff0548a0e76bba21b`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01d633c1d168879e677bf4ae1df835f0488183f94adfde92cd71e18907780fe`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d702b2837f77e23e6382aed6cfd7ee2d6c5193b6d7cbca368050ed8f6dd9df59`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.6` - linux; 386

```console
$ docker pull consul@sha256:9118e82e2e4a9f473ae4981cdc91f1d50fb881c690d270b72e89a5d029abc2a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45642795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6e5c298ebfeb32f526d360cce957e7c1ee66fa0a136ea745d07c972bd52abb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 18:38:31 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 18:38:31 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 18:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 18:38:32 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 18:38:39 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 18:38:40 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 18:38:41 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:38:41 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 18:38:41 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 18:38:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 18:38:42 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 18:38:42 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 18:38:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 18:38:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67944a51f11e6cfa9950c180de11c215b0c98133e61b48100a4dc594e6ea09`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328187fad7df4b51875cef3c8dd1991dc54ec6fcdfd87c709662bb402a41e64e`  
		Last Modified: Mon, 14 Jun 2021 18:39:37 GMT  
		Size: 42.8 MB (42820607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc84186166a357fb3a53365d8eca62e250858278a931735f55e8dfd36f7730e`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d35d86fa7fdb9f375a93645edb75499a747c4f7d3dde8f3273dfec6edf32ac6`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7be79a2532d4db1e4d47bba89c76a514b3ead9ff66c7f79af558f702e74f46`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:b5858e763b09afc1b52faf1117778cb200749ecc3c20b64e194ab8dbd343ce21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:6e9cd324dc3f526e6a6c403f06bb8d2c973df871c4f97a84682bb0343e7eb686
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46264467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a567dca67fd81811f5b1b033a33b7a9387fc51c10f9c009cb2109651f2723b40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 18:23:41 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 18:23:41 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 18:23:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 18:23:42 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 18:23:52 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 18:23:53 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 18:23:54 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:23:54 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 18:23:54 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 18:23:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 18:23:55 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 18:23:55 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 18:23:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 18:23:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde40b69059c31854aa6e77d250e2a397755e55db6405a88894d67be03c89cbc`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223081562ed0234de495edff4fff45707cdce8b902099f0f7947fc9422313d81`  
		Last Modified: Mon, 14 Jun 2021 18:24:35 GMT  
		Size: 43.4 MB (43449203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5c8ab26ca1d55cb5e47b60c34d5f1d8f4497a54013a0a6b8c99069de6f4933`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c9dedbbe1d0e5c35820ea2c7a756b34541b588f030a40877ab83036b9ff09aa`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14795d064a109c17b145a46d9505a7d5a820f2eadec010513cbd79897b29728`  
		Last Modified: Mon, 14 Jun 2021 18:24:29 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:b280acdcf1a14d1a265acd1866b8ed2538244f04af804a7a14c51859733a490c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41468455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d3d3f0c577fd404f8680ebee7527ba4682ac3df36cf38f320309528b7bfc5a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:34 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Tue, 15 Jun 2021 22:57:34 GMT
CMD ["/bin/sh"]
# Wed, 16 Jun 2021 10:07:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Wed, 16 Jun 2021 10:07:31 GMT
ARG CONSUL_VERSION=1.9.6
# Wed, 16 Jun 2021 10:07:31 GMT
LABEL org.opencontainers.image.version=1.9.6
# Wed, 16 Jun 2021 10:07:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 16 Jun 2021 10:07:32 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 16 Jun 2021 10:07:38 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 16 Jun 2021 10:07:39 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 16 Jun 2021 10:07:40 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 16 Jun 2021 10:07:40 GMT
VOLUME [/consul/data]
# Wed, 16 Jun 2021 10:07:40 GMT
EXPOSE 8300
# Wed, 16 Jun 2021 10:07:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 16 Jun 2021 10:07:41 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 16 Jun 2021 10:07:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 16 Jun 2021 10:07:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Jun 2021 10:07:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0108bc74874b22bad588476804a5392c12334b7408c3efc9bba24d4f37746e25`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f272638472210f71307e5fd0748e0f8649b847da70f81b1a0e02747c2fac5cb`  
		Last Modified: Wed, 16 Jun 2021 10:09:35 GMT  
		Size: 38.8 MB (38843030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05382787f20dfcc0c82ea28ef6962460fce2cee09634c90353c98790d87b778`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d44d0014536e85cb30a2bdec47639a491b42b59920d3c72ac97bb365c6a14717`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439e26fc6ee38ef31d867270128d7fec282d844e3cd1aea45d24bd7677c88e0`  
		Last Modified: Wed, 16 Jun 2021 10:09:28 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a5e069a0b66522342081bfba49efb32664adb20714236d8a192f14be554b270a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41703997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1501e07a79c1edb5402ee22f383b8a66641a2ffdb753526a2072694713f35c10`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:25:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 15 Jun 2021 23:26:17 GMT
ARG CONSUL_VERSION=1.9.6
# Tue, 15 Jun 2021 23:26:17 GMT
LABEL org.opencontainers.image.version=1.9.6
# Tue, 15 Jun 2021 23:26:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Jun 2021 23:26:18 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Jun 2021 23:26:24 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Jun 2021 23:26:25 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Jun 2021 23:26:25 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Jun 2021 23:26:26 GMT
VOLUME [/consul/data]
# Tue, 15 Jun 2021 23:26:26 GMT
EXPOSE 8300
# Tue, 15 Jun 2021 23:26:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Jun 2021 23:26:26 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Jun 2021 23:26:26 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Jun 2021 23:26:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Jun 2021 23:26:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fb07849d5b5c564f3eaffc9d79b9af13b69576177e6c87bfb35eb00f2f55f0`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d3e2322fe476ac4da0701e58800e24278997627030f1daeca29e807670ab8e`  
		Last Modified: Tue, 15 Jun 2021 23:27:48 GMT  
		Size: 39.0 MB (38988674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f6a5bd00aa1c40e2f0d29893ca86c9975bc7fe8e681a6ff0548a0e76bba21b`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01d633c1d168879e677bf4ae1df835f0488183f94adfde92cd71e18907780fe`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d702b2837f77e23e6382aed6cfd7ee2d6c5193b6d7cbca368050ed8f6dd9df59`  
		Last Modified: Tue, 15 Jun 2021 23:27:42 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:9118e82e2e4a9f473ae4981cdc91f1d50fb881c690d270b72e89a5d029abc2a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45642795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c6e5c298ebfeb32f526d360cce957e7c1ee66fa0a136ea745d07c972bd52abb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 18:38:31 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 18:38:31 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 18:38:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 18:38:32 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 18:38:39 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 18:38:40 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 18:38:41 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:38:41 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 18:38:41 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 18:38:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 18:38:42 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 18:38:42 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 18:38:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 18:38:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a67944a51f11e6cfa9950c180de11c215b0c98133e61b48100a4dc594e6ea09`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328187fad7df4b51875cef3c8dd1991dc54ec6fcdfd87c709662bb402a41e64e`  
		Last Modified: Mon, 14 Jun 2021 18:39:37 GMT  
		Size: 42.8 MB (42820607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc84186166a357fb3a53365d8eca62e250858278a931735f55e8dfd36f7730e`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d35d86fa7fdb9f375a93645edb75499a747c4f7d3dde8f3273dfec6edf32ac6`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f7be79a2532d4db1e4d47bba89c76a514b3ead9ff66c7f79af558f702e74f46`  
		Last Modified: Mon, 14 Jun 2021 18:39:31 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
