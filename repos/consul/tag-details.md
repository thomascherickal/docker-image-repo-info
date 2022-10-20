<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.11`](#consul111)
-	[`consul:1.11.11`](#consul11111)
-	[`consul:1.12`](#consul112)
-	[`consul:1.12.6`](#consul1126)
-	[`consul:1.13`](#consul113)
-	[`consul:1.13.3`](#consul1133)
-	[`consul:latest`](#consullatest)

## `consul:1.11`

```console
$ docker pull consul@sha256:9c02e7dc7959e1c2a6571cfd2a18ff5f7b2a8a9a86ff75882f78afbb41e8a9a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11` - linux; amd64

```console
$ docker pull consul@sha256:345220f37d6974489a10af67779b5c433f3632f5fb60a9c2aaf4206799134d11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44061699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee4fdcdbbe9accfb490032e70bdbb8e7b901eb33f810a532dd1e76a96aeb1733`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:18:06 GMT
ARG CONSUL_VERSION=1.11.10
# Thu, 06 Oct 2022 20:18:06 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 20:18:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 20:18:07 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 20:18:12 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 20:18:13 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 20:18:14 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:18:14 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 20:18:14 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 20:18:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 20:18:14 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 20:18:14 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 20:18:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:18:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72a43df3dacc3371f92b5b497b890fa32d8c892e2ca5d676abcf568a8d7af6f`  
		Last Modified: Thu, 06 Oct 2022 20:19:01 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dce1671656f1d20a03e9c2d6f00b7bd8b0ac53e397b217b58b4324e212bd10`  
		Last Modified: Thu, 06 Oct 2022 20:19:06 GMT  
		Size: 41.2 MB (41234803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc2577e56d0b39db172432c2a3fd80c68ef2f2350dc52b16f0728fb0f39bb20`  
		Last Modified: Thu, 06 Oct 2022 20:19:01 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be25bead88471409628775ccb5ca64093dda1f8edf17d0c0cba8b1386a9af6ed`  
		Last Modified: Thu, 06 Oct 2022 20:19:01 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df5ae5f1e7eef14ae320e77417a7e0e8093093fac3f0b2a80361561934e0283`  
		Last Modified: Thu, 06 Oct 2022 20:19:01 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:1ac7f047eff72813c74fdedc1bfd57d9b8e197b621448ee65af488d1c8840966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41807847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4b4acd89e751e3296fc901eb96e18e213776cd413e77cb153a33793d8e7b59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 21:49:50 GMT
ARG CONSUL_VERSION=1.11.11
# Thu, 20 Oct 2022 21:49:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 21:49:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 21:49:51 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 21:49:57 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 21:49:58 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 21:49:58 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 21:49:58 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 21:49:58 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 21:49:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 21:49:59 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 21:49:59 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 21:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 21:49:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61941cd529353efed8fc43bab0636e40a0e3e1887d2a2010dda8bf367b1c9e0`  
		Last Modified: Thu, 20 Oct 2022 21:51:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abd7b275bf5c7b848059d650084a29ccc9f0f604f424e548a34d637c166227d`  
		Last Modified: Thu, 20 Oct 2022 21:51:09 GMT  
		Size: 39.2 MB (39173335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa66a2e92a3c38cfedd1f05e166cd74621f92f8bdc8a76e9842695fe65bb48ea`  
		Last Modified: Thu, 20 Oct 2022 21:51:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80af8dd25ddf5a0bf80a5e5988226b01c2cb6ab041787cb3abd57d2590f39bc`  
		Last Modified: Thu, 20 Oct 2022 21:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e59126dfbd7d808497cfef82260a7aaaaa672cc6ba2ece063f11a4b810f21e4`  
		Last Modified: Thu, 20 Oct 2022 21:51:04 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:e07ccb658ff6c0d4009b5674625dede3e742dcb1bba386483384e5e6d8b0bc4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41641210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8b694f3ac46141c25397a4f5df64674df4d06b6c7597a87a0022f7b8701aeba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:55:40 GMT
