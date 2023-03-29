<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.13`](#consul113)
-	[`consul:1.13.7`](#consul1137)
-	[`consul:1.14`](#consul114)
-	[`consul:1.14.5`](#consul1145)
-	[`consul:1.15`](#consul115)
-	[`consul:1.15.1`](#consul1151)
-	[`consul:latest`](#consullatest)

## `consul:1.13`

```console
$ docker pull consul@sha256:2c71456a4a8abd2bec591c479986462dec43f08bd93c99062c41b1916818aa76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13` - linux; amd64

```console
$ docker pull consul@sha256:5b9361b393da3351011c1cf5ac641ed73f5e1c3c3582be354fb8bbba850d1151
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53291737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae60bfb5a07c2f8c6df37d23b3ce2ecace55af69dc3d519a496a64be4b0461e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 20:19:47 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 08 Mar 2023 20:19:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 20:19:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 20:19:48 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 20:19:53 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 20:19:54 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 20:19:55 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 20:19:55 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 20:19:55 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 20:19:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 20:19:55 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 20:19:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 20:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:19:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8b8cc5c40b552642e1177764724215992d29f51c8048013b08dddd2a2ce03f`  
		Last Modified: Wed, 08 Mar 2023 20:20:43 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1083301f4de49afe86996a746b6ed5d1747bd44281f2ca7a85560fd3a2157a8`  
		Last Modified: Wed, 08 Mar 2023 20:20:49 GMT  
		Size: 50.5 MB (50462210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5ec5917610d493798e806edb86755dfd4ee8f48570ae9ed0072634e1e4f0b1`  
		Last Modified: Wed, 08 Mar 2023 20:20:43 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc631ce71b9a1b1b569cc524b404757b024da2476af61f225e419f91455efea4`  
		Last Modified: Wed, 08 Mar 2023 20:20:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d5f891708b436d200c27a13df77f21ac6ba33c3408ca60ecd7a5ae61a0ef1`  
		Last Modified: Wed, 08 Mar 2023 20:20:43 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm variant v6

```console
$ docker pull consul@sha256:18ae376ea91c00ad0338a270b3e311d118818c17ead079dcfc15e0373f0f8311
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50498862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f895a19bbf67d8448f12bf7ac7505d85d341fa53fd4ef36992215394b95d1d5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:41:36 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 29 Mar 2023 18:41:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 18:41:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 18:41:37 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 18:41:44 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 18:41:45 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 18:41:45 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 18:41:45 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 18:41:46 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 18:41:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 18:41:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 18:41:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 18:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:41:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0b2592e24b3be9e300665f22ab3411c541c718233566d1b5f2a2bc19e4c5e5`  
		Last Modified: Wed, 29 Mar 2023 18:43:49 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda52e7c6a75316bc9156fff7291f69837269a4a2d4c66473e0b9df9ef33be57`  
		Last Modified: Wed, 29 Mar 2023 18:43:56 GMT  
		Size: 47.9 MB (47861457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772fd3b0ef6ac173e35e8f16d6e4f71cc96e8f7e959c625ed8989b1e6cf55f70`  
		Last Modified: Wed, 29 Mar 2023 18:43:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50010f1739ef67adf1cba58b77155509ed869836c74f22c2521dc5e61aa6fd55`  
		Last Modified: Wed, 29 Mar 2023 18:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6128ec50a67f7ca19f625924a2879d69a0a7b4802839b116a16bf62155853cf`  
		Last Modified: Wed, 29 Mar 2023 18:43:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:161a2dcd6e59f2f40e1ab708ade03b889bc5e22a8704b58b648222e48b313046
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50318287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af82e1b38341040f91298b806e2f9981f963e2010fca27cd167fd689daa93201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 21:00:38 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 08 Mar 2023 21:00:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 21:00:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 21:00:38 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 21:00:44 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 21:00:45 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 21:00:45 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 21:00:45 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 21:00:45 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 21:00:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 21:00:45 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 21:00:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 21:00:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:00:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58a80420cf5c74a9caee107369b8dec866d22ad13d2cea4eeba3f40605c28b5`  
		Last Modified: Wed, 08 Mar 2023 21:01:30 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9104cbe854e2af35f7c0143e4dc10fe6bb831a6fb8ddec816a60bd187c898e47`  
		Last Modified: Wed, 08 Mar 2023 21:01:35 GMT  
		Size: 47.6 MB (47593347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481f404760a15e46e62b836f31d199b1d4b701a6458498f88929530595cd3091`  
		Last Modified: Wed, 08 Mar 2023 21:01:30 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098ca5cf8acd019ab18dc68cb1771b2fea009325d3a62486e3221d7966b775f7`  
		Last Modified: Wed, 08 Mar 2023 21:01:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58de25f71530889047992d638c12b82e820829c975e28369ac1776d04dd3d87`  
		Last Modified: Wed, 08 Mar 2023 21:01:30 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; 386

```console
$ docker pull consul@sha256:9f3b76508e936a08d608e52f4c001302cdaa5089eeaa6e346bbcc08c5936979a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51845585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f61e56e657f468617356272c7d1264eb027cf099f18a6de69458658ef750d7a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:55:15 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 29 Mar 2023 17:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 17:55:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 17:55:16 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 17:55:23 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 17:55:24 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 17:55:24 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 17:55:25 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 17:55:25 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 17:55:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 17:55:25 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 17:55:25 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 17:55:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 17:55:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44607ec662b885643c2675d6478696eb68908eb5f2cf48ac274a2be58de74ac4`  
		Last Modified: Wed, 29 Mar 2023 17:56:10 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a22ab1e0d92c068ad8cabbae69b28802e9f3c25eccfa9ebbe196517402d6fb`  
		Last Modified: Wed, 29 Mar 2023 17:56:18 GMT  
		Size: 49.0 MB (49009631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a561661dbf49b998eedcc0980686ea0b869df7cf9740f07bddec87ea76b2354`  
		Last Modified: Wed, 29 Mar 2023 17:56:10 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f58f5a48673af836ac1b265f9d3d6c81c4a6bf7f49db89d1385838e602a2a55`  
		Last Modified: Wed, 29 Mar 2023 17:56:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06fd9bfa1669b95e138803b6901d88e2bbe71a6f32c76d7685faab3f2210b38`  
		Last Modified: Wed, 29 Mar 2023 17:56:10 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.13.7`

```console
$ docker pull consul@sha256:2c71456a4a8abd2bec591c479986462dec43f08bd93c99062c41b1916818aa76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13.7` - linux; amd64

```console
$ docker pull consul@sha256:5b9361b393da3351011c1cf5ac641ed73f5e1c3c3582be354fb8bbba850d1151
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53291737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae60bfb5a07c2f8c6df37d23b3ce2ecace55af69dc3d519a496a64be4b0461e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 20:19:47 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 08 Mar 2023 20:19:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 20:19:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 20:19:48 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 20:19:53 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 20:19:54 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 20:19:55 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 20:19:55 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 20:19:55 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 20:19:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 20:19:55 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 20:19:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 20:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:19:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8b8cc5c40b552642e1177764724215992d29f51c8048013b08dddd2a2ce03f`  
		Last Modified: Wed, 08 Mar 2023 20:20:43 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1083301f4de49afe86996a746b6ed5d1747bd44281f2ca7a85560fd3a2157a8`  
		Last Modified: Wed, 08 Mar 2023 20:20:49 GMT  
		Size: 50.5 MB (50462210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5ec5917610d493798e806edb86755dfd4ee8f48570ae9ed0072634e1e4f0b1`  
		Last Modified: Wed, 08 Mar 2023 20:20:43 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc631ce71b9a1b1b569cc524b404757b024da2476af61f225e419f91455efea4`  
		Last Modified: Wed, 08 Mar 2023 20:20:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716d5f891708b436d200c27a13df77f21ac6ba33c3408ca60ecd7a5ae61a0ef1`  
		Last Modified: Wed, 08 Mar 2023 20:20:43 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:18ae376ea91c00ad0338a270b3e311d118818c17ead079dcfc15e0373f0f8311
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50498862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f895a19bbf67d8448f12bf7ac7505d85d341fa53fd4ef36992215394b95d1d5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:41:36 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 29 Mar 2023 18:41:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 18:41:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 18:41:37 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 18:41:44 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 18:41:45 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 18:41:45 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 18:41:45 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 18:41:46 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 18:41:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 18:41:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 18:41:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 18:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:41:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0b2592e24b3be9e300665f22ab3411c541c718233566d1b5f2a2bc19e4c5e5`  
		Last Modified: Wed, 29 Mar 2023 18:43:49 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda52e7c6a75316bc9156fff7291f69837269a4a2d4c66473e0b9df9ef33be57`  
		Last Modified: Wed, 29 Mar 2023 18:43:56 GMT  
		Size: 47.9 MB (47861457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772fd3b0ef6ac173e35e8f16d6e4f71cc96e8f7e959c625ed8989b1e6cf55f70`  
		Last Modified: Wed, 29 Mar 2023 18:43:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50010f1739ef67adf1cba58b77155509ed869836c74f22c2521dc5e61aa6fd55`  
		Last Modified: Wed, 29 Mar 2023 18:43:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6128ec50a67f7ca19f625924a2879d69a0a7b4802839b116a16bf62155853cf`  
		Last Modified: Wed, 29 Mar 2023 18:43:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:161a2dcd6e59f2f40e1ab708ade03b889bc5e22a8704b58b648222e48b313046
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50318287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af82e1b38341040f91298b806e2f9981f963e2010fca27cd167fd689daa93201`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 21:00:38 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 08 Mar 2023 21:00:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 21:00:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 21:00:38 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 21:00:44 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 21:00:45 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 21:00:45 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 21:00:45 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 21:00:45 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 21:00:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 21:00:45 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 21:00:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 21:00:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:00:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58a80420cf5c74a9caee107369b8dec866d22ad13d2cea4eeba3f40605c28b5`  
		Last Modified: Wed, 08 Mar 2023 21:01:30 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9104cbe854e2af35f7c0143e4dc10fe6bb831a6fb8ddec816a60bd187c898e47`  
		Last Modified: Wed, 08 Mar 2023 21:01:35 GMT  
		Size: 47.6 MB (47593347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481f404760a15e46e62b836f31d199b1d4b701a6458498f88929530595cd3091`  
		Last Modified: Wed, 08 Mar 2023 21:01:30 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098ca5cf8acd019ab18dc68cb1771b2fea009325d3a62486e3221d7966b775f7`  
		Last Modified: Wed, 08 Mar 2023 21:01:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58de25f71530889047992d638c12b82e820829c975e28369ac1776d04dd3d87`  
		Last Modified: Wed, 08 Mar 2023 21:01:30 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.7` - linux; 386

```console
$ docker pull consul@sha256:9f3b76508e936a08d608e52f4c001302cdaa5089eeaa6e346bbcc08c5936979a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51845585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f61e56e657f468617356272c7d1264eb027cf099f18a6de69458658ef750d7a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:55:15 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 29 Mar 2023 17:55:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 17:55:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 17:55:16 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 17:55:23 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 17:55:24 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 17:55:24 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 17:55:25 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 17:55:25 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 17:55:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 17:55:25 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 17:55:25 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 17:55:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 17:55:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44607ec662b885643c2675d6478696eb68908eb5f2cf48ac274a2be58de74ac4`  
		Last Modified: Wed, 29 Mar 2023 17:56:10 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a22ab1e0d92c068ad8cabbae69b28802e9f3c25eccfa9ebbe196517402d6fb`  
		Last Modified: Wed, 29 Mar 2023 17:56:18 GMT  
		Size: 49.0 MB (49009631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a561661dbf49b998eedcc0980686ea0b869df7cf9740f07bddec87ea76b2354`  
		Last Modified: Wed, 29 Mar 2023 17:56:10 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f58f5a48673af836ac1b265f9d3d6c81c4a6bf7f49db89d1385838e602a2a55`  
		Last Modified: Wed, 29 Mar 2023 17:56:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06fd9bfa1669b95e138803b6901d88e2bbe71a6f32c76d7685faab3f2210b38`  
		Last Modified: Wed, 29 Mar 2023 17:56:10 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.14`

```console
$ docker pull consul@sha256:48bf3881b55d4f4cab9d36c372be9e2bd3c456ea72b0df7499df049c94e2356c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14` - linux; amd64

```console
$ docker pull consul@sha256:8415ab45a41257e7c8c418b1038153dadcb47c5b9b42667769ceadf2a0b1272c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56666903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70cd4645097b0545876aeb9b85747095f94ccb36f2995e2a6d54724f51cb942`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 20:19:35 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 08 Mar 2023 20:19:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 20:19:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 20:19:35 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 20:19:41 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 20:19:42 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 20:19:43 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 20:19:43 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 20:19:43 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 20:19:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 20:19:43 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 20:19:43 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 20:19:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:19:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad75a06f1e677cbc90e1e5c39b4adc2410e0bd5140e89d1ffdf8071b851c169c`  
		Last Modified: Wed, 08 Mar 2023 20:20:27 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389e75d0c16957e3e40cdaa5131ee091427381d01f99c238cb2c9134b409c0e3`  
		Last Modified: Wed, 08 Mar 2023 20:20:34 GMT  
		Size: 53.8 MB (53837377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf7586f44ba4cbeb1c0534aea0c5d9ece3d7f4360d6da70f89a5d13a2a99513`  
		Last Modified: Wed, 08 Mar 2023 20:20:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869b4a2e30aeb9a5c3855dfda392335c522dda72f7a06044496a8116c005337`  
		Last Modified: Wed, 08 Mar 2023 20:20:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05c9afe8d61071314ddf3ad528f18726a242849588cab758c126487ac2b60db`  
		Last Modified: Wed, 08 Mar 2023 20:20:27 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; arm variant v6

```console
$ docker pull consul@sha256:194f394fbf59963423ded6520bc93ec06103babfc7ff36a644f93d5021b4cf0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53551942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30a317f26c9042fb64989f32c2896603746df798027dacb98eb5b6a6198f3611`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:41:23 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 29 Mar 2023 18:41:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 18:41:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 18:41:24 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 18:41:31 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 18:41:32 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 18:41:33 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 18:41:33 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 18:41:33 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 18:41:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 18:41:33 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 18:41:33 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 18:41:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:41:33 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e69276520683dae8912f6e5d5856d79737484eec3b4267512ded615e975a27`  
		Last Modified: Wed, 29 Mar 2023 18:43:32 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9420665cdb62f9e16e46cee4917b00b480a00b8206e05925bf8cdcae2d3da58f`  
		Last Modified: Wed, 29 Mar 2023 18:43:39 GMT  
		Size: 50.9 MB (50914536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42839a80927f1f443fef7d98483c4f378cf06c3bcaeb52b9a6879ccfcd91eb8`  
		Last Modified: Wed, 29 Mar 2023 18:43:32 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72759dccce3c62183f079a0cb6e2553c4ad7f1e3f363030f3cf72461e8acaa3f`  
		Last Modified: Wed, 29 Mar 2023 18:43:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cd000a0062aeed66c7ed77f73b2ac86d08bcfe2f97ae34fa7631eadafca838`  
		Last Modified: Wed, 29 Mar 2023 18:43:32 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:7a7da457d8c4e63b7dce4a04d1b1c58c3af2df6d01a6531b632c9a3b63a21f69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53486549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1cbb332e7a8eba6552fd905f441503ae81d3034ec7cd3ac79f45d7cb46a41f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 21:00:26 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 08 Mar 2023 21:00:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 21:00:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 21:00:27 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 21:00:33 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 21:00:34 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 21:00:34 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 21:00:34 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 21:00:34 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 21:00:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 21:00:34 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 21:00:34 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 21:00:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:00:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f514b4855693bd18d4cebdacb895badac8ae685c419bcef69690f9863aa0e`  
		Last Modified: Wed, 08 Mar 2023 21:01:16 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7a32c3d115e45983f6b9d0fd2b16a80fc9cca1b7b0977952b487bedede6052`  
		Last Modified: Wed, 08 Mar 2023 21:01:21 GMT  
		Size: 50.8 MB (50761610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64146d08c0153554c653e6c7cc44ed8b80554ca83e582f30d7cd099aacfcf39`  
		Last Modified: Wed, 08 Mar 2023 21:01:16 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1572a092c4ad6e70cf8847ab3667967d934981d6438cc85fdfc5f00f0ef0a159`  
		Last Modified: Wed, 08 Mar 2023 21:01:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a461b73022d71e9260249d8565f2523f0758f69de1796ea4b56e399259840b96`  
		Last Modified: Wed, 08 Mar 2023 21:01:16 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; 386

```console
$ docker pull consul@sha256:fa7ed691de4fab1e9e3b51cd3e61c8bfc49be7ca8fe1fb1db8a66afa66f0b60e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54934126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a2fe95739d1cba6695f4d10b0feec99e5077675b6ae9cfe45e1f763aa09e858`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:55:02 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 29 Mar 2023 17:55:02 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 17:55:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 17:55:03 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 17:55:10 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 17:55:11 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 17:55:11 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 17:55:11 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 17:55:11 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 17:55:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 17:55:12 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 17:55:12 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 17:55:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 17:55:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae91f4c42486c7c4ddefd5e222e015119d1ee672413dd1ac7a1431c13c027d4f`  
		Last Modified: Wed, 29 Mar 2023 17:55:54 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b897029b6b4b9e7470c065b492cc5922632f0b592fd69d34f3ed3fde9e33f5`  
		Last Modified: Wed, 29 Mar 2023 17:56:02 GMT  
		Size: 52.1 MB (52098179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcffe1728ce4311f650cf443b8dad3c127a8732f2a1a2ca24cc0867d0e09dbd`  
		Last Modified: Wed, 29 Mar 2023 17:55:54 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97b12213bd61199b8b47bbdafcc59604f418471a1db82718f8aade1c0d6a3d5`  
		Last Modified: Wed, 29 Mar 2023 17:55:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51a3f5809412c87cd85f543de3e3b4ed87ae3e24f54328ed45d6b6db4dc747c`  
		Last Modified: Wed, 29 Mar 2023 17:55:54 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.14.5`

```console
$ docker pull consul@sha256:48bf3881b55d4f4cab9d36c372be9e2bd3c456ea72b0df7499df049c94e2356c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14.5` - linux; amd64

```console
$ docker pull consul@sha256:8415ab45a41257e7c8c418b1038153dadcb47c5b9b42667769ceadf2a0b1272c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56666903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e70cd4645097b0545876aeb9b85747095f94ccb36f2995e2a6d54724f51cb942`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 20:19:35 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 08 Mar 2023 20:19:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 20:19:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 20:19:35 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 20:19:41 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 20:19:42 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 20:19:43 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 20:19:43 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 20:19:43 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 20:19:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 20:19:43 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 20:19:43 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 20:19:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:19:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad75a06f1e677cbc90e1e5c39b4adc2410e0bd5140e89d1ffdf8071b851c169c`  
		Last Modified: Wed, 08 Mar 2023 20:20:27 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389e75d0c16957e3e40cdaa5131ee091427381d01f99c238cb2c9134b409c0e3`  
		Last Modified: Wed, 08 Mar 2023 20:20:34 GMT  
		Size: 53.8 MB (53837377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf7586f44ba4cbeb1c0534aea0c5d9ece3d7f4360d6da70f89a5d13a2a99513`  
		Last Modified: Wed, 08 Mar 2023 20:20:27 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f869b4a2e30aeb9a5c3855dfda392335c522dda72f7a06044496a8116c005337`  
		Last Modified: Wed, 08 Mar 2023 20:20:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d05c9afe8d61071314ddf3ad528f18726a242849588cab758c126487ac2b60db`  
		Last Modified: Wed, 08 Mar 2023 20:20:27 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.5` - linux; arm variant v6

```console
$ docker pull consul@sha256:194f394fbf59963423ded6520bc93ec06103babfc7ff36a644f93d5021b4cf0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53551942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30a317f26c9042fb64989f32c2896603746df798027dacb98eb5b6a6198f3611`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:41:23 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 29 Mar 2023 18:41:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 18:41:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 18:41:24 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 18:41:31 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 18:41:32 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 18:41:33 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 18:41:33 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 18:41:33 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 18:41:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 18:41:33 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 18:41:33 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 18:41:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:41:33 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e69276520683dae8912f6e5d5856d79737484eec3b4267512ded615e975a27`  
		Last Modified: Wed, 29 Mar 2023 18:43:32 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9420665cdb62f9e16e46cee4917b00b480a00b8206e05925bf8cdcae2d3da58f`  
		Last Modified: Wed, 29 Mar 2023 18:43:39 GMT  
		Size: 50.9 MB (50914536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42839a80927f1f443fef7d98483c4f378cf06c3bcaeb52b9a6879ccfcd91eb8`  
		Last Modified: Wed, 29 Mar 2023 18:43:32 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72759dccce3c62183f079a0cb6e2553c4ad7f1e3f363030f3cf72461e8acaa3f`  
		Last Modified: Wed, 29 Mar 2023 18:43:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cd000a0062aeed66c7ed77f73b2ac86d08bcfe2f97ae34fa7631eadafca838`  
		Last Modified: Wed, 29 Mar 2023 18:43:32 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.5` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:7a7da457d8c4e63b7dce4a04d1b1c58c3af2df6d01a6531b632c9a3b63a21f69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53486549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1cbb332e7a8eba6552fd905f441503ae81d3034ec7cd3ac79f45d7cb46a41f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 21:00:26 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 08 Mar 2023 21:00:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 21:00:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 21:00:27 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 21:00:33 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 21:00:34 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 21:00:34 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 21:00:34 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 21:00:34 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 21:00:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 21:00:34 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 21:00:34 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 21:00:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:00:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0f514b4855693bd18d4cebdacb895badac8ae685c419bcef69690f9863aa0e`  
		Last Modified: Wed, 08 Mar 2023 21:01:16 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7a32c3d115e45983f6b9d0fd2b16a80fc9cca1b7b0977952b487bedede6052`  
		Last Modified: Wed, 08 Mar 2023 21:01:21 GMT  
		Size: 50.8 MB (50761610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64146d08c0153554c653e6c7cc44ed8b80554ca83e582f30d7cd099aacfcf39`  
		Last Modified: Wed, 08 Mar 2023 21:01:16 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1572a092c4ad6e70cf8847ab3667967d934981d6438cc85fdfc5f00f0ef0a159`  
		Last Modified: Wed, 08 Mar 2023 21:01:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a461b73022d71e9260249d8565f2523f0758f69de1796ea4b56e399259840b96`  
		Last Modified: Wed, 08 Mar 2023 21:01:16 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.5` - linux; 386

```console
$ docker pull consul@sha256:fa7ed691de4fab1e9e3b51cd3e61c8bfc49be7ca8fe1fb1db8a66afa66f0b60e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54934126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a2fe95739d1cba6695f4d10b0feec99e5077675b6ae9cfe45e1f763aa09e858`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:55:02 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 29 Mar 2023 17:55:02 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 17:55:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 17:55:03 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 17:55:10 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 17:55:11 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 17:55:11 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 17:55:11 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 17:55:11 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 17:55:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 17:55:12 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 17:55:12 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 17:55:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 17:55:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae91f4c42486c7c4ddefd5e222e015119d1ee672413dd1ac7a1431c13c027d4f`  
		Last Modified: Wed, 29 Mar 2023 17:55:54 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b897029b6b4b9e7470c065b492cc5922632f0b592fd69d34f3ed3fde9e33f5`  
		Last Modified: Wed, 29 Mar 2023 17:56:02 GMT  
		Size: 52.1 MB (52098179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcffe1728ce4311f650cf443b8dad3c127a8732f2a1a2ca24cc0867d0e09dbd`  
		Last Modified: Wed, 29 Mar 2023 17:55:54 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97b12213bd61199b8b47bbdafcc59604f418471a1db82718f8aade1c0d6a3d5`  
		Last Modified: Wed, 29 Mar 2023 17:55:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51a3f5809412c87cd85f543de3e3b4ed87ae3e24f54328ed45d6b6db4dc747c`  
		Last Modified: Wed, 29 Mar 2023 17:55:54 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.15`

```console
$ docker pull consul@sha256:13f97c23ed3dde89682f32dafe1031b337b4e019b08ab09aabce08c51b982814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.15` - linux; amd64

```console
$ docker pull consul@sha256:bbfb7272cb73ee3e4ef83fe62af90e3107ba8a25093370f01c04084ae245e074
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58254124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abeb15b9ddc0e40def7b19f8d3ce62b59b01b91eab2842c688806ce07b56a0f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 20:19:23 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 08 Mar 2023 20:19:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 20:19:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 20:19:23 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 20:19:30 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 20:19:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 20:19:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 20:19:32 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 20:19:32 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 20:19:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 20:19:32 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 20:19:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 20:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:19:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b324295dd03a6cf331d4a02cb36bbf8f6ed3f70b953ae2369ef38e779c1dd4`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba21ab1eb9f525edf01d247d3669250181c5376548d9a99f5bd660d772356d1`  
		Last Modified: Wed, 08 Mar 2023 20:20:16 GMT  
		Size: 55.4 MB (55424594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c08861b7dc52dbd6fbf691d23c917df82d0e1f88390a333e71405feffb1d9d4`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c643221233c30d8734b65af733908793c5c1a8a086ab97e153cded745bccf9`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe56612bde98b5cde4e35d27483c06c3802d8da573ddbcb5d26b3f27d1c0658f`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15` - linux; arm variant v6

```console
$ docker pull consul@sha256:075097bc2cf3b615a6755fdbdd8221de516d0066165200df7cea0a6c859d8550
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55056765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4027e762e66883974a7d197877878b691518068a44e533f95079b0a2c501bbe8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:41:06 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 29 Mar 2023 18:41:06 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 18:41:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 18:41:07 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 18:41:19 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 18:41:19 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 18:41:20 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 18:41:20 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 18:41:20 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 18:41:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 18:41:20 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 18:41:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 18:41:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:41:20 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f943ab582225f789f8df5e20ea50348b40ca976ae39c1fe34d64ee41f5de5f0d`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e5ae6cb32e435e094a2636243064561de2a0a53c0b828315b63736447f62d6`  
		Last Modified: Wed, 29 Mar 2023 18:43:22 GMT  
		Size: 52.4 MB (52419359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02107783537cd9f076d338ec3f67d7de3aac478c07b428d59fb043eaf9a9f681`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87747cd79f988871c3d04cf1c1b5a59035e676663fc1e67820a2a99beb7c6ec6`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72c2e7cf99c21075babc33ceeda3f2335e5154ee6d7038844451872d4fd6c49`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:662987b59763ef83e15863408a15b51ce4efca13bc73c91e0bcc2b0426147241
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54977469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c61e12fa6c77dfe8b52e98a4a7632d9bdee3c5388a49df3ab325a477a0186df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 21:00:15 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 08 Mar 2023 21:00:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 21:00:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 21:00:16 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 21:00:21 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 21:00:22 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 21:00:23 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 21:00:23 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 21:00:23 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 21:00:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 21:00:23 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 21:00:23 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 21:00:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:00:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7157d90cce1f088fbba9c907768f5945710afc3bb84150de3cb59c5d00978d`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65f55c5f2684ce00b7624b63f988feeefb701328e817165a13822ebcf77512c`  
		Last Modified: Wed, 08 Mar 2023 21:01:05 GMT  
		Size: 52.3 MB (52252533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88b7623eb2f729eda24846a44d7dab5fa9aadd218d51457846d49cda56ade2e`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f277283afb0270bbf32ee345a025b907d5600f2a57d75fcded51c30bfc95563a`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21afe3f708be7aceac151a8a44180deb00009e6bb2125f1732122b39371c4a0d`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15` - linux; 386

```console
$ docker pull consul@sha256:3cd77af99b0165e0164a77ccad690bfe1e04011e08176bd3fd373b7bee63105d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56473907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5334ec6e01f45142db2942cd847241440b0fc3958b810ca341f199fef4db8959`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:54:43 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 29 Mar 2023 17:54:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 17:54:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 17:54:43 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 17:54:56 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 17:54:57 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 17:54:57 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 17:54:57 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 17:54:58 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 17:54:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 17:54:58 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 17:54:58 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 17:54:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 17:54:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b13556e68f2b9c9adb9cd02a8cf1df9e58f2cd6d81df25181c67be1d1a3c20`  
		Last Modified: Wed, 29 Mar 2023 17:55:36 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641d086a647f9ff43dcd02f5ad85442f927600b6bf102486b8c2401453cb1f8a`  
		Last Modified: Wed, 29 Mar 2023 17:55:44 GMT  
		Size: 53.6 MB (53637960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f012612a86102a2f0a2d613722b1817be563a199bd7ba1f3ab7364ed6ff2d92`  
		Last Modified: Wed, 29 Mar 2023 17:55:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3385843be8b35c1162a966477a35aa41b7b437253ae18dbebd0990b986f7cd8`  
		Last Modified: Wed, 29 Mar 2023 17:55:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3dd6230007d9ece7ef3ae146d9db2764ceea2c02d791a9b387b9bd7625615e`  
		Last Modified: Wed, 29 Mar 2023 17:55:36 GMT  
		Size: 1.8 KB (1779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.15.1`

```console
$ docker pull consul@sha256:13f97c23ed3dde89682f32dafe1031b337b4e019b08ab09aabce08c51b982814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.15.1` - linux; amd64

```console
$ docker pull consul@sha256:bbfb7272cb73ee3e4ef83fe62af90e3107ba8a25093370f01c04084ae245e074
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58254124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abeb15b9ddc0e40def7b19f8d3ce62b59b01b91eab2842c688806ce07b56a0f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 20:19:23 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 08 Mar 2023 20:19:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 20:19:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 20:19:23 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 20:19:30 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 20:19:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 20:19:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 20:19:32 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 20:19:32 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 20:19:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 20:19:32 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 20:19:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 20:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:19:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b324295dd03a6cf331d4a02cb36bbf8f6ed3f70b953ae2369ef38e779c1dd4`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba21ab1eb9f525edf01d247d3669250181c5376548d9a99f5bd660d772356d1`  
		Last Modified: Wed, 08 Mar 2023 20:20:16 GMT  
		Size: 55.4 MB (55424594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c08861b7dc52dbd6fbf691d23c917df82d0e1f88390a333e71405feffb1d9d4`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c643221233c30d8734b65af733908793c5c1a8a086ab97e153cded745bccf9`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe56612bde98b5cde4e35d27483c06c3802d8da573ddbcb5d26b3f27d1c0658f`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:075097bc2cf3b615a6755fdbdd8221de516d0066165200df7cea0a6c859d8550
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55056765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4027e762e66883974a7d197877878b691518068a44e533f95079b0a2c501bbe8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:41:06 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 29 Mar 2023 18:41:06 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 18:41:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 18:41:07 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 18:41:19 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 18:41:19 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 18:41:20 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 18:41:20 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 18:41:20 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 18:41:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 18:41:20 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 18:41:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 18:41:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:41:20 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f943ab582225f789f8df5e20ea50348b40ca976ae39c1fe34d64ee41f5de5f0d`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e5ae6cb32e435e094a2636243064561de2a0a53c0b828315b63736447f62d6`  
		Last Modified: Wed, 29 Mar 2023 18:43:22 GMT  
		Size: 52.4 MB (52419359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02107783537cd9f076d338ec3f67d7de3aac478c07b428d59fb043eaf9a9f681`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87747cd79f988871c3d04cf1c1b5a59035e676663fc1e67820a2a99beb7c6ec6`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72c2e7cf99c21075babc33ceeda3f2335e5154ee6d7038844451872d4fd6c49`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15.1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:662987b59763ef83e15863408a15b51ce4efca13bc73c91e0bcc2b0426147241
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54977469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c61e12fa6c77dfe8b52e98a4a7632d9bdee3c5388a49df3ab325a477a0186df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 21:00:15 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 08 Mar 2023 21:00:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 21:00:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 21:00:16 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 21:00:21 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 21:00:22 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 21:00:23 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 21:00:23 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 21:00:23 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 21:00:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 21:00:23 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 21:00:23 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 21:00:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:00:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7157d90cce1f088fbba9c907768f5945710afc3bb84150de3cb59c5d00978d`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65f55c5f2684ce00b7624b63f988feeefb701328e817165a13822ebcf77512c`  
		Last Modified: Wed, 08 Mar 2023 21:01:05 GMT  
		Size: 52.3 MB (52252533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88b7623eb2f729eda24846a44d7dab5fa9aadd218d51457846d49cda56ade2e`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f277283afb0270bbf32ee345a025b907d5600f2a57d75fcded51c30bfc95563a`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21afe3f708be7aceac151a8a44180deb00009e6bb2125f1732122b39371c4a0d`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15.1` - linux; 386

```console
$ docker pull consul@sha256:3cd77af99b0165e0164a77ccad690bfe1e04011e08176bd3fd373b7bee63105d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56473907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5334ec6e01f45142db2942cd847241440b0fc3958b810ca341f199fef4db8959`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:54:43 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 29 Mar 2023 17:54:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 17:54:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 17:54:43 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 17:54:56 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 17:54:57 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 17:54:57 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 17:54:57 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 17:54:58 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 17:54:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 17:54:58 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 17:54:58 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 17:54:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 17:54:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b13556e68f2b9c9adb9cd02a8cf1df9e58f2cd6d81df25181c67be1d1a3c20`  
		Last Modified: Wed, 29 Mar 2023 17:55:36 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641d086a647f9ff43dcd02f5ad85442f927600b6bf102486b8c2401453cb1f8a`  
		Last Modified: Wed, 29 Mar 2023 17:55:44 GMT  
		Size: 53.6 MB (53637960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f012612a86102a2f0a2d613722b1817be563a199bd7ba1f3ab7364ed6ff2d92`  
		Last Modified: Wed, 29 Mar 2023 17:55:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3385843be8b35c1162a966477a35aa41b7b437253ae18dbebd0990b986f7cd8`  
		Last Modified: Wed, 29 Mar 2023 17:55:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3dd6230007d9ece7ef3ae146d9db2764ceea2c02d791a9b387b9bd7625615e`  
		Last Modified: Wed, 29 Mar 2023 17:55:36 GMT  
		Size: 1.8 KB (1779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:13f97c23ed3dde89682f32dafe1031b337b4e019b08ab09aabce08c51b982814
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:bbfb7272cb73ee3e4ef83fe62af90e3107ba8a25093370f01c04084ae245e074
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.3 MB (58254124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abeb15b9ddc0e40def7b19f8d3ce62b59b01b91eab2842c688806ce07b56a0f1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 20:19:23 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 08 Mar 2023 20:19:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 20:19:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 20:19:23 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 20:19:30 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 20:19:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 20:19:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 20:19:32 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 20:19:32 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 20:19:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 20:19:32 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 20:19:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 20:19:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 20:19:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b324295dd03a6cf331d4a02cb36bbf8f6ed3f70b953ae2369ef38e779c1dd4`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba21ab1eb9f525edf01d247d3669250181c5376548d9a99f5bd660d772356d1`  
		Last Modified: Wed, 08 Mar 2023 20:20:16 GMT  
		Size: 55.4 MB (55424594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c08861b7dc52dbd6fbf691d23c917df82d0e1f88390a333e71405feffb1d9d4`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c643221233c30d8734b65af733908793c5c1a8a086ab97e153cded745bccf9`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe56612bde98b5cde4e35d27483c06c3802d8da573ddbcb5d26b3f27d1c0658f`  
		Last Modified: Wed, 08 Mar 2023 20:20:09 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:075097bc2cf3b615a6755fdbdd8221de516d0066165200df7cea0a6c859d8550
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55056765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4027e762e66883974a7d197877878b691518068a44e533f95079b0a2c501bbe8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:13 GMT
ADD file:3fb55ad8134002858be264c3c2477d784e4a60f2f6501afa7cf3b10bfede51aa in / 
# Wed, 29 Mar 2023 18:01:13 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:41:06 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 29 Mar 2023 18:41:06 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 18:41:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 18:41:07 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 18:41:19 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 18:41:19 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 18:41:20 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 18:41:20 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 18:41:20 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 18:41:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 18:41:20 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 18:41:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 18:41:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 18:41:20 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:872c99a87729fa48dce303fb615edbb1a5da837f627a0b3d28495a0400ca8335`  
		Last Modified: Wed, 29 Mar 2023 18:02:12 GMT  
		Size: 2.6 MB (2634030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f943ab582225f789f8df5e20ea50348b40ca976ae39c1fe34d64ee41f5de5f0d`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e5ae6cb32e435e094a2636243064561de2a0a53c0b828315b63736447f62d6`  
		Last Modified: Wed, 29 Mar 2023 18:43:22 GMT  
		Size: 52.4 MB (52419359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02107783537cd9f076d338ec3f67d7de3aac478c07b428d59fb043eaf9a9f681`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87747cd79f988871c3d04cf1c1b5a59035e676663fc1e67820a2a99beb7c6ec6`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72c2e7cf99c21075babc33ceeda3f2335e5154ee6d7038844451872d4fd6c49`  
		Last Modified: Wed, 29 Mar 2023 18:43:15 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:662987b59763ef83e15863408a15b51ce4efca13bc73c91e0bcc2b0426147241
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54977469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c61e12fa6c77dfe8b52e98a4a7632d9bdee3c5388a49df3ab325a477a0186df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 21:00:15 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 08 Mar 2023 21:00:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 21:00:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 21:00:16 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 21:00:21 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 21:00:22 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 21:00:23 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 21:00:23 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 21:00:23 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 21:00:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 21:00:23 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 21:00:23 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 21:00:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 21:00:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7157d90cce1f088fbba9c907768f5945710afc3bb84150de3cb59c5d00978d`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65f55c5f2684ce00b7624b63f988feeefb701328e817165a13822ebcf77512c`  
		Last Modified: Wed, 08 Mar 2023 21:01:05 GMT  
		Size: 52.3 MB (52252533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88b7623eb2f729eda24846a44d7dab5fa9aadd218d51457846d49cda56ade2e`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f277283afb0270bbf32ee345a025b907d5600f2a57d75fcded51c30bfc95563a`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21afe3f708be7aceac151a8a44180deb00009e6bb2125f1732122b39371c4a0d`  
		Last Modified: Wed, 08 Mar 2023 21:01:00 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:3cd77af99b0165e0164a77ccad690bfe1e04011e08176bd3fd373b7bee63105d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56473907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5334ec6e01f45142db2942cd847241440b0fc3958b810ca341f199fef4db8959`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 17:54:43 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 29 Mar 2023 17:54:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 17:54:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 17:54:43 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 17:54:56 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 17:54:57 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 17:54:57 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 17:54:57 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 17:54:58 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 17:54:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 17:54:58 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 17:54:58 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 17:54:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 17:54:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b13556e68f2b9c9adb9cd02a8cf1df9e58f2cd6d81df25181c67be1d1a3c20`  
		Last Modified: Wed, 29 Mar 2023 17:55:36 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641d086a647f9ff43dcd02f5ad85442f927600b6bf102486b8c2401453cb1f8a`  
		Last Modified: Wed, 29 Mar 2023 17:55:44 GMT  
		Size: 53.6 MB (53637960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f012612a86102a2f0a2d613722b1817be563a199bd7ba1f3ab7364ed6ff2d92`  
		Last Modified: Wed, 29 Mar 2023 17:55:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3385843be8b35c1162a966477a35aa41b7b437253ae18dbebd0990b986f7cd8`  
		Last Modified: Wed, 29 Mar 2023 17:55:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3dd6230007d9ece7ef3ae146d9db2764ceea2c02d791a9b387b9bd7625615e`  
		Last Modified: Wed, 29 Mar 2023 17:55:36 GMT  
		Size: 1.8 KB (1779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
