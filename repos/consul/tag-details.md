<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10.0-beta`](#consul1100-beta)
-	[`consul:1.10.0-beta4`](#consul1100-beta4)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.14`](#consul1714)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.12`](#consul1812)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.6`](#consul196)
-	[`consul:latest`](#consullatest)

## `consul:1.10.0-beta`

```console
$ docker pull consul@sha256:d41e22296f1de4caca66942673672124df8ec17ccc08677d585187925dea40f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.0-beta` - linux; amd64

```console
$ docker pull consul@sha256:8d9043c9c9c7dd8a4c3a3be4cc5435748d2f7872b49a696509c2da7df2586840
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43598491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01b476d5e738a9b6fea3e740e409d507af4a8aeeae10514f73bda5e45407e93`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 10 Jun 2021 18:19:29 GMT
ARG CONSUL_VERSION=1.10.0-beta4
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.version=1.10.0-beta4
# Thu, 10 Jun 2021 18:19:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Jun 2021 18:19:31 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Jun 2021 18:19:37 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Jun 2021 18:19:38 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Jun 2021 18:19:39 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Jun 2021 18:19:39 GMT
VOLUME [/consul/data]
# Thu, 10 Jun 2021 18:19:39 GMT
EXPOSE 8300
# Thu, 10 Jun 2021 18:19:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Jun 2021 18:19:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Jun 2021 18:19:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Jun 2021 18:19:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Jun 2021 18:19:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10702266d38dc67c665be845ec1a25804973fee188dcf4d73471112360453c71`  
		Last Modified: Thu, 10 Jun 2021 18:20:03 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c2906d900e6a9bb894e6df8861caa928bb150e3dc5ba3a5f9e25814ff2628c`  
		Last Modified: Thu, 10 Jun 2021 18:20:09 GMT  
		Size: 40.8 MB (40783229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730bacbfa2967a7f9978120e922ff5ef7164eda58eda6d7f068eab3f8db28c54`  
		Last Modified: Thu, 10 Jun 2021 18:20:04 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a5574a17158a1eb4677134dd9afadc9941f7622479cf5b371f4123a267d289`  
		Last Modified: Thu, 10 Jun 2021 18:20:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4512d76b24eac44f8281715c3dcf9f5b45bce4673170ffc7bcc0edfbb4d77831`  
		Last Modified: Thu, 10 Jun 2021 18:20:04 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-beta` - linux; arm variant v6

```console
$ docker pull consul@sha256:2ddd89a9689c5d487c14326911d95f1217e107f2342dc0ee57fe2248bab9548e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39634130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f1ba93ab3270f92b64eaf6dc5ae26f79380ed37125166b03f2ac80c9e89630`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:50:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 10 Jun 2021 17:50:58 GMT
ARG CONSUL_VERSION=1.10.0-beta4
# Thu, 10 Jun 2021 17:50:58 GMT
LABEL org.opencontainers.image.version=1.10.0-beta4
# Thu, 10 Jun 2021 17:50:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Jun 2021 17:50:59 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Jun 2021 17:53:16 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Jun 2021 17:53:17 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Jun 2021 17:53:17 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Jun 2021 17:53:18 GMT
VOLUME [/consul/data]
# Thu, 10 Jun 2021 17:53:18 GMT
EXPOSE 8300
# Thu, 10 Jun 2021 17:53:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Jun 2021 17:53:18 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Jun 2021 17:53:18 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Jun 2021 17:53:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Jun 2021 17:53:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a21e960df5e4cc7db85559d6c166965238ff0d676e45e059d7b7ca70e40932e`  
		Last Modified: Thu, 10 Jun 2021 17:54:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0387f49d28c74c4d99a926938baf0282fcfd027a1da40dcb7035784a3aa6c34c`  
		Last Modified: Thu, 10 Jun 2021 17:54:22 GMT  
		Size: 37.0 MB (37008708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f509ea9e4c0fb00253888bcad0765bea67045a06af8012bfb4c7733d8acbcb68`  
		Last Modified: Thu, 10 Jun 2021 17:54:16 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331a8dfc8dc4504280476c24f8911e94b610dfa7782a1d657b9beb617b256291`  
		Last Modified: Thu, 10 Jun 2021 17:54:16 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47e6fb8841393cb104f3d7277a1b1569cfd9c4a6c5332c375520a659d8bac6b`  
		Last Modified: Thu, 10 Jun 2021 17:54:16 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-beta` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:9ed6e0dd66269596c95682bbcf5dfd0b840ded2f64be7ffc169a62a45db5307f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39562357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a51ea3755af5a3fbd326b69836b72e227a388b9da8e7556b836e0bb9bebd296`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:40:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 10 Jun 2021 17:40:35 GMT
ARG CONSUL_VERSION=1.10.0-beta4
# Thu, 10 Jun 2021 17:40:35 GMT
LABEL org.opencontainers.image.version=1.10.0-beta4
# Thu, 10 Jun 2021 17:40:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Jun 2021 17:40:36 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Jun 2021 17:40:42 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Jun 2021 17:40:43 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Jun 2021 17:40:44 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Jun 2021 17:40:44 GMT
VOLUME [/consul/data]
# Thu, 10 Jun 2021 17:40:44 GMT
EXPOSE 8300
# Thu, 10 Jun 2021 17:40:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Jun 2021 17:40:44 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Jun 2021 17:40:45 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Jun 2021 17:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Jun 2021 17:40:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8865ae44b77912e14ffc1b659d684c92c8091128bec63998f9f889f066550972`  
		Last Modified: Thu, 10 Jun 2021 17:41:26 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe592fe5c07ebd867a30e7c9fa6dfb8ab8a7dda047eb77a29851c95f414eee`  
		Last Modified: Thu, 10 Jun 2021 17:41:31 GMT  
		Size: 36.8 MB (36847039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bdcc2cd3aed7389e9ae7c848c3e64cd7216e83882e6df717d28305d7b1c74a`  
		Last Modified: Thu, 10 Jun 2021 17:41:26 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dc937c34ac5eb20b4803b74844b98d9a223938555400a4556f59261cbf1db8`  
		Last Modified: Thu, 10 Jun 2021 17:41:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e5803a2de0b65abc538ad12f402a479ff83e6285a7c07523a682d26e7262cc`  
		Last Modified: Thu, 10 Jun 2021 17:41:26 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-beta` - linux; 386

```console
$ docker pull consul@sha256:f0951b75fd61b904b2c2cfb9a8d4884b2548040f726b7239193d8c9694c8d0a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (42985755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea34052e60c16b797520f2aab216ae19e2177e626dd7909a037538581f5320d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 10 Jun 2021 17:39:34 GMT
ARG CONSUL_VERSION=1.10.0-beta4
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.version=1.10.0-beta4
# Thu, 10 Jun 2021 17:39:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Jun 2021 17:39:35 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Jun 2021 17:39:42 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Jun 2021 17:39:43 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Jun 2021 17:39:44 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Jun 2021 17:39:44 GMT
VOLUME [/consul/data]
# Thu, 10 Jun 2021 17:39:45 GMT
EXPOSE 8300
# Thu, 10 Jun 2021 17:39:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Jun 2021 17:39:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Jun 2021 17:39:45 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Jun 2021 17:39:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Jun 2021 17:39:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c6930237fe0c8fea571fef987fb29d9af4eba8e89e51afb8693f52f33899d5`  
		Last Modified: Thu, 10 Jun 2021 17:40:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6877008275fed8f5e13f47d006b09cd6b3d7619b0a49932e30f2f37444d7f4fd`  
		Last Modified: Thu, 10 Jun 2021 17:40:31 GMT  
		Size: 40.2 MB (40163564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12d0c4e2bb2025dc5ded9d308360590b689724f42507227c38406e60757766`  
		Last Modified: Thu, 10 Jun 2021 17:40:24 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e4cf72f4e3d62b55f5c424d1f21816eb5be81b9c2ec2c8e3770dc487676cee`  
		Last Modified: Thu, 10 Jun 2021 17:40:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6b3df55eb565a9ade2e9a9f6c595686ee81a1e2d9fbd23c4122025afff6853`  
		Last Modified: Thu, 10 Jun 2021 17:40:25 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.0-beta4`

```console
$ docker pull consul@sha256:d41e22296f1de4caca66942673672124df8ec17ccc08677d585187925dea40f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.0-beta4` - linux; amd64

```console
$ docker pull consul@sha256:8d9043c9c9c7dd8a4c3a3be4cc5435748d2f7872b49a696509c2da7df2586840
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43598491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01b476d5e738a9b6fea3e740e409d507af4a8aeeae10514f73bda5e45407e93`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 10 Jun 2021 18:19:29 GMT
ARG CONSUL_VERSION=1.10.0-beta4
# Thu, 10 Jun 2021 18:19:29 GMT
LABEL org.opencontainers.image.version=1.10.0-beta4
# Thu, 10 Jun 2021 18:19:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Jun 2021 18:19:31 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Jun 2021 18:19:37 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Jun 2021 18:19:38 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Jun 2021 18:19:39 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Jun 2021 18:19:39 GMT
VOLUME [/consul/data]
# Thu, 10 Jun 2021 18:19:39 GMT
EXPOSE 8300
# Thu, 10 Jun 2021 18:19:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Jun 2021 18:19:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Jun 2021 18:19:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Jun 2021 18:19:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Jun 2021 18:19:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10702266d38dc67c665be845ec1a25804973fee188dcf4d73471112360453c71`  
		Last Modified: Thu, 10 Jun 2021 18:20:03 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c2906d900e6a9bb894e6df8861caa928bb150e3dc5ba3a5f9e25814ff2628c`  
		Last Modified: Thu, 10 Jun 2021 18:20:09 GMT  
		Size: 40.8 MB (40783229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730bacbfa2967a7f9978120e922ff5ef7164eda58eda6d7f068eab3f8db28c54`  
		Last Modified: Thu, 10 Jun 2021 18:20:04 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a5574a17158a1eb4677134dd9afadc9941f7622479cf5b371f4123a267d289`  
		Last Modified: Thu, 10 Jun 2021 18:20:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4512d76b24eac44f8281715c3dcf9f5b45bce4673170ffc7bcc0edfbb4d77831`  
		Last Modified: Thu, 10 Jun 2021 18:20:04 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-beta4` - linux; arm variant v6

```console
$ docker pull consul@sha256:2ddd89a9689c5d487c14326911d95f1217e107f2342dc0ee57fe2248bab9548e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39634130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f1ba93ab3270f92b64eaf6dc5ae26f79380ed37125166b03f2ac80c9e89630`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:50:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 10 Jun 2021 17:50:58 GMT
ARG CONSUL_VERSION=1.10.0-beta4
# Thu, 10 Jun 2021 17:50:58 GMT
LABEL org.opencontainers.image.version=1.10.0-beta4
# Thu, 10 Jun 2021 17:50:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Jun 2021 17:50:59 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Jun 2021 17:53:16 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Jun 2021 17:53:17 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Jun 2021 17:53:17 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Jun 2021 17:53:18 GMT
VOLUME [/consul/data]
# Thu, 10 Jun 2021 17:53:18 GMT
EXPOSE 8300
# Thu, 10 Jun 2021 17:53:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Jun 2021 17:53:18 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Jun 2021 17:53:18 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Jun 2021 17:53:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Jun 2021 17:53:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a21e960df5e4cc7db85559d6c166965238ff0d676e45e059d7b7ca70e40932e`  
		Last Modified: Thu, 10 Jun 2021 17:54:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0387f49d28c74c4d99a926938baf0282fcfd027a1da40dcb7035784a3aa6c34c`  
		Last Modified: Thu, 10 Jun 2021 17:54:22 GMT  
		Size: 37.0 MB (37008708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f509ea9e4c0fb00253888bcad0765bea67045a06af8012bfb4c7733d8acbcb68`  
		Last Modified: Thu, 10 Jun 2021 17:54:16 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331a8dfc8dc4504280476c24f8911e94b610dfa7782a1d657b9beb617b256291`  
		Last Modified: Thu, 10 Jun 2021 17:54:16 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47e6fb8841393cb104f3d7277a1b1569cfd9c4a6c5332c375520a659d8bac6b`  
		Last Modified: Thu, 10 Jun 2021 17:54:16 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-beta4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:9ed6e0dd66269596c95682bbcf5dfd0b840ded2f64be7ffc169a62a45db5307f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39562357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a51ea3755af5a3fbd326b69836b72e227a388b9da8e7556b836e0bb9bebd296`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:40:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 10 Jun 2021 17:40:35 GMT
ARG CONSUL_VERSION=1.10.0-beta4
# Thu, 10 Jun 2021 17:40:35 GMT
LABEL org.opencontainers.image.version=1.10.0-beta4
# Thu, 10 Jun 2021 17:40:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Jun 2021 17:40:36 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Jun 2021 17:40:42 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Jun 2021 17:40:43 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Jun 2021 17:40:44 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Jun 2021 17:40:44 GMT
VOLUME [/consul/data]
# Thu, 10 Jun 2021 17:40:44 GMT
EXPOSE 8300
# Thu, 10 Jun 2021 17:40:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Jun 2021 17:40:44 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Jun 2021 17:40:45 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Jun 2021 17:40:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Jun 2021 17:40:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8865ae44b77912e14ffc1b659d684c92c8091128bec63998f9f889f066550972`  
		Last Modified: Thu, 10 Jun 2021 17:41:26 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe592fe5c07ebd867a30e7c9fa6dfb8ab8a7dda047eb77a29851c95f414eee`  
		Last Modified: Thu, 10 Jun 2021 17:41:31 GMT  
		Size: 36.8 MB (36847039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bdcc2cd3aed7389e9ae7c848c3e64cd7216e83882e6df717d28305d7b1c74a`  
		Last Modified: Thu, 10 Jun 2021 17:41:26 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dc937c34ac5eb20b4803b74844b98d9a223938555400a4556f59261cbf1db8`  
		Last Modified: Thu, 10 Jun 2021 17:41:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e5803a2de0b65abc538ad12f402a479ff83e6285a7c07523a682d26e7262cc`  
		Last Modified: Thu, 10 Jun 2021 17:41:26 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.0-beta4` - linux; 386

```console
$ docker pull consul@sha256:f0951b75fd61b904b2c2cfb9a8d4884b2548040f726b7239193d8c9694c8d0a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (42985755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ea34052e60c16b797520f2aab216ae19e2177e626dd7909a037538581f5320d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 10 Jun 2021 17:39:34 GMT
ARG CONSUL_VERSION=1.10.0-beta4
# Thu, 10 Jun 2021 17:39:34 GMT
LABEL org.opencontainers.image.version=1.10.0-beta4
# Thu, 10 Jun 2021 17:39:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Jun 2021 17:39:35 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Jun 2021 17:39:42 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Jun 2021 17:39:43 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Jun 2021 17:39:44 GMT
# ARGS: CONSUL_VERSION=1.10.0-beta4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Jun 2021 17:39:44 GMT
VOLUME [/consul/data]
# Thu, 10 Jun 2021 17:39:45 GMT
EXPOSE 8300
# Thu, 10 Jun 2021 17:39:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Jun 2021 17:39:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Jun 2021 17:39:45 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Jun 2021 17:39:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Jun 2021 17:39:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c6930237fe0c8fea571fef987fb29d9af4eba8e89e51afb8693f52f33899d5`  
		Last Modified: Thu, 10 Jun 2021 17:40:24 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6877008275fed8f5e13f47d006b09cd6b3d7619b0a49932e30f2f37444d7f4fd`  
		Last Modified: Thu, 10 Jun 2021 17:40:31 GMT  
		Size: 40.2 MB (40163564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d12d0c4e2bb2025dc5ded9d308360590b689724f42507227c38406e60757766`  
		Last Modified: Thu, 10 Jun 2021 17:40:24 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e4cf72f4e3d62b55f5c424d1f21816eb5be81b9c2ec2c8e3770dc487676cee`  
		Last Modified: Thu, 10 Jun 2021 17:40:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6b3df55eb565a9ade2e9a9f6c595686ee81a1e2d9fbd23c4122025afff6853`  
		Last Modified: Thu, 10 Jun 2021 17:40:25 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7`

```console
$ docker pull consul@sha256:04a38222c287d0403e7662eb403db7409d84281163ccd62912aa5f13e47c213c
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
$ docker pull consul@sha256:005dbbf58bc1403ac04cfbc4e765352a466b896bb09dbffa68ad96aeb059cca3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39269558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95796f649ed1d8ce69cfafcfca9df0114f3b5a809ce2dd562ed1c6e94fd9645c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 18:49:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 27 May 2021 18:50:54 GMT
ARG CONSUL_VERSION=1.7.14
# Thu, 27 May 2021 18:50:54 GMT
LABEL org.opencontainers.image.version=1.7.14
# Thu, 27 May 2021 18:50:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 27 May 2021 18:50:56 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 27 May 2021 18:51:03 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 27 May 2021 18:51:04 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 27 May 2021 18:51:05 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 18:51:05 GMT
VOLUME [/consul/data]
# Thu, 27 May 2021 18:51:06 GMT
EXPOSE 8300
# Thu, 27 May 2021 18:51:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 27 May 2021 18:51:06 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 27 May 2021 18:51:06 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 27 May 2021 18:51:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 May 2021 18:51:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb7a805d14d4dd60741e623bb7c9942a34e99a0164299924bf0057c0e04782c`  
		Last Modified: Thu, 27 May 2021 18:53:00 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187393928ee725f5b2093435f08e7974e030f5cebb4df9c65ef15a4acd5e9952`  
		Last Modified: Thu, 27 May 2021 18:53:09 GMT  
		Size: 36.7 MB (36661010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5404ac7d5e69bbc3cf976f7d3fe564d2f1f388d9a1200d9e991a4cd2cba1e51c`  
		Last Modified: Thu, 27 May 2021 18:53:00 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ed607ad3c36647ad714a1900e3712524ef36b4d2def06b147cf3af6fcdb4ae`  
		Last Modified: Thu, 27 May 2021 18:53:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7987082bd8043531ce033d1e8127167b9e0b28d8cac814d5ff4b70e318556943`  
		Last Modified: Thu, 27 May 2021 18:53:00 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:094d6c52657e088899e1d0ea8d956d32561f3efcbb6617404755ee1bbf5d194a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39546893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:911fdfb898ea5d7cdb531b99615a68eec104179258a03685ef677f482be7687b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:02:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 27 May 2021 22:03:54 GMT
ARG CONSUL_VERSION=1.7.14
# Thu, 27 May 2021 22:03:54 GMT
LABEL org.opencontainers.image.version=1.7.14
# Thu, 27 May 2021 22:03:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 27 May 2021 22:03:55 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 27 May 2021 22:03:59 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 27 May 2021 22:04:00 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 27 May 2021 22:04:01 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:04:01 GMT
VOLUME [/consul/data]
# Thu, 27 May 2021 22:04:01 GMT
EXPOSE 8300
# Thu, 27 May 2021 22:04:02 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 27 May 2021 22:04:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 27 May 2021 22:04:02 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 27 May 2021 22:04:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 May 2021 22:04:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa0a158ae271fcd11844dba1dccf9979d4f6366d27c676f33c9a6598cbe5ef2`  
		Last Modified: Thu, 27 May 2021 22:05:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3b246eb81fd4e2bc713798b889332a2bd9a4339a6b7305ffa736aa583065e6`  
		Last Modified: Thu, 27 May 2021 22:05:34 GMT  
		Size: 36.8 MB (36832906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be52bed9e7cc30dc2b5240834c16088bd6f085f655b11a00d8f2a5b540139f6`  
		Last Modified: Thu, 27 May 2021 22:05:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a2dda76301f0e3af98a369db6b272a2b2b3206a86a1c8641599f8434be41e`  
		Last Modified: Thu, 27 May 2021 22:05:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95eab3746c8b82bd4cb387dbfc822bfcaabc377d5e83b87e3a56a55140d7cac0`  
		Last Modified: Thu, 27 May 2021 22:05:29 GMT  
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
$ docker pull consul@sha256:04a38222c287d0403e7662eb403db7409d84281163ccd62912aa5f13e47c213c
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
$ docker pull consul@sha256:005dbbf58bc1403ac04cfbc4e765352a466b896bb09dbffa68ad96aeb059cca3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39269558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95796f649ed1d8ce69cfafcfca9df0114f3b5a809ce2dd562ed1c6e94fd9645c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 18:49:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 27 May 2021 18:50:54 GMT
ARG CONSUL_VERSION=1.7.14
# Thu, 27 May 2021 18:50:54 GMT
LABEL org.opencontainers.image.version=1.7.14
# Thu, 27 May 2021 18:50:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 27 May 2021 18:50:56 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 27 May 2021 18:51:03 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 27 May 2021 18:51:04 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 27 May 2021 18:51:05 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 18:51:05 GMT
VOLUME [/consul/data]
# Thu, 27 May 2021 18:51:06 GMT
EXPOSE 8300
# Thu, 27 May 2021 18:51:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 27 May 2021 18:51:06 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 27 May 2021 18:51:06 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 27 May 2021 18:51:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 May 2021 18:51:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb7a805d14d4dd60741e623bb7c9942a34e99a0164299924bf0057c0e04782c`  
		Last Modified: Thu, 27 May 2021 18:53:00 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187393928ee725f5b2093435f08e7974e030f5cebb4df9c65ef15a4acd5e9952`  
		Last Modified: Thu, 27 May 2021 18:53:09 GMT  
		Size: 36.7 MB (36661010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5404ac7d5e69bbc3cf976f7d3fe564d2f1f388d9a1200d9e991a4cd2cba1e51c`  
		Last Modified: Thu, 27 May 2021 18:53:00 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ed607ad3c36647ad714a1900e3712524ef36b4d2def06b147cf3af6fcdb4ae`  
		Last Modified: Thu, 27 May 2021 18:53:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7987082bd8043531ce033d1e8127167b9e0b28d8cac814d5ff4b70e318556943`  
		Last Modified: Thu, 27 May 2021 18:53:00 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.14` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:094d6c52657e088899e1d0ea8d956d32561f3efcbb6617404755ee1bbf5d194a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39546893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:911fdfb898ea5d7cdb531b99615a68eec104179258a03685ef677f482be7687b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Thu, 27 May 2021 22:02:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Thu, 27 May 2021 22:03:54 GMT
ARG CONSUL_VERSION=1.7.14
# Thu, 27 May 2021 22:03:54 GMT
LABEL org.opencontainers.image.version=1.7.14
# Thu, 27 May 2021 22:03:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 27 May 2021 22:03:55 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 27 May 2021 22:03:59 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 27 May 2021 22:04:00 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 27 May 2021 22:04:01 GMT
# ARGS: CONSUL_VERSION=1.7.14
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 27 May 2021 22:04:01 GMT
VOLUME [/consul/data]
# Thu, 27 May 2021 22:04:01 GMT
EXPOSE 8300
# Thu, 27 May 2021 22:04:02 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 27 May 2021 22:04:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 27 May 2021 22:04:02 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 27 May 2021 22:04:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 27 May 2021 22:04:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa0a158ae271fcd11844dba1dccf9979d4f6366d27c676f33c9a6598cbe5ef2`  
		Last Modified: Thu, 27 May 2021 22:05:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3b246eb81fd4e2bc713798b889332a2bd9a4339a6b7305ffa736aa583065e6`  
		Last Modified: Thu, 27 May 2021 22:05:34 GMT  
		Size: 36.8 MB (36832906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be52bed9e7cc30dc2b5240834c16088bd6f085f655b11a00d8f2a5b540139f6`  
		Last Modified: Thu, 27 May 2021 22:05:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903a2dda76301f0e3af98a369db6b272a2b2b3206a86a1c8641599f8434be41e`  
		Last Modified: Thu, 27 May 2021 22:05:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95eab3746c8b82bd4cb387dbfc822bfcaabc377d5e83b87e3a56a55140d7cac0`  
		Last Modified: Thu, 27 May 2021 22:05:29 GMT  
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
$ docker pull consul@sha256:1e34322bddfd6ed1a1123baaa21a775a21a9d47ecbe0bfd0643150da5a57dd5c
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
$ docker pull consul@sha256:72d77a67dd4708ceadf79815f287e82d2ac17df849ae317e13f15bb1dca587c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43013072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86b3a93918f3a3cd0aff1eb9cfb1cd7a669609472c5685be8375e870d5c969b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:50:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 20:49:39 GMT
ARG CONSUL_VERSION=1.8.12
# Mon, 14 Jun 2021 20:49:39 GMT
LABEL org.opencontainers.image.version=1.8.12
# Mon, 14 Jun 2021 20:49:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 20:49:40 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 20:49:47 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 20:49:48 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 20:49:49 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 20:49:49 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 20:49:49 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 20:49:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 20:49:50 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 20:49:50 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 20:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 20:49:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b047b6b4aecbc7dd8c979dee0de26c3857c4dafb7d47dd1ee380e2d9c35e80a7`  
		Last Modified: Mon, 14 Jun 2021 20:50:39 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c42e614fb3bf1dd6d2153b5156f28fa3646e9b88b237f1c771aca669daa0b47`  
		Last Modified: Mon, 14 Jun 2021 20:50:46 GMT  
		Size: 40.4 MB (40387647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88857bce8ee9d7249d8949f9bd5060e7b6df2ff50d81c762ff27c627beeb37c1`  
		Last Modified: Mon, 14 Jun 2021 20:50:38 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed3a469d0034b181cf4dd824384a7e01fd05f54b1ec4fb2cec3784274a334b`  
		Last Modified: Mon, 14 Jun 2021 20:50:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd99c0f7d1021f7f9e09a60ddbfa7b210e404af0e6605ad8bc430f76b09c8142`  
		Last Modified: Mon, 14 Jun 2021 20:50:39 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1ae4a063ed9a10e41683cc0a9e13a2ff2b9261d9b7dd9ddaa831d56595ee11be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43214816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1a27e0ea2c0fe8478be74253c230c8ac0358db19e00e4d96653a17d6a85784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:40:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 20:39:47 GMT
ARG CONSUL_VERSION=1.8.12
# Mon, 14 Jun 2021 20:39:48 GMT
LABEL org.opencontainers.image.version=1.8.12
# Mon, 14 Jun 2021 20:39:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 20:39:49 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 20:39:54 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 20:39:55 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 20:39:56 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 20:39:56 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 20:39:56 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 20:39:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 20:39:57 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 20:39:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 20:39:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 20:39:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596f17ce7ab96a4f249ab845245a5bdeb655cf79d7e78d527b5903501a66fd10`  
		Last Modified: Mon, 14 Jun 2021 20:40:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3936b6bb938cf9c30f85f0ad9f9c0934e7435bcc6889996412834e808643e8`  
		Last Modified: Mon, 14 Jun 2021 20:40:38 GMT  
		Size: 40.5 MB (40499498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bb67deb557068e62503e56501552da9737a41aaf0da8a0272ee3d8f8ad91e4`  
		Last Modified: Mon, 14 Jun 2021 20:40:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31d9ca2fe9364754d7845bdef0b7c42bf9fa0aae2aadea0ab19f5d5e66e0f2`  
		Last Modified: Mon, 14 Jun 2021 20:40:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4458b3107606c51c2f311a4a2a68e74dff33d36bed45d38ea8f35ca1eb5cdc7`  
		Last Modified: Mon, 14 Jun 2021 20:40:31 GMT  
		Size: 1.7 KB (1705 bytes)  
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
$ docker pull consul@sha256:1e34322bddfd6ed1a1123baaa21a775a21a9d47ecbe0bfd0643150da5a57dd5c
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
$ docker pull consul@sha256:72d77a67dd4708ceadf79815f287e82d2ac17df849ae317e13f15bb1dca587c8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43013072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86b3a93918f3a3cd0aff1eb9cfb1cd7a669609472c5685be8375e870d5c969b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:50:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 20:49:39 GMT
ARG CONSUL_VERSION=1.8.12
# Mon, 14 Jun 2021 20:49:39 GMT
LABEL org.opencontainers.image.version=1.8.12
# Mon, 14 Jun 2021 20:49:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 20:49:40 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 20:49:47 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 20:49:48 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 20:49:49 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 20:49:49 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 20:49:49 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 20:49:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 20:49:50 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 20:49:50 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 20:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 20:49:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b047b6b4aecbc7dd8c979dee0de26c3857c4dafb7d47dd1ee380e2d9c35e80a7`  
		Last Modified: Mon, 14 Jun 2021 20:50:39 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c42e614fb3bf1dd6d2153b5156f28fa3646e9b88b237f1c771aca669daa0b47`  
		Last Modified: Mon, 14 Jun 2021 20:50:46 GMT  
		Size: 40.4 MB (40387647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88857bce8ee9d7249d8949f9bd5060e7b6df2ff50d81c762ff27c627beeb37c1`  
		Last Modified: Mon, 14 Jun 2021 20:50:38 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ed3a469d0034b181cf4dd824384a7e01fd05f54b1ec4fb2cec3784274a334b`  
		Last Modified: Mon, 14 Jun 2021 20:50:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd99c0f7d1021f7f9e09a60ddbfa7b210e404af0e6605ad8bc430f76b09c8142`  
		Last Modified: Mon, 14 Jun 2021 20:50:39 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.12` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:1ae4a063ed9a10e41683cc0a9e13a2ff2b9261d9b7dd9ddaa831d56595ee11be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43214816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab1a27e0ea2c0fe8478be74253c230c8ac0358db19e00e4d96653a17d6a85784`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:40:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 20:39:47 GMT
ARG CONSUL_VERSION=1.8.12
# Mon, 14 Jun 2021 20:39:48 GMT
LABEL org.opencontainers.image.version=1.8.12
# Mon, 14 Jun 2021 20:39:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 20:39:49 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 20:39:54 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 20:39:55 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 20:39:56 GMT
# ARGS: CONSUL_VERSION=1.8.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 20:39:56 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 20:39:56 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 20:39:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 20:39:57 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 20:39:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 20:39:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 20:39:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596f17ce7ab96a4f249ab845245a5bdeb655cf79d7e78d527b5903501a66fd10`  
		Last Modified: Mon, 14 Jun 2021 20:40:31 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3936b6bb938cf9c30f85f0ad9f9c0934e7435bcc6889996412834e808643e8`  
		Last Modified: Mon, 14 Jun 2021 20:40:38 GMT  
		Size: 40.5 MB (40499498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bb67deb557068e62503e56501552da9737a41aaf0da8a0272ee3d8f8ad91e4`  
		Last Modified: Mon, 14 Jun 2021 20:40:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31d9ca2fe9364754d7845bdef0b7c42bf9fa0aae2aadea0ab19f5d5e66e0f2`  
		Last Modified: Mon, 14 Jun 2021 20:40:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4458b3107606c51c2f311a4a2a68e74dff33d36bed45d38ea8f35ca1eb5cdc7`  
		Last Modified: Mon, 14 Jun 2021 20:40:31 GMT  
		Size: 1.7 KB (1705 bytes)  
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
$ docker pull consul@sha256:a024930436e6830b2a00b8e8883df58ce76b92d28dccc8f9866d31ca799d79c3
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
$ docker pull consul@sha256:db5f5a20d64ea817c23a6139ed0144162c6ddc8d37d9de8cedb84643631dc32d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41468424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:740c869d081b44e4372647a3e889a12fc527f7dde54db6211357efc82cc1668c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:50:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 17:52:01 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 17:52:01 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 17:52:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 17:52:02 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 17:52:09 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 17:52:10 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 17:52:11 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:52:11 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 17:52:11 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 17:52:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 17:52:12 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 17:52:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 17:52:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 17:52:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e06d7f4fd30704db1b763dff4530f8f02b521191faddb0ec591355bce3d3d9`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185da06c12613adfabcb4fe797da489c20164ec1523b0e227ad860c107fea592`  
		Last Modified: Mon, 14 Jun 2021 17:53:25 GMT  
		Size: 38.8 MB (38842999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7a750e1b2dd60d53ce3ca7e723f0395663892da20a81756e17450471263869`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84afc802a043ee70b20bfa43670452461e35d6c19acedd177fefc10f88e2ba05`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edb52996b16a1615a1245ff077fce48823d2884b20366c218de6924852b51bb`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:41e0924e6fd81aa0edfe2ccd201aeb1e959b918247748787fc1d43a801032524
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41703997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5335b50edc1e06710efde802dac7a8550e4ec7a469db00612bef9f97ab0c97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:40:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 18:39:37 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 18:39:37 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 18:39:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 18:39:38 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 18:39:43 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 18:39:44 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 18:39:45 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:39:45 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 18:39:45 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 18:39:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 18:39:46 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 18:39:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 18:39:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8a953d0c87ecdf7fef98adb6cd0afd66b128aa3bec41ebb0fc7ba5de09a7a6`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f68cbfa95e128c51838b580ffa1f9638b62d08c5d305a3c0100f7b21921061`  
		Last Modified: Mon, 14 Jun 2021 18:40:38 GMT  
		Size: 39.0 MB (38988679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb9536818987cdfe4f9b2371b0c75b4ad09884d366fd9fb8a3e9037003a3810`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22379632c2d4676026ef63f1699ba03718fd34fb8ea0ee433b61fa44638cf34f`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402835d3a672cabe740f7a4ca3679efc021c2faba77ea717f723946a2af40b7`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 1.7 KB (1707 bytes)  
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
$ docker pull consul@sha256:a024930436e6830b2a00b8e8883df58ce76b92d28dccc8f9866d31ca799d79c3
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
$ docker pull consul@sha256:db5f5a20d64ea817c23a6139ed0144162c6ddc8d37d9de8cedb84643631dc32d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41468424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:740c869d081b44e4372647a3e889a12fc527f7dde54db6211357efc82cc1668c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:50:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 17:52:01 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 17:52:01 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 17:52:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 17:52:02 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 17:52:09 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 17:52:10 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 17:52:11 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:52:11 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 17:52:11 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 17:52:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 17:52:12 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 17:52:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 17:52:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 17:52:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e06d7f4fd30704db1b763dff4530f8f02b521191faddb0ec591355bce3d3d9`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185da06c12613adfabcb4fe797da489c20164ec1523b0e227ad860c107fea592`  
		Last Modified: Mon, 14 Jun 2021 17:53:25 GMT  
		Size: 38.8 MB (38842999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7a750e1b2dd60d53ce3ca7e723f0395663892da20a81756e17450471263869`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84afc802a043ee70b20bfa43670452461e35d6c19acedd177fefc10f88e2ba05`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edb52996b16a1615a1245ff077fce48823d2884b20366c218de6924852b51bb`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:41e0924e6fd81aa0edfe2ccd201aeb1e959b918247748787fc1d43a801032524
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41703997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5335b50edc1e06710efde802dac7a8550e4ec7a469db00612bef9f97ab0c97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:40:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 18:39:37 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 18:39:37 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 18:39:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 18:39:38 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 18:39:43 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 18:39:44 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 18:39:45 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:39:45 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 18:39:45 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 18:39:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 18:39:46 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 18:39:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 18:39:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8a953d0c87ecdf7fef98adb6cd0afd66b128aa3bec41ebb0fc7ba5de09a7a6`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f68cbfa95e128c51838b580ffa1f9638b62d08c5d305a3c0100f7b21921061`  
		Last Modified: Mon, 14 Jun 2021 18:40:38 GMT  
		Size: 39.0 MB (38988679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb9536818987cdfe4f9b2371b0c75b4ad09884d366fd9fb8a3e9037003a3810`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22379632c2d4676026ef63f1699ba03718fd34fb8ea0ee433b61fa44638cf34f`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402835d3a672cabe740f7a4ca3679efc021c2faba77ea717f723946a2af40b7`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 1.7 KB (1707 bytes)  
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
$ docker pull consul@sha256:a024930436e6830b2a00b8e8883df58ce76b92d28dccc8f9866d31ca799d79c3
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
$ docker pull consul@sha256:db5f5a20d64ea817c23a6139ed0144162c6ddc8d37d9de8cedb84643631dc32d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41468424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:740c869d081b44e4372647a3e889a12fc527f7dde54db6211357efc82cc1668c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:50:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 17:52:01 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 17:52:01 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 17:52:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 17:52:02 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 17:52:09 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 17:52:10 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 17:52:11 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 17:52:11 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 17:52:11 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 17:52:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 17:52:12 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 17:52:12 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 17:52:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 17:52:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e06d7f4fd30704db1b763dff4530f8f02b521191faddb0ec591355bce3d3d9`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185da06c12613adfabcb4fe797da489c20164ec1523b0e227ad860c107fea592`  
		Last Modified: Mon, 14 Jun 2021 17:53:25 GMT  
		Size: 38.8 MB (38842999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7a750e1b2dd60d53ce3ca7e723f0395663892da20a81756e17450471263869`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84afc802a043ee70b20bfa43670452461e35d6c19acedd177fefc10f88e2ba05`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edb52996b16a1615a1245ff077fce48823d2884b20366c218de6924852b51bb`  
		Last Modified: Mon, 14 Jun 2021 17:53:18 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:41e0924e6fd81aa0edfe2ccd201aeb1e959b918247748787fc1d43a801032524
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41703997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d5335b50edc1e06710efde802dac7a8550e4ec7a469db00612bef9f97ab0c97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 10 Jun 2021 17:40:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Mon, 14 Jun 2021 18:39:37 GMT
ARG CONSUL_VERSION=1.9.6
# Mon, 14 Jun 2021 18:39:37 GMT
LABEL org.opencontainers.image.version=1.9.6
# Mon, 14 Jun 2021 18:39:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 14 Jun 2021 18:39:38 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 14 Jun 2021 18:39:43 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver pool.sks-keyservers.net --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 14 Jun 2021 18:39:44 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 14 Jun 2021 18:39:45 GMT
# ARGS: CONSUL_VERSION=1.9.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 14 Jun 2021 18:39:45 GMT
VOLUME [/consul/data]
# Mon, 14 Jun 2021 18:39:45 GMT
EXPOSE 8300
# Mon, 14 Jun 2021 18:39:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 14 Jun 2021 18:39:46 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 14 Jun 2021 18:39:46 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 14 Jun 2021 18:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Jun 2021 18:39:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8a953d0c87ecdf7fef98adb6cd0afd66b128aa3bec41ebb0fc7ba5de09a7a6`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f68cbfa95e128c51838b580ffa1f9638b62d08c5d305a3c0100f7b21921061`  
		Last Modified: Mon, 14 Jun 2021 18:40:38 GMT  
		Size: 39.0 MB (38988679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb9536818987cdfe4f9b2371b0c75b4ad09884d366fd9fb8a3e9037003a3810`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22379632c2d4676026ef63f1699ba03718fd34fb8ea0ee433b61fa44638cf34f`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6402835d3a672cabe740f7a4ca3679efc021c2faba77ea717f723946a2af40b7`  
		Last Modified: Mon, 14 Jun 2021 18:40:32 GMT  
		Size: 1.7 KB (1707 bytes)  
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
