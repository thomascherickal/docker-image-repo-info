<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.13`](#consul113)
-	[`consul:1.13.7`](#consul1137)
-	[`consul:1.14`](#consul114)
-	[`consul:1.14.6`](#consul1146)
-	[`consul:1.15`](#consul115)
-	[`consul:1.15.2`](#consul1152)
-	[`consul:latest`](#consullatest)

## `consul:1.13`

```console
$ docker pull consul@sha256:04add05a3cde401446ecee85de6c30055a18481f6ecfa59caf609c7991391b3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13` - linux; amd64

```console
$ docker pull consul@sha256:5bc8996c057a1bb615f293c9940fbb1ae264692d0b3adfde3d6dee55ef115688
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52901469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01abd2cb975023f9b7a2c37634ab45f11a3919e320041b4bdd8ff9c513fdf05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:41:53 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 29 Mar 2023 19:41:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 19:41:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 19:41:54 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 19:42:00 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 19:42:00 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 19:42:01 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:42:01 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 19:42:01 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 19:42:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 19:42:01 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 19:42:01 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 19:42:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:42:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97ce603c901e7094c87020e923aeb2b128428cfc680f1f0ab3478e55735d5c9`  
		Last Modified: Wed, 29 Mar 2023 19:42:39 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5db1a9fb0a203781110be9049813e538f5a3abe451e73d06430e0fffb60c53f`  
		Last Modified: Wed, 29 Mar 2023 19:42:45 GMT  
		Size: 50.1 MB (50071496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9203956c7919ff7156b839d9d5405084d65ec5ba7b6dc9341261e2b9ca70549`  
		Last Modified: Wed, 29 Mar 2023 19:42:39 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0ed56e88e35985c34401ee82b19e011398546feae58c0f9a6e937eb4f1d005`  
		Last Modified: Wed, 29 Mar 2023 19:42:39 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694555e962ca7dc0b2061739f4f3fa087eaf02a44be373bdfe0f7d06776c1065`  
		Last Modified: Wed, 29 Mar 2023 19:42:39 GMT  
		Size: 1.8 KB (1784 bytes)  
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
$ docker pull consul@sha256:bd1a959bc9b33cb8a0f1d5a8b23a9a6a192ddd821918d7e726446eaf6c638037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49917738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10bff44ebffac9bc88bb6f42c2db4626b359357f929a70d1407584e5fa520397`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:55:52 GMT
ARG CONSUL_VERSION=1.13.7
# Thu, 30 Mar 2023 03:55:52 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 30 Mar 2023 03:55:52 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Mar 2023 03:55:52 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Mar 2023 03:55:57 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Mar 2023 03:55:58 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Mar 2023 03:55:58 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Mar 2023 03:55:59 GMT
VOLUME [/consul/data]
# Thu, 30 Mar 2023 03:55:59 GMT
EXPOSE 8300
# Thu, 30 Mar 2023 03:55:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Mar 2023 03:55:59 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Mar 2023 03:55:59 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Mar 2023 03:55:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 03:55:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b44f3d8c21792a96353f993bd3186487e14bdefb63f42311cc8043ba230d6e`  
		Last Modified: Thu, 30 Mar 2023 03:56:35 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7876c162dfcf7e0941c27019dea300c38b1a27f573da31b50a06a4904996c`  
		Last Modified: Thu, 30 Mar 2023 03:56:39 GMT  
		Size: 47.2 MB (47192357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e98b006bfb180688415b7b953b482a28a1684619a61289ab899f2faac8ba6e`  
		Last Modified: Thu, 30 Mar 2023 03:56:35 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c3f82d4e6d9992e0f2a9fe515cd7be844a995d51172e8c2495bc4a24d192b`  
		Last Modified: Thu, 30 Mar 2023 03:56:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7970a823b41c1a19c1be8c9a8aaf5f2d104cd92a2a4822087bd5910cb651a32f`  
		Last Modified: Thu, 30 Mar 2023 03:56:35 GMT  
		Size: 1.8 KB (1784 bytes)  
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
$ docker pull consul@sha256:04add05a3cde401446ecee85de6c30055a18481f6ecfa59caf609c7991391b3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13.7` - linux; amd64

```console
$ docker pull consul@sha256:5bc8996c057a1bb615f293c9940fbb1ae264692d0b3adfde3d6dee55ef115688
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52901469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d01abd2cb975023f9b7a2c37634ab45f11a3919e320041b4bdd8ff9c513fdf05`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:41:53 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 29 Mar 2023 19:41:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 19:41:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 19:41:54 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 19:42:00 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 19:42:00 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 19:42:01 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:42:01 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 19:42:01 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 19:42:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 19:42:01 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 19:42:01 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 19:42:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:42:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97ce603c901e7094c87020e923aeb2b128428cfc680f1f0ab3478e55735d5c9`  
		Last Modified: Wed, 29 Mar 2023 19:42:39 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5db1a9fb0a203781110be9049813e538f5a3abe451e73d06430e0fffb60c53f`  
		Last Modified: Wed, 29 Mar 2023 19:42:45 GMT  
		Size: 50.1 MB (50071496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9203956c7919ff7156b839d9d5405084d65ec5ba7b6dc9341261e2b9ca70549`  
		Last Modified: Wed, 29 Mar 2023 19:42:39 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0ed56e88e35985c34401ee82b19e011398546feae58c0f9a6e937eb4f1d005`  
		Last Modified: Wed, 29 Mar 2023 19:42:39 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694555e962ca7dc0b2061739f4f3fa087eaf02a44be373bdfe0f7d06776c1065`  
		Last Modified: Wed, 29 Mar 2023 19:42:39 GMT  
		Size: 1.8 KB (1784 bytes)  
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
$ docker pull consul@sha256:bd1a959bc9b33cb8a0f1d5a8b23a9a6a192ddd821918d7e726446eaf6c638037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49917738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10bff44ebffac9bc88bb6f42c2db4626b359357f929a70d1407584e5fa520397`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:55:52 GMT
ARG CONSUL_VERSION=1.13.7
# Thu, 30 Mar 2023 03:55:52 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 30 Mar 2023 03:55:52 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Mar 2023 03:55:52 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Mar 2023 03:55:57 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Mar 2023 03:55:58 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Mar 2023 03:55:58 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Mar 2023 03:55:59 GMT
VOLUME [/consul/data]
# Thu, 30 Mar 2023 03:55:59 GMT
EXPOSE 8300
# Thu, 30 Mar 2023 03:55:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Mar 2023 03:55:59 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Mar 2023 03:55:59 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Mar 2023 03:55:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 03:55:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b44f3d8c21792a96353f993bd3186487e14bdefb63f42311cc8043ba230d6e`  
		Last Modified: Thu, 30 Mar 2023 03:56:35 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7876c162dfcf7e0941c27019dea300c38b1a27f573da31b50a06a4904996c`  
		Last Modified: Thu, 30 Mar 2023 03:56:39 GMT  
		Size: 47.2 MB (47192357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e98b006bfb180688415b7b953b482a28a1684619a61289ab899f2faac8ba6e`  
		Last Modified: Thu, 30 Mar 2023 03:56:35 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f67c3f82d4e6d9992e0f2a9fe515cd7be844a995d51172e8c2495bc4a24d192b`  
		Last Modified: Thu, 30 Mar 2023 03:56:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7970a823b41c1a19c1be8c9a8aaf5f2d104cd92a2a4822087bd5910cb651a32f`  
		Last Modified: Thu, 30 Mar 2023 03:56:35 GMT  
		Size: 1.8 KB (1784 bytes)  
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
$ docker pull consul@sha256:93677eaa6bf1025787a93ac35519bfb3311ca4e809df3c416ae26cca10ff18a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14` - linux; amd64

```console
$ docker pull consul@sha256:307908ceb07d639ec15b0c3087a74c7a21d6d9534bc356fc78288152eeef10a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56198093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fc55119ea2b76a475fa9d2eb56f2b6862466eff1444928aa153cb6087e39c04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 06 Apr 2023 00:42:26 GMT
ARG CONSUL_VERSION=1.14.6
# Thu, 06 Apr 2023 00:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Apr 2023 00:42:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Apr 2023 00:42:27 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Apr 2023 00:42:33 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Apr 2023 00:42:33 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Apr 2023 00:42:34 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Apr 2023 00:42:34 GMT
VOLUME [/consul/data]
# Thu, 06 Apr 2023 00:42:34 GMT
EXPOSE 8300
# Thu, 06 Apr 2023 00:42:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Apr 2023 00:42:34 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Apr 2023 00:42:34 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Apr 2023 00:42:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Apr 2023 00:42:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766a40ab52bd0288ceb79c119ac9d2cfaa18d4e1023e61c6ca05380b21f30204`  
		Last Modified: Thu, 06 Apr 2023 00:43:04 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1945ba49379162c18e23619c6af14482d6fb0b9a9de78116c54fbb53d7c8d1`  
		Last Modified: Thu, 06 Apr 2023 00:43:10 GMT  
		Size: 53.4 MB (53368073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d776f2bce4653c14139846bb76c437ffcdab35a6200893bb818cbaa503db5`  
		Last Modified: Thu, 06 Apr 2023 00:43:04 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3172e8000cc2e1152688f41dae704eab4ff2adaf368e61d2b81c6dc1eed4bc`  
		Last Modified: Thu, 06 Apr 2023 00:43:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6354f11bfa45e8718a6e5ef1faae0576f84995ac93aec8683d1db6df311a1e1`  
		Last Modified: Thu, 06 Apr 2023 00:43:04 GMT  
		Size: 1.8 KB (1831 bytes)  
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
$ docker pull consul@sha256:7a41e8ddf32decc1d3b87ee60f3542544e8e0f837dbc65b65d8ea1080b8d2917
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53013945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24116fe44782e7fa5659d7756dab9a63f41ffe22044aeb24488e5268fd2fd422`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Wed, 05 Apr 2023 21:39:28 GMT
ARG CONSUL_VERSION=1.14.6
# Wed, 05 Apr 2023 21:39:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 05 Apr 2023 21:39:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 05 Apr 2023 21:39:28 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 05 Apr 2023 21:39:34 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 05 Apr 2023 21:39:35 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 05 Apr 2023 21:39:35 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 05 Apr 2023 21:39:35 GMT
VOLUME [/consul/data]
# Wed, 05 Apr 2023 21:39:35 GMT
EXPOSE 8300
# Wed, 05 Apr 2023 21:39:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 05 Apr 2023 21:39:35 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 05 Apr 2023 21:39:35 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 05 Apr 2023 21:39:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Apr 2023 21:39:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef87d286cd75f76b175e0df1000ad1780d00a38b47a75bc1063bc4ea0ae506`  
		Last Modified: Wed, 05 Apr 2023 21:40:00 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527fbc5532484069328ff2b26ac9b10ec5d7b311213922eae4c1445a7f41c523`  
		Last Modified: Wed, 05 Apr 2023 21:40:05 GMT  
		Size: 50.3 MB (50288510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161215c14995100d777d55dd50f4ccdc47b50673149e1895b610789cc7232c26`  
		Last Modified: Wed, 05 Apr 2023 21:40:00 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342fb6d7ea203e62320cf723a25279fcbbbe90f3a74c063e4d64eb4b92351629`  
		Last Modified: Wed, 05 Apr 2023 21:40:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5eb6aa68deb8626207bd4a4d9d0c763166be2a3e1a20c6cfcbd6a627f1f76e`  
		Last Modified: Wed, 05 Apr 2023 21:40:00 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; 386

```console
$ docker pull consul@sha256:aa4c418fc4fa5b5cc7e73e36c368549399f2938e8b85e49b0ed939a3140bc05c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54860825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b459e939bd1c3a8d05d55240489eeaef960332b2df3f49b27a47eeb72ed475a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 05 Apr 2023 21:38:27 GMT
ARG CONSUL_VERSION=1.14.6
# Wed, 05 Apr 2023 21:38:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 05 Apr 2023 21:38:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 05 Apr 2023 21:38:28 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 05 Apr 2023 21:38:36 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 05 Apr 2023 21:38:36 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 05 Apr 2023 21:38:37 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 05 Apr 2023 21:38:37 GMT
VOLUME [/consul/data]
# Wed, 05 Apr 2023 21:38:37 GMT
EXPOSE 8300
# Wed, 05 Apr 2023 21:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 05 Apr 2023 21:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 05 Apr 2023 21:38:38 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 05 Apr 2023 21:38:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Apr 2023 21:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae18c92befa8a646902059c6dcd4b6130af39572a9ed4e4e3e90a9f565db122`  
		Last Modified: Wed, 05 Apr 2023 21:39:07 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0605026de461acc24885a3cee5e1a9f56da2c71a0a0dce712bf660099a1c1b92`  
		Last Modified: Wed, 05 Apr 2023 21:39:15 GMT  
		Size: 52.0 MB (52024817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044e7bd27d40529e870e2801596c82d4a40ada1f4b3406d5861d5178d3cd285a`  
		Last Modified: Wed, 05 Apr 2023 21:39:07 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d860cf7f2822a2da2cf8dde8c1cb291dd332a8523707d655658da17863940ca9`  
		Last Modified: Wed, 05 Apr 2023 21:39:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e64295ccf101b2698d9e3961340e989d1a202060da7c1ec9d05ad6c51f1fdf`  
		Last Modified: Wed, 05 Apr 2023 21:39:07 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.14.6`

```console
$ docker pull consul@sha256:0a845786ae1ae26ed096c5d7551df6cd1fcaa45d37690ee1e5dcb15270db9746
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14.6` - linux; amd64

```console
$ docker pull consul@sha256:307908ceb07d639ec15b0c3087a74c7a21d6d9534bc356fc78288152eeef10a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56198093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fc55119ea2b76a475fa9d2eb56f2b6862466eff1444928aa153cb6087e39c04`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 06 Apr 2023 00:42:26 GMT
ARG CONSUL_VERSION=1.14.6
# Thu, 06 Apr 2023 00:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Apr 2023 00:42:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Apr 2023 00:42:27 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Apr 2023 00:42:33 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Apr 2023 00:42:33 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Apr 2023 00:42:34 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Apr 2023 00:42:34 GMT
VOLUME [/consul/data]
# Thu, 06 Apr 2023 00:42:34 GMT
EXPOSE 8300
# Thu, 06 Apr 2023 00:42:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Apr 2023 00:42:34 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Apr 2023 00:42:34 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Apr 2023 00:42:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Apr 2023 00:42:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766a40ab52bd0288ceb79c119ac9d2cfaa18d4e1023e61c6ca05380b21f30204`  
		Last Modified: Thu, 06 Apr 2023 00:43:04 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1945ba49379162c18e23619c6af14482d6fb0b9a9de78116c54fbb53d7c8d1`  
		Last Modified: Thu, 06 Apr 2023 00:43:10 GMT  
		Size: 53.4 MB (53368073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4d776f2bce4653c14139846bb76c437ffcdab35a6200893bb818cbaa503db5`  
		Last Modified: Thu, 06 Apr 2023 00:43:04 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c3172e8000cc2e1152688f41dae704eab4ff2adaf368e61d2b81c6dc1eed4bc`  
		Last Modified: Thu, 06 Apr 2023 00:43:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6354f11bfa45e8718a6e5ef1faae0576f84995ac93aec8683d1db6df311a1e1`  
		Last Modified: Thu, 06 Apr 2023 00:43:04 GMT  
		Size: 1.8 KB (1831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:7a41e8ddf32decc1d3b87ee60f3542544e8e0f837dbc65b65d8ea1080b8d2917
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53013945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24116fe44782e7fa5659d7756dab9a63f41ffe22044aeb24488e5268fd2fd422`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Wed, 05 Apr 2023 21:39:28 GMT
ARG CONSUL_VERSION=1.14.6
# Wed, 05 Apr 2023 21:39:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 05 Apr 2023 21:39:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 05 Apr 2023 21:39:28 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 05 Apr 2023 21:39:34 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 05 Apr 2023 21:39:35 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 05 Apr 2023 21:39:35 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 05 Apr 2023 21:39:35 GMT
VOLUME [/consul/data]
# Wed, 05 Apr 2023 21:39:35 GMT
EXPOSE 8300
# Wed, 05 Apr 2023 21:39:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 05 Apr 2023 21:39:35 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 05 Apr 2023 21:39:35 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 05 Apr 2023 21:39:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Apr 2023 21:39:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef87d286cd75f76b175e0df1000ad1780d00a38b47a75bc1063bc4ea0ae506`  
		Last Modified: Wed, 05 Apr 2023 21:40:00 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527fbc5532484069328ff2b26ac9b10ec5d7b311213922eae4c1445a7f41c523`  
		Last Modified: Wed, 05 Apr 2023 21:40:05 GMT  
		Size: 50.3 MB (50288510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161215c14995100d777d55dd50f4ccdc47b50673149e1895b610789cc7232c26`  
		Last Modified: Wed, 05 Apr 2023 21:40:00 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342fb6d7ea203e62320cf723a25279fcbbbe90f3a74c063e4d64eb4b92351629`  
		Last Modified: Wed, 05 Apr 2023 21:40:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5eb6aa68deb8626207bd4a4d9d0c763166be2a3e1a20c6cfcbd6a627f1f76e`  
		Last Modified: Wed, 05 Apr 2023 21:40:00 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.6` - linux; 386

```console
$ docker pull consul@sha256:aa4c418fc4fa5b5cc7e73e36c368549399f2938e8b85e49b0ed939a3140bc05c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54860825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b459e939bd1c3a8d05d55240489eeaef960332b2df3f49b27a47eeb72ed475a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 05 Apr 2023 21:38:27 GMT
ARG CONSUL_VERSION=1.14.6
# Wed, 05 Apr 2023 21:38:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 05 Apr 2023 21:38:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 05 Apr 2023 21:38:28 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 05 Apr 2023 21:38:36 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 05 Apr 2023 21:38:36 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 05 Apr 2023 21:38:37 GMT
# ARGS: CONSUL_VERSION=1.14.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 05 Apr 2023 21:38:37 GMT
VOLUME [/consul/data]
# Wed, 05 Apr 2023 21:38:37 GMT
EXPOSE 8300
# Wed, 05 Apr 2023 21:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 05 Apr 2023 21:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 05 Apr 2023 21:38:38 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 05 Apr 2023 21:38:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Apr 2023 21:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae18c92befa8a646902059c6dcd4b6130af39572a9ed4e4e3e90a9f565db122`  
		Last Modified: Wed, 05 Apr 2023 21:39:07 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0605026de461acc24885a3cee5e1a9f56da2c71a0a0dce712bf660099a1c1b92`  
		Last Modified: Wed, 05 Apr 2023 21:39:15 GMT  
		Size: 52.0 MB (52024817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044e7bd27d40529e870e2801596c82d4a40ada1f4b3406d5861d5178d3cd285a`  
		Last Modified: Wed, 05 Apr 2023 21:39:07 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d860cf7f2822a2da2cf8dde8c1cb291dd332a8523707d655658da17863940ca9`  
		Last Modified: Wed, 05 Apr 2023 21:39:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6e64295ccf101b2698d9e3961340e989d1a202060da7c1ec9d05ad6c51f1fdf`  
		Last Modified: Wed, 05 Apr 2023 21:39:07 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.15`

```console
$ docker pull consul@sha256:45382eda8ea18e49e5de659258b1ac85adfd5030a9ccf5918f0405cf04a4c33b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.15` - linux; amd64

```console
$ docker pull consul@sha256:3f274bcbebc9bf00aeaca52e017c69c91291097eb42d0222db6e772b62cf6ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57884738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90b65cf94569cb74e2385cf536270955f34035cbef796424dba86d1c2597cc9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 06 Apr 2023 00:42:15 GMT
ARG CONSUL_VERSION=1.15.2
# Thu, 06 Apr 2023 00:42:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Apr 2023 00:42:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Apr 2023 00:42:16 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Apr 2023 00:42:22 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Apr 2023 00:42:22 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Apr 2023 00:42:23 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Apr 2023 00:42:23 GMT
VOLUME [/consul/data]
# Thu, 06 Apr 2023 00:42:23 GMT
EXPOSE 8300
# Thu, 06 Apr 2023 00:42:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Apr 2023 00:42:23 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Apr 2023 00:42:23 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Apr 2023 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Apr 2023 00:42:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7eaa7623341dcdcd19667586a357f9fa1f16a516cfca1708ea42a939edd103f`  
		Last Modified: Thu, 06 Apr 2023 00:42:47 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab5510ca10cd210f1addfb06722800a94f5f86d8451860f4b53d5570851549b`  
		Last Modified: Thu, 06 Apr 2023 00:42:54 GMT  
		Size: 55.1 MB (55054712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d644556841f7b410e0b46c716eb24a38c533dc437409dcc271404cf5cef2764`  
		Last Modified: Thu, 06 Apr 2023 00:42:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8f4ec7d14f832b39d6e0040926d3dbb86418538877ad74a984e0b04e720dc6`  
		Last Modified: Thu, 06 Apr 2023 00:42:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2203105424481f400c06fced45cb4377e6687d32cfe1c94f670151dc8e998c81`  
		Last Modified: Thu, 06 Apr 2023 00:42:47 GMT  
		Size: 1.8 KB (1833 bytes)  
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
$ docker pull consul@sha256:52cfe5ca87cd6d9eee367728e49ca8519ac5ca2b8a8e0874f2bebecfb1fe4da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54616131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1c43c667c1541ff08e60fa3d7bc240f6ba68b1c5db00da73799437c3f368bf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Wed, 05 Apr 2023 21:39:19 GMT
ARG CONSUL_VERSION=1.15.2
# Wed, 05 Apr 2023 21:39:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 05 Apr 2023 21:39:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 05 Apr 2023 21:39:19 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 05 Apr 2023 21:39:25 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 05 Apr 2023 21:39:26 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 05 Apr 2023 21:39:26 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 05 Apr 2023 21:39:26 GMT
VOLUME [/consul/data]
# Wed, 05 Apr 2023 21:39:26 GMT
EXPOSE 8300
# Wed, 05 Apr 2023 21:39:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 05 Apr 2023 21:39:26 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 05 Apr 2023 21:39:27 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 05 Apr 2023 21:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Apr 2023 21:39:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c4ac647a9065ab2457edc74cf3474ff3fc0f99abb0f4bcdeedefae76d7a18`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a881b25c6d47c862c7a9a94d962f5c32d09001dbf69c93a511a21967858d1e0`  
		Last Modified: Wed, 05 Apr 2023 21:39:49 GMT  
		Size: 51.9 MB (51890697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c0f54213a586f33bffb0129217b1880aeae49608b246c5ea3cd4d108b89afc`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968d2f636f50783cb1a0d980fa3563f2e1968181938ef5ba0b7f3909a130cfae`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e983f78d40d7e93f4db18e98a5bae1148ab5501e725f677717b95c301fbf8b`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15` - linux; 386

```console
$ docker pull consul@sha256:c26e328afd45439d21af8047f0161128a5211f80637fb419cc5d382f06bd563a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56491277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:997c75dc349d14caa8c1d1bb2e03107364426b2299dee87597dde7d44c0f3b1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 05 Apr 2023 21:38:14 GMT
ARG CONSUL_VERSION=1.15.2
# Wed, 05 Apr 2023 21:38:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 05 Apr 2023 21:38:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 05 Apr 2023 21:38:15 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 05 Apr 2023 21:38:23 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 05 Apr 2023 21:38:24 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 05 Apr 2023 21:38:24 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 05 Apr 2023 21:38:24 GMT
VOLUME [/consul/data]
# Wed, 05 Apr 2023 21:38:24 GMT
EXPOSE 8300
# Wed, 05 Apr 2023 21:38:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 05 Apr 2023 21:38:24 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 05 Apr 2023 21:38:25 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 05 Apr 2023 21:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Apr 2023 21:38:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6566a12b4567db564f9ccefa1b2b956260bdfa6434af3aebc63e18ec73d9f2`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54aeeb52b806f12c3014fb42c9e0d8b4eea07d122a320d586ab6a41c2d1995d`  
		Last Modified: Wed, 05 Apr 2023 21:38:57 GMT  
		Size: 53.7 MB (53655268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49a004da8a6887dc498c65616da55ee9d58f2fcc89b8ca85eea0ddf67372d14`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a5e9b64b62d1d42540d622638324f184b555fbd13c5ad5fb7a79919949fe59`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6535a01cb5522906a5a7255cae41ee4f47a1f275dda3562f2b815234d9de6989`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.15.2`

```console
$ docker pull consul@sha256:9e6dbebd3f728709b52f72f0d29a6f93cdce33f6eda758e7de3769cc8846b651
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.15.2` - linux; amd64

```console
$ docker pull consul@sha256:3f274bcbebc9bf00aeaca52e017c69c91291097eb42d0222db6e772b62cf6ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57884738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90b65cf94569cb74e2385cf536270955f34035cbef796424dba86d1c2597cc9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 06 Apr 2023 00:42:15 GMT
ARG CONSUL_VERSION=1.15.2
# Thu, 06 Apr 2023 00:42:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Apr 2023 00:42:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Apr 2023 00:42:16 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Apr 2023 00:42:22 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Apr 2023 00:42:22 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Apr 2023 00:42:23 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Apr 2023 00:42:23 GMT
VOLUME [/consul/data]
# Thu, 06 Apr 2023 00:42:23 GMT
EXPOSE 8300
# Thu, 06 Apr 2023 00:42:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Apr 2023 00:42:23 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Apr 2023 00:42:23 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Apr 2023 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Apr 2023 00:42:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7eaa7623341dcdcd19667586a357f9fa1f16a516cfca1708ea42a939edd103f`  
		Last Modified: Thu, 06 Apr 2023 00:42:47 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab5510ca10cd210f1addfb06722800a94f5f86d8451860f4b53d5570851549b`  
		Last Modified: Thu, 06 Apr 2023 00:42:54 GMT  
		Size: 55.1 MB (55054712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d644556841f7b410e0b46c716eb24a38c533dc437409dcc271404cf5cef2764`  
		Last Modified: Thu, 06 Apr 2023 00:42:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8f4ec7d14f832b39d6e0040926d3dbb86418538877ad74a984e0b04e720dc6`  
		Last Modified: Thu, 06 Apr 2023 00:42:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2203105424481f400c06fced45cb4377e6687d32cfe1c94f670151dc8e998c81`  
		Last Modified: Thu, 06 Apr 2023 00:42:47 GMT  
		Size: 1.8 KB (1833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15.2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:52cfe5ca87cd6d9eee367728e49ca8519ac5ca2b8a8e0874f2bebecfb1fe4da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54616131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1c43c667c1541ff08e60fa3d7bc240f6ba68b1c5db00da73799437c3f368bf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Wed, 05 Apr 2023 21:39:19 GMT
ARG CONSUL_VERSION=1.15.2
# Wed, 05 Apr 2023 21:39:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 05 Apr 2023 21:39:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 05 Apr 2023 21:39:19 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 05 Apr 2023 21:39:25 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 05 Apr 2023 21:39:26 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 05 Apr 2023 21:39:26 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 05 Apr 2023 21:39:26 GMT
VOLUME [/consul/data]
# Wed, 05 Apr 2023 21:39:26 GMT
EXPOSE 8300
# Wed, 05 Apr 2023 21:39:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 05 Apr 2023 21:39:26 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 05 Apr 2023 21:39:27 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 05 Apr 2023 21:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Apr 2023 21:39:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c4ac647a9065ab2457edc74cf3474ff3fc0f99abb0f4bcdeedefae76d7a18`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a881b25c6d47c862c7a9a94d962f5c32d09001dbf69c93a511a21967858d1e0`  
		Last Modified: Wed, 05 Apr 2023 21:39:49 GMT  
		Size: 51.9 MB (51890697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c0f54213a586f33bffb0129217b1880aeae49608b246c5ea3cd4d108b89afc`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968d2f636f50783cb1a0d980fa3563f2e1968181938ef5ba0b7f3909a130cfae`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e983f78d40d7e93f4db18e98a5bae1148ab5501e725f677717b95c301fbf8b`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15.2` - linux; 386

```console
$ docker pull consul@sha256:c26e328afd45439d21af8047f0161128a5211f80637fb419cc5d382f06bd563a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56491277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:997c75dc349d14caa8c1d1bb2e03107364426b2299dee87597dde7d44c0f3b1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 05 Apr 2023 21:38:14 GMT
ARG CONSUL_VERSION=1.15.2
# Wed, 05 Apr 2023 21:38:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 05 Apr 2023 21:38:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 05 Apr 2023 21:38:15 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 05 Apr 2023 21:38:23 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 05 Apr 2023 21:38:24 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 05 Apr 2023 21:38:24 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 05 Apr 2023 21:38:24 GMT
VOLUME [/consul/data]
# Wed, 05 Apr 2023 21:38:24 GMT
EXPOSE 8300
# Wed, 05 Apr 2023 21:38:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 05 Apr 2023 21:38:24 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 05 Apr 2023 21:38:25 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 05 Apr 2023 21:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Apr 2023 21:38:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6566a12b4567db564f9ccefa1b2b956260bdfa6434af3aebc63e18ec73d9f2`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54aeeb52b806f12c3014fb42c9e0d8b4eea07d122a320d586ab6a41c2d1995d`  
		Last Modified: Wed, 05 Apr 2023 21:38:57 GMT  
		Size: 53.7 MB (53655268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49a004da8a6887dc498c65616da55ee9d58f2fcc89b8ca85eea0ddf67372d14`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a5e9b64b62d1d42540d622638324f184b555fbd13c5ad5fb7a79919949fe59`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6535a01cb5522906a5a7255cae41ee4f47a1f275dda3562f2b815234d9de6989`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:45382eda8ea18e49e5de659258b1ac85adfd5030a9ccf5918f0405cf04a4c33b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:3f274bcbebc9bf00aeaca52e017c69c91291097eb42d0222db6e772b62cf6ce0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57884738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90b65cf94569cb74e2385cf536270955f34035cbef796424dba86d1c2597cc9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Thu, 06 Apr 2023 00:42:15 GMT
ARG CONSUL_VERSION=1.15.2
# Thu, 06 Apr 2023 00:42:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Apr 2023 00:42:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Apr 2023 00:42:16 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Apr 2023 00:42:22 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Apr 2023 00:42:22 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Apr 2023 00:42:23 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Apr 2023 00:42:23 GMT
VOLUME [/consul/data]
# Thu, 06 Apr 2023 00:42:23 GMT
EXPOSE 8300
# Thu, 06 Apr 2023 00:42:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Apr 2023 00:42:23 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Apr 2023 00:42:23 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Apr 2023 00:42:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Apr 2023 00:42:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7eaa7623341dcdcd19667586a357f9fa1f16a516cfca1708ea42a939edd103f`  
		Last Modified: Thu, 06 Apr 2023 00:42:47 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ab5510ca10cd210f1addfb06722800a94f5f86d8451860f4b53d5570851549b`  
		Last Modified: Thu, 06 Apr 2023 00:42:54 GMT  
		Size: 55.1 MB (55054712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d644556841f7b410e0b46c716eb24a38c533dc437409dcc271404cf5cef2764`  
		Last Modified: Thu, 06 Apr 2023 00:42:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8f4ec7d14f832b39d6e0040926d3dbb86418538877ad74a984e0b04e720dc6`  
		Last Modified: Thu, 06 Apr 2023 00:42:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2203105424481f400c06fced45cb4377e6687d32cfe1c94f670151dc8e998c81`  
		Last Modified: Thu, 06 Apr 2023 00:42:47 GMT  
		Size: 1.8 KB (1833 bytes)  
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
$ docker pull consul@sha256:52cfe5ca87cd6d9eee367728e49ca8519ac5ca2b8a8e0874f2bebecfb1fe4da5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54616131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1c43c667c1541ff08e60fa3d7bc240f6ba68b1c5db00da73799437c3f368bf3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Wed, 05 Apr 2023 21:39:19 GMT
ARG CONSUL_VERSION=1.15.2
# Wed, 05 Apr 2023 21:39:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 05 Apr 2023 21:39:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 05 Apr 2023 21:39:19 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 05 Apr 2023 21:39:25 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 05 Apr 2023 21:39:26 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 05 Apr 2023 21:39:26 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 05 Apr 2023 21:39:26 GMT
VOLUME [/consul/data]
# Wed, 05 Apr 2023 21:39:26 GMT
EXPOSE 8300
# Wed, 05 Apr 2023 21:39:26 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 05 Apr 2023 21:39:26 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 05 Apr 2023 21:39:27 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 05 Apr 2023 21:39:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Apr 2023 21:39:27 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7c4ac647a9065ab2457edc74cf3474ff3fc0f99abb0f4bcdeedefae76d7a18`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a881b25c6d47c862c7a9a94d962f5c32d09001dbf69c93a511a21967858d1e0`  
		Last Modified: Wed, 05 Apr 2023 21:39:49 GMT  
		Size: 51.9 MB (51890697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c0f54213a586f33bffb0129217b1880aeae49608b246c5ea3cd4d108b89afc`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968d2f636f50783cb1a0d980fa3563f2e1968181938ef5ba0b7f3909a130cfae`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e983f78d40d7e93f4db18e98a5bae1148ab5501e725f677717b95c301fbf8b`  
		Last Modified: Wed, 05 Apr 2023 21:39:45 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:c26e328afd45439d21af8047f0161128a5211f80637fb419cc5d382f06bd563a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56491277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:997c75dc349d14caa8c1d1bb2e03107364426b2299dee87597dde7d44c0f3b1a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:36 GMT
ADD file:fca96dde137b6b045359aec9d24257996738ac6cb7cce9518460a66802a27bd7 in / 
# Wed, 29 Mar 2023 17:38:36 GMT
CMD ["/bin/sh"]
# Wed, 05 Apr 2023 21:38:14 GMT
ARG CONSUL_VERSION=1.15.2
# Wed, 05 Apr 2023 21:38:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 05 Apr 2023 21:38:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 05 Apr 2023 21:38:15 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 05 Apr 2023 21:38:23 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 05 Apr 2023 21:38:24 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 05 Apr 2023 21:38:24 GMT
# ARGS: CONSUL_VERSION=1.15.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 05 Apr 2023 21:38:24 GMT
VOLUME [/consul/data]
# Wed, 05 Apr 2023 21:38:24 GMT
EXPOSE 8300
# Wed, 05 Apr 2023 21:38:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 05 Apr 2023 21:38:24 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 05 Apr 2023 21:38:25 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 05 Apr 2023 21:38:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 05 Apr 2023 21:38:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:333f5f619d7efe58316b2d71276f19d0a59bcb471f4dadaa85762b2c9e02775c`  
		Last Modified: Wed, 29 Mar 2023 17:39:19 GMT  
		Size: 2.8 MB (2832576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6566a12b4567db564f9ccefa1b2b956260bdfa6434af3aebc63e18ec73d9f2`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54aeeb52b806f12c3014fb42c9e0d8b4eea07d122a320d586ab6a41c2d1995d`  
		Last Modified: Wed, 05 Apr 2023 21:38:57 GMT  
		Size: 53.7 MB (53655268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49a004da8a6887dc498c65616da55ee9d58f2fcc89b8ca85eea0ddf67372d14`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a5e9b64b62d1d42540d622638324f184b555fbd13c5ad5fb7a79919949fe59`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6535a01cb5522906a5a7255cae41ee4f47a1f275dda3562f2b815234d9de6989`  
		Last Modified: Wed, 05 Apr 2023 21:38:49 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
