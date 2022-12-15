<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.12`](#consul112)
-	[`consul:1.12.8`](#consul1128)
-	[`consul:1.13`](#consul113)
-	[`consul:1.13.5`](#consul1135)
-	[`consul:1.14`](#consul114)
-	[`consul:1.14.3`](#consul1143)
-	[`consul:latest`](#consullatest)

## `consul:1.12`

```console
$ docker pull consul@sha256:d9b777007a545ecf9e9c5c127761d0cffc0a8814d6b3aabad1f4e9e3a6e22586
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.12` - linux; amd64

```console
$ docker pull consul@sha256:01436f12e4cdf761fbe63c02e2c79bedb5633f4ca9c59622f1e4e99c43ed9b34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49579230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de9133c86cdfa09dca48ab479217180b237375e6a9d6c635455d09652d2f841a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:19:59 GMT
ARG CONSUL_VERSION=1.12.7
# Thu, 01 Dec 2022 19:19:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:19:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:19:59 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:20:05 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:20:06 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:20:07 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:20:07 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:20:07 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:20:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:20:07 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:20:07 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:20:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:20:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6c0c4ca12424304f056bf4d03f3861c7cb727d1aee1e38599a238832bc4a55`  
		Last Modified: Thu, 01 Dec 2022 19:20:53 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64b90c416620787d02e51c1433bdafcc5edcb967ab1686601fc2e49f6b7621f`  
		Last Modified: Thu, 01 Dec 2022 19:20:58 GMT  
		Size: 46.8 MB (46752338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292b84260db71cc1111e8e0aa9411e4f5ba2bb7b3fe0143d3ec771fb020ce03e`  
		Last Modified: Thu, 01 Dec 2022 19:20:53 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295702eecf5bf51fc7df29f90ab89fa037b657a2a92631ec321f2124c5f0ddfa`  
		Last Modified: Thu, 01 Dec 2022 19:20:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9801960a1ef027388614a3970a19270391624336e0aa501cb88678a36ef732d5`  
		Last Modified: Thu, 01 Dec 2022 19:20:53 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm variant v6

```console
$ docker pull consul@sha256:b04bc4585dc688c3569d76bac547029c1d6ea6644e2099020467c067193b8bd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47457012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef450c888eed6f1ca8cc3d1b5315aa157ebcae96e518839d83d381e0ebbbe0b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 18:49:54 GMT
ARG CONSUL_VERSION=1.12.7
# Thu, 01 Dec 2022 18:49:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 18:49:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 18:49:55 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 18:50:01 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 18:50:02 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 18:50:03 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 18:50:03 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 18:50:03 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 18:50:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 18:50:03 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 18:50:03 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 18:50:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 18:50:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9704c26a8a40ab29ed9a52d42e4c004849b9bb773f13fd272f9c544988ef9e87`  
		Last Modified: Thu, 01 Dec 2022 18:51:11 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053cd078ac865cff102a65a2501493c16e4b5966fe290ac5f2b64595e613ae7d`  
		Last Modified: Thu, 01 Dec 2022 18:51:18 GMT  
		Size: 44.8 MB (44822558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcf87db781194f55b822c3fa8680e0fb08512dd0fe71798677e9a23ed08f750`  
		Last Modified: Thu, 01 Dec 2022 18:51:11 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18224d7bd4083269f5a0ba702200ea48cf1eebed7af9d14bc05465a595949003`  
		Last Modified: Thu, 01 Dec 2022 18:51:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1724b84b3c2816e7605ed3365bb92526e05726c7196343a09a47cb5809d4802a`  
		Last Modified: Thu, 01 Dec 2022 18:51:11 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2b4da75474a55fb71bc6a59a51093196d72a2ec6f82bab633b7fd53e2f6db760
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47172808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3308e8034a1e93185c37fe5ccc584e3da2659860ab23cfb393d43879eba3d429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:39:50 GMT
ARG CONSUL_VERSION=1.12.7
# Thu, 01 Dec 2022 19:39:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:39:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:39:51 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:39:55 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:39:56 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:39:57 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:39:57 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:39:57 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:39:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:39:57 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:39:57 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:39:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:39:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f478a0e024cb96dd6ea78d6a030d19201415fd068d6bac03cafd986fbbf3fb`  
		Last Modified: Thu, 01 Dec 2022 19:40:37 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3042a43bdfc290bac7b5ce1555586f2fb5b106eab420598f40fcf68dbe8bb3ea`  
		Last Modified: Thu, 01 Dec 2022 19:40:41 GMT  
		Size: 44.5 MB (44450988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60de4f4fa162d9e87ef341a1178cdd0a755dd82c325bdbd485369f39840fbdf4`  
		Last Modified: Thu, 01 Dec 2022 19:40:37 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898e14427fb510bee33d241fbc1cf7adbed5e8594afe1615e085592f759462cb`  
		Last Modified: Thu, 01 Dec 2022 19:40:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3eade590675f1eadb4ef5aafb924d4a636bbafef5b712ecfca2402e68fd7a1`  
		Last Modified: Thu, 01 Dec 2022 19:40:36 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; 386