ARG CONSUL_VERSION=1.11.10
# Thu, 06 Oct 2022 19:55:41 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 19:55:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 19:55:43 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 19:55:48 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 19:55:49 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 19:55:50 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:55:51 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 19:55:52 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 19:55:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 19:55:54 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 19:55:56 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 19:55:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:55:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4352ce334764a0f55f156b86ca907ebfd91d2ee6a073a6c2942eeb29be79ae`  
		Last Modified: Thu, 06 Oct 2022 19:56:54 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79b979b81cef9983e9ad956b513f1a73a54af98f6dda2dcaa1402746c46172b`  
		Last Modified: Thu, 06 Oct 2022 19:56:59 GMT  
		Size: 38.9 MB (38919445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda747340e7fb80e56b467bf0e2879adfc7bc6b6e3c00691a166f04d6bc7cf61`  
		Last Modified: Thu, 06 Oct 2022 19:56:54 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f0afae559e58411038e9ef46ad49588c276df1a618d9c20f384dd44e24ab80`  
		Last Modified: Thu, 06 Oct 2022 19:56:54 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b6029d87cc9d50f18807f2c90d1009ab337f330712b0da3552383115cf1bc1`  
		Last Modified: Thu, 06 Oct 2022 19:56:54 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; 386

```console
$ docker pull consul@sha256:941679736705b378be4ca9968ef48ebecdb5e3bb093696216b1b9f7184fada21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42872332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132ae038304342357d0f9af9f49e7c4024d79125b8dcf901f31e7266b2382b81`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:21:22 GMT
ARG CONSUL_VERSION=1.11.10
# Thu, 06 Oct 2022 19:21:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 19:21:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 19:21:25 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 19:21:31 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 19:21:32 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 19:21:33 GMT
# ARGS: CONSUL_VERSION=1.11.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:21:34 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 19:21:35 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 19:21:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 19:21:37 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 19:21:39 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 19:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:21:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02b1ff2f8c930392d4210892db04848184bf1eb30c7a56cedaac127346aefba`  
		Last Modified: Thu, 06 Oct 2022 19:22:42 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dab01d2b7ad13289cd5f7939d2e86dfb8eeccc0128bf2ad1a432fb160d9c24a`  
		Last Modified: Thu, 06 Oct 2022 19:22:46 GMT  
		Size: 40.0 MB (40040489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93a795d6320fd00d702d524245741f0ca29cd9bddc033cfaf8811f649cce234`  
		Last Modified: Thu, 06 Oct 2022 19:22:42 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f487d591d1fa304db444b08afb539dac82866f6fa7be0ceee8270b5a4db1b7c3`  
		Last Modified: Thu, 06 Oct 2022 19:22:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4685be7f89be1d9b040fb48c2d477d50364802e567b61c26edaad1f9faefc754`  
		Last Modified: Thu, 06 Oct 2022 19:22:42 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.11`

```console
$ docker pull consul@sha256:8ab77ef3e35d5c8e7686f25c8bad1d7de3d7049ff2adad15c13de864cf7a685a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `consul:1.11.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:1ac7f047eff72813c74fdedc1bfd57d9b8e197b621448ee65af488d1c8840966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41807847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4b4acd89e751e3296fc901eb96e18e213776cd413e77cb153a33793d8e7b59`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 21:49:50 GMT
ARG CONSUL_VERSION=1.11.11
# Thu, 20 Oct 2022 21:49:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 21:49:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 21:49:51 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 21:49:57 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 21:49:58 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 21:49:58 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 21:49:58 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 21:49:58 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 21:49:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 21:49:59 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 21:49:59 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 21:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 21:49:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61941cd529353efed8fc43bab0636e40a0e3e1887d2a2010dda8bf367b1c9e0`  
		Last Modified: Thu, 20 Oct 2022 21:51:04 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abd7b275bf5c7b848059d650084a29ccc9f0f604f424e548a34d637c166227d`  
		Last Modified: Thu, 20 Oct 2022 21:51:09 GMT  
		Size: 39.2 MB (39173335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa66a2e92a3c38cfedd1f05e166cd74621f92f8bdc8a76e9842695fe65bb48ea`  
		Last Modified: Thu, 20 Oct 2022 21:51:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80af8dd25ddf5a0bf80a5e5988226b01c2cb6ab041787cb3abd57d2590f39bc`  
		Last Modified: Thu, 20 Oct 2022 21:51:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e59126dfbd7d808497cfef82260a7aaaaa672cc6ba2ece063f11a4b810f21e4`  
		Last Modified: Thu, 20 Oct 2022 21:51:04 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12`

```console
$ docker pull consul@sha256:0ed1b83c9f4d62ed596c95caca9ddcee5bb2351bd4dca7cdc299b9cc29786194
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.12` - linux; amd64

```console
$ docker pull consul@sha256:0de0d6c5cb5b40559c365247412e4b3eccf922e7d66a204d9600ecd193e325e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49593561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dbc674c802b4a324ff25aee9c74f61348be830cf64b22155c46426e120e06a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:17:54 GMT
ARG CONSUL_VERSION=1.12.5
# Thu, 06 Oct 2022 20:17:55 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 20:17:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 20:17:55 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 20:18:01 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 20:18:02 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 20:18:02 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:18:02 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 20:18:02 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 20:18:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 20:18:03 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 20:18:03 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 20:18:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:18:03 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ace0f7b1032b7ef5a34aa605dcc516dc67280068380ff2cffd7842258f490f`  
		Last Modified: Thu, 06 Oct 2022 20:18:46 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639130d7d0a5f2810cbf76233d43a93aa08abb517b7d2a0a6ad9393c408d4c7a`  
		Last Modified: Thu, 06 Oct 2022 20:18:51 GMT  
		Size: 46.8 MB (46766665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788c37358f70e19be1f900fe4533768b4056b4b97dc155b1c396f11522e9973f`  
		Last Modified: Thu, 06 Oct 2022 20:18:46 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c82f45fb69a8d9dab88ada4ef0572025f0753e7df56e286883cca5a5f2f9e2`  
		Last Modified: Thu, 06 Oct 2022 20:18:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a03560d04cea4ff15f1df92f7eca2f1a8c2e798e8cc1081b1830175ece19104`  
		Last Modified: Thu, 06 Oct 2022 20:18:46 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm variant v6

