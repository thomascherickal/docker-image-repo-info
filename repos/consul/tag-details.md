<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.12`](#consul112)
-	[`consul:1.12.6`](#consul1126)
-	[`consul:1.13`](#consul113)
-	[`consul:1.13.3`](#consul1133)
-	[`consul:1.14`](#consul114)
-	[`consul:1.14.0`](#consul1140)
-	[`consul:latest`](#consullatest)

## `consul:1.12`

```console
$ docker pull consul@sha256:4dce476b684b658e6a22b2a64eed16a1b33052fa255beaf70dbe4aa55cc03ceb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.12` - linux; amd64

```console
$ docker pull consul@sha256:89dcfa9c7fe552fd25221b8320969748c95bb673d4f08ebb5eb4f79147e53b0d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49575983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e07ac887390bd05f4fce36980d9bf2ace44e477e5c8d20e1da9ced6544491fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:19:41 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 20 Oct 2022 22:19:41 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:19:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:19:42 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:19:48 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:19:48 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:19:49 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:19:49 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:19:49 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:19:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:19:49 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:19:49 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:19:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209242f96fda74b1a639617f4142b5f7ffa4e9c256a171c56fcff3c4e114e993`  
		Last Modified: Thu, 20 Oct 2022 22:20:34 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b682db2167ecc99968981f03df83845098054e1847459d35325b195f16f4c0`  
		Last Modified: Thu, 20 Oct 2022 22:20:40 GMT  
		Size: 46.7 MB (46749086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b339551b0464217749058feccecc01bd03d2ea319ed10efabf0df458163bc1d`  
		Last Modified: Thu, 20 Oct 2022 22:20:34 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f912e922e249c816acc84577902adc529a8943800ce591502905f3652fe603`  
		Last Modified: Thu, 20 Oct 2022 22:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91df91f08206d3c2ee0e640031e790ca36cbf600842771381324969ad587f7b1`  
		Last Modified: Thu, 20 Oct 2022 22:20:34 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm variant v6

```console
$ docker pull consul@sha256:aec0adf361f0a13de86c2a6f783d1ed0800d126b1f457d3c61d19e265d085f80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47445918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52e73543f53a4c7d743b891ed8c8480761bf2fd79d738ee8684daf3a29a39767`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:46:26 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 10 Nov 2022 21:46:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 10 Nov 2022 21:46:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Nov 2022 21:46:29 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Nov 2022 21:46:38 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Nov 2022 21:46:40 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Nov 2022 21:46:41 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:46:42 GMT
VOLUME [/consul/data]
# Thu, 10 Nov 2022 21:46:42 GMT
EXPOSE 8300
# Thu, 10 Nov 2022 21:46:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Nov 2022 21:46:43 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Nov 2022 21:46:44 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Nov 2022 21:46:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:46:44 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1151804df74760a58044c678dfc979d3fb19fa2130cdd3b39aef76073bb03af`  
		Last Modified: Thu, 10 Nov 2022 21:48:04 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c15450d5500fc9deb4d91eaec6399780acf54aba109ebeb8e06cbf9f0da98f7`  
		Last Modified: Thu, 10 Nov 2022 21:48:13 GMT  
		Size: 44.8 MB (44811461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcedc6a861ef5218084290f89193413b69d543f9dc7b1d83991e2b9597c6fca`  
		Last Modified: Thu, 10 Nov 2022 21:48:04 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56b39e49a0d69aa2ab7622ed1816935358b7b13fca8d65713ad69d96679ef8e`  
		Last Modified: Thu, 10 Nov 2022 21:48:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ed6357b018d72e24434cafb87c4c38eae58fe2a95353a78933d80cabf2615b`  
		Last Modified: Thu, 10 Nov 2022 21:48:04 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:395987ad01e36b9c558279686b715e00480c88b7734e875604ea91a0f4aa4ff5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47179880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3fbdd2291af47539cf728705c081ed5d61c2a9a37ec20c7548caeca1659d2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:58:50 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 10 Nov 2022 21:58:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 10 Nov 2022 21:58:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Nov 2022 21:58:51 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Nov 2022 21:58:55 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Nov 2022 21:58:56 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Nov 2022 21:58:57 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:58:57 GMT
VOLUME [/consul/data]
# Thu, 10 Nov 2022 21:58:57 GMT
EXPOSE 8300
# Thu, 10 Nov 2022 21:58:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Nov 2022 21:58:57 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Nov 2022 21:58:57 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Nov 2022 21:58:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:58:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72da3ce6eaa1ef2e62dc478e3852a30a184e3e72a6d993eecb7c0b5ebd0d0df`  
		Last Modified: Thu, 10 Nov 2022 21:59:36 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d434724d3a5d1e86f185d3b9c7b20c9d2522faabb62d912e151e89fe9b234f58`  
		Last Modified: Thu, 10 Nov 2022 21:59:40 GMT  
		Size: 44.5 MB (44458057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6c3dbe69939a92b6a26dcc7ba3fc4272666337e9362b0c41e47d551aaeb0db`  
		Last Modified: Thu, 10 Nov 2022 21:59:36 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b09f578a37a5ce2c77511deba4ecb5345f0f96451579931b998c5b4e81a7865`  
		Last Modified: Thu, 10 Nov 2022 21:59:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d70e28fb6b9086b3dcd0cffca475563cb1dd5e8cef728ffec5d13782aee1d8`  
		Last Modified: Thu, 10 Nov 2022 21:59:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; 386

```console
$ docker pull consul@sha256:bfcfe778fe96c7a8f05adcd96dc8e3c08d34fbfe9c4a1fe24adc3fcc9bc8f437
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48646271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3170cb6e25aa0aaa7d0fc5e646981fd6ad5b53b65aabfd5f5894a340cd674dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:38:49 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 20 Oct 2022 22:38:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:38:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:38:52 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:38:59 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:39:00 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:39:01 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:39:02 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:39:03 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:39:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:39:05 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:39:07 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:39:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:39:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e8a70d3699a7d5fac506f6a0ba4c679af437fa8d0039ee0ecf8bec641d38b5`  
		Last Modified: Thu, 20 Oct 2022 22:40:15 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172f4d811d49e6a0d97fa8d9218b69ffc164cee3962b0769e1725aeef107f49c`  
		Last Modified: Thu, 20 Oct 2022 22:40:20 GMT  
		Size: 45.8 MB (45814427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecef6af5a3802b54d56bc1d703f5a1d078280b091c88894979a36000c3c7b91`  
		Last Modified: Thu, 20 Oct 2022 22:40:15 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173c858084e1b4859769e873c4a7c7f1f94fc3bf20c3424cd597e4b61752332`  
		Last Modified: Thu, 20 Oct 2022 22:40:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec720085247d3883ce601e3d4875cd10737568f0647224dc04569be60e1b772`  
		Last Modified: Thu, 20 Oct 2022 22:40:15 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12.6`

```console
$ docker pull consul@sha256:4dce476b684b658e6a22b2a64eed16a1b33052fa255beaf70dbe4aa55cc03ceb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.12.6` - linux; amd64

```console
$ docker pull consul@sha256:89dcfa9c7fe552fd25221b8320969748c95bb673d4f08ebb5eb4f79147e53b0d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49575983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e07ac887390bd05f4fce36980d9bf2ace44e477e5c8d20e1da9ced6544491fa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:19:41 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 20 Oct 2022 22:19:41 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:19:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:19:42 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:19:48 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:19:48 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:19:49 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:19:49 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:19:49 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:19:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:19:49 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:19:49 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:19:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209242f96fda74b1a639617f4142b5f7ffa4e9c256a171c56fcff3c4e114e993`  
		Last Modified: Thu, 20 Oct 2022 22:20:34 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b682db2167ecc99968981f03df83845098054e1847459d35325b195f16f4c0`  
		Last Modified: Thu, 20 Oct 2022 22:20:40 GMT  
		Size: 46.7 MB (46749086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b339551b0464217749058feccecc01bd03d2ea319ed10efabf0df458163bc1d`  
		Last Modified: Thu, 20 Oct 2022 22:20:34 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f912e922e249c816acc84577902adc529a8943800ce591502905f3652fe603`  
		Last Modified: Thu, 20 Oct 2022 22:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91df91f08206d3c2ee0e640031e790ca36cbf600842771381324969ad587f7b1`  
		Last Modified: Thu, 20 Oct 2022 22:20:34 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:aec0adf361f0a13de86c2a6f783d1ed0800d126b1f457d3c61d19e265d085f80
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47445918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52e73543f53a4c7d743b891ed8c8480761bf2fd79d738ee8684daf3a29a39767`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:46:26 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 10 Nov 2022 21:46:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 10 Nov 2022 21:46:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Nov 2022 21:46:29 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Nov 2022 21:46:38 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Nov 2022 21:46:40 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Nov 2022 21:46:41 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:46:42 GMT
VOLUME [/consul/data]
# Thu, 10 Nov 2022 21:46:42 GMT
EXPOSE 8300
# Thu, 10 Nov 2022 21:46:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Nov 2022 21:46:43 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Nov 2022 21:46:44 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Nov 2022 21:46:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:46:44 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1151804df74760a58044c678dfc979d3fb19fa2130cdd3b39aef76073bb03af`  
		Last Modified: Thu, 10 Nov 2022 21:48:04 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c15450d5500fc9deb4d91eaec6399780acf54aba109ebeb8e06cbf9f0da98f7`  
		Last Modified: Thu, 10 Nov 2022 21:48:13 GMT  
		Size: 44.8 MB (44811461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcedc6a861ef5218084290f89193413b69d543f9dc7b1d83991e2b9597c6fca`  
		Last Modified: Thu, 10 Nov 2022 21:48:04 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56b39e49a0d69aa2ab7622ed1816935358b7b13fca8d65713ad69d96679ef8e`  
		Last Modified: Thu, 10 Nov 2022 21:48:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ed6357b018d72e24434cafb87c4c38eae58fe2a95353a78933d80cabf2615b`  
		Last Modified: Thu, 10 Nov 2022 21:48:04 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:395987ad01e36b9c558279686b715e00480c88b7734e875604ea91a0f4aa4ff5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47179880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3fbdd2291af47539cf728705c081ed5d61c2a9a37ec20c7548caeca1659d2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:58:50 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 10 Nov 2022 21:58:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 10 Nov 2022 21:58:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Nov 2022 21:58:51 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Nov 2022 21:58:55 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Nov 2022 21:58:56 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Nov 2022 21:58:57 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:58:57 GMT
VOLUME [/consul/data]
# Thu, 10 Nov 2022 21:58:57 GMT
EXPOSE 8300
# Thu, 10 Nov 2022 21:58:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Nov 2022 21:58:57 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Nov 2022 21:58:57 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Nov 2022 21:58:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:58:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72da3ce6eaa1ef2e62dc478e3852a30a184e3e72a6d993eecb7c0b5ebd0d0df`  
		Last Modified: Thu, 10 Nov 2022 21:59:36 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d434724d3a5d1e86f185d3b9c7b20c9d2522faabb62d912e151e89fe9b234f58`  
		Last Modified: Thu, 10 Nov 2022 21:59:40 GMT  
		Size: 44.5 MB (44458057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6c3dbe69939a92b6a26dcc7ba3fc4272666337e9362b0c41e47d551aaeb0db`  
		Last Modified: Thu, 10 Nov 2022 21:59:36 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b09f578a37a5ce2c77511deba4ecb5345f0f96451579931b998c5b4e81a7865`  
		Last Modified: Thu, 10 Nov 2022 21:59:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d70e28fb6b9086b3dcd0cffca475563cb1dd5e8cef728ffec5d13782aee1d8`  
		Last Modified: Thu, 10 Nov 2022 21:59:36 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.6` - linux; 386

```console
$ docker pull consul@sha256:bfcfe778fe96c7a8f05adcd96dc8e3c08d34fbfe9c4a1fe24adc3fcc9bc8f437
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48646271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3170cb6e25aa0aaa7d0fc5e646981fd6ad5b53b65aabfd5f5894a340cd674dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:38:49 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 20 Oct 2022 22:38:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:38:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:38:52 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:38:59 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:39:00 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:39:01 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:39:02 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:39:03 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:39:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:39:05 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:39:07 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:39:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:39:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e8a70d3699a7d5fac506f6a0ba4c679af437fa8d0039ee0ecf8bec641d38b5`  
		Last Modified: Thu, 20 Oct 2022 22:40:15 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172f4d811d49e6a0d97fa8d9218b69ffc164cee3962b0769e1725aeef107f49c`  
		Last Modified: Thu, 20 Oct 2022 22:40:20 GMT  
		Size: 45.8 MB (45814427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecef6af5a3802b54d56bc1d703f5a1d078280b091c88894979a36000c3c7b91`  
		Last Modified: Thu, 20 Oct 2022 22:40:15 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9173c858084e1b4859769e873c4a7c7f1f94fc3bf20c3424cd597e4b61752332`  
		Last Modified: Thu, 20 Oct 2022 22:40:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec720085247d3883ce601e3d4875cd10737568f0647224dc04569be60e1b772`  
		Last Modified: Thu, 20 Oct 2022 22:40:15 GMT  
		Size: 1.8 KB (1791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.13`

```console
$ docker pull consul@sha256:af77bcb370db135046de257a7d98c4e2e0fd32a30507683d0f6e45a7de4e18d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13` - linux; amd64

```console
$ docker pull consul@sha256:6afb7a04ee7f088bdc7b08d58b6271b924af3f0b95830e57e355996d05eb6a16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51855936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6608222931a019f0658c775357d35ab0e45321547728eaccef8e7e296e6fb384`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:19:30 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 22:19:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:19:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:19:31 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:19:37 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:19:37 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:19:38 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:19:38 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:19:38 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:19:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:19:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:19:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:19:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:19:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00394ff436377c2ae3f1ca19dfe233d1e943a4a15f98f5e18d7cc8ee507c5aad`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036575c53ebc9949f4aa974af5bc7412dd5f66e5042d35562c44675d74a5e7cb`  
		Last Modified: Thu, 20 Oct 2022 22:20:21 GMT  
		Size: 49.0 MB (49029040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ece016dc23d737e697fc51f2d331e7977cd6af4bd99a864f68f1da58cd91f8`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86338dd101579990eecfc50fd3e93010255265d836d5e22a33d43959e0504ba`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eede053ff767f6f4e47143538c24b94d0d44acb4ff8a085e477eaae46a0a1bd`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm variant v6

```console
$ docker pull consul@sha256:1e91f52efdbcb7cffa5421c2425d3b7fe171713a3c3d9df3e9c2ab9d2b27408c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49447571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2848ed01c29b5e3eeb1e68fb9cbcb913831f8e96e3535697a66d40264320891e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:46:01 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 10 Nov 2022 21:46:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 10 Nov 2022 21:46:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Nov 2022 21:46:03 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Nov 2022 21:46:12 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Nov 2022 21:46:14 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Nov 2022 21:46:16 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:46:17 GMT
VOLUME [/consul/data]
# Thu, 10 Nov 2022 21:46:17 GMT
EXPOSE 8300
# Thu, 10 Nov 2022 21:46:17 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Nov 2022 21:46:17 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Nov 2022 21:46:18 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Nov 2022 21:46:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:46:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1207d959d423d5b5b88917ddeaa619ec925217bfae77ec336b44251f9786f529`  
		Last Modified: Thu, 10 Nov 2022 21:47:39 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155c19019bfc9b643e800543009adb9ca8a5964a2a2e53168f82906d6a4e2dc8`  
		Last Modified: Thu, 10 Nov 2022 21:47:48 GMT  
		Size: 46.8 MB (46813120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b4eb968630b76992240b0af75157b5dd2914446e2d7c9c31d93ef604a4f54`  
		Last Modified: Thu, 10 Nov 2022 21:47:39 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfce51e5c34e21f9210a5db4ead93b53d355d3440e87fc977802d3efa17bd259`  
		Last Modified: Thu, 10 Nov 2022 21:47:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5648c2367237436258662ffe3b3fd4bba673b17c3732f088a2d0f398a32c6b39`  
		Last Modified: Thu, 10 Nov 2022 21:47:39 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:17e4ef4e78779df30d6f23604798255de28e450857a61edd6ff9b527c0b9ac07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49025344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b869d28544071514bdc62a2103cf4d0435cd497e922ed73c4e920eee2b77bb24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:58:40 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 10 Nov 2022 21:58:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 10 Nov 2022 21:58:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Nov 2022 21:58:41 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Nov 2022 21:58:46 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Nov 2022 21:58:47 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Nov 2022 21:58:47 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:58:48 GMT
VOLUME [/consul/data]
# Thu, 10 Nov 2022 21:58:48 GMT
EXPOSE 8300
# Thu, 10 Nov 2022 21:58:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Nov 2022 21:58:48 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Nov 2022 21:58:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Nov 2022 21:58:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:58:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cbe1b3bf92e11e488c34488461f0b292032eba542f41a4aae28451df56fc00`  
		Last Modified: Thu, 10 Nov 2022 21:59:19 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a265352cb9e4d34170bda2552ff37e549dc35260ed30e961e7a538727feebb92`  
		Last Modified: Thu, 10 Nov 2022 21:59:24 GMT  
		Size: 46.3 MB (46303523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69166e5aa15d5da10bcd4f03e068ae08a799dee9078108cbf77ed5301392234`  
		Last Modified: Thu, 10 Nov 2022 21:59:19 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572cffea91c94f3260acaee20321f6399376e84c7505c5bbf86fc49ad73c3879`  
		Last Modified: Thu, 10 Nov 2022 21:59:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fad6c87d760db39e95221e3e1d03a554b56c761fbb9c6f897e33e7da8871bd`  
		Last Modified: Thu, 10 Nov 2022 21:59:19 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; 386

```console
$ docker pull consul@sha256:94181e48fe1c03c0227e23e1196d0a7722e3a3912a0e6c13b12b8b555f21f568
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50729283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b19d998a1ac09881d13112e72f28dbb35a584aa3cb20175703a3ee4b879c9f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:38:23 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 22:38:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:38:25 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:38:26 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:38:33 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:38:34 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:38:35 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:38:36 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:38:37 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:38:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:38:39 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:38:41 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:38:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b511d0d85425cbc09a9d8d62d59f5365888df7d82c1f6a1855b7d36256ac6b61`  
		Last Modified: Thu, 20 Oct 2022 22:39:54 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ac5250791b73c51a7fa65e8dc74d329c0106e21b011eb046ca344c82e02ed9`  
		Last Modified: Thu, 20 Oct 2022 22:40:00 GMT  
		Size: 47.9 MB (47897443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f5884f57cf7c945feab1302f5d34ec1be900ca91470ca60cd47d05c3f4b4f2`  
		Last Modified: Thu, 20 Oct 2022 22:39:54 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cc41b97288a4fe7631fb93e5537830c6ee40f00edf472563a678fe26fe3885`  
		Last Modified: Thu, 20 Oct 2022 22:39:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a17329c963aa144e4815bd6d1776faaac8ab5beb9a149457a3d48229c20ffa`  
		Last Modified: Thu, 20 Oct 2022 22:39:54 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.13.3`

```console
$ docker pull consul@sha256:af77bcb370db135046de257a7d98c4e2e0fd32a30507683d0f6e45a7de4e18d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13.3` - linux; amd64

```console
$ docker pull consul@sha256:6afb7a04ee7f088bdc7b08d58b6271b924af3f0b95830e57e355996d05eb6a16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51855936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6608222931a019f0658c775357d35ab0e45321547728eaccef8e7e296e6fb384`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:19:30 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 22:19:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:19:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:19:31 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:19:37 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:19:37 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:19:38 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:19:38 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:19:38 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:19:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:19:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:19:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:19:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:19:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00394ff436377c2ae3f1ca19dfe233d1e943a4a15f98f5e18d7cc8ee507c5aad`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036575c53ebc9949f4aa974af5bc7412dd5f66e5042d35562c44675d74a5e7cb`  
		Last Modified: Thu, 20 Oct 2022 22:20:21 GMT  
		Size: 49.0 MB (49029040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ece016dc23d737e697fc51f2d331e7977cd6af4bd99a864f68f1da58cd91f8`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86338dd101579990eecfc50fd3e93010255265d836d5e22a33d43959e0504ba`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eede053ff767f6f4e47143538c24b94d0d44acb4ff8a085e477eaae46a0a1bd`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.3` - linux; arm variant v6

```console
$ docker pull consul@sha256:1e91f52efdbcb7cffa5421c2425d3b7fe171713a3c3d9df3e9c2ab9d2b27408c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49447571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2848ed01c29b5e3eeb1e68fb9cbcb913831f8e96e3535697a66d40264320891e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:46:01 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 10 Nov 2022 21:46:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 10 Nov 2022 21:46:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Nov 2022 21:46:03 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Nov 2022 21:46:12 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Nov 2022 21:46:14 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Nov 2022 21:46:16 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:46:17 GMT
VOLUME [/consul/data]
# Thu, 10 Nov 2022 21:46:17 GMT
EXPOSE 8300
# Thu, 10 Nov 2022 21:46:17 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Nov 2022 21:46:17 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Nov 2022 21:46:18 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Nov 2022 21:46:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:46:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1207d959d423d5b5b88917ddeaa619ec925217bfae77ec336b44251f9786f529`  
		Last Modified: Thu, 10 Nov 2022 21:47:39 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155c19019bfc9b643e800543009adb9ca8a5964a2a2e53168f82906d6a4e2dc8`  
		Last Modified: Thu, 10 Nov 2022 21:47:48 GMT  
		Size: 46.8 MB (46813120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b4eb968630b76992240b0af75157b5dd2914446e2d7c9c31d93ef604a4f54`  
		Last Modified: Thu, 10 Nov 2022 21:47:39 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfce51e5c34e21f9210a5db4ead93b53d355d3440e87fc977802d3efa17bd259`  
		Last Modified: Thu, 10 Nov 2022 21:47:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5648c2367237436258662ffe3b3fd4bba673b17c3732f088a2d0f398a32c6b39`  
		Last Modified: Thu, 10 Nov 2022 21:47:39 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:17e4ef4e78779df30d6f23604798255de28e450857a61edd6ff9b527c0b9ac07
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49025344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b869d28544071514bdc62a2103cf4d0435cd497e922ed73c4e920eee2b77bb24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 21:58:40 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 10 Nov 2022 21:58:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 10 Nov 2022 21:58:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 10 Nov 2022 21:58:41 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 10 Nov 2022 21:58:46 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 10 Nov 2022 21:58:47 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 10 Nov 2022 21:58:47 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 10 Nov 2022 21:58:48 GMT
VOLUME [/consul/data]
# Thu, 10 Nov 2022 21:58:48 GMT
EXPOSE 8300
# Thu, 10 Nov 2022 21:58:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 10 Nov 2022 21:58:48 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 10 Nov 2022 21:58:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 10 Nov 2022 21:58:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 21:58:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cbe1b3bf92e11e488c34488461f0b292032eba542f41a4aae28451df56fc00`  
		Last Modified: Thu, 10 Nov 2022 21:59:19 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a265352cb9e4d34170bda2552ff37e549dc35260ed30e961e7a538727feebb92`  
		Last Modified: Thu, 10 Nov 2022 21:59:24 GMT  
		Size: 46.3 MB (46303523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69166e5aa15d5da10bcd4f03e068ae08a799dee9078108cbf77ed5301392234`  
		Last Modified: Thu, 10 Nov 2022 21:59:19 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572cffea91c94f3260acaee20321f6399376e84c7505c5bbf86fc49ad73c3879`  
		Last Modified: Thu, 10 Nov 2022 21:59:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fad6c87d760db39e95221e3e1d03a554b56c761fbb9c6f897e33e7da8871bd`  
		Last Modified: Thu, 10 Nov 2022 21:59:19 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.3` - linux; 386

```console
$ docker pull consul@sha256:94181e48fe1c03c0227e23e1196d0a7722e3a3912a0e6c13b12b8b555f21f568
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50729283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b19d998a1ac09881d13112e72f28dbb35a584aa3cb20175703a3ee4b879c9f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:38:23 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 22:38:24 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:38:25 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:38:26 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:38:33 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:38:34 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:38:35 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:38:36 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:38:37 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:38:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:38:39 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:38:41 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:38:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b511d0d85425cbc09a9d8d62d59f5365888df7d82c1f6a1855b7d36256ac6b61`  
		Last Modified: Thu, 20 Oct 2022 22:39:54 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ac5250791b73c51a7fa65e8dc74d329c0106e21b011eb046ca344c82e02ed9`  
		Last Modified: Thu, 20 Oct 2022 22:40:00 GMT  
		Size: 47.9 MB (47897443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f5884f57cf7c945feab1302f5d34ec1be900ca91470ca60cd47d05c3f4b4f2`  
		Last Modified: Thu, 20 Oct 2022 22:39:54 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cc41b97288a4fe7631fb93e5537830c6ee40f00edf472563a678fe26fe3885`  
		Last Modified: Thu, 20 Oct 2022 22:39:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a17329c963aa144e4815bd6d1776faaac8ab5beb9a149457a3d48229c20ffa`  
		Last Modified: Thu, 20 Oct 2022 22:39:54 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.14`

```console
$ docker pull consul@sha256:74d2cadfd445d1fbc00e4a24e7035b22279e55e4efd28ec7ad91d89bac3e6601
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14` - linux; arm variant v6

```console
$ docker pull consul@sha256:4615b6a5ed5f1f1d193bce5f92331c63be4cba7dc6426414ace8cdf0489ce593
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53569059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd1987c1bd04461c5d204d137d597c1dda018e0d23c6adc0fde6d124c1a3526c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 23:49:34 GMT
ARG CONSUL_VERSION=1.14.0
# Tue, 15 Nov 2022 23:49:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 15 Nov 2022 23:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Nov 2022 23:49:36 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Nov 2022 23:49:45 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Nov 2022 23:49:47 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Nov 2022 23:49:48 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Nov 2022 23:49:48 GMT
VOLUME [/consul/data]
# Tue, 15 Nov 2022 23:49:49 GMT
EXPOSE 8300
# Tue, 15 Nov 2022 23:49:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Nov 2022 23:49:49 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Nov 2022 23:49:49 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Nov 2022 23:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 23:49:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d46f6732f3361c39c017c9813a98e72dee4b0be870b55fbc9dfd44a32aa0615`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ab31975ce52a3dc3769ab782fa4932201b0d58f61baaddbcc199ade6220e0`  
		Last Modified: Tue, 15 Nov 2022 23:50:46 GMT  
		Size: 50.9 MB (50934609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ddfcd0f4ae0b84279348a74fac1e56e704af32e8b87153dbbd06106b996bb`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2f4c860256384e1ad59b3d8f73238f427c1089c7648c42e950577f884c8f32`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4d126dc9cb4c4107e4d3c519fb0704be027dd60a69fd76b8c46735ba3029c5`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:7b7d2b038889b257d35b2136c15f0846184adeb768a8acbafefac73ceeb1868f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52977520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f10ea9c64d4b00e9b910ac1f3d086e45ec8d6a452b9cf7f7b5548974a88c95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 23:39:23 GMT
ARG CONSUL_VERSION=1.14.0
# Tue, 15 Nov 2022 23:39:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 15 Nov 2022 23:39:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Nov 2022 23:39:24 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Nov 2022 23:39:30 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Nov 2022 23:39:31 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Nov 2022 23:39:31 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Nov 2022 23:39:31 GMT
VOLUME [/consul/data]
# Tue, 15 Nov 2022 23:39:31 GMT
EXPOSE 8300
# Tue, 15 Nov 2022 23:39:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Nov 2022 23:39:31 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Nov 2022 23:39:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Nov 2022 23:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 23:39:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac06a996baf6147b888319bd6784ef204cbe7d61a8ad320aafe35ce7d7bfd789`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531269224bff8dded9d8494dc3d047fd01dd8e5cbfda516bc45586e2d0280aee`  
		Last Modified: Tue, 15 Nov 2022 23:39:53 GMT  
		Size: 50.3 MB (50255697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9219a50b0a5f9585fe647e91fd6353590340b64fb94472becd11ec9dfd7ae4d7`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac7f4108db1d821d2deab163058d322c3064550209a9b487b4a8e5d816be056`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0acd0ba01e973e78cb9e7197802b3f21fc0a903e3580ed2f54b5523117cde6`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; 386

```console
$ docker pull consul@sha256:f25a66a33365bf000da1af9795cc33c3b1d38fd5c871076389737702e848b647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54967457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfe52a88b58d3d694955510c5dcbfa257a3261d64543a44049bcebc0148a244`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 23:40:04 GMT
ARG CONSUL_VERSION=1.14.0
# Tue, 15 Nov 2022 23:40:04 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 15 Nov 2022 23:40:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Nov 2022 23:40:06 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Nov 2022 23:40:14 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Nov 2022 23:40:15 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Nov 2022 23:40:16 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Nov 2022 23:40:17 GMT
VOLUME [/consul/data]
# Tue, 15 Nov 2022 23:40:18 GMT
EXPOSE 8300
# Tue, 15 Nov 2022 23:40:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Nov 2022 23:40:20 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Nov 2022 23:40:22 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Nov 2022 23:40:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 23:40:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0d18046f8061edd59c8ed998cf6dc764cf701a6dd0b6c30d33b1e67ca67eee`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b593f664127c7088ac7c064de125eefd2d8e99951fa06ff8932371da1b9b052`  
		Last Modified: Tue, 15 Nov 2022 23:41:01 GMT  
		Size: 52.1 MB (52135619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c17fbdd942d59ab2d174e42ca2e5d58e7e01b94f54174a3ff737f6285f0fdd9`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f8fbe7050f96ef7d91dd11710cffd7e4d164d2000f11c320a8b89f502d14ba`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a5c5cd06f482ce420d8d33e65b7e65fbb3bfc0fe5fed8547dcb1a22b3e21a4`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.14.0`

```console
$ docker pull consul@sha256:74d2cadfd445d1fbc00e4a24e7035b22279e55e4efd28ec7ad91d89bac3e6601
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14.0` - linux; arm variant v6

```console
$ docker pull consul@sha256:4615b6a5ed5f1f1d193bce5f92331c63be4cba7dc6426414ace8cdf0489ce593
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53569059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd1987c1bd04461c5d204d137d597c1dda018e0d23c6adc0fde6d124c1a3526c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 23:49:34 GMT
ARG CONSUL_VERSION=1.14.0
# Tue, 15 Nov 2022 23:49:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 15 Nov 2022 23:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Nov 2022 23:49:36 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Nov 2022 23:49:45 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Nov 2022 23:49:47 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Nov 2022 23:49:48 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Nov 2022 23:49:48 GMT
VOLUME [/consul/data]
# Tue, 15 Nov 2022 23:49:49 GMT
EXPOSE 8300
# Tue, 15 Nov 2022 23:49:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Nov 2022 23:49:49 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Nov 2022 23:49:49 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Nov 2022 23:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 23:49:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d46f6732f3361c39c017c9813a98e72dee4b0be870b55fbc9dfd44a32aa0615`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ab31975ce52a3dc3769ab782fa4932201b0d58f61baaddbcc199ade6220e0`  
		Last Modified: Tue, 15 Nov 2022 23:50:46 GMT  
		Size: 50.9 MB (50934609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ddfcd0f4ae0b84279348a74fac1e56e704af32e8b87153dbbd06106b996bb`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2f4c860256384e1ad59b3d8f73238f427c1089c7648c42e950577f884c8f32`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4d126dc9cb4c4107e4d3c519fb0704be027dd60a69fd76b8c46735ba3029c5`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.0` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:7b7d2b038889b257d35b2136c15f0846184adeb768a8acbafefac73ceeb1868f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52977520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f10ea9c64d4b00e9b910ac1f3d086e45ec8d6a452b9cf7f7b5548974a88c95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 23:39:23 GMT
ARG CONSUL_VERSION=1.14.0
# Tue, 15 Nov 2022 23:39:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 15 Nov 2022 23:39:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Nov 2022 23:39:24 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Nov 2022 23:39:30 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Nov 2022 23:39:31 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Nov 2022 23:39:31 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Nov 2022 23:39:31 GMT
VOLUME [/consul/data]
# Tue, 15 Nov 2022 23:39:31 GMT
EXPOSE 8300
# Tue, 15 Nov 2022 23:39:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Nov 2022 23:39:31 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Nov 2022 23:39:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Nov 2022 23:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 23:39:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac06a996baf6147b888319bd6784ef204cbe7d61a8ad320aafe35ce7d7bfd789`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531269224bff8dded9d8494dc3d047fd01dd8e5cbfda516bc45586e2d0280aee`  
		Last Modified: Tue, 15 Nov 2022 23:39:53 GMT  
		Size: 50.3 MB (50255697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9219a50b0a5f9585fe647e91fd6353590340b64fb94472becd11ec9dfd7ae4d7`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac7f4108db1d821d2deab163058d322c3064550209a9b487b4a8e5d816be056`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0acd0ba01e973e78cb9e7197802b3f21fc0a903e3580ed2f54b5523117cde6`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.0` - linux; 386

```console
$ docker pull consul@sha256:f25a66a33365bf000da1af9795cc33c3b1d38fd5c871076389737702e848b647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54967457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfe52a88b58d3d694955510c5dcbfa257a3261d64543a44049bcebc0148a244`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 23:40:04 GMT
ARG CONSUL_VERSION=1.14.0
# Tue, 15 Nov 2022 23:40:04 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 15 Nov 2022 23:40:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Nov 2022 23:40:06 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Nov 2022 23:40:14 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Nov 2022 23:40:15 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Nov 2022 23:40:16 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Nov 2022 23:40:17 GMT
VOLUME [/consul/data]
# Tue, 15 Nov 2022 23:40:18 GMT
EXPOSE 8300
# Tue, 15 Nov 2022 23:40:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Nov 2022 23:40:20 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Nov 2022 23:40:22 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Nov 2022 23:40:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 23:40:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0d18046f8061edd59c8ed998cf6dc764cf701a6dd0b6c30d33b1e67ca67eee`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b593f664127c7088ac7c064de125eefd2d8e99951fa06ff8932371da1b9b052`  
		Last Modified: Tue, 15 Nov 2022 23:41:01 GMT  
		Size: 52.1 MB (52135619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c17fbdd942d59ab2d174e42ca2e5d58e7e01b94f54174a3ff737f6285f0fdd9`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f8fbe7050f96ef7d91dd11710cffd7e4d164d2000f11c320a8b89f502d14ba`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a5c5cd06f482ce420d8d33e65b7e65fbb3bfc0fe5fed8547dcb1a22b3e21a4`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:8d6ea7714ae7aa36fd1f4baa4437d27dd231d98801d72b57b207fa18274fcc41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:6afb7a04ee7f088bdc7b08d58b6271b924af3f0b95830e57e355996d05eb6a16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51855936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6608222931a019f0658c775357d35ab0e45321547728eaccef8e7e296e6fb384`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:19:30 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 22:19:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:19:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:19:31 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:19:37 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:19:37 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:19:38 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:19:38 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:19:38 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:19:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:19:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:19:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:19:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:19:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00394ff436377c2ae3f1ca19dfe233d1e943a4a15f98f5e18d7cc8ee507c5aad`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036575c53ebc9949f4aa974af5bc7412dd5f66e5042d35562c44675d74a5e7cb`  
		Last Modified: Thu, 20 Oct 2022 22:20:21 GMT  
		Size: 49.0 MB (49029040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ece016dc23d737e697fc51f2d331e7977cd6af4bd99a864f68f1da58cd91f8`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86338dd101579990eecfc50fd3e93010255265d836d5e22a33d43959e0504ba`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eede053ff767f6f4e47143538c24b94d0d44acb4ff8a085e477eaae46a0a1bd`  
		Last Modified: Thu, 20 Oct 2022 22:20:15 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:4615b6a5ed5f1f1d193bce5f92331c63be4cba7dc6426414ace8cdf0489ce593
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53569059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd1987c1bd04461c5d204d137d597c1dda018e0d23c6adc0fde6d124c1a3526c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 23:49:34 GMT
ARG CONSUL_VERSION=1.14.0
# Tue, 15 Nov 2022 23:49:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 15 Nov 2022 23:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Nov 2022 23:49:36 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Nov 2022 23:49:45 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Nov 2022 23:49:47 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Nov 2022 23:49:48 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Nov 2022 23:49:48 GMT
VOLUME [/consul/data]
# Tue, 15 Nov 2022 23:49:49 GMT
EXPOSE 8300
# Tue, 15 Nov 2022 23:49:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Nov 2022 23:49:49 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Nov 2022 23:49:49 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Nov 2022 23:49:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 23:49:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d46f6732f3361c39c017c9813a98e72dee4b0be870b55fbc9dfd44a32aa0615`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ab31975ce52a3dc3769ab782fa4932201b0d58f61baaddbcc199ade6220e0`  
		Last Modified: Tue, 15 Nov 2022 23:50:46 GMT  
		Size: 50.9 MB (50934609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9ddfcd0f4ae0b84279348a74fac1e56e704af32e8b87153dbbd06106b996bb`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2f4c860256384e1ad59b3d8f73238f427c1089c7648c42e950577f884c8f32`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4d126dc9cb4c4107e4d3c519fb0704be027dd60a69fd76b8c46735ba3029c5`  
		Last Modified: Tue, 15 Nov 2022 23:50:37 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:7b7d2b038889b257d35b2136c15f0846184adeb768a8acbafefac73ceeb1868f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52977520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f10ea9c64d4b00e9b910ac1f3d086e45ec8d6a452b9cf7f7b5548974a88c95`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 23:39:23 GMT
ARG CONSUL_VERSION=1.14.0
# Tue, 15 Nov 2022 23:39:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 15 Nov 2022 23:39:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Nov 2022 23:39:24 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Nov 2022 23:39:30 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Nov 2022 23:39:31 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Nov 2022 23:39:31 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Nov 2022 23:39:31 GMT
VOLUME [/consul/data]
# Tue, 15 Nov 2022 23:39:31 GMT
EXPOSE 8300
# Tue, 15 Nov 2022 23:39:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Nov 2022 23:39:31 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Nov 2022 23:39:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Nov 2022 23:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 23:39:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac06a996baf6147b888319bd6784ef204cbe7d61a8ad320aafe35ce7d7bfd789`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531269224bff8dded9d8494dc3d047fd01dd8e5cbfda516bc45586e2d0280aee`  
		Last Modified: Tue, 15 Nov 2022 23:39:53 GMT  
		Size: 50.3 MB (50255697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9219a50b0a5f9585fe647e91fd6353590340b64fb94472becd11ec9dfd7ae4d7`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac7f4108db1d821d2deab163058d322c3064550209a9b487b4a8e5d816be056`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0acd0ba01e973e78cb9e7197802b3f21fc0a903e3580ed2f54b5523117cde6`  
		Last Modified: Tue, 15 Nov 2022 23:39:48 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:f25a66a33365bf000da1af9795cc33c3b1d38fd5c871076389737702e848b647
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54967457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bfe52a88b58d3d694955510c5dcbfa257a3261d64543a44049bcebc0148a244`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Tue, 15 Nov 2022 23:40:04 GMT
ARG CONSUL_VERSION=1.14.0
# Tue, 15 Nov 2022 23:40:04 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 15 Nov 2022 23:40:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 15 Nov 2022 23:40:06 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 15 Nov 2022 23:40:14 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 15 Nov 2022 23:40:15 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 15 Nov 2022 23:40:16 GMT
# ARGS: CONSUL_VERSION=1.14.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 15 Nov 2022 23:40:17 GMT
VOLUME [/consul/data]
# Tue, 15 Nov 2022 23:40:18 GMT
EXPOSE 8300
# Tue, 15 Nov 2022 23:40:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 15 Nov 2022 23:40:20 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 15 Nov 2022 23:40:22 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 15 Nov 2022 23:40:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 15 Nov 2022 23:40:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0d18046f8061edd59c8ed998cf6dc764cf701a6dd0b6c30d33b1e67ca67eee`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b593f664127c7088ac7c064de125eefd2d8e99951fa06ff8932371da1b9b052`  
		Last Modified: Tue, 15 Nov 2022 23:41:01 GMT  
		Size: 52.1 MB (52135619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c17fbdd942d59ab2d174e42ca2e5d58e7e01b94f54174a3ff737f6285f0fdd9`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68f8fbe7050f96ef7d91dd11710cffd7e4d164d2000f11c320a8b89f502d14ba`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a5c5cd06f482ce420d8d33e65b7e65fbb3bfc0fe5fed8547dcb1a22b3e21a4`  
		Last Modified: Tue, 15 Nov 2022 23:40:56 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
