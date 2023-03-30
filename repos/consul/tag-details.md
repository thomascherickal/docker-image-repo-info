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
$ docker pull consul@sha256:6e1f152161b0e2e3244073d6598fb2855634f0495ec573aa2e50f27762d0fd2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14` - linux; amd64

```console
$ docker pull consul@sha256:9c0fcf269c0c4eda29b0d1b8e4abd7bb2fe4f6c249bb63cc3eab07bd0186a72c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.3 MB (56276647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff07597da659672c93112c25363069d4e84c72260d491a973dc45b36b6269fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:41:42 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 29 Mar 2023 19:41:42 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 19:41:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 19:41:43 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 19:41:49 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 19:41:50 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 19:41:50 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:41:50 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 19:41:50 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 19:41:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 19:41:50 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 19:41:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 19:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:41:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d3bc1fe58aeeb4895a6a34841a464be34d553c7529c19d7cda9296a48f198`  
		Last Modified: Wed, 29 Mar 2023 19:42:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cfd612915e47e2c834eb37813d96c38b6ace9de7944df5f621f0263baa5617`  
		Last Modified: Wed, 29 Mar 2023 19:42:31 GMT  
		Size: 53.4 MB (53446673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719d892cb38b0d519868c97fa4fcd905dc7bad83e9ca4be7381cf171889ebc8d`  
		Last Modified: Wed, 29 Mar 2023 19:42:25 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311f896f1afa0178287d56dceb8d29723fac94e59811bf8208ef9fb8e498403a`  
		Last Modified: Wed, 29 Mar 2023 19:42:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac9567c4eb2404a877090987032ee1ac5228fe64752274fc82f5b8334056d9a`  
		Last Modified: Wed, 29 Mar 2023 19:42:25 GMT  
		Size: 1.8 KB (1783 bytes)  
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
$ docker pull consul@sha256:9f2dec39578cc7e9f2fbf50ce944926779311e1ca75e39542289a2749eadb7ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53083539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13198c063b1c98a5a0b969feb237401a883f6189ca01cd7b1608f1ec1549456f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:55:43 GMT
ARG CONSUL_VERSION=1.14.5
# Thu, 30 Mar 2023 03:55:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 30 Mar 2023 03:55:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Mar 2023 03:55:43 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Mar 2023 03:55:48 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Mar 2023 03:55:49 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Mar 2023 03:55:50 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Mar 2023 03:55:50 GMT
VOLUME [/consul/data]
# Thu, 30 Mar 2023 03:55:50 GMT
EXPOSE 8300
# Thu, 30 Mar 2023 03:55:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Mar 2023 03:55:50 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Mar 2023 03:55:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Mar 2023 03:55:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 03:55:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0af305f621261206a328022b1cfb957621f0e8ef3955ab7a6884a30c1edf3b7`  
		Last Modified: Thu, 30 Mar 2023 03:56:22 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df962497fe647bad6eda4a275dc05e1cd733b39d33920d198959145377fe2073`  
		Last Modified: Thu, 30 Mar 2023 03:56:27 GMT  
		Size: 50.4 MB (50358158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35817705fdb64872a95855bbb05d0fd5e44995ba887b62e8e49d4b8118b8b442`  
		Last Modified: Thu, 30 Mar 2023 03:56:22 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c384d35d896a468c9d432f01ab35e09dde741e0dbb4bb85bacff2693ecc7ce35`  
		Last Modified: Thu, 30 Mar 2023 03:56:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f057082403770d29572e6cf501f3919298f0ab8fdf5dc050a7bad6761a0d4391`  
		Last Modified: Thu, 30 Mar 2023 03:56:22 GMT  
		Size: 1.8 KB (1785 bytes)  
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
$ docker pull consul@sha256:6e1f152161b0e2e3244073d6598fb2855634f0495ec573aa2e50f27762d0fd2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14.5` - linux; amd64

```console
$ docker pull consul@sha256:9c0fcf269c0c4eda29b0d1b8e4abd7bb2fe4f6c249bb63cc3eab07bd0186a72c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.3 MB (56276647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bff07597da659672c93112c25363069d4e84c72260d491a973dc45b36b6269fb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:41:42 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 29 Mar 2023 19:41:42 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 19:41:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 19:41:43 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 19:41:49 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 19:41:50 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 19:41:50 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:41:50 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 19:41:50 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 19:41:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 19:41:50 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 19:41:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 19:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:41:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d3bc1fe58aeeb4895a6a34841a464be34d553c7529c19d7cda9296a48f198`  
		Last Modified: Wed, 29 Mar 2023 19:42:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cfd612915e47e2c834eb37813d96c38b6ace9de7944df5f621f0263baa5617`  
		Last Modified: Wed, 29 Mar 2023 19:42:31 GMT  
		Size: 53.4 MB (53446673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719d892cb38b0d519868c97fa4fcd905dc7bad83e9ca4be7381cf171889ebc8d`  
		Last Modified: Wed, 29 Mar 2023 19:42:25 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311f896f1afa0178287d56dceb8d29723fac94e59811bf8208ef9fb8e498403a`  
		Last Modified: Wed, 29 Mar 2023 19:42:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac9567c4eb2404a877090987032ee1ac5228fe64752274fc82f5b8334056d9a`  
		Last Modified: Wed, 29 Mar 2023 19:42:25 GMT  
		Size: 1.8 KB (1783 bytes)  
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
$ docker pull consul@sha256:9f2dec39578cc7e9f2fbf50ce944926779311e1ca75e39542289a2749eadb7ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53083539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13198c063b1c98a5a0b969feb237401a883f6189ca01cd7b1608f1ec1549456f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:55:43 GMT
ARG CONSUL_VERSION=1.14.5
# Thu, 30 Mar 2023 03:55:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 30 Mar 2023 03:55:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Mar 2023 03:55:43 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Mar 2023 03:55:48 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Mar 2023 03:55:49 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Mar 2023 03:55:50 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Mar 2023 03:55:50 GMT
VOLUME [/consul/data]
# Thu, 30 Mar 2023 03:55:50 GMT
EXPOSE 8300
# Thu, 30 Mar 2023 03:55:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Mar 2023 03:55:50 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Mar 2023 03:55:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Mar 2023 03:55:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 03:55:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0af305f621261206a328022b1cfb957621f0e8ef3955ab7a6884a30c1edf3b7`  
		Last Modified: Thu, 30 Mar 2023 03:56:22 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df962497fe647bad6eda4a275dc05e1cd733b39d33920d198959145377fe2073`  
		Last Modified: Thu, 30 Mar 2023 03:56:27 GMT  
		Size: 50.4 MB (50358158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35817705fdb64872a95855bbb05d0fd5e44995ba887b62e8e49d4b8118b8b442`  
		Last Modified: Thu, 30 Mar 2023 03:56:22 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c384d35d896a468c9d432f01ab35e09dde741e0dbb4bb85bacff2693ecc7ce35`  
		Last Modified: Thu, 30 Mar 2023 03:56:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f057082403770d29572e6cf501f3919298f0ab8fdf5dc050a7bad6761a0d4391`  
		Last Modified: Thu, 30 Mar 2023 03:56:22 GMT  
		Size: 1.8 KB (1785 bytes)  
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
$ docker pull consul@sha256:0d9b18330980a2918e576bdd6be44ad746b9e2f0c47139e5f8ef9e55b7789db4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.15` - linux; amd64

```console
$ docker pull consul@sha256:f7d7f31289176687415ec29f0c663b39fb7c30c950852040fd7d589d5f82da88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57865402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4576d5e11b38aae1d58d09f9a18f84be6adbc3fc55c760136d6a95a33912681b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:41:30 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 29 Mar 2023 19:41:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 19:41:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 19:41:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 19:41:38 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 19:41:38 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 19:41:39 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:41:39 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 19:41:39 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 19:41:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 19:41:39 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 19:41:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 19:41:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:41:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52886d54418c878cecb368bc18fe9f8bb8f8ec82bae3b705d6670f9c1355c5ab`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a49b3fbb7ca4b2774957e3eba53160905fc54dd4ba47a8e1c40288dda00924a`  
		Last Modified: Wed, 29 Mar 2023 19:42:16 GMT  
		Size: 55.0 MB (55035430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0301256aa9aa055ecbe91733aa5dc3c0b86e9a798a26e5d4ad857481917b2c2c`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e2dc2276d59327825e6e83f46e497dce161d51d08d7331225bd1e77f2b700a`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d17243ac56b435745a7e806e55d0143c9fc981b93e337cc883e03b412308f9f`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 1.8 KB (1785 bytes)  
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
$ docker pull consul@sha256:0d40f37502d80b2f438bab8572a5431d1c891ac71ec75cb7521c12eeba81a00d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54574360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d0f32aaf903b91bcbb72c7e6e4b8c27285b199edde192c327ece78ee1d65d27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:55:32 GMT
ARG CONSUL_VERSION=1.15.1
# Thu, 30 Mar 2023 03:55:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 30 Mar 2023 03:55:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Mar 2023 03:55:32 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Mar 2023 03:55:38 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Mar 2023 03:55:39 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Mar 2023 03:55:39 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Mar 2023 03:55:39 GMT
VOLUME [/consul/data]
# Thu, 30 Mar 2023 03:55:39 GMT
EXPOSE 8300
# Thu, 30 Mar 2023 03:55:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Mar 2023 03:55:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Mar 2023 03:55:40 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Mar 2023 03:55:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 03:55:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c39e03fc8bb8c6285eff1f0ad66d72acec2f8eae04006e2469440522fb67bc`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f1f2b6ada3c1ac84221d4ac7bc9f83c1d15797ed732d70f97058bfaf1218bb`  
		Last Modified: Thu, 30 Mar 2023 03:56:13 GMT  
		Size: 51.8 MB (51848983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f4a5555239e31e7d09ec122f633d7878fa0d17e997b18d451e595b9d7ac256`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01df5159699b8a07fa793f3fdfe5910b5bf5ef0cbda5cd0d1ddbb9f966546754`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156bef4b5405821b57a187a59615544b81cb874f40aa2587381a4f27b34e887a`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 1.8 KB (1780 bytes)  
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
$ docker pull consul@sha256:0d9b18330980a2918e576bdd6be44ad746b9e2f0c47139e5f8ef9e55b7789db4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.15.1` - linux; amd64

```console
$ docker pull consul@sha256:f7d7f31289176687415ec29f0c663b39fb7c30c950852040fd7d589d5f82da88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57865402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4576d5e11b38aae1d58d09f9a18f84be6adbc3fc55c760136d6a95a33912681b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:41:30 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 29 Mar 2023 19:41:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 19:41:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 19:41:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 19:41:38 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 19:41:38 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 19:41:39 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:41:39 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 19:41:39 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 19:41:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 19:41:39 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 19:41:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 19:41:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:41:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52886d54418c878cecb368bc18fe9f8bb8f8ec82bae3b705d6670f9c1355c5ab`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a49b3fbb7ca4b2774957e3eba53160905fc54dd4ba47a8e1c40288dda00924a`  
		Last Modified: Wed, 29 Mar 2023 19:42:16 GMT  
		Size: 55.0 MB (55035430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0301256aa9aa055ecbe91733aa5dc3c0b86e9a798a26e5d4ad857481917b2c2c`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e2dc2276d59327825e6e83f46e497dce161d51d08d7331225bd1e77f2b700a`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d17243ac56b435745a7e806e55d0143c9fc981b93e337cc883e03b412308f9f`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 1.8 KB (1785 bytes)  
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
$ docker pull consul@sha256:0d40f37502d80b2f438bab8572a5431d1c891ac71ec75cb7521c12eeba81a00d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54574360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d0f32aaf903b91bcbb72c7e6e4b8c27285b199edde192c327ece78ee1d65d27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:55:32 GMT
ARG CONSUL_VERSION=1.15.1
# Thu, 30 Mar 2023 03:55:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 30 Mar 2023 03:55:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Mar 2023 03:55:32 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Mar 2023 03:55:38 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Mar 2023 03:55:39 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Mar 2023 03:55:39 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Mar 2023 03:55:39 GMT
VOLUME [/consul/data]
# Thu, 30 Mar 2023 03:55:39 GMT
EXPOSE 8300
# Thu, 30 Mar 2023 03:55:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Mar 2023 03:55:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Mar 2023 03:55:40 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Mar 2023 03:55:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 03:55:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c39e03fc8bb8c6285eff1f0ad66d72acec2f8eae04006e2469440522fb67bc`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f1f2b6ada3c1ac84221d4ac7bc9f83c1d15797ed732d70f97058bfaf1218bb`  
		Last Modified: Thu, 30 Mar 2023 03:56:13 GMT  
		Size: 51.8 MB (51848983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f4a5555239e31e7d09ec122f633d7878fa0d17e997b18d451e595b9d7ac256`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01df5159699b8a07fa793f3fdfe5910b5bf5ef0cbda5cd0d1ddbb9f966546754`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156bef4b5405821b57a187a59615544b81cb874f40aa2587381a4f27b34e887a`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 1.8 KB (1780 bytes)  
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
$ docker pull consul@sha256:0d9b18330980a2918e576bdd6be44ad746b9e2f0c47139e5f8ef9e55b7789db4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:f7d7f31289176687415ec29f0c663b39fb7c30c950852040fd7d589d5f82da88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57865402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4576d5e11b38aae1d58d09f9a18f84be6adbc3fc55c760136d6a95a33912681b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:33 GMT
ADD file:08ad6c1c886a26e30ae4ab103ff377ee6cfbc1be2437fa227ec28a335c63d78a in / 
# Wed, 29 Mar 2023 18:19:33 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:41:30 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 29 Mar 2023 19:41:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Mar 2023 19:41:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Mar 2023 19:41:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Mar 2023 19:41:38 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Mar 2023 19:41:38 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Mar 2023 19:41:39 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Mar 2023 19:41:39 GMT
VOLUME [/consul/data]
# Wed, 29 Mar 2023 19:41:39 GMT
EXPOSE 8300
# Wed, 29 Mar 2023 19:41:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Mar 2023 19:41:39 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Mar 2023 19:41:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Mar 2023 19:41:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:41:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0ce1dd7918a48990ab749aab2e805c26f691a3a8103495530e7ea5a1d168af4a`  
		Last Modified: Wed, 29 Mar 2023 18:20:17 GMT  
		Size: 2.8 MB (2826596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52886d54418c878cecb368bc18fe9f8bb8f8ec82bae3b705d6670f9c1355c5ab`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a49b3fbb7ca4b2774957e3eba53160905fc54dd4ba47a8e1c40288dda00924a`  
		Last Modified: Wed, 29 Mar 2023 19:42:16 GMT  
		Size: 55.0 MB (55035430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0301256aa9aa055ecbe91733aa5dc3c0b86e9a798a26e5d4ad857481917b2c2c`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e2dc2276d59327825e6e83f46e497dce161d51d08d7331225bd1e77f2b700a`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d17243ac56b435745a7e806e55d0143c9fc981b93e337cc883e03b412308f9f`  
		Last Modified: Wed, 29 Mar 2023 19:42:10 GMT  
		Size: 1.8 KB (1785 bytes)  
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
$ docker pull consul@sha256:0d40f37502d80b2f438bab8572a5431d1c891ac71ec75cb7521c12eeba81a00d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54574360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d0f32aaf903b91bcbb72c7e6e4b8c27285b199edde192c327ece78ee1d65d27`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:22 GMT
ADD file:4acfda16c71abce07068ed23839e9de60c1d1145ab8002b3a92c15b1e80d4356 in / 
# Wed, 29 Mar 2023 17:39:23 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:55:32 GMT
ARG CONSUL_VERSION=1.15.1
# Thu, 30 Mar 2023 03:55:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 30 Mar 2023 03:55:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 30 Mar 2023 03:55:32 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 30 Mar 2023 03:55:38 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 30 Mar 2023 03:55:39 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 30 Mar 2023 03:55:39 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 30 Mar 2023 03:55:39 GMT
VOLUME [/consul/data]
# Thu, 30 Mar 2023 03:55:39 GMT
EXPOSE 8300
# Thu, 30 Mar 2023 03:55:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 30 Mar 2023 03:55:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 30 Mar 2023 03:55:40 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 30 Mar 2023 03:55:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 03:55:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:60a00c11adf5202a365ec8215b889c3390d67fa295ab79940e1c5dc4cbed9db1`  
		Last Modified: Wed, 29 Mar 2023 17:40:04 GMT  
		Size: 2.7 MB (2722002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c39e03fc8bb8c6285eff1f0ad66d72acec2f8eae04006e2469440522fb67bc`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f1f2b6ada3c1ac84221d4ac7bc9f83c1d15797ed732d70f97058bfaf1218bb`  
		Last Modified: Thu, 30 Mar 2023 03:56:13 GMT  
		Size: 51.8 MB (51848983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f4a5555239e31e7d09ec122f633d7878fa0d17e997b18d451e595b9d7ac256`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01df5159699b8a07fa793f3fdfe5910b5bf5ef0cbda5cd0d1ddbb9f966546754`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156bef4b5405821b57a187a59615544b81cb874f40aa2587381a4f27b34e887a`  
		Last Modified: Thu, 30 Mar 2023 03:56:08 GMT  
		Size: 1.8 KB (1780 bytes)  
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
