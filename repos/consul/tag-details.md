<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10`](#consul110)
-	[`consul:1.10.11`](#consul11011)
-	[`consul:1.11`](#consul111)
-	[`consul:1.11.6`](#consul1116)
-	[`consul:1.12`](#consul112)
-	[`consul:1.12.2`](#consul1122)
-	[`consul:latest`](#consullatest)

## `consul:1.10`

```console
$ docker pull consul@sha256:644f8d0032fdb8af9f693892cb15bc734fff1f3ab821c709eb0cb432c07c4332
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10` - linux; amd64

```console
$ docker pull consul@sha256:101d674b79b7b03e86ee357307545089eeb03d50c46b58d30cbda2f8037c515d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43251406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0c94fcddc533b1971aa19e2946147561bb3ac9003f7b545cc8e685bf29e5b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:19:48 GMT
ARG CONSUL_VERSION=1.10.11
# Fri, 27 May 2022 00:19:48 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:19:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:19:49 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:19:58 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:19:58 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:19:59 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:19:59 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:19:59 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:19:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:19:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:20:00 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:20:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441fc160a4dba269a9f2ee63095fcc8594350f02233d7ff9b8394c9da9a823ff`  
		Last Modified: Fri, 27 May 2022 00:20:49 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac91e983ee97584c340abe73f4049739a93716f5c208be14dc26ba263f9de1`  
		Last Modified: Fri, 27 May 2022 00:20:54 GMT  
		Size: 40.4 MB (40433467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc4432828ac748096beab217c318148c7698787b61b9c611a342d8c29419247`  
		Last Modified: Fri, 27 May 2022 00:20:49 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab48179f03310dd83ed4951281816ae068dc9f321894e745392f8f58f2dc7ff5`  
		Last Modified: Fri, 27 May 2022 00:20:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f17bde121172606dbed2e8ae78595bb942d27bb9c818d2491a9071c52b6ba74`  
		Last Modified: Fri, 27 May 2022 00:20:49 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:3d34f893f6e381a2943f4ea7d6492ab53c647aa9604b7275abafb0a102fd3875
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41046249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe84a8d68d01ecbc65891465ca0bfb0a3ece35a299061a5f712c2974c764a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Thu, 26 May 2022 23:50:43 GMT
ARG CONSUL_VERSION=1.10.11
# Thu, 26 May 2022 23:50:44 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 26 May 2022 23:50:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 26 May 2022 23:50:46 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 26 May 2022 23:50:58 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 26 May 2022 23:50:59 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 26 May 2022 23:51:01 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 May 2022 23:51:01 GMT
VOLUME [/consul/data]
# Thu, 26 May 2022 23:51:02 GMT
EXPOSE 8300
# Thu, 26 May 2022 23:51:02 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 26 May 2022 23:51:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 26 May 2022 23:51:03 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 26 May 2022 23:51:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 23:51:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85f47b15b49c2d17c8518b4def5d0c8f69bdd2a6d50fb2b0377f5ca1ec83d28`  
		Last Modified: Thu, 26 May 2022 23:53:04 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0be30b6ecd8982cb34d3b4ccd27ee22a76d76512e08ab96dca712713baff30`  
		Last Modified: Thu, 26 May 2022 23:53:25 GMT  
		Size: 38.4 MB (38420896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fed5886c3dc32059ae7c2538da7eca422d7fe96edb39aac10c99eb203c78b84`  
		Last Modified: Thu, 26 May 2022 23:53:04 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a01ff2d793fefa726d212b2ce24cea646bba43fe3a8457cedbe5590a88b91ae`  
		Last Modified: Thu, 26 May 2022 23:53:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c387612e8ac8800367959696281c9105d733c534cffe6d79657624d0777cf0`  
		Last Modified: Thu, 26 May 2022 23:53:04 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:fa83ee1f5379318b63dab83203fd38a0e869ae1752f5a745a5a9779320ed2299
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40901758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9f6835f3724199c62de00e27ed927f3969c3d49fa09cdb05593d5078dbb9c58`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:40:24 GMT
ARG CONSUL_VERSION=1.10.11
# Fri, 27 May 2022 00:40:25 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:40:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:40:27 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:40:34 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:40:34 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:40:35 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:40:36 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:40:37 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:40:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:40:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:40:41 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:40:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:40:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a11d7278c03c19a87844fbdc2c59b2b044b60b83b5c1f4246cfaa140af31c9e`  
		Last Modified: Fri, 27 May 2022 00:41:38 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069e66c8fce25292117394faf9d96cd893f8b480cf245048689572865f972d00`  
		Last Modified: Fri, 27 May 2022 00:41:43 GMT  
		Size: 38.2 MB (38181964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445018c86525b50a229e2007e1d87bf9a436df667aa94b3f83cf10d28d465ae0`  
		Last Modified: Fri, 27 May 2022 00:41:38 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd36f5ba23fad6451356e2fa158b333562f83e5376307ac09f216db89c663c3`  
		Last Modified: Fri, 27 May 2022 00:41:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1471267d920a645a46625022d73dfc1b707fe6609fbb5d4ff5848bb3d74dc9`  
		Last Modified: Fri, 27 May 2022 00:41:38 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; 386