```console
$ docker pull consul@sha256:ee8792cd7b260b17d4b32f413d7121a08c9242768323588f6e5d8f8148566f8f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48641587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f5f65746964354577e84e344ef5a8c256d9084ca2f73453108d846d07ba2f32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:39:14 GMT
ARG CONSUL_VERSION=1.12.7
# Thu, 01 Dec 2022 19:39:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:39:16 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:39:17 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:39:24 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:39:25 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:39:26 GMT
# ARGS: CONSUL_VERSION=1.12.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:39:27 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:39:28 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:39:29 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:39:30 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:39:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:39:33 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e99c3af2101555a924df15eb060a8748a96e501521fb6b5df2a4c8e29e6433`  
		Last Modified: Thu, 01 Dec 2022 19:40:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ce5d69914b0aea58975a79a7e52625cbe89fb33dda368d239a9814a2c1e08b`  
		Last Modified: Thu, 01 Dec 2022 19:40:36 GMT  
		Size: 45.8 MB (45809745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea975d097d97ba27c1f1bd32095fb8279d034514f0cecf33b9abc3494b97947`  
		Last Modified: Thu, 01 Dec 2022 19:40:31 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c37ee234354161c67ec73a1efaf9ba965bdfa637c288a8fac5442cacbd16fef`  
		Last Modified: Thu, 01 Dec 2022 19:40:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdfe8a168efb9b51b9fbc503c89ed6d9a16c257b7de0c7551683e779f8a72e0`  
		Last Modified: Thu, 01 Dec 2022 19:40:30 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12.8`

**does not exist** (yet?)

## `consul:1.13`

```console
$ docker pull consul@sha256:d8ac1e333b4dd8326c0650fb7e7d884227ce3bd020c3c9cdeaf27a04543fc3ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13` - linux; amd64

```console
$ docker pull consul@sha256:e25ada792c2acd43bfc6087a53f4e40025c16a37c74df1e5570016964261d005
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51850730 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca9ae929e8b09c70c0fdf9a01bc26e2f7630421d868a3be7e575b3f5369a322d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:19:47 GMT
ARG CONSUL_VERSION=1.13.4
# Thu, 01 Dec 2022 19:19:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:19:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:19:48 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:19:53 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:19:54 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:19:55 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:19:55 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:19:55 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:19:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:19:55 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:19:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:19:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f704c5c7407419236fec20086dbfbba25437675ab5ee5066cad9ee64e3fc5a4c`  
		Last Modified: Thu, 01 Dec 2022 19:20:37 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af4b4e8bd825452958f05aeb8b7ab9ca9ebb498d023d05a2f937b4d43c9291d`  
		Last Modified: Thu, 01 Dec 2022 19:20:44 GMT  
		Size: 49.0 MB (49023833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5362781d3f576e0d8c12da2c4dcd0a9d9ae848b8d3cfe7f7c57ba2225e26f0e9`  
		Last Modified: Thu, 01 Dec 2022 19:20:37 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820fd821f29d355d8c91937edc66cda2291d192c089ef1f7b01e3fa2be3b87e1`  
		Last Modified: Thu, 01 Dec 2022 19:20:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1293ec9cd7aaae0c70738fcba3beadd9e04b218e467d5e8c2e451ca58803454`  
		Last Modified: Thu, 01 Dec 2022 19:20:38 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm variant v6

