<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.11`](#consul111)
-	[`consul:1.11.8`](#consul1118)
-	[`consul:1.12`](#consul112)
-	[`consul:1.12.4`](#consul1124)
-	[`consul:1.13`](#consul113)
-	[`consul:1.13.1`](#consul1131)
-	[`consul:latest`](#consullatest)

## `consul:1.11`

```console
$ docker pull consul@sha256:a9854b69e72f7e35fea1bc52cae0313b1ee4877364023cacfc510b1063e9951a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11` - linux; amd64

```console
$ docker pull consul@sha256:9164b6c513fec9a03abc6efe99d9355c589feacbc47225eb96bbfa6ae3a39ba9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (44020540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e56a326ea43b0885cd532da157a5af6dd6c52854797548efbe67d0d8319926c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:19:19 GMT
ARG CONSUL_VERSION=1.11.7
# Tue, 09 Aug 2022 18:19:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 09 Aug 2022 18:19:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 09 Aug 2022 18:19:20 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 09 Aug 2022 18:19:26 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 09 Aug 2022 18:19:27 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 09 Aug 2022 18:19:27 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:19:27 GMT
VOLUME [/consul/data]
# Tue, 09 Aug 2022 18:19:27 GMT
EXPOSE 8300
# Tue, 09 Aug 2022 18:19:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 09 Aug 2022 18:19:28 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 09 Aug 2022 18:19:28 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 09 Aug 2022 18:19:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 18:19:28 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115bd9fd340206331a072729749154d993456e00bb0f277a840ef38ceab8b26b`  
		Last Modified: Tue, 09 Aug 2022 18:20:12 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2844531ef329af6bfb23606f53c4239f8360ccbc91f0063deef0c3bced84712`  
		Last Modified: Tue, 09 Aug 2022 18:20:17 GMT  
		Size: 41.2 MB (41193650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547b9bad8c7936b047f559a82ec8076994fc86fd7a8f16d8bc0f50b87d2e1ee4`  
		Last Modified: Tue, 09 Aug 2022 18:20:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff1ca68141b5e77239e341fc8bbc5bc521162ef2f7544d3606c91cfa23e5177`  
		Last Modified: Tue, 09 Aug 2022 18:20:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1406366761f2acadf0deb7925d86c70c2ad6623b4731c0ab6787212bd8f12ad0`  
		Last Modified: Tue, 09 Aug 2022 18:20:12 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:3e066acf1250fba681ced37371819241261b1b63e5552e55bfd0756f0d6f7e2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41769592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:087fb06329d5932f03c33a1de9df73f0a0a06efdb3d85700a3750a4a83d075f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:49:43 GMT
ARG CONSUL_VERSION=1.11.8
# Thu, 11 Aug 2022 22:49:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:49:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:49:44 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:49:50 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:49:50 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:49:51 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:49:51 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:49:51 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:49:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:49:51 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:49:51 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:49:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:49:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc61f7cd05e3d7c90cfb674f3dcf3e65c0d8fd45abbe1eba0fa287c136900d20`  
		Last Modified: Thu, 11 Aug 2022 22:50:56 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe7a122f926c1df20dce4c7a0b5fc5368b4274fba8e8d982e86591200d1f3ca`  
		Last Modified: Thu, 11 Aug 2022 22:51:02 GMT  
		Size: 39.1 MB (39135087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70386ce0ccfe94c519f4f7cdd9da0e38bff5136309a5408968a64d2f5233729f`  
		Last Modified: Thu, 11 Aug 2022 22:50:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3752d7325172698b30216909bb5ed61116d8664aef4f39d68fd4336dd239dcc`  
		Last Modified: Thu, 11 Aug 2022 22:50:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353df991f0193b44a053d8ba2ca2279a02b86b4bcaeade15f8d97c9f5efcfa17`  
		Last Modified: Thu, 11 Aug 2022 22:50:56 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2b5e3065ab8d9e8f22008c6388e65fda6674a580ad8b3789486b8e236c8e01bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41591497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7761c1facd1786a2796a99f471cdb44e0ca671be562737001b26f4d9b6c110f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:53:18 GMT
ARG CONSUL_VERSION=1.11.8
# Thu, 11 Aug 2022 22:53:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:53:20 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:53:21 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:53:27 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:53:28 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:53:29 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:53:30 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:53:31 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:53:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:53:33 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:53:35 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:53:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:53:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34c13cc2f40d7e602b325187c4d22c8278b9134a91bb22bc700aa0ef687f847`  
		Last Modified: Thu, 11 Aug 2022 22:54:35 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4081125678580515f8106713a13ddabbe7e0fda799a9d87ead562981391f480`  
		Last Modified: Thu, 11 Aug 2022 22:54:40 GMT  
		Size: 38.9 MB (38869738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a61dbb5da06c3a365f08270cdab72a55ece04ed522c2afd0e30210029d9ae8d`  
		Last Modified: Thu, 11 Aug 2022 22:54:35 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ea7acaa756df89e16813df098ab271a610e7a4aee15294c19f97eabc79249d`  
		Last Modified: Thu, 11 Aug 2022 22:54:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59caff0a91576f9bd0386b1b702c36afa07a6e958c549b75b4ceeb1272f4ff`  
		Last Modified: Thu, 11 Aug 2022 22:54:35 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; 386

```console
$ docker pull consul@sha256:d48eae82ffa720e69c308518952b36f26416c1073ea9b588b17e08d0ab1833ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42832685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b3f9ed93658ef308b10f99c7d3bf44da7d997c274bd6a4974c3a0b693088b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:39:12 GMT
ARG CONSUL_VERSION=1.11.8
# Thu, 11 Aug 2022 22:39:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:39:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:39:15 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:39:23 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:39:24 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:39:25 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:39:26 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:39:27 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:39:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:39:29 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:39:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:39:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:39:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef3a923f99a92545cc634b08654c7c82c2772d058b2e8121a1a6b9f6b787a04`  
		Last Modified: Thu, 11 Aug 2022 22:40:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bf6a52577599b8829ebc7498c13c4118339e136e6ea6bcfa55c94155500a04`  
		Last Modified: Thu, 11 Aug 2022 22:40:48 GMT  
		Size: 40.0 MB (40000846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a00837f912ba03de987281d7e299c69eb8297721626dc64c7971bd4ae6ad84a`  
		Last Modified: Thu, 11 Aug 2022 22:40:41 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae27b2088ff6aad72b6285cbe488d9f4f5192f476a3057e6a27036011fee9c7`  
		Last Modified: Thu, 11 Aug 2022 22:40:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf92f61fac3a733bd21af7354f429ddc989f1565ab6a93bfa481d9705cf888`  
		Last Modified: Thu, 11 Aug 2022 22:40:41 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.8`

```console
$ docker pull consul@sha256:cf6ee745543d18094822663735c334d874c6fcec9dab31248aa203543a166a61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:3e066acf1250fba681ced37371819241261b1b63e5552e55bfd0756f0d6f7e2f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41769592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:087fb06329d5932f03c33a1de9df73f0a0a06efdb3d85700a3750a4a83d075f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:49:43 GMT
ARG CONSUL_VERSION=1.11.8
# Thu, 11 Aug 2022 22:49:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:49:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:49:44 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:49:50 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:49:50 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:49:51 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:49:51 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:49:51 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:49:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:49:51 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:49:51 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:49:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:49:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc61f7cd05e3d7c90cfb674f3dcf3e65c0d8fd45abbe1eba0fa287c136900d20`  
		Last Modified: Thu, 11 Aug 2022 22:50:56 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe7a122f926c1df20dce4c7a0b5fc5368b4274fba8e8d982e86591200d1f3ca`  
		Last Modified: Thu, 11 Aug 2022 22:51:02 GMT  
		Size: 39.1 MB (39135087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70386ce0ccfe94c519f4f7cdd9da0e38bff5136309a5408968a64d2f5233729f`  
		Last Modified: Thu, 11 Aug 2022 22:50:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3752d7325172698b30216909bb5ed61116d8664aef4f39d68fd4336dd239dcc`  
		Last Modified: Thu, 11 Aug 2022 22:50:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353df991f0193b44a053d8ba2ca2279a02b86b4bcaeade15f8d97c9f5efcfa17`  
		Last Modified: Thu, 11 Aug 2022 22:50:56 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2b5e3065ab8d9e8f22008c6388e65fda6674a580ad8b3789486b8e236c8e01bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41591497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7761c1facd1786a2796a99f471cdb44e0ca671be562737001b26f4d9b6c110f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:53:18 GMT
ARG CONSUL_VERSION=1.11.8
# Thu, 11 Aug 2022 22:53:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:53:20 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:53:21 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:53:27 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:53:28 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:53:29 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:53:30 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:53:31 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:53:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:53:33 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:53:35 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:53:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:53:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34c13cc2f40d7e602b325187c4d22c8278b9134a91bb22bc700aa0ef687f847`  
		Last Modified: Thu, 11 Aug 2022 22:54:35 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4081125678580515f8106713a13ddabbe7e0fda799a9d87ead562981391f480`  
		Last Modified: Thu, 11 Aug 2022 22:54:40 GMT  
		Size: 38.9 MB (38869738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a61dbb5da06c3a365f08270cdab72a55ece04ed522c2afd0e30210029d9ae8d`  
		Last Modified: Thu, 11 Aug 2022 22:54:35 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ea7acaa756df89e16813df098ab271a610e7a4aee15294c19f97eabc79249d`  
		Last Modified: Thu, 11 Aug 2022 22:54:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b59caff0a91576f9bd0386b1b702c36afa07a6e958c549b75b4ceeb1272f4ff`  
		Last Modified: Thu, 11 Aug 2022 22:54:35 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.8` - linux; 386

```console
$ docker pull consul@sha256:d48eae82ffa720e69c308518952b36f26416c1073ea9b588b17e08d0ab1833ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42832685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b3f9ed93658ef308b10f99c7d3bf44da7d997c274bd6a4974c3a0b693088b7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:39:12 GMT
ARG CONSUL_VERSION=1.11.8
# Thu, 11 Aug 2022 22:39:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:39:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:39:15 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:39:23 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:39:24 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:39:25 GMT
# ARGS: CONSUL_VERSION=1.11.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:39:26 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:39:27 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:39:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:39:29 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:39:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:39:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:39:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef3a923f99a92545cc634b08654c7c82c2772d058b2e8121a1a6b9f6b787a04`  
		Last Modified: Thu, 11 Aug 2022 22:40:41 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4bf6a52577599b8829ebc7498c13c4118339e136e6ea6bcfa55c94155500a04`  
		Last Modified: Thu, 11 Aug 2022 22:40:48 GMT  
		Size: 40.0 MB (40000846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a00837f912ba03de987281d7e299c69eb8297721626dc64c7971bd4ae6ad84a`  
		Last Modified: Thu, 11 Aug 2022 22:40:41 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae27b2088ff6aad72b6285cbe488d9f4f5192f476a3057e6a27036011fee9c7`  
		Last Modified: Thu, 11 Aug 2022 22:40:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1bf92f61fac3a733bd21af7354f429ddc989f1565ab6a93bfa481d9705cf888`  
		Last Modified: Thu, 11 Aug 2022 22:40:41 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12`

```console
$ docker pull consul@sha256:55c2f0fb9b85ed24ed80f9fbbf5e7f71a3bc32cbe719b50054036e269220d4d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.12` - linux; amd64

```console
$ docker pull consul@sha256:80ba62902f5a4dae5ad4810da3eac37cb948ae59a6ec0524465985f44957d9a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49586454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1216943db9d18e2613fd812bd4b6447daeca27b5550fb687f576219cdc5a5080`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:19:08 GMT
ARG CONSUL_VERSION=1.12.3
# Tue, 09 Aug 2022 18:19:08 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 09 Aug 2022 18:19:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 09 Aug 2022 18:19:08 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 09 Aug 2022 18:19:14 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 09 Aug 2022 18:19:14 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 09 Aug 2022 18:19:15 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:19:15 GMT
VOLUME [/consul/data]
# Tue, 09 Aug 2022 18:19:15 GMT
EXPOSE 8300
# Tue, 09 Aug 2022 18:19:15 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 09 Aug 2022 18:19:15 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 09 Aug 2022 18:19:16 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 09 Aug 2022 18:19:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 09 Aug 2022 18:19:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb9e335269b18d0845e0d82b72c7d3d2f0571c5954f6734337b8c4d60d95f65`  
		Last Modified: Tue, 09 Aug 2022 18:19:54 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e4d825a41c32a2e07ecae383245ded626738fc5f86fdd2149b388c164b4c35`  
		Last Modified: Tue, 09 Aug 2022 18:19:59 GMT  
		Size: 46.8 MB (46759568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef5c29d9b704cd1356870c2484a20f546037973d57c0a7c8d8c982ecd28cee51`  
		Last Modified: Tue, 09 Aug 2022 18:19:54 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5dc3bdb3260a4989b28366b5e794b041d63af3ec202f55d0a64ea0c0041942`  
		Last Modified: Tue, 09 Aug 2022 18:19:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c265a329c716dd93cfa6a6def5b846253e9fdb039345f81067aa0db68df70d33`  
		Last Modified: Tue, 09 Aug 2022 18:19:54 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm variant v6

```console
$ docker pull consul@sha256:a1931e72875c50ec991b71d5ef7bdd55e4790526c39d48e0d27abcec95214aa3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47453703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0fcdbc92707c7b87c86cb5608a029399c6d0c5388c69df605e920666884e93`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:49:30 GMT
ARG CONSUL_VERSION=1.12.4
# Thu, 11 Aug 2022 22:49:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:49:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:49:31 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:49:37 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:49:38 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:49:38 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:49:38 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:49:38 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:49:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:49:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:49:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:49:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6451242bec767d620c6265b3112ef194423ce471b51847448023bbf89e67c859`  
		Last Modified: Thu, 11 Aug 2022 22:50:39 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e866c690e9f1ce2e9e0cfdc5c2a54179e7a57c33b8895b23df86e69e326e76`  
		Last Modified: Thu, 11 Aug 2022 22:50:45 GMT  
		Size: 44.8 MB (44819191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f536d4585003b52a82e5f2a64c789361ec98506c162e288868dd6d14443ea534`  
		Last Modified: Thu, 11 Aug 2022 22:50:39 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced22612bddd9b889492fb2bd73cf7ede7760b7c8595077c9c05d6206fe6b2e2`  
		Last Modified: Thu, 11 Aug 2022 22:50:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8c75f862e6f336f55f5a674cac9f77dac78ecf9143db4b92fe421c53adcd3`  
		Last Modified: Thu, 11 Aug 2022 22:50:39 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:43d9ab0dff2cf263dc9e3a063b0c6ecfb89cafd54c9990803440ad33e063ef41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47184100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7efc51542efad08e8232fa2bdde29fc2446437d7cb207595017f49e74b832ab7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:52:56 GMT
ARG CONSUL_VERSION=1.12.4
# Thu, 11 Aug 2022 22:52:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:52:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:52:58 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:53:04 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:53:04 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:53:05 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:53:06 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:53:07 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:53:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:53:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:53:11 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:53:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebc9eb1cad92bea54bd6c8b8d791786c30a59d293c9cde5ef4ea9050fc00f61`  
		Last Modified: Thu, 11 Aug 2022 22:54:18 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97a00cf65dcf0ca3ce31cc5b4b378f809e2860c9fddd222c0a66b08eca909aa`  
		Last Modified: Thu, 11 Aug 2022 22:54:24 GMT  
		Size: 44.5 MB (44462341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7873db2828d0175b1595d51b3083a9261e50fac0884ba114493e6302e47039`  
		Last Modified: Thu, 11 Aug 2022 22:54:19 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d02b0b5227407560e4f127ce71290770398216b737ad583474284fb2f0bb3b`  
		Last Modified: Thu, 11 Aug 2022 22:54:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9df2290d5feaf2da44d94559315440dae60700642668ac0d0303b567a579b5`  
		Last Modified: Thu, 11 Aug 2022 22:54:18 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; 386

```console
$ docker pull consul@sha256:fd2fbd1756ef7044a32f25fce8eaefaf0231a7694511813d4ee685912d65ad6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48650846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc966a2dd18f9b2bc37a41cfbfd0c5a6500ccf0b48b9a1e1cc96b9c50edb11c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:38:46 GMT
ARG CONSUL_VERSION=1.12.4
# Thu, 11 Aug 2022 22:38:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:38:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:38:49 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:38:56 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:38:57 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:38:58 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:38:59 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:39:00 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:39:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:39:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:39:04 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:39:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4c70757d9649000a2128bd4a0ba8db363664760cd2943af7381a483271c605`  
		Last Modified: Thu, 11 Aug 2022 22:40:19 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bedb2aac041d8cff1c1ef05bf4ba0e3ef1c39ea77ed01186e8bb6a7da21dd84b`  
		Last Modified: Thu, 11 Aug 2022 22:40:30 GMT  
		Size: 45.8 MB (45819007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678185050c7ba884397a3481d630c8c28207bac8cde54eb1b982ecb41b46b952`  
		Last Modified: Thu, 11 Aug 2022 22:40:19 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461050fa92fa84b39a85ff7f139a64c70528c802bfed6f5fd0fdbd4b01477155`  
		Last Modified: Thu, 11 Aug 2022 22:40:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61829b5746a0db0bce420420be233c61d316ad2f0816ea1674137933934535ae`  
		Last Modified: Thu, 11 Aug 2022 22:40:19 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12.4`

```console
$ docker pull consul@sha256:16b867311dd11fb6bf6c7ec6c1a2a71a3ec4eca2f06349b1a01b48f192ff905a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.12.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:a1931e72875c50ec991b71d5ef7bdd55e4790526c39d48e0d27abcec95214aa3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47453703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0fcdbc92707c7b87c86cb5608a029399c6d0c5388c69df605e920666884e93`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:49:30 GMT
ARG CONSUL_VERSION=1.12.4
# Thu, 11 Aug 2022 22:49:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:49:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:49:31 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:49:37 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:49:38 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:49:38 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:49:38 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:49:38 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:49:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:49:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:49:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:49:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:49:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6451242bec767d620c6265b3112ef194423ce471b51847448023bbf89e67c859`  
		Last Modified: Thu, 11 Aug 2022 22:50:39 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e866c690e9f1ce2e9e0cfdc5c2a54179e7a57c33b8895b23df86e69e326e76`  
		Last Modified: Thu, 11 Aug 2022 22:50:45 GMT  
		Size: 44.8 MB (44819191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f536d4585003b52a82e5f2a64c789361ec98506c162e288868dd6d14443ea534`  
		Last Modified: Thu, 11 Aug 2022 22:50:39 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced22612bddd9b889492fb2bd73cf7ede7760b7c8595077c9c05d6206fe6b2e2`  
		Last Modified: Thu, 11 Aug 2022 22:50:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b8c75f862e6f336f55f5a674cac9f77dac78ecf9143db4b92fe421c53adcd3`  
		Last Modified: Thu, 11 Aug 2022 22:50:39 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:43d9ab0dff2cf263dc9e3a063b0c6ecfb89cafd54c9990803440ad33e063ef41
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47184100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7efc51542efad08e8232fa2bdde29fc2446437d7cb207595017f49e74b832ab7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:52:56 GMT
ARG CONSUL_VERSION=1.12.4
# Thu, 11 Aug 2022 22:52:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:52:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:52:58 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:53:04 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:53:04 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:53:05 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:53:06 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:53:07 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:53:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:53:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:53:11 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:53:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:53:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eebc9eb1cad92bea54bd6c8b8d791786c30a59d293c9cde5ef4ea9050fc00f61`  
		Last Modified: Thu, 11 Aug 2022 22:54:18 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97a00cf65dcf0ca3ce31cc5b4b378f809e2860c9fddd222c0a66b08eca909aa`  
		Last Modified: Thu, 11 Aug 2022 22:54:24 GMT  
		Size: 44.5 MB (44462341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7873db2828d0175b1595d51b3083a9261e50fac0884ba114493e6302e47039`  
		Last Modified: Thu, 11 Aug 2022 22:54:19 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d02b0b5227407560e4f127ce71290770398216b737ad583474284fb2f0bb3b`  
		Last Modified: Thu, 11 Aug 2022 22:54:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9df2290d5feaf2da44d94559315440dae60700642668ac0d0303b567a579b5`  
		Last Modified: Thu, 11 Aug 2022 22:54:18 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.4` - linux; 386

```console
$ docker pull consul@sha256:fd2fbd1756ef7044a32f25fce8eaefaf0231a7694511813d4ee685912d65ad6d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48650846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bc966a2dd18f9b2bc37a41cfbfd0c5a6500ccf0b48b9a1e1cc96b9c50edb11c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:38:46 GMT
ARG CONSUL_VERSION=1.12.4
# Thu, 11 Aug 2022 22:38:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:38:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:38:49 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:38:56 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:38:57 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:38:58 GMT
# ARGS: CONSUL_VERSION=1.12.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:38:59 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:39:00 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:39:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:39:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:39:04 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:39:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4c70757d9649000a2128bd4a0ba8db363664760cd2943af7381a483271c605`  
		Last Modified: Thu, 11 Aug 2022 22:40:19 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bedb2aac041d8cff1c1ef05bf4ba0e3ef1c39ea77ed01186e8bb6a7da21dd84b`  
		Last Modified: Thu, 11 Aug 2022 22:40:30 GMT  
		Size: 45.8 MB (45819007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678185050c7ba884397a3481d630c8c28207bac8cde54eb1b982ecb41b46b952`  
		Last Modified: Thu, 11 Aug 2022 22:40:19 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461050fa92fa84b39a85ff7f139a64c70528c802bfed6f5fd0fdbd4b01477155`  
		Last Modified: Thu, 11 Aug 2022 22:40:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61829b5746a0db0bce420420be233c61d316ad2f0816ea1674137933934535ae`  
		Last Modified: Thu, 11 Aug 2022 22:40:19 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.13`

```console
$ docker pull consul@sha256:a5a6d5a4b4230561cf34411f6cb1ea7a1e44d203fe49206147dcb2e4c28ba135
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13` - linux; amd64

```console
$ docker pull consul@sha256:e07491091e0c65f27ebe3c4fb037e272b5e7177b1d7f62d08413d46d7c0c03c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51587265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe4f4303f823392f742d6a888860cdaf04917e02ff09aa20bf8d8f3cf5f754f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 22:19:25 GMT
ARG CONSUL_VERSION=1.13.0
# Wed, 10 Aug 2022 22:19:26 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 10 Aug 2022 22:19:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 10 Aug 2022 22:19:26 GMT
# ARGS: CONSUL_VERSION=1.13.0
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 10 Aug 2022 22:19:32 GMT
# ARGS: CONSUL_VERSION=1.13.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 10 Aug 2022 22:19:33 GMT
# ARGS: CONSUL_VERSION=1.13.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 10 Aug 2022 22:19:34 GMT
# ARGS: CONSUL_VERSION=1.13.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Aug 2022 22:19:34 GMT
VOLUME [/consul/data]
# Wed, 10 Aug 2022 22:19:34 GMT
EXPOSE 8300
# Wed, 10 Aug 2022 22:19:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 10 Aug 2022 22:19:34 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 10 Aug 2022 22:19:34 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 22:19:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 22:19:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7328d06cf748717f6da62b95ba4e11134e4e98b458ad31ef6eee48366d7198a8`  
		Last Modified: Wed, 10 Aug 2022 22:19:50 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b8dfedc9911204dac788eda045cc4601c6483d83e4adba3351fefcb9e7313f`  
		Last Modified: Wed, 10 Aug 2022 22:19:56 GMT  
		Size: 48.8 MB (48760375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e534af17d54d07e93288f0c702c7113603b9e19dc3727c1426196919d68d6b64`  
		Last Modified: Wed, 10 Aug 2022 22:19:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f373a77125e024e5f3ff52fd0d420eb19dd120e99f78c06e22d39c0e549dd3`  
		Last Modified: Wed, 10 Aug 2022 22:19:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1a07d3072634144cb7627e32bdc869fbfd8eea0eb12fad426c775aacc96f1b`  
		Last Modified: Wed, 10 Aug 2022 22:19:50 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm variant v6

```console
$ docker pull consul@sha256:cfe6522ba8a80b5adda61f890f3421e9224f202a1896cee285bea74014262c0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49216223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:166066751ddc5bbb28cfbc8ec7b19da95a6bf832860426a30a518337af2a4dc4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:49:16 GMT
ARG CONSUL_VERSION=1.13.1
# Thu, 11 Aug 2022 22:49:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:49:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:49:16 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:49:23 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:49:24 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:49:24 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:49:24 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:49:24 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:49:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:49:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:49:24 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:49:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a829e32ad23591f9d39bd236b8923c091ca0bb3a2f273188265ba15c27c6bf`  
		Last Modified: Thu, 11 Aug 2022 22:50:18 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a70395a8e0716cbe7723ff8bedcad198a0797a795663e35706882e50638bbb0`  
		Last Modified: Thu, 11 Aug 2022 22:50:24 GMT  
		Size: 46.6 MB (46581714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577dac226ce8cb2c9d853fc2767afaa3b0ccf2346c276bac234255f787f192b2`  
		Last Modified: Thu, 11 Aug 2022 22:50:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7927ba3f3e9aed82c3ae348f1ec59bdca100cde7af39746ddfa5fa71050e6e90`  
		Last Modified: Thu, 11 Aug 2022 22:50:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfcbc2d77ace20d9f829bb27117d3dce6ab811392c361a950fc5208e6bc0457`  
		Last Modified: Thu, 11 Aug 2022 22:50:18 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b03945a3170579d7cb0969e0031c45a155a3fd92042c9ad43835f9b848ba11d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48799642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9007f41829e337334d8962243493d29e7f4d5de1a14c3bd8658d17263ebead72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:52:32 GMT
ARG CONSUL_VERSION=1.13.1
# Thu, 11 Aug 2022 22:52:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:52:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:52:35 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:52:41 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:52:42 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:52:43 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:52:44 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:52:45 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:52:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:52:47 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:52:49 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:52:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:52:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2536ca403a04548bf065764eb6239c5cd128363ab5d015dcc387bb4764194e2e`  
		Last Modified: Thu, 11 Aug 2022 22:53:58 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dce7338760e77513deb98c640aaffcff1bd8ab749205d679a9d17d86abc7db5`  
		Last Modified: Thu, 11 Aug 2022 22:54:05 GMT  
		Size: 46.1 MB (46077881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d32d230ac2ed9fc13f3a1bee3e24bfe7dd7e64adb999e92eda4a9cfa347d61`  
		Last Modified: Thu, 11 Aug 2022 22:53:58 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f37d39f0376a55b0681004e9711d1e1305db16ce07fe47e7e07aef2afff2bfc`  
		Last Modified: Thu, 11 Aug 2022 22:53:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2aaa794857d67e9eed2dfb35b6bb52f8b6f1e3fbc0f809d7c5f75be937ea1b`  
		Last Modified: Thu, 11 Aug 2022 22:53:59 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; 386

```console
$ docker pull consul@sha256:439d20f605d70b477e677117878fa2c8337f0b3bab9ccad9b474026f1f7d1b2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50473851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecf23e19c5ce4de455954f8fb10fe1d57b5bdd92c7a99f404b63015c509914c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:38:22 GMT
ARG CONSUL_VERSION=1.13.1
# Thu, 11 Aug 2022 22:38:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:38:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:38:25 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:38:32 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:38:32 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:38:33 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:38:34 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:38:35 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:38:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:38:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:38:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:38:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9a39f2c901b53d3f492284fce6f1e9c4ece8bf134a3405fde8be036d064c21`  
		Last Modified: Thu, 11 Aug 2022 22:39:56 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52437e1ee992db5a9e662a93c29ba94d9aef59a94b7404709f61445520737b7e`  
		Last Modified: Thu, 11 Aug 2022 22:40:04 GMT  
		Size: 47.6 MB (47642014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ab659a8d4e0f4630374a5e26ff79ac3c593b90ebba9f6e8f3987cdd7dcd004`  
		Last Modified: Thu, 11 Aug 2022 22:39:56 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3217697fdc30874e808159dfafe561c84d6e1c42cb4e3e88114ce7ae50c0c1`  
		Last Modified: Thu, 11 Aug 2022 22:39:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58460d57078da0325b7d9180f62ea2cc40675a6ca77cfe89a9e6563140fd179f`  
		Last Modified: Thu, 11 Aug 2022 22:39:57 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.13.1`

```console
$ docker pull consul@sha256:25480cd259a69bff32a789931739f2c7d6be23715e492771611c4d9c6959ac1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:cfe6522ba8a80b5adda61f890f3421e9224f202a1896cee285bea74014262c0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49216223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:166066751ddc5bbb28cfbc8ec7b19da95a6bf832860426a30a518337af2a4dc4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:49:16 GMT
ARG CONSUL_VERSION=1.13.1
# Thu, 11 Aug 2022 22:49:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:49:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:49:16 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:49:23 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:49:24 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:49:24 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:49:24 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:49:24 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:49:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:49:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:49:24 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:49:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a829e32ad23591f9d39bd236b8923c091ca0bb3a2f273188265ba15c27c6bf`  
		Last Modified: Thu, 11 Aug 2022 22:50:18 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a70395a8e0716cbe7723ff8bedcad198a0797a795663e35706882e50638bbb0`  
		Last Modified: Thu, 11 Aug 2022 22:50:24 GMT  
		Size: 46.6 MB (46581714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577dac226ce8cb2c9d853fc2767afaa3b0ccf2346c276bac234255f787f192b2`  
		Last Modified: Thu, 11 Aug 2022 22:50:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7927ba3f3e9aed82c3ae348f1ec59bdca100cde7af39746ddfa5fa71050e6e90`  
		Last Modified: Thu, 11 Aug 2022 22:50:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfcbc2d77ace20d9f829bb27117d3dce6ab811392c361a950fc5208e6bc0457`  
		Last Modified: Thu, 11 Aug 2022 22:50:18 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b03945a3170579d7cb0969e0031c45a155a3fd92042c9ad43835f9b848ba11d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48799642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9007f41829e337334d8962243493d29e7f4d5de1a14c3bd8658d17263ebead72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:52:32 GMT
ARG CONSUL_VERSION=1.13.1
# Thu, 11 Aug 2022 22:52:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:52:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:52:35 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:52:41 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:52:42 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:52:43 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:52:44 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:52:45 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:52:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:52:47 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:52:49 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:52:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:52:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2536ca403a04548bf065764eb6239c5cd128363ab5d015dcc387bb4764194e2e`  
		Last Modified: Thu, 11 Aug 2022 22:53:58 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dce7338760e77513deb98c640aaffcff1bd8ab749205d679a9d17d86abc7db5`  
		Last Modified: Thu, 11 Aug 2022 22:54:05 GMT  
		Size: 46.1 MB (46077881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d32d230ac2ed9fc13f3a1bee3e24bfe7dd7e64adb999e92eda4a9cfa347d61`  
		Last Modified: Thu, 11 Aug 2022 22:53:58 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f37d39f0376a55b0681004e9711d1e1305db16ce07fe47e7e07aef2afff2bfc`  
		Last Modified: Thu, 11 Aug 2022 22:53:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2aaa794857d67e9eed2dfb35b6bb52f8b6f1e3fbc0f809d7c5f75be937ea1b`  
		Last Modified: Thu, 11 Aug 2022 22:53:59 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.1` - linux; 386

```console
$ docker pull consul@sha256:439d20f605d70b477e677117878fa2c8337f0b3bab9ccad9b474026f1f7d1b2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50473851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecf23e19c5ce4de455954f8fb10fe1d57b5bdd92c7a99f404b63015c509914c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:38:22 GMT
ARG CONSUL_VERSION=1.13.1
# Thu, 11 Aug 2022 22:38:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:38:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:38:25 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:38:32 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:38:32 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:38:33 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:38:34 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:38:35 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:38:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:38:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:38:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:38:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9a39f2c901b53d3f492284fce6f1e9c4ece8bf134a3405fde8be036d064c21`  
		Last Modified: Thu, 11 Aug 2022 22:39:56 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52437e1ee992db5a9e662a93c29ba94d9aef59a94b7404709f61445520737b7e`  
		Last Modified: Thu, 11 Aug 2022 22:40:04 GMT  
		Size: 47.6 MB (47642014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ab659a8d4e0f4630374a5e26ff79ac3c593b90ebba9f6e8f3987cdd7dcd004`  
		Last Modified: Thu, 11 Aug 2022 22:39:56 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3217697fdc30874e808159dfafe561c84d6e1c42cb4e3e88114ce7ae50c0c1`  
		Last Modified: Thu, 11 Aug 2022 22:39:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58460d57078da0325b7d9180f62ea2cc40675a6ca77cfe89a9e6563140fd179f`  
		Last Modified: Thu, 11 Aug 2022 22:39:57 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:a5a6d5a4b4230561cf34411f6cb1ea7a1e44d203fe49206147dcb2e4c28ba135
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:e07491091e0c65f27ebe3c4fb037e272b5e7177b1d7f62d08413d46d7c0c03c6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51587265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbe4f4303f823392f742d6a888860cdaf04917e02ff09aa20bf8d8f3cf5f754f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 22:19:25 GMT
ARG CONSUL_VERSION=1.13.0
# Wed, 10 Aug 2022 22:19:26 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 10 Aug 2022 22:19:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 10 Aug 2022 22:19:26 GMT
# ARGS: CONSUL_VERSION=1.13.0
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 10 Aug 2022 22:19:32 GMT
# ARGS: CONSUL_VERSION=1.13.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 10 Aug 2022 22:19:33 GMT
# ARGS: CONSUL_VERSION=1.13.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 10 Aug 2022 22:19:34 GMT
# ARGS: CONSUL_VERSION=1.13.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Aug 2022 22:19:34 GMT
VOLUME [/consul/data]
# Wed, 10 Aug 2022 22:19:34 GMT
EXPOSE 8300
# Wed, 10 Aug 2022 22:19:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 10 Aug 2022 22:19:34 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 10 Aug 2022 22:19:34 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Aug 2022 22:19:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 22:19:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7328d06cf748717f6da62b95ba4e11134e4e98b458ad31ef6eee48366d7198a8`  
		Last Modified: Wed, 10 Aug 2022 22:19:50 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b8dfedc9911204dac788eda045cc4601c6483d83e4adba3351fefcb9e7313f`  
		Last Modified: Wed, 10 Aug 2022 22:19:56 GMT  
		Size: 48.8 MB (48760375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e534af17d54d07e93288f0c702c7113603b9e19dc3727c1426196919d68d6b64`  
		Last Modified: Wed, 10 Aug 2022 22:19:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f373a77125e024e5f3ff52fd0d420eb19dd120e99f78c06e22d39c0e549dd3`  
		Last Modified: Wed, 10 Aug 2022 22:19:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1a07d3072634144cb7627e32bdc869fbfd8eea0eb12fad426c775aacc96f1b`  
		Last Modified: Wed, 10 Aug 2022 22:19:50 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:cfe6522ba8a80b5adda61f890f3421e9224f202a1896cee285bea74014262c0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49216223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:166066751ddc5bbb28cfbc8ec7b19da95a6bf832860426a30a518337af2a4dc4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:49:16 GMT
ARG CONSUL_VERSION=1.13.1
# Thu, 11 Aug 2022 22:49:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:49:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:49:16 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:49:23 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:49:24 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:49:24 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:49:24 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:49:24 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:49:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:49:24 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:49:24 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:49:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:49:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a829e32ad23591f9d39bd236b8923c091ca0bb3a2f273188265ba15c27c6bf`  
		Last Modified: Thu, 11 Aug 2022 22:50:18 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a70395a8e0716cbe7723ff8bedcad198a0797a795663e35706882e50638bbb0`  
		Last Modified: Thu, 11 Aug 2022 22:50:24 GMT  
		Size: 46.6 MB (46581714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577dac226ce8cb2c9d853fc2767afaa3b0ccf2346c276bac234255f787f192b2`  
		Last Modified: Thu, 11 Aug 2022 22:50:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7927ba3f3e9aed82c3ae348f1ec59bdca100cde7af39746ddfa5fa71050e6e90`  
		Last Modified: Thu, 11 Aug 2022 22:50:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfcbc2d77ace20d9f829bb27117d3dce6ab811392c361a950fc5208e6bc0457`  
		Last Modified: Thu, 11 Aug 2022 22:50:18 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b03945a3170579d7cb0969e0031c45a155a3fd92042c9ad43835f9b848ba11d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48799642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9007f41829e337334d8962243493d29e7f4d5de1a14c3bd8658d17263ebead72`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:52:32 GMT
ARG CONSUL_VERSION=1.13.1
# Thu, 11 Aug 2022 22:52:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:52:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:52:35 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:52:41 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:52:42 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:52:43 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:52:44 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:52:45 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:52:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:52:47 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:52:49 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:52:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:52:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2536ca403a04548bf065764eb6239c5cd128363ab5d015dcc387bb4764194e2e`  
		Last Modified: Thu, 11 Aug 2022 22:53:58 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dce7338760e77513deb98c640aaffcff1bd8ab749205d679a9d17d86abc7db5`  
		Last Modified: Thu, 11 Aug 2022 22:54:05 GMT  
		Size: 46.1 MB (46077881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d32d230ac2ed9fc13f3a1bee3e24bfe7dd7e64adb999e92eda4a9cfa347d61`  
		Last Modified: Thu, 11 Aug 2022 22:53:58 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f37d39f0376a55b0681004e9711d1e1305db16ce07fe47e7e07aef2afff2bfc`  
		Last Modified: Thu, 11 Aug 2022 22:53:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2aaa794857d67e9eed2dfb35b6bb52f8b6f1e3fbc0f809d7c5f75be937ea1b`  
		Last Modified: Thu, 11 Aug 2022 22:53:59 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:439d20f605d70b477e677117878fa2c8337f0b3bab9ccad9b474026f1f7d1b2d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50473851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ecf23e19c5ce4de455954f8fb10fe1d57b5bdd92c7a99f404b63015c509914c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 22:38:22 GMT
ARG CONSUL_VERSION=1.13.1
# Thu, 11 Aug 2022 22:38:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 11 Aug 2022 22:38:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 11 Aug 2022 22:38:25 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 11 Aug 2022 22:38:32 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 11 Aug 2022 22:38:32 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 11 Aug 2022 22:38:33 GMT
# ARGS: CONSUL_VERSION=1.13.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 22:38:34 GMT
VOLUME [/consul/data]
# Thu, 11 Aug 2022 22:38:35 GMT
EXPOSE 8300
# Thu, 11 Aug 2022 22:38:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 11 Aug 2022 22:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 11 Aug 2022 22:38:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 11 Aug 2022 22:38:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 22:38:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9a39f2c901b53d3f492284fce6f1e9c4ece8bf134a3405fde8be036d064c21`  
		Last Modified: Thu, 11 Aug 2022 22:39:56 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52437e1ee992db5a9e662a93c29ba94d9aef59a94b7404709f61445520737b7e`  
		Last Modified: Thu, 11 Aug 2022 22:40:04 GMT  
		Size: 47.6 MB (47642014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ab659a8d4e0f4630374a5e26ff79ac3c593b90ebba9f6e8f3987cdd7dcd004`  
		Last Modified: Thu, 11 Aug 2022 22:39:56 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3217697fdc30874e808159dfafe561c84d6e1c42cb4e3e88114ce7ae50c0c1`  
		Last Modified: Thu, 11 Aug 2022 22:39:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58460d57078da0325b7d9180f62ea2cc40675a6ca77cfe89a9e6563140fd179f`  
		Last Modified: Thu, 11 Aug 2022 22:39:57 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