```console
$ docker pull consul@sha256:771a34f5c6d08c8ae96d7ec0fb50a1d22b37a38e5a24438cb94c665a87ffac54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42095527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:745b41dfc79d5497d6b6560987ad72f14bcfdb083d7af3ac1fd384a6a055ac3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:39:15 GMT
ARG CONSUL_VERSION=1.10.11
# Fri, 27 May 2022 00:39:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:39:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:39:18 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:39:24 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:39:25 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:39:25 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:39:26 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:39:27 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:39:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:39:29 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:39:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:39:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:39:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31036bfa2e3e357eb6a54ace83c992312aaba6754181bf265ef3916503c668e`  
		Last Modified: Fri, 27 May 2022 00:40:35 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ad31debaa271a5cb6a7825e95412fb82481abcf2d429608c0a5d967625162`  
		Last Modified: Fri, 27 May 2022 00:40:41 GMT  
		Size: 39.3 MB (39273232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075a0377545d83b7699674c6f98cc5c12dfe1015d1edb2191596a88c3a105b39`  
		Last Modified: Fri, 27 May 2022 00:40:35 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7198f40072f7330e7b0dff1dd5a939aacb26dd75baa7d584c3d4acb90f4ade17`  
		Last Modified: Fri, 27 May 2022 00:40:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27f924bc6e60bfb4530259160625453162a858585c019e76eb3d3bc32373953`  
		Last Modified: Fri, 27 May 2022 00:40:35 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.11`

```console
$ docker pull consul@sha256:644f8d0032fdb8af9f693892cb15bc734fff1f3ab821c709eb0cb432c07c4332
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.11` - linux; amd64

```console
$ docker pull consul@sha256:101d674b79b7b03e86ee357307545089eeb03d50c46b58d30cbda2f8037c515d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43251406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc0c94fcddc533b1971aa19e2946147561bb3ac9003f7b545cc8e685bf29e5b0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:19:48 GMT
ARG CONSUL_VERSION=1.10.11
# Fri, 27 May 2022 00:19:48 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:19:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:19:49 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:19:58 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:19:58 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:19:59 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:19:59 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:19:59 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:19:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:19:59 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:20:00 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:20:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:441fc160a4dba269a9f2ee63095fcc8594350f02233d7ff9b8394c9da9a823ff`  
		Last Modified: Fri, 27 May 2022 00:20:49 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac91e983ee97584c340abe73f4049739a93716f5c208be14dc26ba263f9de1`  
		Last Modified: Fri, 27 May 2022 00:20:54 GMT  
		Size: 40.4 MB (40433467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc4432828ac748096beab217c318148c7698787b61b9c611a342d8c29419247`  
		Last Modified: Fri, 27 May 2022 00:20:49 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab48179f03310dd83ed4951281816ae068dc9f321894e745392f8f58f2dc7ff5`  
		Last Modified: Fri, 27 May 2022 00:20:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f17bde121172606dbed2e8ae78595bb942d27bb9c818d2491a9071c52b6ba74`  
		Last Modified: Fri, 27 May 2022 00:20:49 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:3d34f893f6e381a2943f4ea7d6492ab53c647aa9604b7275abafb0a102fd3875
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41046249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe84a8d68d01ecbc65891465ca0bfb0a3ece35a299061a5f712c2974c764a4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Thu, 26 May 2022 23:50:43 GMT
ARG CONSUL_VERSION=1.10.11
# Thu, 26 May 2022 23:50:44 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 26 May 2022 23:50:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 26 May 2022 23:50:46 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 26 May 2022 23:50:58 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 26 May 2022 23:50:59 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 26 May 2022 23:51:01 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 May 2022 23:51:01 GMT
VOLUME [/consul/data]
# Thu, 26 May 2022 23:51:02 GMT
EXPOSE 8300
# Thu, 26 May 2022 23:51:02 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 26 May 2022 23:51:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 26 May 2022 23:51:03 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 26 May 2022 23:51:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 23:51:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85f47b15b49c2d17c8518b4def5d0c8f69bdd2a6d50fb2b0377f5ca1ec83d28`  
		Last Modified: Thu, 26 May 2022 23:53:04 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0be30b6ecd8982cb34d3b4ccd27ee22a76d76512e08ab96dca712713baff30`  
		Last Modified: Thu, 26 May 2022 23:53:25 GMT  
		Size: 38.4 MB (38420896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fed5886c3dc32059ae7c2538da7eca422d7fe96edb39aac10c99eb203c78b84`  
		Last Modified: Thu, 26 May 2022 23:53:04 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a01ff2d793fefa726d212b2ce24cea646bba43fe3a8457cedbe5590a88b91ae`  
		Last Modified: Thu, 26 May 2022 23:53:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c387612e8ac8800367959696281c9105d733c534cffe6d79657624d0777cf0`  
		Last Modified: Thu, 26 May 2022 23:53:04 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:fa83ee1f5379318b63dab83203fd38a0e869ae1752f5a745a5a9779320ed2299
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40901758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9f6835f3724199c62de00e27ed927f3969c3d49fa09cdb05593d5078dbb9c58`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:40:24 GMT
ARG CONSUL_VERSION=1.10.11
# Fri, 27 May 2022 00:40:25 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:40:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:40:27 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:40:34 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:40:34 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:40:35 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:40:36 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:40:37 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:40:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:40:39 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:40:41 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:40:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:40:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a11d7278c03c19a87844fbdc2c59b2b044b60b83b5c1f4246cfaa140af31c9e`  
		Last Modified: Fri, 27 May 2022 00:41:38 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:069e66c8fce25292117394faf9d96cd893f8b480cf245048689572865f972d00`  
		Last Modified: Fri, 27 May 2022 00:41:43 GMT  
		Size: 38.2 MB (38181964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:445018c86525b50a229e2007e1d87bf9a436df667aa94b3f83cf10d28d465ae0`  
		Last Modified: Fri, 27 May 2022 00:41:38 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd36f5ba23fad6451356e2fa158b333562f83e5376307ac09f216db89c663c3`  
		Last Modified: Fri, 27 May 2022 00:41:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1471267d920a645a46625022d73dfc1b707fe6609fbb5d4ff5848bb3d74dc9`  
		Last Modified: Fri, 27 May 2022 00:41:38 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.11` - linux; 386

```console
$ docker pull consul@sha256:771a34f5c6d08c8ae96d7ec0fb50a1d22b37a38e5a24438cb94c665a87ffac54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42095527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:745b41dfc79d5497d6b6560987ad72f14bcfdb083d7af3ac1fd384a6a055ac3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:39:15 GMT
ARG CONSUL_VERSION=1.10.11
# Fri, 27 May 2022 00:39:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:39:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:39:18 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:39:24 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:39:25 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:39:25 GMT
# ARGS: CONSUL_VERSION=1.10.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:39:26 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:39:27 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:39:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:39:29 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:39:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:39:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:39:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31036bfa2e3e357eb6a54ace83c992312aaba6754181bf265ef3916503c668e`  
		Last Modified: Fri, 27 May 2022 00:40:35 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ad31debaa271a5cb6a7825e95412fb82481abcf2d429608c0a5d967625162`  
		Last Modified: Fri, 27 May 2022 00:40:41 GMT  
		Size: 39.3 MB (39273232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075a0377545d83b7699674c6f98cc5c12dfe1015d1edb2191596a88c3a105b39`  
		Last Modified: Fri, 27 May 2022 00:40:35 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7198f40072f7330e7b0dff1dd5a939aacb26dd75baa7d584c3d4acb90f4ade17`  
		Last Modified: Fri, 27 May 2022 00:40:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27f924bc6e60bfb4530259160625453162a858585c019e76eb3d3bc32373953`  
		Last Modified: Fri, 27 May 2022 00:40:35 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11`

```console
$ docker pull consul@sha256:b046770864f58edfa6bb58640677396a66a29efb6e193c973d7f87e15ee6f6fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11` - linux; amd64

```console
$ docker pull consul@sha256:f635a0327619fee7a807aa60bc41c9363d83f74957ec401687a71904d40e1d12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43999576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0182250079300c4983bdfc3594bcdce66cce94ffff76f61c0ec085c7dafb4f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:19:37 GMT
ARG CONSUL_VERSION=1.11.6
# Fri, 27 May 2022 00:19:37 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:19:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:19:37 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:19:43 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:19:44 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:19:44 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:19:44 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:19:45 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:19:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:19:45 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:19:45 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:19:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e060967d83fd13054eac8345ce33089f36ef96a9212da4441d9e9e0f1aae715`  
		Last Modified: Fri, 27 May 2022 00:20:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afc5de97f6f148731fc215772200fbb798431083eaa19a9c1acd888d1d8533d`  
		Last Modified: Fri, 27 May 2022 00:20:39 GMT  
		Size: 41.2 MB (41181636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eadbb99bd2de2f202eaf541edc8509c5d23027eb0a2cb55feb3735ac447521c`  
		Last Modified: Fri, 27 May 2022 00:20:34 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8f98fca8aa52f1c60d7e9efe3865288c4026683209895a0f9eae9bf48414aa`  
		Last Modified: Fri, 27 May 2022 00:20:34 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982c5b7b1b2d73a8554dbd4769e697db52a63952f1c37b89bc6cba7b4104309c`  
		Last Modified: Fri, 27 May 2022 00:20:34 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:b5d070929a1a1c2ce05580a16bb268698ec1e3357dbabb9d860c8c27acdfe648
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41740329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a434e27df12ba6e558a03e0f3d21dc57b6b6af6a37e08eed9fc6cd18d88cb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Thu, 26 May 2022 23:50:10 GMT
ARG CONSUL_VERSION=1.11.6
# Thu, 26 May 2022 23:50:11 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 26 May 2022 23:50:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 26 May 2022 23:50:13 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 26 May 2022 23:50:25 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 26 May 2022 23:50:27 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 26 May 2022 23:50:28 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 May 2022 23:50:29 GMT
VOLUME [/consul/data]
# Thu, 26 May 2022 23:50:29 GMT
EXPOSE 8300
# Thu, 26 May 2022 23:50:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 26 May 2022 23:50:30 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 26 May 2022 23:50:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 26 May 2022 23:50:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 23:50:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5455d64af8ec5ece27e3defed7b2381775bf872f113f6dffa9fc12de2284a349`  
		Last Modified: Thu, 26 May 2022 23:52:31 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2ec5f53771ec91089cc7efebaa218b65a0650a3255b1b758b83b090a38642c`  
		Last Modified: Thu, 26 May 2022 23:52:52 GMT  
		Size: 39.1 MB (39114977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4448084cb407eacd57aa5a72bfe67a130e39d278e0eecb8c61c6ad06f586f951`  
		Last Modified: Thu, 26 May 2022 23:52:31 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd01ffbfd7795bb3a1c5e188edbf58496ae2e8b8211e38e615a1c0642bca99e`  
		Last Modified: Thu, 26 May 2022 23:52:31 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db437298dcbbf73af4a6d80916ad40afe55eee4dd3c88a9c3ebee3e96befb17`  
		Last Modified: Thu, 26 May 2022 23:52:31 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:c7917d1fa7200d5c642126de1aa361372253e3d83a6ce8081f109791d268639d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604fdb7ec285be7d3e0ac6a18f714b765ff00521c567ea75d2adf2a2c8436059`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:39:57 GMT
ARG CONSUL_VERSION=1.11.6
# Fri, 27 May 2022 00:39:58 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:39:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:40:00 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:40:07 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:40:08 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:40:09 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:40:10 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:40:11 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:40:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:40:13 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:40:15 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:40:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:40:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2adf05ea5ec5e42eb9f9f2ec956e905676aa1f830f9482e447cbb11b3d1cf43`  
		Last Modified: Fri, 27 May 2022 00:41:22 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2000b267bedcb17f0acd679e05cc08aceecfa396144bdd42d3e30b875563ed`  
		Last Modified: Fri, 27 May 2022 00:41:27 GMT  
		Size: 38.8 MB (38837858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf010f6fdedb228bc57d3c6659c8260201b55399a8d64e0a2f65fbd44b238e9`  
		Last Modified: Fri, 27 May 2022 00:41:22 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f006b4aaaa3b4eef3ac73a24e60c2d8eb9ecc30c8730b6787cbbf8fbac5c4884`  
		Last Modified: Fri, 27 May 2022 00:41:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4beab7e92453c1c9f92ac1d0f0931e2929f9b45a71d960ed7536d16de6eaa8`  
		Last Modified: Fri, 27 May 2022 00:41:22 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; 386