```console
$ docker pull consul@sha256:ec276438c0b38b94266ca4d562ac6a30af3b23e5172dcba4c302939627c32bd4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49451563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3692201638c2a2975819e8968b3367d148b35605bb2c43d3b2c523e62d5bd0e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 18:49:38 GMT
ARG CONSUL_VERSION=1.13.4
# Thu, 01 Dec 2022 18:49:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 18:49:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 18:49:39 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 18:49:46 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 18:49:47 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 18:49:47 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 18:49:47 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 18:49:47 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 18:49:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 18:49:48 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 18:49:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 18:49:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 18:49:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45942d0a05af7d6f2068730fd569fc8733577e603871b11fdfd374a070e49436`  
		Last Modified: Thu, 01 Dec 2022 18:50:52 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92fd861e85a2597fe8d15018b051a4698b0e5b6024bd9f1f269684fe54fe582`  
		Last Modified: Thu, 01 Dec 2022 18:51:00 GMT  
		Size: 46.8 MB (46817113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88015292fd5d509b84340f7d425769076f211fda32426777832202a695ae3d7b`  
		Last Modified: Thu, 01 Dec 2022 18:50:52 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ca5117bd648e6063e5e292a85a196064cc85ce940ff1b28b74ebdbfd2bf365`  
		Last Modified: Thu, 01 Dec 2022 18:50:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65264676bca2daabce6c62e17580f48a81695e44d4e466f558caff125d581cac`  
		Last Modified: Thu, 01 Dec 2022 18:50:52 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:8046605b92b11c2accdf8ba7d1909f6ac84473f8cd1b2aabbb47db994e9af3fc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49013314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:deccfd885b7ff0a04916aa73a73e8a9354f95ee2f48ec6cc09dd5164156d8b7d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:39:40 GMT
ARG CONSUL_VERSION=1.13.4
# Thu, 01 Dec 2022 19:39:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:39:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:39:41 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:39:46 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:39:47 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:39:47 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:39:47 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:39:47 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:39:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:39:48 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:39:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:39:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689745f190c551102e8649c93682d96e49abf90e0cf4203cf2ba4b4a6459fce5`  
		Last Modified: Thu, 01 Dec 2022 19:40:25 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00677390c1fbceb57460cb38f14ccae599aa27dbbbde5b9fe6bf15cae6c5e7a`  
		Last Modified: Thu, 01 Dec 2022 19:40:29 GMT  
		Size: 46.3 MB (46291494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33685d4ed2597d16a56371b1421df1261ac5ebc2f1fed8f6be95124d4a22b01c`  
		Last Modified: Thu, 01 Dec 2022 19:40:24 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19723cdb688380bf9ee411993895f94c54203b15cfdc8fafdd464bbb47bc121`  
		Last Modified: Thu, 01 Dec 2022 19:40:24 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ad46308416a78476f6364ebdb0a2e113058c6a1597e267441c848c8a93a09e`  
		Last Modified: Thu, 01 Dec 2022 19:40:24 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; 386

