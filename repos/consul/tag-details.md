<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10`](#consul110)
-	[`consul:1.10.8`](#consul1108)
-	[`consul:1.11`](#consul111)
-	[`consul:1.11.3`](#consul1113)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.15`](#consul1915)
-	[`consul:latest`](#consullatest)

## `consul:1.10`

```console
$ docker pull consul@sha256:b1511f5b9c6d3e1155d2e97c00003e47481df6fd90b71bcfd28a17ca893361f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10` - linux; amd64

```console
$ docker pull consul@sha256:c2a4cd7f5ff87c295f31a8e236bd0c0642dff0b43bb5f3f8e673914da1e1f603
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43707576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28277ec29f604ba942414cc21e5fdc31ef19aea562ab9b47de7a2beaaa507330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 07:22:42 GMT
ARG CONSUL_VERSION=1.10.8
# Sat, 12 Feb 2022 07:22:42 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 07:22:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 07:22:43 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 07:23:23 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 07:23:24 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 07:23:25 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 07:23:25 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 07:23:25 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 07:23:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 07:23:26 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 07:23:26 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 07:23:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 07:23:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15f99d5b4c32f7a15f0adc4a03eb22b60e49773e4d8c3c7f2e316c9ea06583d`  
		Last Modified: Sat, 12 Feb 2022 07:24:46 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2f6e959774726d464c51b5db734bdc23b69385dcde600096877ff6de64c554`  
		Last Modified: Sat, 12 Feb 2022 07:24:51 GMT  
		Size: 40.9 MB (40881777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b4c7025a4704669d43b5195bd12cd430b8c41b25692d380767570ab759a7af`  
		Last Modified: Sat, 12 Feb 2022 07:24:46 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb411ddd0d0a86f03fabc54edc3f6b937d2743de40f1f2b82a67f02adafe82`  
		Last Modified: Sat, 12 Feb 2022 07:24:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8580800d3e36f5f159f19a2fe48de2bf749850095fbeffc27663f97d1ac1845`  
		Last Modified: Sat, 12 Feb 2022 07:24:46 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:298ac8d6cb57014379dfeea323a4f40253234e0346bc4855db3c7f939646c918
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41767102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7146de82d58c8360314657ab9f3bb7d74aac8b75d8cc255f6965bb8eb9bdf8aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:50:21 GMT
ARG CONSUL_VERSION=1.10.8
# Sat, 12 Feb 2022 01:50:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:50:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:50:24 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:50:51 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:50:52 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:50:54 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:50:55 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:50:55 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:50:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:50:56 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:50:56 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:50:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:50:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6433b6bf5bed8b3be159441dfeb9712971674bac4560ce7f8a4eff5ce13a7565`  
		Last Modified: Sat, 12 Feb 2022 01:53:02 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878f28cb8b52e741264e9f23c9e4b5591c3d645ad1f067025f9dd4d593c75def`  
		Last Modified: Sat, 12 Feb 2022 01:53:24 GMT  
		Size: 39.1 MB (39130384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a653e69a81e17e79e5c5c36302da1cfa43006b3728d594d6d7e7c2fb4858d2`  
		Last Modified: Sat, 12 Feb 2022 01:53:03 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9424e86dc77f20fb6ec25edf6c8122ceead8b081ec1f0da24ef376da60e31f`  
		Last Modified: Sat, 12 Feb 2022 01:53:02 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6919833dce23fe2753532ef08cc421715f317809ba4e185fbc8811c8fa7c3a`  
		Last Modified: Sat, 12 Feb 2022 01:53:02 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:024760593a5382fcb164da6ccf64917521b31a4022d554159df0cfdf6f9a93fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41722147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6152a0a0674b4d510143d2ef85cd83b6b18f50d2baf4e548c59fa3c4766a3d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 05:35:00 GMT
ARG CONSUL_VERSION=1.10.8
# Sat, 12 Feb 2022 05:35:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 05:35:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 05:35:03 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 05:35:17 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 05:35:18 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 05:35:18 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 05:35:19 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 05:35:20 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 05:35:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 05:35:22 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 05:35:24 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 05:35:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 05:35:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25aefc06e82caf22b59a89763786c40b81524f525dfcfc8dadac69a2ab2632ab`  
		Last Modified: Sat, 12 Feb 2022 05:36:33 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86316f29383a9851e34be85e1750acbf793a9d15df411ef25cb9fe4634c76d96`  
		Last Modified: Sat, 12 Feb 2022 05:36:39 GMT  
		Size: 39.0 MB (38999191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46dc202bffe4c9c2f3546afb9a871802b238b0e173d64c68f922e107704ed8fd`  
		Last Modified: Sat, 12 Feb 2022 05:36:34 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d1e85b96c64681f5c9141ae4a76db015a707f367579ef7dea37537d3065638`  
		Last Modified: Sat, 12 Feb 2022 05:36:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8357f4730f10146ed93b5604a8f992571671e257bc00c377168b777e50d5a32`  
		Last Modified: Sat, 12 Feb 2022 05:36:33 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; 386

```console
$ docker pull consul@sha256:be64a2fed0233627503f4541fa778d07dcd424ff4da861b425e3c2c3f9564238
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23295a8e8cbbfd6e3304c88db6c1c927efb08848165f1b2914e85d71457e0271`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:41:32 GMT
ARG CONSUL_VERSION=1.10.8
# Sat, 12 Feb 2022 01:41:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:41:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:41:33 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:42:11 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:42:12 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:42:13 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:42:13 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:42:13 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:42:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:42:14 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:42:14 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:42:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:42:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3259d3be13e1fda280e5018f614200af83e3e58eefe3dc0cb7174a325253d5c5`  
		Last Modified: Sat, 12 Feb 2022 01:43:48 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5a2980bd7e4eee5cda163a94f9adccae5e306cc64592af53d019a776dd25bf`  
		Last Modified: Sat, 12 Feb 2022 01:43:55 GMT  
		Size: 40.3 MB (40262442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28a217fece634a56740b237cf65ff30148c35190d97d26ff0694f25052aafa9`  
		Last Modified: Sat, 12 Feb 2022 01:43:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6e01be3cf21cc803ab05104e8b2c25c381df12a8330a7da8215823dbedbe40`  
		Last Modified: Sat, 12 Feb 2022 01:43:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f34f69bc3459c2893ea74360bd5a1da6c08468c085b9105759d663d6429f314`  
		Last Modified: Sat, 12 Feb 2022 01:43:48 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.8`

```console
$ docker pull consul@sha256:b1511f5b9c6d3e1155d2e97c00003e47481df6fd90b71bcfd28a17ca893361f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.8` - linux; amd64

```console
$ docker pull consul@sha256:c2a4cd7f5ff87c295f31a8e236bd0c0642dff0b43bb5f3f8e673914da1e1f603
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43707576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28277ec29f604ba942414cc21e5fdc31ef19aea562ab9b47de7a2beaaa507330`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 07:22:42 GMT
ARG CONSUL_VERSION=1.10.8
# Sat, 12 Feb 2022 07:22:42 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 07:22:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 07:22:43 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 07:23:23 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 07:23:24 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 07:23:25 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 07:23:25 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 07:23:25 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 07:23:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 07:23:26 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 07:23:26 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 07:23:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 07:23:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15f99d5b4c32f7a15f0adc4a03eb22b60e49773e4d8c3c7f2e316c9ea06583d`  
		Last Modified: Sat, 12 Feb 2022 07:24:46 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2f6e959774726d464c51b5db734bdc23b69385dcde600096877ff6de64c554`  
		Last Modified: Sat, 12 Feb 2022 07:24:51 GMT  
		Size: 40.9 MB (40881777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b4c7025a4704669d43b5195bd12cd430b8c41b25692d380767570ab759a7af`  
		Last Modified: Sat, 12 Feb 2022 07:24:46 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bb411ddd0d0a86f03fabc54edc3f6b937d2743de40f1f2b82a67f02adafe82`  
		Last Modified: Sat, 12 Feb 2022 07:24:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8580800d3e36f5f159f19a2fe48de2bf749850095fbeffc27663f97d1ac1845`  
		Last Modified: Sat, 12 Feb 2022 07:24:46 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:298ac8d6cb57014379dfeea323a4f40253234e0346bc4855db3c7f939646c918
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41767102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7146de82d58c8360314657ab9f3bb7d74aac8b75d8cc255f6965bb8eb9bdf8aa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:50:21 GMT
ARG CONSUL_VERSION=1.10.8
# Sat, 12 Feb 2022 01:50:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:50:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:50:24 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:50:51 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:50:52 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:50:54 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:50:55 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:50:55 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:50:56 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:50:56 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:50:56 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:50:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:50:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6433b6bf5bed8b3be159441dfeb9712971674bac4560ce7f8a4eff5ce13a7565`  
		Last Modified: Sat, 12 Feb 2022 01:53:02 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878f28cb8b52e741264e9f23c9e4b5591c3d645ad1f067025f9dd4d593c75def`  
		Last Modified: Sat, 12 Feb 2022 01:53:24 GMT  
		Size: 39.1 MB (39130384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a653e69a81e17e79e5c5c36302da1cfa43006b3728d594d6d7e7c2fb4858d2`  
		Last Modified: Sat, 12 Feb 2022 01:53:03 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9424e86dc77f20fb6ec25edf6c8122ceead8b081ec1f0da24ef376da60e31f`  
		Last Modified: Sat, 12 Feb 2022 01:53:02 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6919833dce23fe2753532ef08cc421715f317809ba4e185fbc8811c8fa7c3a`  
		Last Modified: Sat, 12 Feb 2022 01:53:02 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:024760593a5382fcb164da6ccf64917521b31a4022d554159df0cfdf6f9a93fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41722147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6152a0a0674b4d510143d2ef85cd83b6b18f50d2baf4e548c59fa3c4766a3d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 05:35:00 GMT
ARG CONSUL_VERSION=1.10.8
# Sat, 12 Feb 2022 05:35:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 05:35:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 05:35:03 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 05:35:17 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 05:35:18 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 05:35:18 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 05:35:19 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 05:35:20 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 05:35:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 05:35:22 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 05:35:24 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 05:35:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 05:35:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25aefc06e82caf22b59a89763786c40b81524f525dfcfc8dadac69a2ab2632ab`  
		Last Modified: Sat, 12 Feb 2022 05:36:33 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86316f29383a9851e34be85e1750acbf793a9d15df411ef25cb9fe4634c76d96`  
		Last Modified: Sat, 12 Feb 2022 05:36:39 GMT  
		Size: 39.0 MB (38999191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46dc202bffe4c9c2f3546afb9a871802b238b0e173d64c68f922e107704ed8fd`  
		Last Modified: Sat, 12 Feb 2022 05:36:34 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d1e85b96c64681f5c9141ae4a76db015a707f367579ef7dea37537d3065638`  
		Last Modified: Sat, 12 Feb 2022 05:36:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8357f4730f10146ed93b5604a8f992571671e257bc00c377168b777e50d5a32`  
		Last Modified: Sat, 12 Feb 2022 05:36:33 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.8` - linux; 386

```console
$ docker pull consul@sha256:be64a2fed0233627503f4541fa778d07dcd424ff4da861b425e3c2c3f9564238
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43094625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23295a8e8cbbfd6e3304c88db6c1c927efb08848165f1b2914e85d71457e0271`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:41:32 GMT
ARG CONSUL_VERSION=1.10.8
# Sat, 12 Feb 2022 01:41:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:41:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:41:33 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:42:11 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:42:12 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:42:13 GMT
# ARGS: CONSUL_VERSION=1.10.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:42:13 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:42:13 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:42:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:42:14 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:42:14 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:42:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:42:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3259d3be13e1fda280e5018f614200af83e3e58eefe3dc0cb7174a325253d5c5`  
		Last Modified: Sat, 12 Feb 2022 01:43:48 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e5a2980bd7e4eee5cda163a94f9adccae5e306cc64592af53d019a776dd25bf`  
		Last Modified: Sat, 12 Feb 2022 01:43:55 GMT  
		Size: 40.3 MB (40262442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28a217fece634a56740b237cf65ff30148c35190d97d26ff0694f25052aafa9`  
		Last Modified: Sat, 12 Feb 2022 01:43:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c6e01be3cf21cc803ab05104e8b2c25c381df12a8330a7da8215823dbedbe40`  
		Last Modified: Sat, 12 Feb 2022 01:43:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f34f69bc3459c2893ea74360bd5a1da6c08468c085b9105759d663d6429f314`  
		Last Modified: Sat, 12 Feb 2022 01:43:48 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11`

```console
$ docker pull consul@sha256:019e7f964280cd5719d60b8887fe20a349d1a0365acd06290ac1b055101d4e1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11` - linux; amd64

```console
$ docker pull consul@sha256:f99ee518f528354e5cd26a83ae8e79f6af91fd3a400a7f7a14df5d9b44b92edc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43914800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3fcb78af95a35b5fef1897f529b6a36606c8808d874a58f4de20e28c15062bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 07:21:45 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 07:21:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 07:21:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 07:21:46 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 07:22:29 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 07:22:30 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 07:22:31 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 07:22:31 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 07:22:31 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 07:22:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 07:22:32 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 07:22:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 07:22:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 07:22:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d27ad99797459cfe439f4d21342a1ab965047dca0e429f7dde81a103159966`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27825406a65b0ec2b2bbf6438bfcb532be9a0a5666a06936bda7915c46fa2300`  
		Last Modified: Sat, 12 Feb 2022 07:24:34 GMT  
		Size: 41.1 MB (41089003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d469d357853eb97127e5794d998b4da36b55c8646d821ceeb92ffb61369da2`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91da9c992cabc72868bb6e087b0e132bd21739deffbd605a633e02ce1e2b8f9b`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508d5646e7dc01f848081e2d57757483d4b2fca09bb7747bd516851ee166859b`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:dbbfd2b35c83bf48da8b50ffad63773357b3e694f66cb06caa93f08534708838
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41682452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c03b367769374b1a71345ab0c2186a0c83919bd442e8e118be0262d6984b46f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:49:33 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 01:49:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:49:35 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:50:00 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:50:02 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:50:04 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:50:04 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:50:05 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:50:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:50:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:50:07 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:50:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:50:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87008e907ff201560ab56249dd1fe2e0f38bef1f5607ba09eaf4426e29bc28b3`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17fa1c0968f07bbcf8466495b357c19a158f4899674e2893740d832c54bf55d`  
		Last Modified: Sat, 12 Feb 2022 01:52:47 GMT  
		Size: 39.0 MB (39045731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f7c3cf0aa9b8598143005b4a18a66a01deddf3a6d8bd68a8a894980a623ce1`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8f3ed270d044d28bb625f443e8feb3f47f4c0778a862389d185897088151f0`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c2d53002a37c745be8236d738a0c2f947f0f12facb6237a5550a407466983d`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:cc5070045e034b1d3f174a0f2ae07c0b9793205ec47c0e7885ea7c1d2637e184
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41512339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:914a15c49b3644619729ff16b1b5aed8c69bfc1ce785efa37d9cab57d5ab9cea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 05:33:59 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 05:33:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 05:34:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 05:34:01 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 05:34:40 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 05:34:41 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 05:34:42 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 05:34:43 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 05:34:44 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 05:34:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 05:34:46 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 05:34:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 05:34:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 05:34:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ea336a92bf8f73e3070ab338a8f12cb975d2b3d73ef22cd2407e49d8be7de9`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c33e691ddce6d3ef0585963707aef7e278ef31907dfd98111a399585c61de4`  
		Last Modified: Sat, 12 Feb 2022 05:36:20 GMT  
		Size: 38.8 MB (38789382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da5ccdab3234aa94b4dbfa8e40f5a9b7eaeabfee379f7ee06d2a974be5c2555`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea12eaec7f7d4880aee5242e5f1e57b7cc2f98fd9166e3c926d8070e943ba29`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68495a169dffb993d98286854bb2b1b08d3c28987c241649db2c8468e35cee9f`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; 386

```console
$ docker pull consul@sha256:1304773a9fe880a58e228887819f227f1e3702246c34602a5a5a2ca7bce3d0d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42735297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa0b311cd86f249cb811d35a57cffe14cf609863798aa111922ab2918842ab4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:38:37 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 01:38:37 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:38:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:38:39 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:41:10 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:41:11 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:41:12 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:41:12 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:41:13 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:41:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:41:13 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:41:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:41:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:41:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbd61929fc21fd52ad4759e0e3d437b2e1aa30ad7e8d4ae6daf652e6ae8403b`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bad2d753f0541317860d8bc2f2962125b4f4eea60f19a31633d666e38c8418`  
		Last Modified: Sat, 12 Feb 2022 01:43:27 GMT  
		Size: 39.9 MB (39903112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc31b349a8590c9fb6b4cdd492db6d8ee0c2a1633f71d9862dfb7102c66342`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ffe2fca8726b330c2452bad3261605b912b590481a82c00ae8ec3da02f9e72`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea127a71de44806c1cf6109eae7118a56eed39379cef7fd64c5fb96a9c84c37d`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.3`

```console
$ docker pull consul@sha256:019e7f964280cd5719d60b8887fe20a349d1a0365acd06290ac1b055101d4e1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.3` - linux; amd64

```console
$ docker pull consul@sha256:f99ee518f528354e5cd26a83ae8e79f6af91fd3a400a7f7a14df5d9b44b92edc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43914800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3fcb78af95a35b5fef1897f529b6a36606c8808d874a58f4de20e28c15062bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 07:21:45 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 07:21:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 07:21:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 07:21:46 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 07:22:29 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 07:22:30 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 07:22:31 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 07:22:31 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 07:22:31 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 07:22:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 07:22:32 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 07:22:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 07:22:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 07:22:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d27ad99797459cfe439f4d21342a1ab965047dca0e429f7dde81a103159966`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27825406a65b0ec2b2bbf6438bfcb532be9a0a5666a06936bda7915c46fa2300`  
		Last Modified: Sat, 12 Feb 2022 07:24:34 GMT  
		Size: 41.1 MB (41089003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d469d357853eb97127e5794d998b4da36b55c8646d821ceeb92ffb61369da2`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91da9c992cabc72868bb6e087b0e132bd21739deffbd605a633e02ce1e2b8f9b`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508d5646e7dc01f848081e2d57757483d4b2fca09bb7747bd516851ee166859b`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.3` - linux; arm variant v6

```console
$ docker pull consul@sha256:dbbfd2b35c83bf48da8b50ffad63773357b3e694f66cb06caa93f08534708838
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41682452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c03b367769374b1a71345ab0c2186a0c83919bd442e8e118be0262d6984b46f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:49:33 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 01:49:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:49:35 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:50:00 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:50:02 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:50:04 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:50:04 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:50:05 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:50:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:50:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:50:07 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:50:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:50:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87008e907ff201560ab56249dd1fe2e0f38bef1f5607ba09eaf4426e29bc28b3`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17fa1c0968f07bbcf8466495b357c19a158f4899674e2893740d832c54bf55d`  
		Last Modified: Sat, 12 Feb 2022 01:52:47 GMT  
		Size: 39.0 MB (39045731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f7c3cf0aa9b8598143005b4a18a66a01deddf3a6d8bd68a8a894980a623ce1`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8f3ed270d044d28bb625f443e8feb3f47f4c0778a862389d185897088151f0`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c2d53002a37c745be8236d738a0c2f947f0f12facb6237a5550a407466983d`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:cc5070045e034b1d3f174a0f2ae07c0b9793205ec47c0e7885ea7c1d2637e184
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41512339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:914a15c49b3644619729ff16b1b5aed8c69bfc1ce785efa37d9cab57d5ab9cea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 05:33:59 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 05:33:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 05:34:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 05:34:01 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 05:34:40 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 05:34:41 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 05:34:42 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 05:34:43 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 05:34:44 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 05:34:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 05:34:46 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 05:34:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 05:34:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 05:34:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ea336a92bf8f73e3070ab338a8f12cb975d2b3d73ef22cd2407e49d8be7de9`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c33e691ddce6d3ef0585963707aef7e278ef31907dfd98111a399585c61de4`  
		Last Modified: Sat, 12 Feb 2022 05:36:20 GMT  
		Size: 38.8 MB (38789382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da5ccdab3234aa94b4dbfa8e40f5a9b7eaeabfee379f7ee06d2a974be5c2555`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea12eaec7f7d4880aee5242e5f1e57b7cc2f98fd9166e3c926d8070e943ba29`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68495a169dffb993d98286854bb2b1b08d3c28987c241649db2c8468e35cee9f`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.3` - linux; 386

```console
$ docker pull consul@sha256:1304773a9fe880a58e228887819f227f1e3702246c34602a5a5a2ca7bce3d0d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42735297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa0b311cd86f249cb811d35a57cffe14cf609863798aa111922ab2918842ab4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:38:37 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 01:38:37 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:38:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:38:39 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:41:10 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:41:11 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:41:12 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:41:12 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:41:13 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:41:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:41:13 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:41:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:41:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:41:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbd61929fc21fd52ad4759e0e3d437b2e1aa30ad7e8d4ae6daf652e6ae8403b`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bad2d753f0541317860d8bc2f2962125b4f4eea60f19a31633d666e38c8418`  
		Last Modified: Sat, 12 Feb 2022 01:43:27 GMT  
		Size: 39.9 MB (39903112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc31b349a8590c9fb6b4cdd492db6d8ee0c2a1633f71d9862dfb7102c66342`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ffe2fca8726b330c2452bad3261605b912b590481a82c00ae8ec3da02f9e72`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea127a71de44806c1cf6109eae7118a56eed39379cef7fd64c5fb96a9c84c37d`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:671bd81da269da30192b65b2f630494164c4c5e2ab2f55dbd3b41e8817b4e25c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:2c290d091387db42da8168ba0ee07d6bddc97942962094c15cef4c1977709c28
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40158852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d03e471c6602db1256eecaf32462dd68d0ac952a05d14c794bb486fda99988e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 07:23:30 GMT
ARG CONSUL_VERSION=1.9.15
# Sat, 12 Feb 2022 07:23:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.15 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 07:23:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 07:23:31 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 07:24:11 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 07:24:12 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 07:24:13 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 07:24:13 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 07:24:13 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 07:24:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 07:24:13 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 07:24:14 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 07:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 07:24:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943154e69384903df18a528867e8166ce2323b6e5d0011a48ee392bc5397ce08`  
		Last Modified: Sat, 12 Feb 2022 07:25:00 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74a136b2f53c3669c75f7fa127b0e03362bdbe611ae22c41bc1d2b09515e474`  
		Last Modified: Sat, 12 Feb 2022 07:25:05 GMT  
		Size: 37.3 MB (37333055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10995bbe189b97ee0690408bb2da8eccf5611bdb3a02aeb685ab179b0d45f010`  
		Last Modified: Sat, 12 Feb 2022 07:25:00 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd2f600efda82794de5345973d02e259762b8b2aad69cb557dcd11f58453d8`  
		Last Modified: Sat, 12 Feb 2022 07:25:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02655599ee5afa20f4776a0539f6b1020510d57a9e14a76a82e85fd8968ee5af`  
		Last Modified: Sat, 12 Feb 2022 07:25:00 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:114d0fa7fbf8364b43de2be40dd4fe7f85019156dbbc8e57e268c0ce10d7d6d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38215792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:308a6fa2bf51e81b458920abbbb8a09dc28a0e9a56ad9c3c8a74c6090675e8ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:51:11 GMT
ARG CONSUL_VERSION=1.9.15
# Sat, 12 Feb 2022 01:51:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.15 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:51:12 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:51:14 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:51:36 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:51:38 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:51:39 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:51:40 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:51:40 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:51:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:51:41 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:51:42 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:51:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f6f3c9568b47c4bf44b4099672264efbf0dcbbbde4863686d69734b848d7ff`  
		Last Modified: Sat, 12 Feb 2022 01:53:35 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57af4e673ca60e6ec30cf030ea2e3b2c24a94a130f4968c84f74032ef3dc2f3`  
		Last Modified: Sat, 12 Feb 2022 01:53:54 GMT  
		Size: 35.6 MB (35579077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c36b13f758b324e17d809a7adbdf33b67e159b245e4b28fbcb33d75bb19c1`  
		Last Modified: Sat, 12 Feb 2022 01:53:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff8f832057f753e41d4ab053e1e5b0729f0758f618cbafb539edc33465fe3b6`  
		Last Modified: Sat, 12 Feb 2022 01:53:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6635806208ab7c02bcf738f7f96e45b0de027117964965ec9da5d4448e2df1`  
		Last Modified: Sat, 12 Feb 2022 01:53:35 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:cf31df6f329cdffe99933cbbbf02a65ef1533088d2b6b5408b6177b8f4677bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38160732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5c5678c8e60aa447dfc3697454315c21d60ac442f435680d0b6a55662add49e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 05:35:31 GMT
ARG CONSUL_VERSION=1.9.15
# Sat, 12 Feb 2022 05:35:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.15 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 05:35:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 05:35:34 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 05:35:44 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 05:35:44 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 05:35:45 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 05:35:46 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 05:35:47 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 05:35:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 05:35:49 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 05:35:51 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 05:35:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 05:35:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb72b6badac587cf22d2521704eb3cfd59e76846747bcce965a4e168a384acb`  
		Last Modified: Sat, 12 Feb 2022 05:36:50 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e6379da08e0632ead1dc178aebe4272be24ab7aed68f42403b096008156815`  
		Last Modified: Sat, 12 Feb 2022 05:36:55 GMT  
		Size: 35.4 MB (35437774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2059ec9e2695dffd78727fa4b7d2c40b0778e589ca76c7018779de3004a006`  
		Last Modified: Sat, 12 Feb 2022 05:36:50 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a58e4cff6ff8fa57a88669eeb1cc31c22a52ece7ced61552e405d90c5b2337`  
		Last Modified: Sat, 12 Feb 2022 05:36:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1800babce3f9238fd5bb6c088ac2e44bb0ebad4699ce75ba2ca1f4044d4ea71`  
		Last Modified: Sat, 12 Feb 2022 05:36:50 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:ce64644d31515aaa842ab6622af9938ff5ec55435f5ce5400cfcf9d2366655c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39514404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3db905419e5e28d054293da6b934f8d1948c822dc557baf57e9faf156fb33d43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:42:21 GMT
ARG CONSUL_VERSION=1.9.15
# Sat, 12 Feb 2022 01:42:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.15 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:42:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:42:23 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:42:51 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:42:52 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:42:53 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:42:54 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:42:54 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:42:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:42:54 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:42:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:42:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:42:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dacf6bfcd05ebee4b7814c1e2458230bc530ec3032332b864478262b32709b`  
		Last Modified: Sat, 12 Feb 2022 01:44:06 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c2f315c27b3d7dfb65ae29709d1eca3816562f0f1dace9d6e1035d5804a76c`  
		Last Modified: Sat, 12 Feb 2022 01:44:12 GMT  
		Size: 36.7 MB (36682221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a900872b2300734d9ce3cef3365280fe46505ac36583d43ca032ca78b2430fcf`  
		Last Modified: Sat, 12 Feb 2022 01:44:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c153625bb4bef08683d407250abd66ba10f71d027c761158eb362657287591`  
		Last Modified: Sat, 12 Feb 2022 01:44:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cfa48ca2fd0f3bc310d77e51d7fd852609e549dd9368534c6231e3ecc176cc`  
		Last Modified: Sat, 12 Feb 2022 01:44:06 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.15`

```console
$ docker pull consul@sha256:671bd81da269da30192b65b2f630494164c4c5e2ab2f55dbd3b41e8817b4e25c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.15` - linux; amd64

```console
$ docker pull consul@sha256:2c290d091387db42da8168ba0ee07d6bddc97942962094c15cef4c1977709c28
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40158852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d03e471c6602db1256eecaf32462dd68d0ac952a05d14c794bb486fda99988e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 07:23:30 GMT
ARG CONSUL_VERSION=1.9.15
# Sat, 12 Feb 2022 07:23:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.15 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 07:23:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 07:23:31 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 07:24:11 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 07:24:12 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 07:24:13 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 07:24:13 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 07:24:13 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 07:24:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 07:24:13 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 07:24:14 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 07:24:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 07:24:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943154e69384903df18a528867e8166ce2323b6e5d0011a48ee392bc5397ce08`  
		Last Modified: Sat, 12 Feb 2022 07:25:00 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74a136b2f53c3669c75f7fa127b0e03362bdbe611ae22c41bc1d2b09515e474`  
		Last Modified: Sat, 12 Feb 2022 07:25:05 GMT  
		Size: 37.3 MB (37333055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10995bbe189b97ee0690408bb2da8eccf5611bdb3a02aeb685ab179b0d45f010`  
		Last Modified: Sat, 12 Feb 2022 07:25:00 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcd2f600efda82794de5345973d02e259762b8b2aad69cb557dcd11f58453d8`  
		Last Modified: Sat, 12 Feb 2022 07:25:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02655599ee5afa20f4776a0539f6b1020510d57a9e14a76a82e85fd8968ee5af`  
		Last Modified: Sat, 12 Feb 2022 07:25:00 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.15` - linux; arm variant v6

```console
$ docker pull consul@sha256:114d0fa7fbf8364b43de2be40dd4fe7f85019156dbbc8e57e268c0ce10d7d6d8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38215792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:308a6fa2bf51e81b458920abbbb8a09dc28a0e9a56ad9c3c8a74c6090675e8ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:51:11 GMT
ARG CONSUL_VERSION=1.9.15
# Sat, 12 Feb 2022 01:51:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.15 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:51:12 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:51:14 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:51:36 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:51:38 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:51:39 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:51:40 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:51:40 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:51:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:51:41 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:51:42 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:51:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:51:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6f6f3c9568b47c4bf44b4099672264efbf0dcbbbde4863686d69734b848d7ff`  
		Last Modified: Sat, 12 Feb 2022 01:53:35 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57af4e673ca60e6ec30cf030ea2e3b2c24a94a130f4968c84f74032ef3dc2f3`  
		Last Modified: Sat, 12 Feb 2022 01:53:54 GMT  
		Size: 35.6 MB (35579077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154c36b13f758b324e17d809a7adbdf33b67e159b245e4b28fbcb33d75bb19c1`  
		Last Modified: Sat, 12 Feb 2022 01:53:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff8f832057f753e41d4ab053e1e5b0729f0758f618cbafb539edc33465fe3b6`  
		Last Modified: Sat, 12 Feb 2022 01:53:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6635806208ab7c02bcf738f7f96e45b0de027117964965ec9da5d4448e2df1`  
		Last Modified: Sat, 12 Feb 2022 01:53:35 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.15` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:cf31df6f329cdffe99933cbbbf02a65ef1533088d2b6b5408b6177b8f4677bd8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38160732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5c5678c8e60aa447dfc3697454315c21d60ac442f435680d0b6a55662add49e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 05:35:31 GMT
ARG CONSUL_VERSION=1.9.15
# Sat, 12 Feb 2022 05:35:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.15 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 05:35:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 05:35:34 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 05:35:44 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 05:35:44 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 05:35:45 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 05:35:46 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 05:35:47 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 05:35:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 05:35:49 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 05:35:51 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 05:35:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 05:35:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb72b6badac587cf22d2521704eb3cfd59e76846747bcce965a4e168a384acb`  
		Last Modified: Sat, 12 Feb 2022 05:36:50 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e6379da08e0632ead1dc178aebe4272be24ab7aed68f42403b096008156815`  
		Last Modified: Sat, 12 Feb 2022 05:36:55 GMT  
		Size: 35.4 MB (35437774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2059ec9e2695dffd78727fa4b7d2c40b0778e589ca76c7018779de3004a006`  
		Last Modified: Sat, 12 Feb 2022 05:36:50 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a58e4cff6ff8fa57a88669eeb1cc31c22a52ece7ced61552e405d90c5b2337`  
		Last Modified: Sat, 12 Feb 2022 05:36:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1800babce3f9238fd5bb6c088ac2e44bb0ebad4699ce75ba2ca1f4044d4ea71`  
		Last Modified: Sat, 12 Feb 2022 05:36:50 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.15` - linux; 386

```console
$ docker pull consul@sha256:ce64644d31515aaa842ab6622af9938ff5ec55435f5ce5400cfcf9d2366655c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39514404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3db905419e5e28d054293da6b934f8d1948c822dc557baf57e9faf156fb33d43`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:42:21 GMT
ARG CONSUL_VERSION=1.9.15
# Sat, 12 Feb 2022 01:42:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.15 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:42:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:42:23 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:42:51 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:42:52 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:42:53 GMT
# ARGS: CONSUL_VERSION=1.9.15
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:42:54 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:42:54 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:42:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:42:54 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:42:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:42:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:42:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6dacf6bfcd05ebee4b7814c1e2458230bc530ec3032332b864478262b32709b`  
		Last Modified: Sat, 12 Feb 2022 01:44:06 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c2f315c27b3d7dfb65ae29709d1eca3816562f0f1dace9d6e1035d5804a76c`  
		Last Modified: Sat, 12 Feb 2022 01:44:12 GMT  
		Size: 36.7 MB (36682221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a900872b2300734d9ce3cef3365280fe46505ac36583d43ca032ca78b2430fcf`  
		Last Modified: Sat, 12 Feb 2022 01:44:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c153625bb4bef08683d407250abd66ba10f71d027c761158eb362657287591`  
		Last Modified: Sat, 12 Feb 2022 01:44:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cfa48ca2fd0f3bc310d77e51d7fd852609e549dd9368534c6231e3ecc176cc`  
		Last Modified: Sat, 12 Feb 2022 01:44:06 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:019e7f964280cd5719d60b8887fe20a349d1a0365acd06290ac1b055101d4e1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:f99ee518f528354e5cd26a83ae8e79f6af91fd3a400a7f7a14df5d9b44b92edc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43914800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3fcb78af95a35b5fef1897f529b6a36606c8808d874a58f4de20e28c15062bd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 07:21:45 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 07:21:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 07:21:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 07:21:46 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 07:22:29 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 07:22:30 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 07:22:31 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 07:22:31 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 07:22:31 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 07:22:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 07:22:32 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 07:22:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 07:22:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 07:22:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d27ad99797459cfe439f4d21342a1ab965047dca0e429f7dde81a103159966`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27825406a65b0ec2b2bbf6438bfcb532be9a0a5666a06936bda7915c46fa2300`  
		Last Modified: Sat, 12 Feb 2022 07:24:34 GMT  
		Size: 41.1 MB (41089003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d469d357853eb97127e5794d998b4da36b55c8646d821ceeb92ffb61369da2`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91da9c992cabc72868bb6e087b0e132bd21739deffbd605a633e02ce1e2b8f9b`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508d5646e7dc01f848081e2d57757483d4b2fca09bb7747bd516851ee166859b`  
		Last Modified: Sat, 12 Feb 2022 07:24:29 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:dbbfd2b35c83bf48da8b50ffad63773357b3e694f66cb06caa93f08534708838
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41682452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c03b367769374b1a71345ab0c2186a0c83919bd442e8e118be0262d6984b46f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:49:33 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 01:49:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:49:35 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:50:00 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:50:02 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:50:04 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:50:04 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:50:05 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:50:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:50:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:50:07 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:50:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:50:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87008e907ff201560ab56249dd1fe2e0f38bef1f5607ba09eaf4426e29bc28b3`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17fa1c0968f07bbcf8466495b357c19a158f4899674e2893740d832c54bf55d`  
		Last Modified: Sat, 12 Feb 2022 01:52:47 GMT  
		Size: 39.0 MB (39045731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47f7c3cf0aa9b8598143005b4a18a66a01deddf3a6d8bd68a8a894980a623ce1`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8f3ed270d044d28bb625f443e8feb3f47f4c0778a862389d185897088151f0`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c2d53002a37c745be8236d738a0c2f947f0f12facb6237a5550a407466983d`  
		Last Modified: Sat, 12 Feb 2022 01:52:26 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:cc5070045e034b1d3f174a0f2ae07c0b9793205ec47c0e7885ea7c1d2637e184
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41512339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:914a15c49b3644619729ff16b1b5aed8c69bfc1ce785efa37d9cab57d5ab9cea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 05:33:59 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 05:33:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 05:34:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 05:34:01 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 05:34:40 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 05:34:41 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 05:34:42 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 05:34:43 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 05:34:44 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 05:34:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 05:34:46 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 05:34:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 05:34:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 05:34:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ea336a92bf8f73e3070ab338a8f12cb975d2b3d73ef22cd2407e49d8be7de9`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c33e691ddce6d3ef0585963707aef7e278ef31907dfd98111a399585c61de4`  
		Last Modified: Sat, 12 Feb 2022 05:36:20 GMT  
		Size: 38.8 MB (38789382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da5ccdab3234aa94b4dbfa8e40f5a9b7eaeabfee379f7ee06d2a974be5c2555`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea12eaec7f7d4880aee5242e5f1e57b7cc2f98fd9166e3c926d8070e943ba29`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68495a169dffb993d98286854bb2b1b08d3c28987c241649db2c8468e35cee9f`  
		Last Modified: Sat, 12 Feb 2022 05:36:15 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:1304773a9fe880a58e228887819f227f1e3702246c34602a5a5a2ca7bce3d0d5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42735297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfa0b311cd86f249cb811d35a57cffe14cf609863798aa111922ab2918842ab4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 12 Feb 2022 01:38:37 GMT
ARG CONSUL_VERSION=1.11.3
# Sat, 12 Feb 2022 01:38:37 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 12 Feb 2022 01:38:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 12 Feb 2022 01:38:39 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 12 Feb 2022 01:41:10 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 12 Feb 2022 01:41:11 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 12 Feb 2022 01:41:12 GMT
# ARGS: CONSUL_VERSION=1.11.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 12 Feb 2022 01:41:12 GMT
VOLUME [/consul/data]
# Sat, 12 Feb 2022 01:41:13 GMT
EXPOSE 8300
# Sat, 12 Feb 2022 01:41:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 12 Feb 2022 01:41:13 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 12 Feb 2022 01:41:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 12 Feb 2022 01:41:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 12 Feb 2022 01:41:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbd61929fc21fd52ad4759e0e3d437b2e1aa30ad7e8d4ae6daf652e6ae8403b`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bad2d753f0541317860d8bc2f2962125b4f4eea60f19a31633d666e38c8418`  
		Last Modified: Sat, 12 Feb 2022 01:43:27 GMT  
		Size: 39.9 MB (39903112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cbc31b349a8590c9fb6b4cdd492db6d8ee0c2a1633f71d9862dfb7102c66342`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ffe2fca8726b330c2452bad3261605b912b590481a82c00ae8ec3da02f9e72`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea127a71de44806c1cf6109eae7118a56eed39379cef7fd64c5fb96a9c84c37d`  
		Last Modified: Sat, 12 Feb 2022 01:43:21 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