```console
$ docker pull consul@sha256:7449336589b4fb2a325bde8a5399b32b21cbd077d738d33ed90ac4ef590f9a99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47458239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638ea957aa58c6f4ffe801251224e59dae44bfcc9f9c27279db1f3ed6433cd4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 21:49:37 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 20 Oct 2022 21:49:37 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 21:49:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 21:49:37 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 21:49:44 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 21:49:45 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 21:49:45 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 21:49:45 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 21:49:45 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 21:49:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 21:49:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 21:49:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 21:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 21:49:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fe45a82ef234761d985261b4981a469b75414c01e2a93bcce0c85aa66b5956`  
		Last Modified: Thu, 20 Oct 2022 21:50:46 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006d9db05f7c3500f3b8f7325ce7ba40f4f643af11d82d27b5a7e7a0afce0620`  
		Last Modified: Thu, 20 Oct 2022 21:50:52 GMT  
		Size: 44.8 MB (44823729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6081654ef87d7a5cf4a8ea9f7963bca794286df807ba1066fb4ff4cc3e3d90`  
		Last Modified: Thu, 20 Oct 2022 21:50:46 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8242cdbcedd475746f728fbab9bb1fc12d72b033682b833c78519b8894595b53`  
		Last Modified: Thu, 20 Oct 2022 21:50:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886c504ce9785e2485b91abe305974afbf1f706cf0af5101851b605fa57d7a60`  
		Last Modified: Thu, 20 Oct 2022 21:50:46 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:44cd4ccfc0cdd24f981fcbcb50b56a2594f80426fee459966d43f3211a388cf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47192789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c76372a989f8fef7d83cce81518202cc9ccb9f53d02a3ad3c09c159204098e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:55:18 GMT