```console
$ docker pull consul@sha256:18022baf5b4a705e52a8310236469e732070cdd9ba1f9d2b5efeb4f3b93219ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50732874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e20ce815ea9b8fb8f9e2ec9dd33adc762e71772e3597ebc985f9bde35895c37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:38:51 GMT
ARG CONSUL_VERSION=1.13.4
# Thu, 01 Dec 2022 19:38:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:38:52 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:38:53 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:39:00 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:39:01 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:39:02 GMT
# ARGS: CONSUL_VERSION=1.13.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:39:03 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:39:04 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:39:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:39:06 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:39:08 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:39:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:39:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7177299877adf2fc004e8c9ca1dbe96ffda8732e083324160e839dd91456b38e`  
		Last Modified: Thu, 01 Dec 2022 19:40:15 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:324c8f86d6d33f4703e7892552ddd4197533ff2a07460744d20a7d7665f1f6db`  
		Last Modified: Thu, 01 Dec 2022 19:40:21 GMT  
		Size: 47.9 MB (47901034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92df99a8b6d7798eaee2f595ec1652d0560d35d45f57951f08523e4479bd80b8`  
		Last Modified: Thu, 01 Dec 2022 19:40:15 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167bbc43da7edb9b66ed040e7930084e61645c626185e692ae7d4aa67e262a6b`  
		Last Modified: Thu, 01 Dec 2022 19:40:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fff46d1a9e0575fd4f3ebd23001ea3f1cf69ed78e12a05165d99b06a4603422`  
		Last Modified: Thu, 01 Dec 2022 19:40:15 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.13.5`

**does not exist** (yet?)

## `consul:1.14`

```console
$ docker pull consul@sha256:ee2fa19164afda5d3b6dc811acfdc8760d86e60a7514dc509b3a3ce52378b9c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14` - linux; amd64

```console
$ docker pull consul@sha256:c4e4157f8d75cecd09ddd2a91f47c1b8be494c8d9a5ab1a8fddd8bbb2789f93a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56172091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228be3c080bd59121376ea6e413a5f9c06ea96f4a28ab8c183df412f1f337bd9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:19:35 GMT
ARG CONSUL_VERSION=1.14.2
# Thu, 01 Dec 2022 19:19:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:19:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:19:36 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:19:42 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:19:43 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:19:43 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:19:43 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:19:44 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:19:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:19:44 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:19:44 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:19:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:19:44 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7737695e55ca701d9939ae6a5f2890c502bddb502dcbe416cff2486cc11564`  
		Last Modified: Thu, 01 Dec 2022 19:20:20 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5fe520af524f5d64ed8c1810e20b4ba8b37816e4336ab511976285c5e2d2cb`  
		Last Modified: Thu, 01 Dec 2022 19:20:27 GMT  
		Size: 53.3 MB (53345192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72586b0850c739aef048198a64203f98bd15389c4a372afe3db3e21f5be07579`  
		Last Modified: Thu, 01 Dec 2022 19:20:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877c43ad557c1baca4f88cd06d07bfc4d750f22aa1eb61d24c38fd8cdfdd2a4d`  
		Last Modified: Thu, 01 Dec 2022 19:20:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abf1331fb3333c94ff6677f85321713d27314c3b04445ac3e3c69c1bb03415f`  
		Last Modified: Thu, 01 Dec 2022 19:20:20 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; arm variant v6

```console
$ docker pull consul@sha256:2792e3fc1fb86ef3fa6cde0666e0953006d1584a18c1d6323b15e99c936ab360
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53583633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef35f8c215115ee2455c02653ce0b7292fdb2ac46e07be3633bab9318da08ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 18:49:21 GMT
ARG CONSUL_VERSION=1.14.2
# Thu, 01 Dec 2022 18:49:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 18:49:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 18:49:22 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 18:49:29 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 18:49:30 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 18:49:31 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 18:49:31 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 18:49:31 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 18:49:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 18:49:31 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 18:49:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 18:49:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 18:49:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2511d11b8fe1839cae8ccfeb7c5e082d86d1e24192958d74d452761039a6642`  
		Last Modified: Thu, 01 Dec 2022 18:50:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973f3ab39c612a6e9174442d090a76d7294b4dfa30ffe8cf34ceb936b5fb820`  
		Last Modified: Thu, 01 Dec 2022 18:50:38 GMT  
		Size: 50.9 MB (50949180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d341b9c6d36141489eb5b92ab3db9eb93726b704820617b7a2b240e9638e641`  
		Last Modified: Thu, 01 Dec 2022 18:50:30 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4e61270ca8ae60ea4cf93bb3762e60f3749f85f26db134b620780155e6589f`  
		Last Modified: Thu, 01 Dec 2022 18:50:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f8d6cd42225eb09fed6d1f18ca65c976d3b12a5511a71dab76e23640548846`  
		Last Modified: Thu, 01 Dec 2022 18:50:30 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b454204ba03a7114342cf602d205cf5503ca1b90e06be2ce4ba5cfd003fe9918
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52999746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f8314bae5a1b2241d8118f6f0f828b7ee922310c6d87fc6bc67c49870850a55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:39:29 GMT
ARG CONSUL_VERSION=1.14.2
# Thu, 01 Dec 2022 19:39:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:39:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:39:29 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:39:35 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:39:36 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:39:36 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:39:36 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:39:36 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:39:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:39:36 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:39:37 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:39:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:39:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aeb01e7d392f48f8f6bcfa931288ad4af14393d67850be85701fefaec20d6f`  
		Last Modified: Thu, 01 Dec 2022 19:40:09 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3bd7a1c773addd5306e4bb4aeed7a76add11bf9f8a6abfb57ee947db625e58`  
		Last Modified: Thu, 01 Dec 2022 19:40:14 GMT  
		Size: 50.3 MB (50277922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845288ebf54046963be5c2eb2229153d5f74bcf3caf9c0f867d8ef967cb5238d`  
		Last Modified: Thu, 01 Dec 2022 19:40:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06ad9b497362902a37cc18b3c8ef69678c7efc264dd60383f08ce312b35bd01`  
		Last Modified: Thu, 01 Dec 2022 19:40:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ed8b868f544f1a016432923d87a3f0b1c37fd7c50a3b29e659a2054e535205`  
		Last Modified: Thu, 01 Dec 2022 19:40:09 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; 386

