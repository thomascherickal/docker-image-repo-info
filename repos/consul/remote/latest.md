## `consul:latest`

```console
$ docker pull consul@sha256:b6e4c1773a506ee77717e2034cf346f96c6ec978ded1d67fe85f76c21e7fa47d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:61821744f422575e14dc2e71e884cbc9890942a0fc5bfdffa77a044cfc11ab61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57850971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9976413d3a8199bbdc513bff41028d8b638395ea76387dc3e9989316ba6936`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 00:36:36 GMT
ARG CONSUL_VERSION=1.15.0
# Sat, 25 Feb 2023 00:36:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 00:36:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 00:36:37 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 00:36:44 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 00:36:45 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 00:36:46 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 00:36:46 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 00:36:46 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 00:36:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 00:36:46 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 00:36:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 00:36:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 00:36:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd42e3c5627afe1a57d4230be5dc11b0c1de3e793939a10bc9aa4ff9836517f5`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51dfee8f0af07ba1221883e60ce52f0205c116d4946b2beb6e1587ecf2c0023`  
		Last Modified: Sat, 25 Feb 2023 00:37:11 GMT  
		Size: 55.0 MB (55021446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfbefd36cf65c7bdef5ef877f0e20ff7e6bcf6a77a92aebb718168ded978643`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e952e991c0aa96b1d031d8c08e85b06d7a99d339bee758fa79bf3c6d4fccec4f`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6d554e81cd6ac67ccad4bfeea60bf62a2e6ae7a26ca8a48049191118415a90`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:a10b8a74730b73ea84dbd0a0678e87a6af8e9e20652ca57a0608af254fe69d6d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53714998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2229f0feda5c42cde7eaaefc16b767a6146c21233f43deaebdf230e869a9cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 21:30:26 GMT
ARG CONSUL_VERSION=1.14.4
# Fri, 10 Feb 2023 21:30:26 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 10 Feb 2023 21:30:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 10 Feb 2023 21:30:27 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 10 Feb 2023 21:30:35 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 10 Feb 2023 21:30:36 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 10 Feb 2023 21:30:36 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 10 Feb 2023 21:30:36 GMT
VOLUME [/consul/data]
# Fri, 10 Feb 2023 21:30:37 GMT
EXPOSE 8300
# Fri, 10 Feb 2023 21:30:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 10 Feb 2023 21:30:37 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 10 Feb 2023 21:30:37 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 10 Feb 2023 21:30:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 21:30:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15679575500979d2c802ec409d24aac6ccebfec03aa0c84f2ab09ac81e74139`  
		Last Modified: Fri, 10 Feb 2023 21:31:33 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7cfc00fb1b7349584d66f1706a34434f152ee5dd20cfad3f3749652d01833c`  
		Last Modified: Fri, 10 Feb 2023 21:31:40 GMT  
		Size: 51.1 MB (51078033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e6df18df0cf026ae82acec2971fa7305c95363f66344e749876b349ed21612`  
		Last Modified: Fri, 10 Feb 2023 21:31:33 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69191e4c2d1de20f3c7bf3ddf5ac48fce16c885577861e20f9f713cdc33cab43`  
		Last Modified: Fri, 10 Feb 2023 21:31:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4f90a9a21bf4d09a519cb7986d166297834a036cd9bc4afda7dbf06462916`  
		Last Modified: Fri, 10 Feb 2023 21:31:33 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:57355f6f632f1a78305ffc430d940e6630c809eb9a80db54c498489dac3504a1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53141443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d655387a1164567de86de6dd008ac7777c23224421b37ede5ddec85dedbdaf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:01:26 GMT
ARG CONSUL_VERSION=1.14.4
# Fri, 10 Feb 2023 22:01:26 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 10 Feb 2023 22:01:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 10 Feb 2023 22:01:27 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 10 Feb 2023 22:01:33 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 10 Feb 2023 22:01:34 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 10 Feb 2023 22:01:34 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 10 Feb 2023 22:01:34 GMT
VOLUME [/consul/data]
# Fri, 10 Feb 2023 22:01:34 GMT
EXPOSE 8300
# Fri, 10 Feb 2023 22:01:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 10 Feb 2023 22:01:35 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 10 Feb 2023 22:01:35 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:01:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:01:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5f5a93605265de2bf7d1ce0a04b31e9206424042dd482959fa40ae232e004c`  
		Last Modified: Fri, 10 Feb 2023 22:02:11 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2643ebb7531da6503768460e59c74886ed8290708898a767795e01cc43ff35d`  
		Last Modified: Fri, 10 Feb 2023 22:02:16 GMT  
		Size: 50.4 MB (50416508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d229f64652a58dfbe39028360c58d336eeb0d20c9d25472dd0530766bb84bf`  
		Last Modified: Fri, 10 Feb 2023 22:02:11 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833943f861feda487a0c0d67bd4db9cb122b2a3c32160d897d3b30ae71e01924`  
		Last Modified: Fri, 10 Feb 2023 22:02:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8986cc9f0209a2e424ae170ce3a41bdcf3a0e14e1d6ff01d0106d0c979a1eecb`  
		Last Modified: Fri, 10 Feb 2023 22:02:11 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:0c1d3d2994ca511f1bc535f1c8c676edb05fc71cf8f72539219d07a4dcfd9eb0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55105674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3605988f2c033cffa95d60c18b54f2ccb59d1e7fa3e4e388a650401eaecd5e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:34 GMT
ADD file:35855658886412913d05c0f9e29bf8f650c0d37e20100a9de118b468f86f7f30 in / 
# Fri, 10 Feb 2023 21:24:34 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:03:02 GMT
ARG CONSUL_VERSION=1.14.4
# Fri, 10 Feb 2023 22:03:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 10 Feb 2023 22:03:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 10 Feb 2023 22:03:05 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 10 Feb 2023 22:03:12 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 10 Feb 2023 22:03:12 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 10 Feb 2023 22:03:13 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 10 Feb 2023 22:03:14 GMT
VOLUME [/consul/data]
# Fri, 10 Feb 2023 22:03:15 GMT
EXPOSE 8300
# Fri, 10 Feb 2023 22:03:16 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 10 Feb 2023 22:03:17 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 10 Feb 2023 22:03:19 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:03:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:03:20 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13a1d7e543968b1c2bd92ca5f2fb2e964b31713fc7707305c1cdfb935ca3e631`  
		Last Modified: Fri, 10 Feb 2023 21:25:40 GMT  
		Size: 2.8 MB (2832331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0626ffa155376b749904ceb751a1ae408838cca2e5721c6580008f030426cdc7`  
		Last Modified: Fri, 10 Feb 2023 22:04:27 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd233d2be3a37dbe1751e1366adbcd99e61856297d5c6539625a8daeaed6dde7`  
		Last Modified: Fri, 10 Feb 2023 22:04:33 GMT  
		Size: 52.3 MB (52270026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d486f1c16831806e60d70ae53f27852ec83746e1cb76828000bea84f2ae5bc5e`  
		Last Modified: Fri, 10 Feb 2023 22:04:27 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0c72a0c71ba3fd81b8af6ab034d8bb7457187e133e1748c405137bd7e84bb6`  
		Last Modified: Fri, 10 Feb 2023 22:04:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f96af6f4f778791cb130d71bcc0562bcf25d75d234daa29044417547c52e44`  
		Last Modified: Fri, 10 Feb 2023 22:04:27 GMT  
		Size: 1.8 KB (1781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