ARG CONSUL_VERSION=1.12.5
# Thu, 06 Oct 2022 19:55:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 19:55:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 19:55:20 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 19:55:26 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 19:55:26 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 19:55:27 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:55:28 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 19:55:29 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 19:55:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 19:55:31 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 19:55:33 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 19:55:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:55:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa5ec50c46346c24f681201e1872cc44998408d58a8fa00db8591b518c2c011d`  
		Last Modified: Thu, 06 Oct 2022 19:56:38 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c34daa1ba4a1050fcf716626c732230b00af4ec7ed957a3c661e645c508379`  
		Last Modified: Thu, 06 Oct 2022 19:56:43 GMT  
		Size: 44.5 MB (44471026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e259e22868a0ff7c3fa7951a638285f2dfe4258b1eb3fe8838eb1a720dd5cc0b`  
		Last Modified: Thu, 06 Oct 2022 19:56:38 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17df47d8d2fc0d9553808f7714afbf53072d1e676219538b73d68d9946d83352`  
		Last Modified: Thu, 06 Oct 2022 19:56:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd0862756b5fe78156baf322448f68564499e53d2ee6684795feaedecf1aeb2`  
		Last Modified: Thu, 06 Oct 2022 19:56:38 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; 386

```console
$ docker pull consul@sha256:1fe29f91b3e22ff186bc4cceb0d868ce4b47869636b9ad5509216c1b85fa4785
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48658971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d000eb621ad78799ce4bb9774a42980b256b1845876f17b4ed1aa0faa4783dd1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:20:56 GMT
ARG CONSUL_VERSION=1.12.5
# Thu, 06 Oct 2022 19:20:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 19:20:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 19:20:59 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 19:21:06 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 19:21:07 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 19:21:08 GMT
# ARGS: CONSUL_VERSION=1.12.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:21:09 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 19:21:10 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 19:21:11 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 19:21:12 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 19:21:14 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 19:21:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:21:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248b2d6d2922d41b86855a343a91451a710448123634ade9bf09ab3b63562658`  
		Last Modified: Thu, 06 Oct 2022 19:22:24 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf134c98e31568cf62d4f14a3300da745ac2d2d24db0cd2cbfcb4cc6c4a9d2b`  
		Last Modified: Thu, 06 Oct 2022 19:22:29 GMT  
		Size: 45.8 MB (45827130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5466d2a84c45fbbd805f2629551fe0e62ed338187ea965d7a88876082fcd17`  
		Last Modified: Thu, 06 Oct 2022 19:22:25 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff2a5d7f7ce9747e564551c01644e0d330ac29e35a6831edddee2cc4d5ef420`  
		Last Modified: Thu, 06 Oct 2022 19:22:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3e6bd5f052ba3990b9f94eb86e19805ea0a2aab7fa5ab5bff4b78446799d59`  
		Last Modified: Thu, 06 Oct 2022 19:22:24 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12.6`

```console
$ docker pull consul@sha256:22f54914d2f388e599b93608f3534c3df37ab2e01d28d174827bc5c6902fae69
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `consul:1.12.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:7449336589b4fb2a325bde8a5399b32b21cbd077d738d33ed90ac4ef590f9a99
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.5 MB (47458239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:638ea957aa58c6f4ffe801251224e59dae44bfcc9f9c27279db1f3ed6433cd4f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 21:49:37 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 20 Oct 2022 21:49:37 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 21:49:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 21:49:37 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 21:49:44 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 21:49:45 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 21:49:45 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 21:49:45 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 21:49:45 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 21:49:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 21:49:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 21:49:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 21:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 21:49:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66fe45a82ef234761d985261b4981a469b75414c01e2a93bcce0c85aa66b5956`  
		Last Modified: Thu, 20 Oct 2022 21:50:46 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006d9db05f7c3500f3b8f7325ce7ba40f4f643af11d82d27b5a7e7a0afce0620`  
		Last Modified: Thu, 20 Oct 2022 21:50:52 GMT  
		Size: 44.8 MB (44823729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6081654ef87d7a5cf4a8ea9f7963bca794286df807ba1066fb4ff4cc3e3d90`  
		Last Modified: Thu, 20 Oct 2022 21:50:46 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8242cdbcedd475746f728fbab9bb1fc12d72b033682b833c78519b8894595b53`  
		Last Modified: Thu, 20 Oct 2022 21:50:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886c504ce9785e2485b91abe305974afbf1f706cf0af5101851b605fa57d7a60`  
		Last Modified: Thu, 20 Oct 2022 21:50:46 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.13`

```console
$ docker pull consul@sha256:b663240f433c056ec0b608f0611c4dd634ef943b9c6c95c5faeafbb85d7a7f3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13` - linux; amd64

```console
$ docker pull consul@sha256:22ab19cf1326abbfaafec6a14eb68f96e899e88ffe9ce26fa36affcf8ffb582c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51849363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787f84379eafbabf63b5b418b678a7908b37f951b1e04e9c3520c0c694c5b5cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:17:43 GMT
ARG CONSUL_VERSION=1.13.2
# Thu, 06 Oct 2022 20:17:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 20:17:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 20:17:44 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 20:17:49 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 20:17:50 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 20:17:51 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:17:51 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 20:17:51 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 20:17:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 20:17:51 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 20:17:51 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 20:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:17:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7703ab6ccaa4ba994a2db465e78c8d1a197ba9056588381d68d77b3914b3a09`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b470997b25a34c71f1f5b833f9f4352c88ee661795b819706e7fd555607568d0`  
		Last Modified: Thu, 06 Oct 2022 20:18:34 GMT  
		Size: 49.0 MB (49022471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e707243c37d0a3b90c03cc88111fffca187ded34cf343ab02b9bebc80ad34ac2`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c847e17d4f85b903ffff3b20571e5a26fef18646d229c7d52e4d0693ebca15`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94b2ee494f8001ee861b3e4c68b18be1d5a405d690adf9fcfeb2f6afb23cf9`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm variant v6

```console
$ docker pull consul@sha256:0c97b3aa222aca56cecbaa978ebfa9e0c05b44cbe16da8e8952140e6f82e7ab1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49459977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb45de66131b32714df6b11aa393597a000dd01684193476b8e1929e658e9a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 21:49:22 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 21:49:22 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 21:49:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 21:49:22 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 21:49:29 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 21:49:30 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 21:49:31 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 21:49:31 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 21:49:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 21:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 21:49:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443048d871c8058ca30aa43173b7e7f60c743418207efcb821589f96f6e15bb5`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf2e718f1353961618d3a54eef0029a66ed70877ea3c71e04399f7fd644f186`  
		Last Modified: Thu, 20 Oct 2022 21:50:31 GMT  
		Size: 46.8 MB (46825465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce47262e4e154a175c36db31d1032a04e1fbd602ab8925e4b71ee917747fe5`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f5d4969c34c70c6dcbfd0450bbfce0f5822deb44e72aae301b34f7a9f24f60`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6edc3c2492164b420fc5b116dbe565199d792dfdd0bd9fec0d027f8c540298`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a57ab8fdec89d3ddddf86d54c7a5f4333fbf1af45b976ed7bcfeb0c5fd689774
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49011371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221874175f695865d68383786e479f2bafc221a5eff46ca573fbf1a79633ae03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:54:55 GMT
ARG CONSUL_VERSION=1.13.2
# Thu, 06 Oct 2022 19:54:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 19:54:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 19:54:58 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 19:55:04 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 19:55:04 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 19:55:05 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:55:06 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 19:55:07 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 19:55:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 19:55:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 19:55:11 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 19:55:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:55:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6f27f6d0561ce2ff87a56b6f6f45a7eeab78da890685fa3da49b9735c85919`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6c35637f39fdcd8cf012bf51af6a98cc994d0f810c97ad861d3d1aeb19c3`  
		Last Modified: Thu, 06 Oct 2022 19:56:24 GMT  
		Size: 46.3 MB (46289610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caeda6f8e23b0768329412dc32e4ed22d825e0e019831bcec0ad9482781d859`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e377af9fdd97c446d4f87829785a24d0aea12da0efd5d2a2e79fc2d9577c97c`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b50148ce95ff394b0f186ddfc88759a280c44aada4170d0a6f93aa2f791bd1f`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; 386

```console
$ docker pull consul@sha256:e086f100acad2a5464d6787393c9d970acaabb7edeb7f51a4cef44582618745c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50733141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8180c331613d1f241929f14722a9ccd2e7381ab8463d05fe5456ca16a170b868`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:20:30 GMT
ARG CONSUL_VERSION=1.13.2
# Thu, 06 Oct 2022 19:20:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 19:20:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 19:20:33 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 19:20:39 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 19:20:40 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 19:20:41 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:20:42 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 19:20:43 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 19:20:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 19:20:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 19:20:47 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 19:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:20:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67739f835a25118040edfe4f1036773c67b02effd1fc9736ae6d099acd2c9a9`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b084d44964631840ce9d61d85e1bfec9b363703ed46455a85ed998e27e260df`  
		Last Modified: Thu, 06 Oct 2022 19:22:10 GMT  
		Size: 47.9 MB (47901306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251f74b33858a8729ffa21f71626e5d464cf8ed93b00ba6691a61d4e2e76b465`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1089b15843a17da8448c7f79aa2fe2a063889614cd6bbfbe38b6069d63da78`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66e77f6cf894d98b0480bbcf1d653d364b51a70102e42e53124a5e4cc3cd57c`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.13.3`

```console
$ docker pull consul@sha256:10e67125fa7eaa161493d4911f46b1e11a7124296a3588d7e599a9f323f43e2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `consul:1.13.3` - linux; arm variant v6

```console
$ docker pull consul@sha256:0c97b3aa222aca56cecbaa978ebfa9e0c05b44cbe16da8e8952140e6f82e7ab1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49459977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb45de66131b32714df6b11aa393597a000dd01684193476b8e1929e658e9a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 21:49:22 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 21:49:22 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 21:49:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 21:49:22 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 21:49:29 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 21:49:30 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 21:49:31 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 21:49:31 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 21:49:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 21:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 21:49:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443048d871c8058ca30aa43173b7e7f60c743418207efcb821589f96f6e15bb5`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf2e718f1353961618d3a54eef0029a66ed70877ea3c71e04399f7fd644f186`  
		Last Modified: Thu, 20 Oct 2022 21:50:31 GMT  
		Size: 46.8 MB (46825465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce47262e4e154a175c36db31d1032a04e1fbd602ab8925e4b71ee917747fe5`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f5d4969c34c70c6dcbfd0450bbfce0f5822deb44e72aae301b34f7a9f24f60`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6edc3c2492164b420fc5b116dbe565199d792dfdd0bd9fec0d027f8c540298`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:b663240f433c056ec0b608f0611c4dd634ef943b9c6c95c5faeafbb85d7a7f3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:22ab19cf1326abbfaafec6a14eb68f96e899e88ffe9ce26fa36affcf8ffb582c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51849363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787f84379eafbabf63b5b418b678a7908b37f951b1e04e9c3520c0c694c5b5cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:17:43 GMT
ARG CONSUL_VERSION=1.13.2
# Thu, 06 Oct 2022 20:17:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 20:17:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 20:17:44 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 20:17:49 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 20:17:50 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 20:17:51 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:17:51 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 20:17:51 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 20:17:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 20:17:51 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 20:17:51 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 20:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:17:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7703ab6ccaa4ba994a2db465e78c8d1a197ba9056588381d68d77b3914b3a09`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b470997b25a34c71f1f5b833f9f4352c88ee661795b819706e7fd555607568d0`  
		Last Modified: Thu, 06 Oct 2022 20:18:34 GMT  
		Size: 49.0 MB (49022471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e707243c37d0a3b90c03cc88111fffca187ded34cf343ab02b9bebc80ad34ac2`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c847e17d4f85b903ffff3b20571e5a26fef18646d229c7d52e4d0693ebca15`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94b2ee494f8001ee861b3e4c68b18be1d5a405d690adf9fcfeb2f6afb23cf9`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:0c97b3aa222aca56cecbaa978ebfa9e0c05b44cbe16da8e8952140e6f82e7ab1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49459977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb45de66131b32714df6b11aa393597a000dd01684193476b8e1929e658e9a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 21:49:22 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 21:49:22 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 21:49:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 21:49:22 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 21:49:29 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 21:49:30 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 21:49:31 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 21:49:31 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 21:49:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 21:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 21:49:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443048d871c8058ca30aa43173b7e7f60c743418207efcb821589f96f6e15bb5`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf2e718f1353961618d3a54eef0029a66ed70877ea3c71e04399f7fd644f186`  
		Last Modified: Thu, 20 Oct 2022 21:50:31 GMT  
		Size: 46.8 MB (46825465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce47262e4e154a175c36db31d1032a04e1fbd602ab8925e4b71ee917747fe5`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f5d4969c34c70c6dcbfd0450bbfce0f5822deb44e72aae301b34f7a9f24f60`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6edc3c2492164b420fc5b116dbe565199d792dfdd0bd9fec0d027f8c540298`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a57ab8fdec89d3ddddf86d54c7a5f4333fbf1af45b976ed7bcfeb0c5fd689774
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49011371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221874175f695865d68383786e479f2bafc221a5eff46ca573fbf1a79633ae03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:54:55 GMT
ARG CONSUL_VERSION=1.13.2
# Thu, 06 Oct 2022 19:54:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 19:54:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 19:54:58 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 19:55:04 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 19:55:04 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 19:55:05 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:55:06 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 19:55:07 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 19:55:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 19:55:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 19:55:11 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 19:55:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:55:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6f27f6d0561ce2ff87a56b6f6f45a7eeab78da890685fa3da49b9735c85919`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6c35637f39fdcd8cf012bf51af6a98cc994d0f810c97ad861d3d1aeb19c3`  
		Last Modified: Thu, 06 Oct 2022 19:56:24 GMT  
		Size: 46.3 MB (46289610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caeda6f8e23b0768329412dc32e4ed22d825e0e019831bcec0ad9482781d859`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e377af9fdd97c446d4f87829785a24d0aea12da0efd5d2a2e79fc2d9577c97c`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b50148ce95ff394b0f186ddfc88759a280c44aada4170d0a6f93aa2f791bd1f`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:e086f100acad2a5464d6787393c9d970acaabb7edeb7f51a4cef44582618745c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50733141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8180c331613d1f241929f14722a9ccd2e7381ab8463d05fe5456ca16a170b868`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:20:30 GMT
ARG CONSUL_VERSION=1.13.2
# Thu, 06 Oct 2022 19:20:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 19:20:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 19:20:33 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 19:20:39 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 19:20:40 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 19:20:41 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:20:42 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 19:20:43 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 19:20:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 19:20:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 19:20:47 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 19:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:20:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67739f835a25118040edfe4f1036773c67b02effd1fc9736ae6d099acd2c9a9`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b084d44964631840ce9d61d85e1bfec9b363703ed46455a85ed998e27e260df`  
		Last Modified: Thu, 06 Oct 2022 19:22:10 GMT  
		Size: 47.9 MB (47901306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251f74b33858a8729ffa21f71626e5d464cf8ed93b00ba6691a61d4e2e76b465`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1089b15843a17da8448c7f79aa2fe2a063889614cd6bbfbe38b6069d63da78`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66e77f6cf894d98b0480bbcf1d653d364b51a70102e42e53124a5e4cc3cd57c`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