```console
$ docker pull consul@sha256:232f8c35751abd039358e8f09c2fd34ec96973635dba614ea7955fe968fdeb3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54965245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b34da0ea24e793649fffcedf254e165abd143fc141db637d65129b545d5429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:38:24 GMT
ARG CONSUL_VERSION=1.14.2
# Thu, 01 Dec 2022 19:38:25 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:38:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:38:27 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:38:34 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:38:35 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:38:36 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:38:37 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:38:38 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:38:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:38:42 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:38:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:38:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0781c0d981f1f16aa394f6456553f0a70b8972e12290e0c0d5e75c282ffe95`  
		Last Modified: Thu, 01 Dec 2022 19:39:57 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca6998e4e4d019835cfd076c636bc6dc80a774ba8a88eecadb274cb811ce105`  
		Last Modified: Thu, 01 Dec 2022 19:40:03 GMT  
		Size: 52.1 MB (52133403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899451e28fd2e04d5d1fabe3c61766bac5d37d67f59b8add187879e54d20772a`  
		Last Modified: Thu, 01 Dec 2022 19:39:57 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa13cbc8dc4d6943c4876904041f7de64aa3782a616e223352d357becbd417d`  
		Last Modified: Thu, 01 Dec 2022 19:39:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a358a3be61c0a575f352bfdd8edef12a386985ea0632b6601c3d1dd927381ce`  
		Last Modified: Thu, 01 Dec 2022 19:39:57 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.14.3`

**does not exist** (yet?)

## `consul:latest`

```console
$ docker pull consul@sha256:ee2fa19164afda5d3b6dc811acfdc8760d86e60a7514dc509b3a3ce52378b9c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:c4e4157f8d75cecd09ddd2a91f47c1b8be494c8d9a5ab1a8fddd8bbb2789f93a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56172091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:228be3c080bd59121376ea6e413a5f9c06ea96f4a28ab8c183df412f1f337bd9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:19:35 GMT
ARG CONSUL_VERSION=1.14.2
# Thu, 01 Dec 2022 19:19:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:19:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:19:36 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:19:42 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:19:43 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:19:43 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:19:43 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:19:44 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:19:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:19:44 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:19:44 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:19:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:19:44 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7737695e55ca701d9939ae6a5f2890c502bddb502dcbe416cff2486cc11564`  
		Last Modified: Thu, 01 Dec 2022 19:20:20 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5fe520af524f5d64ed8c1810e20b4ba8b37816e4336ab511976285c5e2d2cb`  
		Last Modified: Thu, 01 Dec 2022 19:20:27 GMT  
		Size: 53.3 MB (53345192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72586b0850c739aef048198a64203f98bd15389c4a372afe3db3e21f5be07579`  
		Last Modified: Thu, 01 Dec 2022 19:20:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877c43ad557c1baca4f88cd06d07bfc4d750f22aa1eb61d24c38fd8cdfdd2a4d`  
		Last Modified: Thu, 01 Dec 2022 19:20:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abf1331fb3333c94ff6677f85321713d27314c3b04445ac3e3c69c1bb03415f`  
		Last Modified: Thu, 01 Dec 2022 19:20:20 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:2792e3fc1fb86ef3fa6cde0666e0953006d1584a18c1d6323b15e99c936ab360
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.6 MB (53583633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ef35f8c215115ee2455c02653ce0b7292fdb2ac46e07be3633bab9318da08ab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 18:49:21 GMT
ARG CONSUL_VERSION=1.14.2
# Thu, 01 Dec 2022 18:49:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 18:49:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 18:49:22 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 18:49:29 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 18:49:30 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 18:49:31 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 18:49:31 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 18:49:31 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 18:49:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 18:49:31 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 18:49:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 18:49:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 18:49:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2511d11b8fe1839cae8ccfeb7c5e082d86d1e24192958d74d452761039a6642`  
		Last Modified: Thu, 01 Dec 2022 18:50:30 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8973f3ab39c612a6e9174442d090a76d7294b4dfa30ffe8cf34ceb936b5fb820`  
		Last Modified: Thu, 01 Dec 2022 18:50:38 GMT  
		Size: 50.9 MB (50949180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d341b9c6d36141489eb5b92ab3db9eb93726b704820617b7a2b240e9638e641`  
		Last Modified: Thu, 01 Dec 2022 18:50:30 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4e61270ca8ae60ea4cf93bb3762e60f3749f85f26db134b620780155e6589f`  
		Last Modified: Thu, 01 Dec 2022 18:50:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f8d6cd42225eb09fed6d1f18ca65c976d3b12a5511a71dab76e23640548846`  
		Last Modified: Thu, 01 Dec 2022 18:50:30 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b454204ba03a7114342cf602d205cf5503ca1b90e06be2ce4ba5cfd003fe9918
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52999746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f8314bae5a1b2241d8118f6f0f828b7ee922310c6d87fc6bc67c49870850a55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:39:29 GMT
ARG CONSUL_VERSION=1.14.2
# Thu, 01 Dec 2022 19:39:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:39:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:39:29 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:39:35 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:39:36 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:39:36 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:39:36 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:39:36 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:39:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:39:36 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:39:37 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:39:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:39:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3aeb01e7d392f48f8f6bcfa931288ad4af14393d67850be85701fefaec20d6f`  
		Last Modified: Thu, 01 Dec 2022 19:40:09 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3bd7a1c773addd5306e4bb4aeed7a76add11bf9f8a6abfb57ee947db625e58`  
		Last Modified: Thu, 01 Dec 2022 19:40:14 GMT  
		Size: 50.3 MB (50277922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845288ebf54046963be5c2eb2229153d5f74bcf3caf9c0f867d8ef967cb5238d`  
		Last Modified: Thu, 01 Dec 2022 19:40:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06ad9b497362902a37cc18b3c8ef69678c7efc264dd60383f08ce312b35bd01`  
		Last Modified: Thu, 01 Dec 2022 19:40:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ed8b868f544f1a016432923d87a3f0b1c37fd7c50a3b29e659a2054e535205`  
		Last Modified: Thu, 01 Dec 2022 19:40:09 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:232f8c35751abd039358e8f09c2fd34ec96973635dba614ea7955fe968fdeb3d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (54965245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b34da0ea24e793649fffcedf254e165abd143fc141db637d65129b545d5429`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Dec 2022 19:38:24 GMT
ARG CONSUL_VERSION=1.14.2
# Thu, 01 Dec 2022 19:38:25 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 01 Dec 2022 19:38:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 01 Dec 2022 19:38:27 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 01 Dec 2022 19:38:34 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 01 Dec 2022 19:38:35 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 01 Dec 2022 19:38:36 GMT
# ARGS: CONSUL_VERSION=1.14.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 01 Dec 2022 19:38:37 GMT
VOLUME [/consul/data]
# Thu, 01 Dec 2022 19:38:38 GMT
EXPOSE 8300
# Thu, 01 Dec 2022 19:38:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 01 Dec 2022 19:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 01 Dec 2022 19:38:42 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Dec 2022 19:38:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Dec 2022 19:38:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0781c0d981f1f16aa394f6456553f0a70b8972e12290e0c0d5e75c282ffe95`  
		Last Modified: Thu, 01 Dec 2022 19:39:57 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca6998e4e4d019835cfd076c636bc6dc80a774ba8a88eecadb274cb811ce105`  
		Last Modified: Thu, 01 Dec 2022 19:40:03 GMT  
		Size: 52.1 MB (52133403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899451e28fd2e04d5d1fabe3c61766bac5d37d67f59b8add187879e54d20772a`  
		Last Modified: Thu, 01 Dec 2022 19:39:57 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa13cbc8dc4d6943c4876904041f7de64aa3782a616e223352d357becbd417d`  
		Last Modified: Thu, 01 Dec 2022 19:39:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a358a3be61c0a575f352bfdd8edef12a386985ea0632b6601c3d1dd927381ce`  
		Last Modified: Thu, 01 Dec 2022 19:39:57 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