```console
$ docker pull consul@sha256:fff11e60a399e4aaebd1200e335901d1f1cb21541934cdcc56a558284dcef25f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42806121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933747938b1c368edfc38fe0b3717bd2be7627529a7b36920a0925a85dda0e7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:38:52 GMT
ARG CONSUL_VERSION=1.11.6
# Fri, 27 May 2022 00:38:53 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:38:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:38:55 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:39:01 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:39:01 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:39:02 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:39:03 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:39:04 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:39:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:39:06 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:39:08 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:39:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:39:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d34b2565dddd8974c730d5af54f509ee50cfb6d9150881c729bbb26c1b8a379`  
		Last Modified: Fri, 27 May 2022 00:40:20 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cb6e27b14314d886c6a79d95260c810a54c07ea459e79ca2fffea750659f83`  
		Last Modified: Fri, 27 May 2022 00:40:25 GMT  
		Size: 40.0 MB (39983821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cc8573ff1def4c80e27e3ae25127f055133980ce5426eec42f936e691dcadb`  
		Last Modified: Fri, 27 May 2022 00:40:20 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc9dc0db4f165da6b0a8d12ad2eae4da64cd2637fffdadc03f9f2aafc0e1bf`  
		Last Modified: Fri, 27 May 2022 00:40:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0646ae57c861d1c725052453c1da30c52f223124884404f481fd6de1b3fb8844`  
		Last Modified: Fri, 27 May 2022 00:40:20 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.6`

```console
$ docker pull consul@sha256:b046770864f58edfa6bb58640677396a66a29efb6e193c973d7f87e15ee6f6fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.6` - linux; amd64

```console
$ docker pull consul@sha256:f635a0327619fee7a807aa60bc41c9363d83f74957ec401687a71904d40e1d12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43999576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0182250079300c4983bdfc3594bcdce66cce94ffff76f61c0ec085c7dafb4f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:19:37 GMT
ARG CONSUL_VERSION=1.11.6
# Fri, 27 May 2022 00:19:37 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:19:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:19:37 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:19:43 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:19:44 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:19:44 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:19:44 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:19:45 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:19:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:19:45 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:19:45 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:19:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e060967d83fd13054eac8345ce33089f36ef96a9212da4441d9e9e0f1aae715`  
		Last Modified: Fri, 27 May 2022 00:20:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afc5de97f6f148731fc215772200fbb798431083eaa19a9c1acd888d1d8533d`  
		Last Modified: Fri, 27 May 2022 00:20:39 GMT  
		Size: 41.2 MB (41181636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eadbb99bd2de2f202eaf541edc8509c5d23027eb0a2cb55feb3735ac447521c`  
		Last Modified: Fri, 27 May 2022 00:20:34 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b8f98fca8aa52f1c60d7e9efe3865288c4026683209895a0f9eae9bf48414aa`  
		Last Modified: Fri, 27 May 2022 00:20:34 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982c5b7b1b2d73a8554dbd4769e697db52a63952f1c37b89bc6cba7b4104309c`  
		Last Modified: Fri, 27 May 2022 00:20:34 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:b5d070929a1a1c2ce05580a16bb268698ec1e3357dbabb9d860c8c27acdfe648
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41740329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a434e27df12ba6e558a03e0f3d21dc57b6b6af6a37e08eed9fc6cd18d88cb8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Thu, 26 May 2022 23:50:10 GMT
ARG CONSUL_VERSION=1.11.6
# Thu, 26 May 2022 23:50:11 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 26 May 2022 23:50:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 26 May 2022 23:50:13 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 26 May 2022 23:50:25 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 26 May 2022 23:50:27 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 26 May 2022 23:50:28 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 26 May 2022 23:50:29 GMT
VOLUME [/consul/data]
# Thu, 26 May 2022 23:50:29 GMT
EXPOSE 8300
# Thu, 26 May 2022 23:50:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 26 May 2022 23:50:30 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 26 May 2022 23:50:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 26 May 2022 23:50:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 23:50:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5455d64af8ec5ece27e3defed7b2381775bf872f113f6dffa9fc12de2284a349`  
		Last Modified: Thu, 26 May 2022 23:52:31 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e2ec5f53771ec91089cc7efebaa218b65a0650a3255b1b758b83b090a38642c`  
		Last Modified: Thu, 26 May 2022 23:52:52 GMT  
		Size: 39.1 MB (39114977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4448084cb407eacd57aa5a72bfe67a130e39d278e0eecb8c61c6ad06f586f951`  
		Last Modified: Thu, 26 May 2022 23:52:31 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd01ffbfd7795bb3a1c5e188edbf58496ae2e8b8211e38e615a1c0642bca99e`  
		Last Modified: Thu, 26 May 2022 23:52:31 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db437298dcbbf73af4a6d80916ad40afe55eee4dd3c88a9c3ebee3e96befb17`  
		Last Modified: Thu, 26 May 2022 23:52:31 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:c7917d1fa7200d5c642126de1aa361372253e3d83a6ce8081f109791d268639d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41557655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:604fdb7ec285be7d3e0ac6a18f714b765ff00521c567ea75d2adf2a2c8436059`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:39:57 GMT
ARG CONSUL_VERSION=1.11.6
# Fri, 27 May 2022 00:39:58 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:39:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:40:00 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:40:07 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:40:08 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:40:09 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:40:10 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:40:11 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:40:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:40:13 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:40:15 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:40:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:40:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2adf05ea5ec5e42eb9f9f2ec956e905676aa1f830f9482e447cbb11b3d1cf43`  
		Last Modified: Fri, 27 May 2022 00:41:22 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2000b267bedcb17f0acd679e05cc08aceecfa396144bdd42d3e30b875563ed`  
		Last Modified: Fri, 27 May 2022 00:41:27 GMT  
		Size: 38.8 MB (38837858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf010f6fdedb228bc57d3c6659c8260201b55399a8d64e0a2f65fbd44b238e9`  
		Last Modified: Fri, 27 May 2022 00:41:22 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f006b4aaaa3b4eef3ac73a24e60c2d8eb9ecc30c8730b6787cbbf8fbac5c4884`  
		Last Modified: Fri, 27 May 2022 00:41:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4beab7e92453c1c9f92ac1d0f0931e2929f9b45a71d960ed7536d16de6eaa8`  
		Last Modified: Fri, 27 May 2022 00:41:22 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.6` - linux; 386

```console
$ docker pull consul@sha256:fff11e60a399e4aaebd1200e335901d1f1cb21541934cdcc56a558284dcef25f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42806121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933747938b1c368edfc38fe0b3717bd2be7627529a7b36920a0925a85dda0e7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Fri, 27 May 2022 00:38:52 GMT
ARG CONSUL_VERSION=1.11.6
# Fri, 27 May 2022 00:38:53 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 27 May 2022 00:38:54 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 27 May 2022 00:38:55 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 27 May 2022 00:39:01 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 27 May 2022 00:39:01 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 27 May 2022 00:39:02 GMT
# ARGS: CONSUL_VERSION=1.11.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 27 May 2022 00:39:03 GMT
VOLUME [/consul/data]
# Fri, 27 May 2022 00:39:04 GMT
EXPOSE 8300
# Fri, 27 May 2022 00:39:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 27 May 2022 00:39:06 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 27 May 2022 00:39:08 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 27 May 2022 00:39:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 27 May 2022 00:39:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d34b2565dddd8974c730d5af54f509ee50cfb6d9150881c729bbb26c1b8a379`  
		Last Modified: Fri, 27 May 2022 00:40:20 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cb6e27b14314d886c6a79d95260c810a54c07ea459e79ca2fffea750659f83`  
		Last Modified: Fri, 27 May 2022 00:40:25 GMT  
		Size: 40.0 MB (39983821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cc8573ff1def4c80e27e3ae25127f055133980ce5426eec42f936e691dcadb`  
		Last Modified: Fri, 27 May 2022 00:40:20 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bc9dc0db4f165da6b0a8d12ad2eae4da64cd2637fffdadc03f9f2aafc0e1bf`  
		Last Modified: Fri, 27 May 2022 00:40:20 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0646ae57c861d1c725052453c1da30c52f223124884404f481fd6de1b3fb8844`  
		Last Modified: Fri, 27 May 2022 00:40:20 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12`

```console
$ docker pull consul@sha256:ee0735e34f80030c46002f71bc594f25e3f586202da8784b43b4050993ef2445
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.12` - linux; amd64

```console
$ docker pull consul@sha256:a1a933572cb6f6388501c535af455f77e687c62ff97ed72cd16301b8b535eae0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49530995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8382d411eded180b186fa0dafa69be7eb8900927334e9bab5890768214face2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 18:27:05 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 18:27:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 18:27:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 18:27:06 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 18:27:11 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 18:27:12 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 18:27:12 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:27:12 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 18:27:12 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 18:27:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 18:27:13 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 18:27:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 18:27:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:27:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa48d4bd8bb86e29ae52b54a2008aa622c3781fd6acfa2e44cd5cf859c43b71`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3ef9b012a54ea43a997ab9743977bc7de3f516332dcd8999f4a4910b14122a`  
		Last Modified: Mon, 06 Jun 2022 18:27:35 GMT  
		Size: 46.7 MB (46713053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d239fc798a4c5e4c738352dbdcdd697322a05c5b89a9cd9ccc97a3abf1f2eb46`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199124be58be7085ef632c2297dde8e22271f783567ed177c68c6a2783bb7aec`  
		Last Modified: Mon, 06 Jun 2022 18:27:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3ccfe93b8bfca6058f2fab81810f5ba9c826430efab6bdd28121f00659804f`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm variant v6

```console
$ docker pull consul@sha256:562c2055e7b6163ad791098ab5f7fb763f7b58ef1b3a365326ddeb200af5bc07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47418871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ddedc80aeddd358a9aff2ade7924f8f3a0d19d7bf1a70abebfd2496501abb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:49:33 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:49:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:49:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:49:35 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:49:49 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:49:51 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:49:52 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:49:53 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:49:53 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:49:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:49:54 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:49:54 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:49:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172c64f605f02c13d89a26d7e1de51cf5f9989f437513d0bb157426ce7c9bddb`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99b94fb31045febe567631bd92baee9f2f2910606e6f037fc6a6e2a54cbd4d9`  
		Last Modified: Mon, 06 Jun 2022 17:51:20 GMT  
		Size: 44.8 MB (44793515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714921570995a97c88cc9e28f77625ad774b2608eeb728e8e341e98e6a256124`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adf595d95028707c1de711e10c2f3fa391c3e0a1521bf76b6590ba8d920e9c9`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3f382a916bc2905df02883c1cd108693474e87b57c30644c7f2eb5d2eed41e`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:c945c9f9d79e884233267d9c02105ffc460399dfaf09f31f38b7d7b1f43ab918
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47164176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4164dd78d95ff52b3c182bc2bf7ec45d64e72ce6c393cea25215d8bacea3577d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:47:05 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:47:06 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:47:07 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:47:08 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:47:14 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:47:15 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:47:15 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:47:16 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:47:17 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:47:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:47:19 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:47:21 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:47:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852dd48866308bd671353173a738be13359e088984374548057b76df8a03bdd9`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f57f7ce3f084ee916ca7c8580644f9e0e4e1e6b07b13b5720e572981816050`  
		Last Modified: Mon, 06 Jun 2022 17:47:58 GMT  
		Size: 44.4 MB (44444379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120c060cfede9a3c8d97bfb29222215dad767dfe20514beb78bf941e888e8cad`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be076a16914a6d835a25711f47eac0a9690a1ab7a7362915519b039a761d3d5d`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890c17b7a032ee37b9a6fe51b9dfdfa53b209f35799c507be8ab046f942b3497`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; 386

```console
$ docker pull consul@sha256:c7ee39a9eace8e5a94fbb79b8c659651a058a0ccccba3f3cd7218835ed75f5db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48612065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36be6b9b2a08cdf391475699a481ac9186505965fe95ca32e6caebddae126f89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:42:20 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:42:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:42:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:42:23 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:42:31 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:42:31 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:42:32 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:42:33 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:42:34 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:42:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:42:36 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:42:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:42:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:42:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c036d14492d1b2b557706d2e054d0380f769c81beceb949ed0600c7f58b9851b`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0356a6434d39e3976b4b6f9235bb3c740e70d4149e5c6b710c3653b247d0f07`  
		Last Modified: Mon, 06 Jun 2022 17:43:17 GMT  
		Size: 45.8 MB (45789766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5905d9eeb35e30123e93ddc94dadd6168fea4ecdd6a17474253b445809c33c`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891d5fc673fe12e6017707d85a284b60cd6f8bb339dfe4ed5f5d3565b77f0960`  
		Last Modified: Mon, 06 Jun 2022 17:43:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88d95e4cc9f19bd80a9f01ff330451cea70f9ce4e0e42aca657ccce2c513416`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12.2`

```console
$ docker pull consul@sha256:ee0735e34f80030c46002f71bc594f25e3f586202da8784b43b4050993ef2445
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.12.2` - linux; amd64

```console
$ docker pull consul@sha256:a1a933572cb6f6388501c535af455f77e687c62ff97ed72cd16301b8b535eae0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49530995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8382d411eded180b186fa0dafa69be7eb8900927334e9bab5890768214face2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 18:27:05 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 18:27:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 18:27:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 18:27:06 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 18:27:11 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 18:27:12 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 18:27:12 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:27:12 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 18:27:12 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 18:27:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 18:27:13 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 18:27:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 18:27:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:27:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa48d4bd8bb86e29ae52b54a2008aa622c3781fd6acfa2e44cd5cf859c43b71`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3ef9b012a54ea43a997ab9743977bc7de3f516332dcd8999f4a4910b14122a`  
		Last Modified: Mon, 06 Jun 2022 18:27:35 GMT  
		Size: 46.7 MB (46713053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d239fc798a4c5e4c738352dbdcdd697322a05c5b89a9cd9ccc97a3abf1f2eb46`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199124be58be7085ef632c2297dde8e22271f783567ed177c68c6a2783bb7aec`  
		Last Modified: Mon, 06 Jun 2022 18:27:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3ccfe93b8bfca6058f2fab81810f5ba9c826430efab6bdd28121f00659804f`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.2` - linux; arm variant v6

```console
$ docker pull consul@sha256:562c2055e7b6163ad791098ab5f7fb763f7b58ef1b3a365326ddeb200af5bc07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47418871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ddedc80aeddd358a9aff2ade7924f8f3a0d19d7bf1a70abebfd2496501abb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:49:33 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:49:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:49:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:49:35 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:49:49 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:49:51 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:49:52 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:49:53 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:49:53 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:49:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:49:54 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:49:54 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:49:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172c64f605f02c13d89a26d7e1de51cf5f9989f437513d0bb157426ce7c9bddb`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99b94fb31045febe567631bd92baee9f2f2910606e6f037fc6a6e2a54cbd4d9`  
		Last Modified: Mon, 06 Jun 2022 17:51:20 GMT  
		Size: 44.8 MB (44793515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714921570995a97c88cc9e28f77625ad774b2608eeb728e8e341e98e6a256124`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adf595d95028707c1de711e10c2f3fa391c3e0a1521bf76b6590ba8d920e9c9`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3f382a916bc2905df02883c1cd108693474e87b57c30644c7f2eb5d2eed41e`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:c945c9f9d79e884233267d9c02105ffc460399dfaf09f31f38b7d7b1f43ab918
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47164176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4164dd78d95ff52b3c182bc2bf7ec45d64e72ce6c393cea25215d8bacea3577d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:47:05 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:47:06 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:47:07 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:47:08 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:47:14 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:47:15 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:47:15 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:47:16 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:47:17 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:47:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:47:19 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:47:21 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:47:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852dd48866308bd671353173a738be13359e088984374548057b76df8a03bdd9`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f57f7ce3f084ee916ca7c8580644f9e0e4e1e6b07b13b5720e572981816050`  
		Last Modified: Mon, 06 Jun 2022 17:47:58 GMT  
		Size: 44.4 MB (44444379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120c060cfede9a3c8d97bfb29222215dad767dfe20514beb78bf941e888e8cad`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be076a16914a6d835a25711f47eac0a9690a1ab7a7362915519b039a761d3d5d`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890c17b7a032ee37b9a6fe51b9dfdfa53b209f35799c507be8ab046f942b3497`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.2` - linux; 386

```console
$ docker pull consul@sha256:c7ee39a9eace8e5a94fbb79b8c659651a058a0ccccba3f3cd7218835ed75f5db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48612065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36be6b9b2a08cdf391475699a481ac9186505965fe95ca32e6caebddae126f89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:42:20 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:42:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:42:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:42:23 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:42:31 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:42:31 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:42:32 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:42:33 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:42:34 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:42:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:42:36 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:42:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:42:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:42:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c036d14492d1b2b557706d2e054d0380f769c81beceb949ed0600c7f58b9851b`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0356a6434d39e3976b4b6f9235bb3c740e70d4149e5c6b710c3653b247d0f07`  
		Last Modified: Mon, 06 Jun 2022 17:43:17 GMT  
		Size: 45.8 MB (45789766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5905d9eeb35e30123e93ddc94dadd6168fea4ecdd6a17474253b445809c33c`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891d5fc673fe12e6017707d85a284b60cd6f8bb339dfe4ed5f5d3565b77f0960`  
		Last Modified: Mon, 06 Jun 2022 17:43:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88d95e4cc9f19bd80a9f01ff330451cea70f9ce4e0e42aca657ccce2c513416`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:ee0735e34f80030c46002f71bc594f25e3f586202da8784b43b4050993ef2445
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:a1a933572cb6f6388501c535af455f77e687c62ff97ed72cd16301b8b535eae0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49530995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8382d411eded180b186fa0dafa69be7eb8900927334e9bab5890768214face2b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 18:27:05 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 18:27:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 18:27:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 18:27:06 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 18:27:11 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 18:27:12 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 18:27:12 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 18:27:12 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 18:27:12 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 18:27:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 18:27:13 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 18:27:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 18:27:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 18:27:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa48d4bd8bb86e29ae52b54a2008aa622c3781fd6acfa2e44cd5cf859c43b71`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3ef9b012a54ea43a997ab9743977bc7de3f516332dcd8999f4a4910b14122a`  
		Last Modified: Mon, 06 Jun 2022 18:27:35 GMT  
		Size: 46.7 MB (46713053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d239fc798a4c5e4c738352dbdcdd697322a05c5b89a9cd9ccc97a3abf1f2eb46`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199124be58be7085ef632c2297dde8e22271f783567ed177c68c6a2783bb7aec`  
		Last Modified: Mon, 06 Jun 2022 18:27:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3ccfe93b8bfca6058f2fab81810f5ba9c826430efab6bdd28121f00659804f`  
		Last Modified: Mon, 06 Jun 2022 18:27:30 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:562c2055e7b6163ad791098ab5f7fb763f7b58ef1b3a365326ddeb200af5bc07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47418871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ddedc80aeddd358a9aff2ade7924f8f3a0d19d7bf1a70abebfd2496501abb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:49:33 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:49:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:49:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:49:35 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:49:49 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:49:51 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:49:52 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:49:53 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:49:53 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:49:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:49:54 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:49:54 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:49:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172c64f605f02c13d89a26d7e1de51cf5f9989f437513d0bb157426ce7c9bddb`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99b94fb31045febe567631bd92baee9f2f2910606e6f037fc6a6e2a54cbd4d9`  
		Last Modified: Mon, 06 Jun 2022 17:51:20 GMT  
		Size: 44.8 MB (44793515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714921570995a97c88cc9e28f77625ad774b2608eeb728e8e341e98e6a256124`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5adf595d95028707c1de711e10c2f3fa391c3e0a1521bf76b6590ba8d920e9c9`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3f382a916bc2905df02883c1cd108693474e87b57c30644c7f2eb5d2eed41e`  
		Last Modified: Mon, 06 Jun 2022 17:50:56 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:c945c9f9d79e884233267d9c02105ffc460399dfaf09f31f38b7d7b1f43ab918
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47164176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4164dd78d95ff52b3c182bc2bf7ec45d64e72ce6c393cea25215d8bacea3577d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:47:05 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:47:06 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:47:07 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:47:08 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:47:14 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:47:15 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:47:15 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:47:16 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:47:17 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:47:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:47:19 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:47:21 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:47:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852dd48866308bd671353173a738be13359e088984374548057b76df8a03bdd9`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f57f7ce3f084ee916ca7c8580644f9e0e4e1e6b07b13b5720e572981816050`  
		Last Modified: Mon, 06 Jun 2022 17:47:58 GMT  
		Size: 44.4 MB (44444379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120c060cfede9a3c8d97bfb29222215dad767dfe20514beb78bf941e888e8cad`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be076a16914a6d835a25711f47eac0a9690a1ab7a7362915519b039a761d3d5d`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890c17b7a032ee37b9a6fe51b9dfdfa53b209f35799c507be8ab046f942b3497`  
		Last Modified: Mon, 06 Jun 2022 17:47:52 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:c7ee39a9eace8e5a94fbb79b8c659651a058a0ccccba3f3cd7218835ed75f5db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48612065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36be6b9b2a08cdf391475699a481ac9186505965fe95ca32e6caebddae126f89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Mon, 06 Jun 2022 17:42:20 GMT
ARG CONSUL_VERSION=1.12.2
# Mon, 06 Jun 2022 17:42:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 06 Jun 2022 17:42:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 06 Jun 2022 17:42:23 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 06 Jun 2022 17:42:31 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 06 Jun 2022 17:42:31 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 06 Jun 2022 17:42:32 GMT
# ARGS: CONSUL_VERSION=1.12.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 06 Jun 2022 17:42:33 GMT
VOLUME [/consul/data]
# Mon, 06 Jun 2022 17:42:34 GMT
EXPOSE 8300
# Mon, 06 Jun 2022 17:42:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 06 Jun 2022 17:42:36 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 06 Jun 2022 17:42:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 06 Jun 2022 17:42:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 06 Jun 2022 17:42:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c036d14492d1b2b557706d2e054d0380f769c81beceb949ed0600c7f58b9851b`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0356a6434d39e3976b4b6f9235bb3c740e70d4149e5c6b710c3653b247d0f07`  
		Last Modified: Mon, 06 Jun 2022 17:43:17 GMT  
		Size: 45.8 MB (45789766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5905d9eeb35e30123e93ddc94dadd6168fea4ecdd6a17474253b445809c33c`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:891d5fc673fe12e6017707d85a284b60cd6f8bb339dfe4ed5f5d3565b77f0960`  
		Last Modified: Mon, 06 Jun 2022 17:43:12 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88d95e4cc9f19bd80a9f01ff330451cea70f9ce4e0e42aca657ccce2c513416`  
		Last Modified: Mon, 06 Jun 2022 17:43:11 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
