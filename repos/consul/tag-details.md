<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10`](#consul110)
-	[`consul:1.10.3`](#consul1103)
-	[`consul:1.11.0-beta`](#consul1110-beta)
-	[`consul:1.11.0-beta2`](#consul1110-beta2)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.16`](#consul1816)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.10`](#consul1910)
-	[`consul:latest`](#consullatest)

## `consul:1.10`

```console
$ docker pull consul@sha256:56bc74c3682e3590d4df1ed0c43e3d39277e5c77c0491a519808f129eb499e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10` - linux; amd64

```console
$ docker pull consul@sha256:ea0c81b79ad00b9b0065874b1fe4fc3a7cc7a468383ffd0934931755b10bdcc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43233913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb24f6d4612dbbcde5862f21745735e704c4f1c797ba8424aa79aa0983f2e39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 16:24:35 GMT
ARG CONSUL_VERSION=1.10.3
# Wed, 29 Sep 2021 16:24:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 16:24:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 16:24:36 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 16:24:43 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 16:24:44 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 16:24:45 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 16:24:45 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 16:24:45 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 16:24:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 16:24:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 16:24:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 16:24:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 16:24:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade918541562fa70db457377a9b574f9cf0cc8289c49ac06cb3edb4ecf827aaa`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79820d099ec4772e384e0eaa23e40b98c4d79cf9d439c6ef99dc23128fa2884`  
		Last Modified: Wed, 29 Sep 2021 16:25:53 GMT  
		Size: 40.4 MB (40416462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ca06282b9b5c4cdb099c567e61f1ac6f506c262e846c8f89888d7538308682`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9235f4089669a8cc4a0a88a67aa0d8754f0ecde0da402039e5cb4502a868c06c`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b694e38e70f2e6365e6147df869e8e349fd478149395ce8fa2eb544dd32c41b3`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:ec8833a883ccf61695c9e118f2561cc812ce6081de1c5d6ca99ac64eca263313
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39258860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302051b3bba1f7ac9355a831077280d848dac2c45e05aa37961ff4b352e617e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 28 Sep 2021 22:49:33 GMT
ARG CONSUL_VERSION=1.10.3
# Tue, 28 Sep 2021 22:49:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 28 Sep 2021 22:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 28 Sep 2021 22:49:35 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 28 Sep 2021 22:49:56 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 28 Sep 2021 22:49:58 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 28 Sep 2021 22:49:59 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 28 Sep 2021 22:50:00 GMT
VOLUME [/consul/data]
# Tue, 28 Sep 2021 22:50:00 GMT
EXPOSE 8300
# Tue, 28 Sep 2021 22:50:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 28 Sep 2021 22:50:01 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 28 Sep 2021 22:50:02 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 28 Sep 2021 22:50:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:50:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da7cefa00df6ff78bfc7540608f8d14649f5d72fdb973673d3aa7e9bde2b2c9`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4e2def815a282bc7d6b5f58239973151625a75cff173cc6848adcef176428`  
		Last Modified: Tue, 28 Sep 2021 22:52:31 GMT  
		Size: 36.6 MB (36631725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a0535cc4b7bf1cc2a78c3f39aafed9e8069d5682717d91d22108f7afc66287`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c0e7873b44e40365bbd3553506da5bc0670e4d37b1f417cba61a267f73e7ce`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98806548710feafb3559dbdf485a8df1f51e44d8c3f54f4d624e6043223a070b`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:34988991d554ab9d710529135c77747ba808b12654d1062c5811cb3465078221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39190366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d494725d24cc77ece20111697554c7e44d02326ac63bac482f6c5c7c520a427c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:39:58 GMT
ARG CONSUL_VERSION=1.10.3
# Tue, 02 Nov 2021 19:39:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:40:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:40:01 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:40:14 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:40:15 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:40:16 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:40:17 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:40:18 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:40:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:40:20 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:40:22 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:40:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:40:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37670a2a9dc09fe75ad47ca2b119cfaed5f2978da6f457430dee234dada7ea43`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919087a5490ea994435e800db080ee62a36ba94db46d8b2279447371e06648ad`  
		Last Modified: Tue, 02 Nov 2021 19:42:14 GMT  
		Size: 36.5 MB (36474046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b44e0042b56affa731efc3552e6d27a1c1a27c113ef7c2303abe8fb4a8c6c2`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020cd44b1a8b856d502623a20f69a02ed6f581b1955a5951159a088820f6052`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43e375f5a466436cb3909f15c21a61e93bf531c521f1ba1b6bb737296f910fa`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; 386

```console
$ docker pull consul@sha256:810147172165d1861193f87a55583023f135919737afcc5ddad863e448c7395f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42615890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a4e310ee1a1fa6e171ce608cf2476764a1e654e5a0a8c85c970b52e9e908929`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 06:43:31 GMT
ARG CONSUL_VERSION=1.10.3
# Wed, 29 Sep 2021 06:43:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 06:43:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 06:43:33 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 06:43:49 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 06:43:50 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 06:43:51 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 06:43:51 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 06:43:52 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 06:43:52 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 06:43:52 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 06:43:52 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 06:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 06:43:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f0394e9f2305788f6bafd0975a6a2e3c43418e6809e2ff439872aca4d09da`  
		Last Modified: Wed, 29 Sep 2021 06:45:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f971848c51ab8cf8b89d1b92921f705f9a5a545155a698680d858e779047481`  
		Last Modified: Wed, 29 Sep 2021 06:45:12 GMT  
		Size: 39.8 MB (39791423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73d59ac52bd93d9f63af1624940f851d392f5df22973301a63d1d813fb25f3`  
		Last Modified: Wed, 29 Sep 2021 06:45:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57764966449a0e7bf852ccc6219dcb1440bb2017faf2f7982331a2d1b4933d`  
		Last Modified: Wed, 29 Sep 2021 06:45:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66c11a991a1bc7d745b856c61084aeacc8d7d1eed3dc64e79effab644d8ec91`  
		Last Modified: Wed, 29 Sep 2021 06:45:05 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.3`

```console
$ docker pull consul@sha256:56bc74c3682e3590d4df1ed0c43e3d39277e5c77c0491a519808f129eb499e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.3` - linux; amd64

```console
$ docker pull consul@sha256:ea0c81b79ad00b9b0065874b1fe4fc3a7cc7a468383ffd0934931755b10bdcc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43233913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb24f6d4612dbbcde5862f21745735e704c4f1c797ba8424aa79aa0983f2e39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 16:24:35 GMT
ARG CONSUL_VERSION=1.10.3
# Wed, 29 Sep 2021 16:24:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 16:24:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 16:24:36 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 16:24:43 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 16:24:44 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 16:24:45 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 16:24:45 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 16:24:45 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 16:24:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 16:24:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 16:24:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 16:24:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 16:24:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade918541562fa70db457377a9b574f9cf0cc8289c49ac06cb3edb4ecf827aaa`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79820d099ec4772e384e0eaa23e40b98c4d79cf9d439c6ef99dc23128fa2884`  
		Last Modified: Wed, 29 Sep 2021 16:25:53 GMT  
		Size: 40.4 MB (40416462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ca06282b9b5c4cdb099c567e61f1ac6f506c262e846c8f89888d7538308682`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9235f4089669a8cc4a0a88a67aa0d8754f0ecde0da402039e5cb4502a868c06c`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b694e38e70f2e6365e6147df869e8e349fd478149395ce8fa2eb544dd32c41b3`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.3` - linux; arm variant v6

```console
$ docker pull consul@sha256:ec8833a883ccf61695c9e118f2561cc812ce6081de1c5d6ca99ac64eca263313
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39258860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302051b3bba1f7ac9355a831077280d848dac2c45e05aa37961ff4b352e617e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 28 Sep 2021 22:49:33 GMT
ARG CONSUL_VERSION=1.10.3
# Tue, 28 Sep 2021 22:49:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 28 Sep 2021 22:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 28 Sep 2021 22:49:35 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 28 Sep 2021 22:49:56 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 28 Sep 2021 22:49:58 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 28 Sep 2021 22:49:59 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 28 Sep 2021 22:50:00 GMT
VOLUME [/consul/data]
# Tue, 28 Sep 2021 22:50:00 GMT
EXPOSE 8300
# Tue, 28 Sep 2021 22:50:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 28 Sep 2021 22:50:01 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 28 Sep 2021 22:50:02 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 28 Sep 2021 22:50:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:50:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da7cefa00df6ff78bfc7540608f8d14649f5d72fdb973673d3aa7e9bde2b2c9`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4e2def815a282bc7d6b5f58239973151625a75cff173cc6848adcef176428`  
		Last Modified: Tue, 28 Sep 2021 22:52:31 GMT  
		Size: 36.6 MB (36631725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a0535cc4b7bf1cc2a78c3f39aafed9e8069d5682717d91d22108f7afc66287`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c0e7873b44e40365bbd3553506da5bc0670e4d37b1f417cba61a267f73e7ce`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98806548710feafb3559dbdf485a8df1f51e44d8c3f54f4d624e6043223a070b`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:34988991d554ab9d710529135c77747ba808b12654d1062c5811cb3465078221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39190366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d494725d24cc77ece20111697554c7e44d02326ac63bac482f6c5c7c520a427c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:39:58 GMT
ARG CONSUL_VERSION=1.10.3
# Tue, 02 Nov 2021 19:39:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:40:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:40:01 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:40:14 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:40:15 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:40:16 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:40:17 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:40:18 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:40:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:40:20 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:40:22 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:40:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:40:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37670a2a9dc09fe75ad47ca2b119cfaed5f2978da6f457430dee234dada7ea43`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919087a5490ea994435e800db080ee62a36ba94db46d8b2279447371e06648ad`  
		Last Modified: Tue, 02 Nov 2021 19:42:14 GMT  
		Size: 36.5 MB (36474046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b44e0042b56affa731efc3552e6d27a1c1a27c113ef7c2303abe8fb4a8c6c2`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020cd44b1a8b856d502623a20f69a02ed6f581b1955a5951159a088820f6052`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43e375f5a466436cb3909f15c21a61e93bf531c521f1ba1b6bb737296f910fa`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.3` - linux; 386

```console
$ docker pull consul@sha256:810147172165d1861193f87a55583023f135919737afcc5ddad863e448c7395f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42615890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a4e310ee1a1fa6e171ce608cf2476764a1e654e5a0a8c85c970b52e9e908929`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 06:43:31 GMT
ARG CONSUL_VERSION=1.10.3
# Wed, 29 Sep 2021 06:43:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 06:43:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 06:43:33 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 06:43:49 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 06:43:50 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 06:43:51 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 06:43:51 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 06:43:52 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 06:43:52 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 06:43:52 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 06:43:52 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 06:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 06:43:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f0394e9f2305788f6bafd0975a6a2e3c43418e6809e2ff439872aca4d09da`  
		Last Modified: Wed, 29 Sep 2021 06:45:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f971848c51ab8cf8b89d1b92921f705f9a5a545155a698680d858e779047481`  
		Last Modified: Wed, 29 Sep 2021 06:45:12 GMT  
		Size: 39.8 MB (39791423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73d59ac52bd93d9f63af1624940f851d392f5df22973301a63d1d813fb25f3`  
		Last Modified: Wed, 29 Sep 2021 06:45:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57764966449a0e7bf852ccc6219dcb1440bb2017faf2f7982331a2d1b4933d`  
		Last Modified: Wed, 29 Sep 2021 06:45:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66c11a991a1bc7d745b856c61084aeacc8d7d1eed3dc64e79effab644d8ec91`  
		Last Modified: Wed, 29 Sep 2021 06:45:05 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.0-beta`

```console
$ docker pull consul@sha256:e2fc2d59b052a6dd02fdff26172e063a286d1987c84df4b9a1fcbd61f7e8aa7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.0-beta` - linux; amd64

```console
$ docker pull consul@sha256:807300499b466a6eb6c07d6e3bead29ef8ec90630d9b16c2f4875421744e973c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43704618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4555735b6bcdb11a6a63ffc5dda051e991ed9730d44636b0c25bd5a97ede4a65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 20:22:36 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Tue, 02 Nov 2021 20:22:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 20:22:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 20:22:37 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 20:22:48 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 20:22:49 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 20:22:49 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 20:22:50 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 20:22:50 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 20:22:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 20:22:50 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 20:22:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 20:22:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 20:22:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3cdeb1f53db7e671d95ea2e85f37568d776bebd7dde6d3b4bd07b0c6f2f903`  
		Last Modified: Tue, 02 Nov 2021 20:23:13 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9335ccfbba70b5833768560a15b31b8baa397cc05f3a3719fae3b6a2be34bf7`  
		Last Modified: Tue, 02 Nov 2021 20:23:18 GMT  
		Size: 40.9 MB (40887164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc77a6ceae58ffbad0bf61b880a122bf95193b47f5f2a5b1a5e714b7570ea33`  
		Last Modified: Tue, 02 Nov 2021 20:23:13 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a53719b70379a3e1a6435a8d29adfa2fc6509d8249183de7be50bb8cd9ed12e`  
		Last Modified: Tue, 02 Nov 2021 20:23:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3f1b1579c9e4cc72e1281a4b589ade52c111e5546ab23b5039d86147d375a`  
		Last Modified: Tue, 02 Nov 2021 20:23:13 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; arm variant v6

```console
$ docker pull consul@sha256:e9b76e76dbe6a906f2789bf321f8259547cfd0ba50a6acabeade285737d97162
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39498400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2cc203ba7d8866ad5d24b7b3be9f3207225b6da423d315041d804be4348f67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:50:01 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Tue, 02 Nov 2021 19:50:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:50:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:50:03 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:50:17 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:50:19 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:50:21 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:50:21 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:50:22 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:50:22 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:50:22 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:50:23 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:50:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:50:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92855c656cf3d8ee6f8ac10939a68d9a9bcfa3d84e2c9446a1e3217834404a54`  
		Last Modified: Tue, 02 Nov 2021 19:51:53 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b1da1e7022add5083e24c5726559cfbc5e25a091cf6ff874d3fba31f8d3786`  
		Last Modified: Tue, 02 Nov 2021 19:52:14 GMT  
		Size: 36.9 MB (36871269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8332ee2a09e56f0c090fcd0e732af1d65befaf38e2c9a9e11cb99e6e7b1ea345`  
		Last Modified: Tue, 02 Nov 2021 19:51:54 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672fd51e0cc7f8ed13d6f78e75d53e239db6e320d3ddce43c71633305534a808`  
		Last Modified: Tue, 02 Nov 2021 19:51:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c513023b2ec7a8578c4329f1febbc4b1055308a81e9dc7d9acd3dfeb6740bf`  
		Last Modified: Tue, 02 Nov 2021 19:51:54 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a8d66ee95c5aa8743a06c6f90fa3177d5fc275535e275a0a539143385bddd5f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39280619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f18f696646a7240afa3aa9aebf958fc571a80f8698151bae40f54cd4f06e90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:39:27 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Tue, 02 Nov 2021 19:39:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:39:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:39:30 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:39:42 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:39:43 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:39:44 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:39:45 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:39:46 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:39:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:39:48 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:39:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:39:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38e03b4a2d20bbf14f632859993ac46d9a456f4e63ee8250d97ab3b17ae775c`  
		Last Modified: Tue, 02 Nov 2021 19:41:52 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2339f7564b2332ee170cf608cfa8334783908fabb5a55fa374212ae9a1986c4`  
		Last Modified: Tue, 02 Nov 2021 19:41:58 GMT  
		Size: 36.6 MB (36564296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee872d3decdee5f90f67f9ea5ae7cf3358ca5818b22b94b8678e38da47ec6d`  
		Last Modified: Tue, 02 Nov 2021 19:41:53 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2075ce661067f7b710232633aa4535449a02f57bcacba7ab5182abb02325665`  
		Last Modified: Tue, 02 Nov 2021 19:41:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91c407512d7c7aad5bb7a7c9fdb1ffcce547c49c86d90f6c3531e2cff2f289e`  
		Last Modified: Tue, 02 Nov 2021 19:41:52 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; 386

```console
$ docker pull consul@sha256:bf498d7986f934420337d17e46d6a367add461d305f69e6b721100c6e33d4597
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42535582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09c21942c840107a7f49ffcbd2d5a3392017618987c0c5433fc3d497cbdfe81`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Mon, 08 Nov 2021 21:03:49 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Mon, 08 Nov 2021 21:03:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 08 Nov 2021 21:03:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 08 Nov 2021 21:03:51 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 08 Nov 2021 21:04:00 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 08 Nov 2021 21:04:02 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 08 Nov 2021 21:04:03 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 08 Nov 2021 21:04:03 GMT
VOLUME [/consul/data]
# Mon, 08 Nov 2021 21:04:03 GMT
EXPOSE 8300
# Mon, 08 Nov 2021 21:04:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 08 Nov 2021 21:04:04 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 08 Nov 2021 21:04:04 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 08 Nov 2021 21:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 08 Nov 2021 21:04:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a4a39e678fe5d118e5f6ba9748715cea3d5e9741bf74c5f13badc8b5dcb5a`  
		Last Modified: Mon, 08 Nov 2021 21:04:44 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb041822ddccbef0e086f2c0c15827be1defe953edce8280544cbbd8bc20bf5`  
		Last Modified: Mon, 08 Nov 2021 21:04:50 GMT  
		Size: 39.7 MB (39711111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f86fedfcd8161e9fd06155a23632f746eb059d4be838002b03acabfbd20b1ad`  
		Last Modified: Mon, 08 Nov 2021 21:04:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1331427977e8cdf9efbbe148e277c6a37eb8d0ac1fd8797d46163f9fbae47902`  
		Last Modified: Mon, 08 Nov 2021 21:04:44 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a817d08b2e346bb376b2c329dab5dc350c035243f437c374e641873afd6d9137`  
		Last Modified: Mon, 08 Nov 2021 21:04:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.0-beta2`

```console
$ docker pull consul@sha256:e2fc2d59b052a6dd02fdff26172e063a286d1987c84df4b9a1fcbd61f7e8aa7e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.0-beta2` - linux; amd64

```console
$ docker pull consul@sha256:807300499b466a6eb6c07d6e3bead29ef8ec90630d9b16c2f4875421744e973c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43704618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4555735b6bcdb11a6a63ffc5dda051e991ed9730d44636b0c25bd5a97ede4a65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 20:22:36 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Tue, 02 Nov 2021 20:22:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 20:22:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 20:22:37 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 20:22:48 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 20:22:49 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 20:22:49 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 20:22:50 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 20:22:50 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 20:22:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 20:22:50 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 20:22:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 20:22:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 20:22:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3cdeb1f53db7e671d95ea2e85f37568d776bebd7dde6d3b4bd07b0c6f2f903`  
		Last Modified: Tue, 02 Nov 2021 20:23:13 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9335ccfbba70b5833768560a15b31b8baa397cc05f3a3719fae3b6a2be34bf7`  
		Last Modified: Tue, 02 Nov 2021 20:23:18 GMT  
		Size: 40.9 MB (40887164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc77a6ceae58ffbad0bf61b880a122bf95193b47f5f2a5b1a5e714b7570ea33`  
		Last Modified: Tue, 02 Nov 2021 20:23:13 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a53719b70379a3e1a6435a8d29adfa2fc6509d8249183de7be50bb8cd9ed12e`  
		Last Modified: Tue, 02 Nov 2021 20:23:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c3f1b1579c9e4cc72e1281a4b589ade52c111e5546ab23b5039d86147d375a`  
		Last Modified: Tue, 02 Nov 2021 20:23:13 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta2` - linux; arm variant v6

```console
$ docker pull consul@sha256:e9b76e76dbe6a906f2789bf321f8259547cfd0ba50a6acabeade285737d97162
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39498400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd2cc203ba7d8866ad5d24b7b3be9f3207225b6da423d315041d804be4348f67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:50:01 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Tue, 02 Nov 2021 19:50:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:50:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:50:03 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:50:17 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:50:19 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:50:21 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:50:21 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:50:22 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:50:22 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:50:22 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:50:23 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:50:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:50:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92855c656cf3d8ee6f8ac10939a68d9a9bcfa3d84e2c9446a1e3217834404a54`  
		Last Modified: Tue, 02 Nov 2021 19:51:53 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b1da1e7022add5083e24c5726559cfbc5e25a091cf6ff874d3fba31f8d3786`  
		Last Modified: Tue, 02 Nov 2021 19:52:14 GMT  
		Size: 36.9 MB (36871269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8332ee2a09e56f0c090fcd0e732af1d65befaf38e2c9a9e11cb99e6e7b1ea345`  
		Last Modified: Tue, 02 Nov 2021 19:51:54 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672fd51e0cc7f8ed13d6f78e75d53e239db6e320d3ddce43c71633305534a808`  
		Last Modified: Tue, 02 Nov 2021 19:51:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c513023b2ec7a8578c4329f1febbc4b1055308a81e9dc7d9acd3dfeb6740bf`  
		Last Modified: Tue, 02 Nov 2021 19:51:54 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a8d66ee95c5aa8743a06c6f90fa3177d5fc275535e275a0a539143385bddd5f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39280619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f18f696646a7240afa3aa9aebf958fc571a80f8698151bae40f54cd4f06e90`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:39:27 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Tue, 02 Nov 2021 19:39:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:39:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:39:30 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:39:42 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:39:43 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:39:44 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:39:45 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:39:46 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:39:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:39:48 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:39:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:39:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38e03b4a2d20bbf14f632859993ac46d9a456f4e63ee8250d97ab3b17ae775c`  
		Last Modified: Tue, 02 Nov 2021 19:41:52 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2339f7564b2332ee170cf608cfa8334783908fabb5a55fa374212ae9a1986c4`  
		Last Modified: Tue, 02 Nov 2021 19:41:58 GMT  
		Size: 36.6 MB (36564296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ee872d3decdee5f90f67f9ea5ae7cf3358ca5818b22b94b8678e38da47ec6d`  
		Last Modified: Tue, 02 Nov 2021 19:41:53 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2075ce661067f7b710232633aa4535449a02f57bcacba7ab5182abb02325665`  
		Last Modified: Tue, 02 Nov 2021 19:41:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f91c407512d7c7aad5bb7a7c9fdb1ffcce547c49c86d90f6c3531e2cff2f289e`  
		Last Modified: Tue, 02 Nov 2021 19:41:52 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta2` - linux; 386

```console
$ docker pull consul@sha256:bf498d7986f934420337d17e46d6a367add461d305f69e6b721100c6e33d4597
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42535582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09c21942c840107a7f49ffcbd2d5a3392017618987c0c5433fc3d497cbdfe81`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Mon, 08 Nov 2021 21:03:49 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Mon, 08 Nov 2021 21:03:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 08 Nov 2021 21:03:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 08 Nov 2021 21:03:51 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 08 Nov 2021 21:04:00 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 08 Nov 2021 21:04:02 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 08 Nov 2021 21:04:03 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 08 Nov 2021 21:04:03 GMT
VOLUME [/consul/data]
# Mon, 08 Nov 2021 21:04:03 GMT
EXPOSE 8300
# Mon, 08 Nov 2021 21:04:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 08 Nov 2021 21:04:04 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 08 Nov 2021 21:04:04 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 08 Nov 2021 21:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 08 Nov 2021 21:04:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691a4a39e678fe5d118e5f6ba9748715cea3d5e9741bf74c5f13badc8b5dcb5a`  
		Last Modified: Mon, 08 Nov 2021 21:04:44 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eb041822ddccbef0e086f2c0c15827be1defe953edce8280544cbbd8bc20bf5`  
		Last Modified: Mon, 08 Nov 2021 21:04:50 GMT  
		Size: 39.7 MB (39711111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f86fedfcd8161e9fd06155a23632f746eb059d4be838002b03acabfbd20b1ad`  
		Last Modified: Mon, 08 Nov 2021 21:04:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1331427977e8cdf9efbbe148e277c6a37eb8d0ac1fd8797d46163f9fbae47902`  
		Last Modified: Mon, 08 Nov 2021 21:04:44 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a817d08b2e346bb376b2c329dab5dc350c035243f437c374e641873afd6d9137`  
		Last Modified: Mon, 08 Nov 2021 21:04:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:f81e92a1a6656db3f4328a416f9395a2b9ad7c0b4c0a76467cb04cc63c9c5a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:541e3851f48c040f19e4076000daba05a83bd7e922a0b7fbf661cf5df2d4ccd9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47433180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4bb97d94c111082f2e145d08da6d1b22f684394898513a31d2f70a72b03bb3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 16:25:12 GMT
ARG CONSUL_VERSION=1.8.16
# Wed, 29 Sep 2021 16:25:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 16:25:13 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 16:25:13 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 16:25:25 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 16:25:26 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 16:25:27 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 16:25:27 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 16:25:27 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 16:25:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 16:25:27 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 16:25:28 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 16:25:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 16:25:28 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42c381b420f383a5ebde1ce105439dd93204b9c1768934edada58582acdfe0e`  
		Last Modified: Wed, 29 Sep 2021 16:26:22 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0193536d5c1706f90e9ce8779eb7dde2eeb635dcffffc9ede829fefd947658`  
		Last Modified: Wed, 29 Sep 2021 16:26:28 GMT  
		Size: 44.6 MB (44615731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a625b6289eae5fee0194858300faf871b924493266397090515c32efacc0a758`  
		Last Modified: Wed, 29 Sep 2021 16:26:22 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808664057177f4a857a8cdda43c4ab06884133bb7429a9b45b38035d96e07acd`  
		Last Modified: Wed, 29 Sep 2021 16:26:22 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23dc72228fcb5af219ce025545362599a06be40153900f3d5c9684ed649d102`  
		Last Modified: Wed, 29 Sep 2021 16:26:22 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:212568d44af123b93b4a51b038f451308b9c0fc422616f6f89e622ea95e03079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42637093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a63d875876f14e61e461aff09b97c3b84485a47b1dd5e68b67b6a78d0be7fb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 28 Sep 2021 22:50:58 GMT
ARG CONSUL_VERSION=1.8.16
# Tue, 28 Sep 2021 22:50:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 28 Sep 2021 22:50:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 28 Sep 2021 22:51:02 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 28 Sep 2021 22:51:17 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 28 Sep 2021 22:51:20 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 28 Sep 2021 22:51:23 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 28 Sep 2021 22:51:23 GMT
VOLUME [/consul/data]
# Tue, 28 Sep 2021 22:51:24 GMT
EXPOSE 8300
# Tue, 28 Sep 2021 22:51:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 28 Sep 2021 22:51:25 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 28 Sep 2021 22:51:25 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 28 Sep 2021 22:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:51:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552b65dc67d0c2d8f24041d8539eee777260120a3e7c81b5e24fe47ff3fd326d`  
		Last Modified: Tue, 28 Sep 2021 22:53:20 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d423dcfd9ab7587eb44dd25933fbd105b64a0ddc9673b2f4bcd73fa45ba36d45`  
		Last Modified: Tue, 28 Sep 2021 22:53:41 GMT  
		Size: 40.0 MB (40009963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f59d958324ee13e57568f5c5e887cb7dccac273caecccd1566b539ac8ae15b`  
		Last Modified: Tue, 28 Sep 2021 22:53:20 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6054beb8b485f747924f5b732cd51cb43cb00786d6e4abbc8e0ce83dccfe5b0`  
		Last Modified: Tue, 28 Sep 2021 22:53:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89cf0b300b3ec50d1edc3293a8c73f098643e87d5f2a04a7dd2296e828c24d0`  
		Last Modified: Tue, 28 Sep 2021 22:53:21 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:63ebdf3cdec6f9de9f5e81a0b9725652cc8f5f661bf19448b5cbf2bb0e606abe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42833149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ed7ea3306cdadf65bb608d7b7d63559603c0502e530ac190a4fc9f0c2e7720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:41:01 GMT
ARG CONSUL_VERSION=1.8.16
# Tue, 02 Nov 2021 19:41:02 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:41:03 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:41:04 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:41:14 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:41:15 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:41:16 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:41:17 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:41:18 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:41:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:41:20 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:41:22 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:41:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:41:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5e08520c6a6c13998ee67f4723d0936c944a1303ee767ece56747215c240d2`  
		Last Modified: Tue, 02 Nov 2021 19:42:44 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9ee0b3b0323a479b69a6ba5a64ae9c661df2b7bb25947dae3a0bbaf5abbc37`  
		Last Modified: Tue, 02 Nov 2021 19:42:49 GMT  
		Size: 40.1 MB (40116831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c170f4adc01a379af6cbb87e2460d6525439feffef4af1d60679cdb45430565`  
		Last Modified: Tue, 02 Nov 2021 19:42:44 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483f0f6ff67c8f024e472fcd99832c1e485a4b7bed52923d15aabe146a1c4268`  
		Last Modified: Tue, 02 Nov 2021 19:42:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb796399f053961433f610fda51636a8d2e604dcf33fcdd7d669b6a9c025e06f`  
		Last Modified: Tue, 02 Nov 2021 19:42:44 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:361c717924df5cd6632cb07dd54f3d4f7082637e85509433dfeb069a09054d60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (46989208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e43b746d063c56f847d7d3c5f48fdcc20e3ba16e7d24333f49ab14c6a0552b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 06:44:21 GMT
ARG CONSUL_VERSION=1.8.16
# Wed, 29 Sep 2021 06:44:22 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 06:44:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 06:44:23 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 06:44:36 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 06:44:37 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 06:44:38 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 06:44:38 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 06:44:38 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 06:44:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 06:44:39 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 06:44:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 06:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 06:44:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436e3116e857618df66c0ce22a2efded7fb820518882b8faf212ded43aab2ce3`  
		Last Modified: Wed, 29 Sep 2021 06:45:48 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e03f97f7c9b7cc0be55215c447246aca11123569a9e1c83f32f698f9a7df8e5`  
		Last Modified: Wed, 29 Sep 2021 06:45:55 GMT  
		Size: 44.2 MB (44164743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fe6a8d58e6b8945124e83780b4e355be4faeb4f36802f5a3be15f82d075868`  
		Last Modified: Wed, 29 Sep 2021 06:45:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007abe05f8fe4fd9b551b01e15fc0582ac06f53d9cb7f9f545620b714cf04a5`  
		Last Modified: Wed, 29 Sep 2021 06:45:48 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b411f00b4262e1b8bb8f2e9fab570842d04059220a743e554ba7380a15c53e0`  
		Last Modified: Wed, 29 Sep 2021 06:45:48 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.16`

```console
$ docker pull consul@sha256:f81e92a1a6656db3f4328a416f9395a2b9ad7c0b4c0a76467cb04cc63c9c5a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.16` - linux; amd64

```console
$ docker pull consul@sha256:541e3851f48c040f19e4076000daba05a83bd7e922a0b7fbf661cf5df2d4ccd9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47433180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc4bb97d94c111082f2e145d08da6d1b22f684394898513a31d2f70a72b03bb3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 16:25:12 GMT
ARG CONSUL_VERSION=1.8.16
# Wed, 29 Sep 2021 16:25:12 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 16:25:13 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 16:25:13 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 16:25:25 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 16:25:26 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 16:25:27 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 16:25:27 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 16:25:27 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 16:25:27 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 16:25:27 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 16:25:28 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 16:25:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 16:25:28 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42c381b420f383a5ebde1ce105439dd93204b9c1768934edada58582acdfe0e`  
		Last Modified: Wed, 29 Sep 2021 16:26:22 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0193536d5c1706f90e9ce8779eb7dde2eeb635dcffffc9ede829fefd947658`  
		Last Modified: Wed, 29 Sep 2021 16:26:28 GMT  
		Size: 44.6 MB (44615731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a625b6289eae5fee0194858300faf871b924493266397090515c32efacc0a758`  
		Last Modified: Wed, 29 Sep 2021 16:26:22 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808664057177f4a857a8cdda43c4ab06884133bb7429a9b45b38035d96e07acd`  
		Last Modified: Wed, 29 Sep 2021 16:26:22 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b23dc72228fcb5af219ce025545362599a06be40153900f3d5c9684ed649d102`  
		Last Modified: Wed, 29 Sep 2021 16:26:22 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.16` - linux; arm variant v6

```console
$ docker pull consul@sha256:212568d44af123b93b4a51b038f451308b9c0fc422616f6f89e622ea95e03079
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42637093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a63d875876f14e61e461aff09b97c3b84485a47b1dd5e68b67b6a78d0be7fb1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 28 Sep 2021 22:50:58 GMT
ARG CONSUL_VERSION=1.8.16
# Tue, 28 Sep 2021 22:50:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 28 Sep 2021 22:50:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 28 Sep 2021 22:51:02 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 28 Sep 2021 22:51:17 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 28 Sep 2021 22:51:20 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 28 Sep 2021 22:51:23 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 28 Sep 2021 22:51:23 GMT
VOLUME [/consul/data]
# Tue, 28 Sep 2021 22:51:24 GMT
EXPOSE 8300
# Tue, 28 Sep 2021 22:51:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 28 Sep 2021 22:51:25 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 28 Sep 2021 22:51:25 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 28 Sep 2021 22:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:51:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552b65dc67d0c2d8f24041d8539eee777260120a3e7c81b5e24fe47ff3fd326d`  
		Last Modified: Tue, 28 Sep 2021 22:53:20 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d423dcfd9ab7587eb44dd25933fbd105b64a0ddc9673b2f4bcd73fa45ba36d45`  
		Last Modified: Tue, 28 Sep 2021 22:53:41 GMT  
		Size: 40.0 MB (40009963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f59d958324ee13e57568f5c5e887cb7dccac273caecccd1566b539ac8ae15b`  
		Last Modified: Tue, 28 Sep 2021 22:53:20 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6054beb8b485f747924f5b732cd51cb43cb00786d6e4abbc8e0ce83dccfe5b0`  
		Last Modified: Tue, 28 Sep 2021 22:53:20 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89cf0b300b3ec50d1edc3293a8c73f098643e87d5f2a04a7dd2296e828c24d0`  
		Last Modified: Tue, 28 Sep 2021 22:53:21 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.16` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:63ebdf3cdec6f9de9f5e81a0b9725652cc8f5f661bf19448b5cbf2bb0e606abe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42833149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5ed7ea3306cdadf65bb608d7b7d63559603c0502e530ac190a4fc9f0c2e7720`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:41:01 GMT
ARG CONSUL_VERSION=1.8.16
# Tue, 02 Nov 2021 19:41:02 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:41:03 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:41:04 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:41:14 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:41:15 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:41:16 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:41:17 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:41:18 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:41:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:41:20 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:41:22 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:41:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:41:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5e08520c6a6c13998ee67f4723d0936c944a1303ee767ece56747215c240d2`  
		Last Modified: Tue, 02 Nov 2021 19:42:44 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9ee0b3b0323a479b69a6ba5a64ae9c661df2b7bb25947dae3a0bbaf5abbc37`  
		Last Modified: Tue, 02 Nov 2021 19:42:49 GMT  
		Size: 40.1 MB (40116831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c170f4adc01a379af6cbb87e2460d6525439feffef4af1d60679cdb45430565`  
		Last Modified: Tue, 02 Nov 2021 19:42:44 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483f0f6ff67c8f024e472fcd99832c1e485a4b7bed52923d15aabe146a1c4268`  
		Last Modified: Tue, 02 Nov 2021 19:42:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb796399f053961433f610fda51636a8d2e604dcf33fcdd7d669b6a9c025e06f`  
		Last Modified: Tue, 02 Nov 2021 19:42:44 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.16` - linux; 386

```console
$ docker pull consul@sha256:361c717924df5cd6632cb07dd54f3d4f7082637e85509433dfeb069a09054d60
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (46989208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10e43b746d063c56f847d7d3c5f48fdcc20e3ba16e7d24333f49ab14c6a0552b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 06:44:21 GMT
ARG CONSUL_VERSION=1.8.16
# Wed, 29 Sep 2021 06:44:22 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 06:44:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 06:44:23 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 06:44:36 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 06:44:37 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 06:44:38 GMT
# ARGS: CONSUL_VERSION=1.8.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 06:44:38 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 06:44:38 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 06:44:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 06:44:39 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 06:44:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 06:44:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 06:44:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436e3116e857618df66c0ce22a2efded7fb820518882b8faf212ded43aab2ce3`  
		Last Modified: Wed, 29 Sep 2021 06:45:48 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e03f97f7c9b7cc0be55215c447246aca11123569a9e1c83f32f698f9a7df8e5`  
		Last Modified: Wed, 29 Sep 2021 06:45:55 GMT  
		Size: 44.2 MB (44164743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2fe6a8d58e6b8945124e83780b4e355be4faeb4f36802f5a3be15f82d075868`  
		Last Modified: Wed, 29 Sep 2021 06:45:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007abe05f8fe4fd9b551b01e15fc0582ac06f53d9cb7f9f545620b714cf04a5`  
		Last Modified: Wed, 29 Sep 2021 06:45:48 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b411f00b4262e1b8bb8f2e9fab570842d04059220a743e554ba7380a15c53e0`  
		Last Modified: Wed, 29 Sep 2021 06:45:48 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:897ac6a36eef709846d6a569c958518943eead5bf0009cfe96aba51aad203c03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:b8f1e9c2d0e3c9b2714f89d3c74722b214b7695a540e8c32c34346c228b24a0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45897372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b86a727b9cd5edfe2bb01952b7d03112f5591448f86841679a9b8d9a1de48b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 16:24:51 GMT
ARG CONSUL_VERSION=1.9.10
# Wed, 29 Sep 2021 16:24:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 16:24:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 16:24:52 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 16:25:03 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 16:25:04 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 16:25:05 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 16:25:05 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 16:25:06 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 16:25:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 16:25:06 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 16:25:06 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 16:25:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 16:25:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d20b41a2463dbafecbf30282c8fa3fe27b157c1247ccd1c985a2a0d33941c4e`  
		Last Modified: Wed, 29 Sep 2021 16:26:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4e1de8517000479df2572121a93992c52eb1fddfc2afe95241f667dd00ebb4`  
		Last Modified: Wed, 29 Sep 2021 16:26:12 GMT  
		Size: 43.1 MB (43079922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a4417eedee015c4a740f4a6a8e88308ed076fba8d9ee0bd175679400c412bb`  
		Last Modified: Wed, 29 Sep 2021 16:26:06 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaabccedfe1cedc8a6c5f143e38c5a8ee80f8858654da63aa0d945de90b931e`  
		Last Modified: Wed, 29 Sep 2021 16:26:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485e277202b77c254c8bdacb9692aac90da396f8cb8491457216540155b528f9`  
		Last Modified: Wed, 29 Sep 2021 16:26:06 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:91dfa900b195c54464c486e9529a1f316fc10253345f201cbdeb28a5a161754d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41080020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50e96235aa66d0be636b7fca50e46fd18f82d8f16bf8528b5c170d6e731c745`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 28 Sep 2021 22:50:15 GMT
ARG CONSUL_VERSION=1.9.10
# Tue, 28 Sep 2021 22:50:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 28 Sep 2021 22:50:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 28 Sep 2021 22:50:20 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 28 Sep 2021 22:50:35 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 28 Sep 2021 22:50:38 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 28 Sep 2021 22:50:41 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 28 Sep 2021 22:50:42 GMT
VOLUME [/consul/data]
# Tue, 28 Sep 2021 22:50:43 GMT
EXPOSE 8300
# Tue, 28 Sep 2021 22:50:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 28 Sep 2021 22:50:44 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 28 Sep 2021 22:50:45 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 28 Sep 2021 22:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:50:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca0e30d54b8381f34b7a1e6b27a5cf266a93c3003d4dd958e200a78935acebb`  
		Last Modified: Tue, 28 Sep 2021 22:52:47 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3194cce0709f6da752b841103f390ba550b8527cc8934bd28ef97e589252cbe`  
		Last Modified: Tue, 28 Sep 2021 22:53:08 GMT  
		Size: 38.5 MB (38452887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5308cdfcf6a5e99774de613127df969d670dbd6549fca35ea17ea6a3ca83cee`  
		Last Modified: Tue, 28 Sep 2021 22:52:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5921b2b8c69f70330fc2993534bcb33a52f8de510dcd25e2041acf4da30b408f`  
		Last Modified: Tue, 28 Sep 2021 22:52:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe4aeae5d3513eb375ac5c50b58ef8e6d4cb3541dc3ccb75472eb903bb1297`  
		Last Modified: Tue, 28 Sep 2021 22:52:47 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:864847995ea6be6b70f59cdf7ac09a652343c54d3b8fa82a33e6ba71b10d27f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41339682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5c78c38f9224fd6fe3efc7c5cb5cba24b156615776d4cc4d75540a22994bbd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:40:30 GMT
ARG CONSUL_VERSION=1.9.10
# Tue, 02 Nov 2021 19:40:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:40:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:40:32 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:40:46 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:40:46 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:40:47 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:40:48 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:40:49 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:40:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:40:51 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:40:53 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:40:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b436b54f47049e6069259d7fc8339393760698cc1b644764a7ba3d25b08133c3`  
		Last Modified: Tue, 02 Nov 2021 19:42:28 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b563fadf7d77e4fdcb2a5d95a7071a01cf9bde18eb503f089382d2a4336e415b`  
		Last Modified: Tue, 02 Nov 2021 19:42:33 GMT  
		Size: 38.6 MB (38623361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789f0f14457535ac15fe8eae7c0dd83c57b78fc71b27555e8a997190c33f1cc2`  
		Last Modified: Tue, 02 Nov 2021 19:42:28 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0a2b3ba01475b1b01cca9cbaa1976af2ae0372971eb8787e0378ef013245b`  
		Last Modified: Tue, 02 Nov 2021 19:42:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d351a6b3f0c4ebbb0653488b417036bc49e2bb02a5ad5bceba0874235489e38b`  
		Last Modified: Tue, 02 Nov 2021 19:42:28 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:22ce0571ccf36151c98b515af2f14c04029ef1d6954769dc85609731d3b47d8c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45271915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ec8d54ddc9278a2fef971dd094f71aa4e7c6300873019baabb2acc50bfe790`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 06:43:59 GMT
ARG CONSUL_VERSION=1.9.10
# Wed, 29 Sep 2021 06:43:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 06:43:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 06:44:00 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 06:44:12 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 06:44:13 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 06:44:14 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 06:44:14 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 06:44:15 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 06:44:15 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 06:44:15 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 06:44:15 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 06:44:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 06:44:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101feacb8d52e7d34b0e0c701153e86a1ef24c60762496369dcf0c2597fb8f4f`  
		Last Modified: Wed, 29 Sep 2021 06:45:30 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad94defe75eac084f6836520a04b8aab302d914ad90488973dfc06b9746e202`  
		Last Modified: Wed, 29 Sep 2021 06:45:37 GMT  
		Size: 42.4 MB (42447446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daf12315d1950ac09ece349c87003bf6efe9ec66ecb43ba040768740ed5f969`  
		Last Modified: Wed, 29 Sep 2021 06:45:30 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9ebbdb289f021c8e22969bb3f1a02123c544704aafba5de7f4e373b61a2fe4`  
		Last Modified: Wed, 29 Sep 2021 06:45:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16e0641d298f627a32f6abf782dabc6fd5454b33a25c22049846f7a51fdaebe`  
		Last Modified: Wed, 29 Sep 2021 06:45:31 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.10`

```console
$ docker pull consul@sha256:897ac6a36eef709846d6a569c958518943eead5bf0009cfe96aba51aad203c03
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.10` - linux; amd64

```console
$ docker pull consul@sha256:b8f1e9c2d0e3c9b2714f89d3c74722b214b7695a540e8c32c34346c228b24a0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45897372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90b86a727b9cd5edfe2bb01952b7d03112f5591448f86841679a9b8d9a1de48b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 16:24:51 GMT
ARG CONSUL_VERSION=1.9.10
# Wed, 29 Sep 2021 16:24:51 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 16:24:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 16:24:52 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 16:25:03 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 16:25:04 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 16:25:05 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 16:25:05 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 16:25:06 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 16:25:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 16:25:06 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 16:25:06 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 16:25:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 16:25:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d20b41a2463dbafecbf30282c8fa3fe27b157c1247ccd1c985a2a0d33941c4e`  
		Last Modified: Wed, 29 Sep 2021 16:26:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4e1de8517000479df2572121a93992c52eb1fddfc2afe95241f667dd00ebb4`  
		Last Modified: Wed, 29 Sep 2021 16:26:12 GMT  
		Size: 43.1 MB (43079922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a4417eedee015c4a740f4a6a8e88308ed076fba8d9ee0bd175679400c412bb`  
		Last Modified: Wed, 29 Sep 2021 16:26:06 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eaabccedfe1cedc8a6c5f143e38c5a8ee80f8858654da63aa0d945de90b931e`  
		Last Modified: Wed, 29 Sep 2021 16:26:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485e277202b77c254c8bdacb9692aac90da396f8cb8491457216540155b528f9`  
		Last Modified: Wed, 29 Sep 2021 16:26:06 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:91dfa900b195c54464c486e9529a1f316fc10253345f201cbdeb28a5a161754d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41080020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b50e96235aa66d0be636b7fca50e46fd18f82d8f16bf8528b5c170d6e731c745`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 28 Sep 2021 22:50:15 GMT
ARG CONSUL_VERSION=1.9.10
# Tue, 28 Sep 2021 22:50:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 28 Sep 2021 22:50:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 28 Sep 2021 22:50:20 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 28 Sep 2021 22:50:35 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 28 Sep 2021 22:50:38 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 28 Sep 2021 22:50:41 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 28 Sep 2021 22:50:42 GMT
VOLUME [/consul/data]
# Tue, 28 Sep 2021 22:50:43 GMT
EXPOSE 8300
# Tue, 28 Sep 2021 22:50:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 28 Sep 2021 22:50:44 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 28 Sep 2021 22:50:45 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 28 Sep 2021 22:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:50:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca0e30d54b8381f34b7a1e6b27a5cf266a93c3003d4dd958e200a78935acebb`  
		Last Modified: Tue, 28 Sep 2021 22:52:47 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3194cce0709f6da752b841103f390ba550b8527cc8934bd28ef97e589252cbe`  
		Last Modified: Tue, 28 Sep 2021 22:53:08 GMT  
		Size: 38.5 MB (38452887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5308cdfcf6a5e99774de613127df969d670dbd6549fca35ea17ea6a3ca83cee`  
		Last Modified: Tue, 28 Sep 2021 22:52:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5921b2b8c69f70330fc2993534bcb33a52f8de510dcd25e2041acf4da30b408f`  
		Last Modified: Tue, 28 Sep 2021 22:52:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ebe4aeae5d3513eb375ac5c50b58ef8e6d4cb3541dc3ccb75472eb903bb1297`  
		Last Modified: Tue, 28 Sep 2021 22:52:47 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:864847995ea6be6b70f59cdf7ac09a652343c54d3b8fa82a33e6ba71b10d27f0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41339682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5c78c38f9224fd6fe3efc7c5cb5cba24b156615776d4cc4d75540a22994bbd2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:40:30 GMT
ARG CONSUL_VERSION=1.9.10
# Tue, 02 Nov 2021 19:40:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:40:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:40:32 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:40:46 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:40:46 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:40:47 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:40:48 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:40:49 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:40:50 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:40:51 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:40:53 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:40:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:40:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b436b54f47049e6069259d7fc8339393760698cc1b644764a7ba3d25b08133c3`  
		Last Modified: Tue, 02 Nov 2021 19:42:28 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b563fadf7d77e4fdcb2a5d95a7071a01cf9bde18eb503f089382d2a4336e415b`  
		Last Modified: Tue, 02 Nov 2021 19:42:33 GMT  
		Size: 38.6 MB (38623361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789f0f14457535ac15fe8eae7c0dd83c57b78fc71b27555e8a997190c33f1cc2`  
		Last Modified: Tue, 02 Nov 2021 19:42:28 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee0a2b3ba01475b1b01cca9cbaa1976af2ae0372971eb8787e0378ef013245b`  
		Last Modified: Tue, 02 Nov 2021 19:42:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d351a6b3f0c4ebbb0653488b417036bc49e2bb02a5ad5bceba0874235489e38b`  
		Last Modified: Tue, 02 Nov 2021 19:42:28 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.10` - linux; 386

```console
$ docker pull consul@sha256:22ce0571ccf36151c98b515af2f14c04029ef1d6954769dc85609731d3b47d8c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45271915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ec8d54ddc9278a2fef971dd094f71aa4e7c6300873019baabb2acc50bfe790`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 06:43:59 GMT
ARG CONSUL_VERSION=1.9.10
# Wed, 29 Sep 2021 06:43:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 06:43:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 06:44:00 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 06:44:12 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 06:44:13 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 06:44:14 GMT
# ARGS: CONSUL_VERSION=1.9.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 06:44:14 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 06:44:15 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 06:44:15 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 06:44:15 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 06:44:15 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 06:44:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 06:44:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101feacb8d52e7d34b0e0c701153e86a1ef24c60762496369dcf0c2597fb8f4f`  
		Last Modified: Wed, 29 Sep 2021 06:45:30 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad94defe75eac084f6836520a04b8aab302d914ad90488973dfc06b9746e202`  
		Last Modified: Wed, 29 Sep 2021 06:45:37 GMT  
		Size: 42.4 MB (42447446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daf12315d1950ac09ece349c87003bf6efe9ec66ecb43ba040768740ed5f969`  
		Last Modified: Wed, 29 Sep 2021 06:45:30 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9ebbdb289f021c8e22969bb3f1a02123c544704aafba5de7f4e373b61a2fe4`  
		Last Modified: Wed, 29 Sep 2021 06:45:30 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16e0641d298f627a32f6abf782dabc6fd5454b33a25c22049846f7a51fdaebe`  
		Last Modified: Wed, 29 Sep 2021 06:45:31 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:56bc74c3682e3590d4df1ed0c43e3d39277e5c77c0491a519808f129eb499e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:ea0c81b79ad00b9b0065874b1fe4fc3a7cc7a468383ffd0934931755b10bdcc8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43233913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adb24f6d4612dbbcde5862f21745735e704c4f1c797ba8424aa79aa0983f2e39`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 16:24:35 GMT
ARG CONSUL_VERSION=1.10.3
# Wed, 29 Sep 2021 16:24:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 16:24:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 16:24:36 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 16:24:43 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 16:24:44 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 16:24:45 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 16:24:45 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 16:24:45 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 16:24:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 16:24:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 16:24:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 16:24:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 16:24:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade918541562fa70db457377a9b574f9cf0cc8289c49ac06cb3edb4ecf827aaa`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79820d099ec4772e384e0eaa23e40b98c4d79cf9d439c6ef99dc23128fa2884`  
		Last Modified: Wed, 29 Sep 2021 16:25:53 GMT  
		Size: 40.4 MB (40416462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ca06282b9b5c4cdb099c567e61f1ac6f506c262e846c8f89888d7538308682`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9235f4089669a8cc4a0a88a67aa0d8754f0ecde0da402039e5cb4502a868c06c`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b694e38e70f2e6365e6147df869e8e349fd478149395ce8fa2eb544dd32c41b3`  
		Last Modified: Wed, 29 Sep 2021 16:25:47 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:ec8833a883ccf61695c9e118f2561cc812ce6081de1c5d6ca99ac64eca263313
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39258860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:302051b3bba1f7ac9355a831077280d848dac2c45e05aa37961ff4b352e617e1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Tue, 28 Sep 2021 22:49:33 GMT
ARG CONSUL_VERSION=1.10.3
# Tue, 28 Sep 2021 22:49:33 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 28 Sep 2021 22:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 28 Sep 2021 22:49:35 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 28 Sep 2021 22:49:56 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 28 Sep 2021 22:49:58 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 28 Sep 2021 22:49:59 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 28 Sep 2021 22:50:00 GMT
VOLUME [/consul/data]
# Tue, 28 Sep 2021 22:50:00 GMT
EXPOSE 8300
# Tue, 28 Sep 2021 22:50:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 28 Sep 2021 22:50:01 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 28 Sep 2021 22:50:02 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 28 Sep 2021 22:50:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Sep 2021 22:50:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da7cefa00df6ff78bfc7540608f8d14649f5d72fdb973673d3aa7e9bde2b2c9`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f4e2def815a282bc7d6b5f58239973151625a75cff173cc6848adcef176428`  
		Last Modified: Tue, 28 Sep 2021 22:52:31 GMT  
		Size: 36.6 MB (36631725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a0535cc4b7bf1cc2a78c3f39aafed9e8069d5682717d91d22108f7afc66287`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c0e7873b44e40365bbd3553506da5bc0670e4d37b1f417cba61a267f73e7ce`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98806548710feafb3559dbdf485a8df1f51e44d8c3f54f4d624e6043223a070b`  
		Last Modified: Tue, 28 Sep 2021 22:52:12 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:34988991d554ab9d710529135c77747ba808b12654d1062c5811cb3465078221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39190366 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d494725d24cc77ece20111697554c7e44d02326ac63bac482f6c5c7c520a427c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 01 Sep 2021 02:50:45 GMT
ADD file:924de68748d5d710724ceb45b3bff9d38eedcad50d5744be4ce74f8f731a791f in / 
# Wed, 01 Sep 2021 02:50:45 GMT
CMD ["/bin/sh"]
# Tue, 02 Nov 2021 19:39:58 GMT
ARG CONSUL_VERSION=1.10.3
# Tue, 02 Nov 2021 19:39:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 02 Nov 2021 19:40:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 02 Nov 2021 19:40:01 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 02 Nov 2021 19:40:14 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 02 Nov 2021 19:40:15 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 02 Nov 2021 19:40:16 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 02 Nov 2021 19:40:17 GMT
VOLUME [/consul/data]
# Tue, 02 Nov 2021 19:40:18 GMT
EXPOSE 8300
# Tue, 02 Nov 2021 19:40:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 02 Nov 2021 19:40:20 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 02 Nov 2021 19:40:22 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Nov 2021 19:40:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Nov 2021 19:40:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bbf911997326f5b56d515142e8dbdbe01d2f308276938ddbce3ab347584ed8ce`  
		Last Modified: Wed, 01 Sep 2021 02:51:37 GMT  
		Size: 2.7 MB (2713008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37670a2a9dc09fe75ad47ca2b119cfaed5f2978da6f457430dee234dada7ea43`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919087a5490ea994435e800db080ee62a36ba94db46d8b2279447371e06648ad`  
		Last Modified: Tue, 02 Nov 2021 19:42:14 GMT  
		Size: 36.5 MB (36474046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b44e0042b56affa731efc3552e6d27a1c1a27c113ef7c2303abe8fb4a8c6c2`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b020cd44b1a8b856d502623a20f69a02ed6f581b1955a5951159a088820f6052`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43e375f5a466436cb3909f15c21a61e93bf531c521f1ba1b6bb737296f910fa`  
		Last Modified: Tue, 02 Nov 2021 19:42:09 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:810147172165d1861193f87a55583023f135919737afcc5ddad863e448c7395f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42615890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a4e310ee1a1fa6e171ce608cf2476764a1e654e5a0a8c85c970b52e9e908929`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Wed, 29 Sep 2021 06:43:31 GMT
ARG CONSUL_VERSION=1.10.3
# Wed, 29 Sep 2021 06:43:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 29 Sep 2021 06:43:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 29 Sep 2021 06:43:33 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 29 Sep 2021 06:43:49 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 29 Sep 2021 06:43:50 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 29 Sep 2021 06:43:51 GMT
# ARGS: CONSUL_VERSION=1.10.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 29 Sep 2021 06:43:51 GMT
VOLUME [/consul/data]
# Wed, 29 Sep 2021 06:43:52 GMT
EXPOSE 8300
# Wed, 29 Sep 2021 06:43:52 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 29 Sep 2021 06:43:52 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 29 Sep 2021 06:43:52 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 29 Sep 2021 06:43:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Sep 2021 06:43:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13f0394e9f2305788f6bafd0975a6a2e3c43418e6809e2ff439872aca4d09da`  
		Last Modified: Wed, 29 Sep 2021 06:45:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f971848c51ab8cf8b89d1b92921f705f9a5a545155a698680d858e779047481`  
		Last Modified: Wed, 29 Sep 2021 06:45:12 GMT  
		Size: 39.8 MB (39791423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e73d59ac52bd93d9f63af1624940f851d392f5df22973301a63d1d813fb25f3`  
		Last Modified: Wed, 29 Sep 2021 06:45:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb57764966449a0e7bf852ccc6219dcb1440bb2017faf2f7982331a2d1b4933d`  
		Last Modified: Wed, 29 Sep 2021 06:45:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a66c11a991a1bc7d745b856c61084aeacc8d7d1eed3dc64e79effab644d8ec91`  
		Last Modified: Wed, 29 Sep 2021 06:45:05 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
