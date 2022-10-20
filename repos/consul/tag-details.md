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
$ docker pull consul@sha256:7390300486dc9fb5a298108882bad9ef0ff1e7f1bf4fab9752a0902875613686
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11` - linux; amd64

```console
$ docker pull consul@sha256:a039e9d527918b34b16b5f42206ea65cf4d5c77ebe4f0dc1ed72ddd211f74012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44051372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3218aef7ef51511af5fe84b2a5fbaa2cc7d431a9bee5e14b21df5e84ae5dab0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:19:53 GMT
ARG CONSUL_VERSION=1.11.11
# Thu, 20 Oct 2022 22:19:53 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:19:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:19:54 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:19:59 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:20:00 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:20:00 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:20:01 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:20:01 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:20:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:20:01 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:20:01 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:20:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:20:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db266e13be216fe89d6209928211b185d5d263ee6bd30e6b80e7beeec9bc3619`  
		Last Modified: Thu, 20 Oct 2022 22:20:50 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae1ee8f89bac0c62546e3d91be2ee906a26a16c4e7b3dda1052388088d6b9cc`  
		Last Modified: Thu, 20 Oct 2022 22:20:55 GMT  
		Size: 41.2 MB (41224476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79b20631baef10a707c18e0433b2e98ee9fc2102b67ddf6d8d75c69526591a4`  
		Last Modified: Thu, 20 Oct 2022 22:20:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61631dca3937d5c009dc3a88c81b972168ba17f702347f65bc944c8e29a91f4f`  
		Last Modified: Thu, 20 Oct 2022 22:20:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5690c4072fc638efdd1d1a097184a39db03f8ee274bbc7b86bf8311c6f428aa1`  
		Last Modified: Thu, 20 Oct 2022 22:20:50 GMT  
		Size: 1.8 KB (1788 bytes)  
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
$ docker pull consul@sha256:b5ed1e080ddfa1fe4d0d8c21ca22d4d5e3f3e1fa47910c20c9a576ed7d4af4dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41633161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c65c1167ab2a5f110e6d093ec6b3a3a585dfc03db6bf275a412340999adffe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:40:17 GMT
ARG CONSUL_VERSION=1.11.11
# Thu, 20 Oct 2022 22:40:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:40:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:40:20 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:40:26 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:40:27 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:40:28 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:40:29 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:40:30 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:40:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:40:32 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:40:34 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:40:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:40:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23360ce4bbebb82d7e280656c08f762cfa620185ab963bd64187634d1839e2a`  
		Last Modified: Thu, 20 Oct 2022 22:41:32 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd3eacba1c21ef971918d49b74f0f375d027e493346297f088e252a39643cda`  
		Last Modified: Thu, 20 Oct 2022 22:41:38 GMT  
		Size: 38.9 MB (38911398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e182bb23c8e67b67777cf6bf729d3c5baf55d0c48eaff6f6185bb24213bf97`  
		Last Modified: Thu, 20 Oct 2022 22:41:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e46fe23e03d3704ddc6e03de62658808bebc0f9277366e12d3de2cc9d1bd8a1`  
		Last Modified: Thu, 20 Oct 2022 22:41:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acb81b212e3b07e6d4d1e6a8fc4290197d6de2166ba73267512f693e6e9e3fe`  
		Last Modified: Thu, 20 Oct 2022 22:41:32 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; 386

```console
$ docker pull consul@sha256:570ae0f4fcb9127d7f5485910fc28e7926f977c2a2067073839f6f9711c66c4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42863487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff797f0ee90bafcd3ee859aa89bc4d74725487853f2007e67e65b191a955f99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:39:15 GMT
ARG CONSUL_VERSION=1.11.11
# Thu, 20 Oct 2022 22:39:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:39:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:39:18 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:39:24 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:39:25 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:39:26 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:39:27 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:39:28 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:39:29 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:39:30 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:39:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:39:33 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b745e5dbe38e59d84556a37733b8c0174bfe4eec0fa10d76956e5a056741576`  
		Last Modified: Thu, 20 Oct 2022 22:40:31 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845dba77933323c823a1858b1efaf6a2afc7df8f5c1a957c13d109683ec29348`  
		Last Modified: Thu, 20 Oct 2022 22:40:35 GMT  
		Size: 40.0 MB (40031645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999c9c5600f5fe692d83fa1deddd1c5ec858a9930e33616ff5f662b522da3674`  
		Last Modified: Thu, 20 Oct 2022 22:40:31 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa019ef6f05b1ed16b47537dd960e381ce5e61b4ae37f6410a65a6452f80d40e`  
		Last Modified: Thu, 20 Oct 2022 22:40:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b772927ce7b603d14b628f6c5ba6b1e9551ac4e3aac6b6c6820795a7436313e`  
		Last Modified: Thu, 20 Oct 2022 22:40:31 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.11`

```console
$ docker pull consul@sha256:7390300486dc9fb5a298108882bad9ef0ff1e7f1bf4fab9752a0902875613686
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.11` - linux; amd64

```console
$ docker pull consul@sha256:a039e9d527918b34b16b5f42206ea65cf4d5c77ebe4f0dc1ed72ddd211f74012
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44051372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3218aef7ef51511af5fe84b2a5fbaa2cc7d431a9bee5e14b21df5e84ae5dab0e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:19:53 GMT
ARG CONSUL_VERSION=1.11.11
# Thu, 20 Oct 2022 22:19:53 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:19:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:19:54 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:19:59 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:20:00 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:20:00 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:20:01 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:20:01 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:20:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:20:01 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:20:01 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:20:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:20:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db266e13be216fe89d6209928211b185d5d263ee6bd30e6b80e7beeec9bc3619`  
		Last Modified: Thu, 20 Oct 2022 22:20:50 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae1ee8f89bac0c62546e3d91be2ee906a26a16c4e7b3dda1052388088d6b9cc`  
		Last Modified: Thu, 20 Oct 2022 22:20:55 GMT  
		Size: 41.2 MB (41224476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79b20631baef10a707c18e0433b2e98ee9fc2102b67ddf6d8d75c69526591a4`  
		Last Modified: Thu, 20 Oct 2022 22:20:50 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61631dca3937d5c009dc3a88c81b972168ba17f702347f65bc944c8e29a91f4f`  
		Last Modified: Thu, 20 Oct 2022 22:20:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5690c4072fc638efdd1d1a097184a39db03f8ee274bbc7b86bf8311c6f428aa1`  
		Last Modified: Thu, 20 Oct 2022 22:20:50 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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

### `consul:1.11.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b5ed1e080ddfa1fe4d0d8c21ca22d4d5e3f3e1fa47910c20c9a576ed7d4af4dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41633161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c65c1167ab2a5f110e6d093ec6b3a3a585dfc03db6bf275a412340999adffe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:40:17 GMT
ARG CONSUL_VERSION=1.11.11
# Thu, 20 Oct 2022 22:40:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:40:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:40:20 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:40:26 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:40:27 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:40:28 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:40:29 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:40:30 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:40:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:40:32 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:40:34 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:40:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:40:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23360ce4bbebb82d7e280656c08f762cfa620185ab963bd64187634d1839e2a`  
		Last Modified: Thu, 20 Oct 2022 22:41:32 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd3eacba1c21ef971918d49b74f0f375d027e493346297f088e252a39643cda`  
		Last Modified: Thu, 20 Oct 2022 22:41:38 GMT  
		Size: 38.9 MB (38911398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e182bb23c8e67b67777cf6bf729d3c5baf55d0c48eaff6f6185bb24213bf97`  
		Last Modified: Thu, 20 Oct 2022 22:41:32 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e46fe23e03d3704ddc6e03de62658808bebc0f9277366e12d3de2cc9d1bd8a1`  
		Last Modified: Thu, 20 Oct 2022 22:41:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acb81b212e3b07e6d4d1e6a8fc4290197d6de2166ba73267512f693e6e9e3fe`  
		Last Modified: Thu, 20 Oct 2022 22:41:32 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.11` - linux; 386

```console
$ docker pull consul@sha256:570ae0f4fcb9127d7f5485910fc28e7926f977c2a2067073839f6f9711c66c4f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42863487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff797f0ee90bafcd3ee859aa89bc4d74725487853f2007e67e65b191a955f99`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:39:15 GMT
ARG CONSUL_VERSION=1.11.11
# Thu, 20 Oct 2022 22:39:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:39:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:39:18 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:39:24 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:39:25 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:39:26 GMT
# ARGS: CONSUL_VERSION=1.11.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:39:27 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:39:28 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:39:29 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:39:30 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:39:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:39:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:39:33 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b745e5dbe38e59d84556a37733b8c0174bfe4eec0fa10d76956e5a056741576`  
		Last Modified: Thu, 20 Oct 2022 22:40:31 GMT  
		Size: 1.2 KB (1242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845dba77933323c823a1858b1efaf6a2afc7df8f5c1a957c13d109683ec29348`  
		Last Modified: Thu, 20 Oct 2022 22:40:35 GMT  
		Size: 40.0 MB (40031645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999c9c5600f5fe692d83fa1deddd1c5ec858a9930e33616ff5f662b522da3674`  
		Last Modified: Thu, 20 Oct 2022 22:40:31 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa019ef6f05b1ed16b47537dd960e381ce5e61b4ae37f6410a65a6452f80d40e`  
		Last Modified: Thu, 20 Oct 2022 22:40:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b772927ce7b603d14b628f6c5ba6b1e9551ac4e3aac6b6c6820795a7436313e`  
		Last Modified: Thu, 20 Oct 2022 22:40:31 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12`

```console
$ docker pull consul@sha256:1ccc5587660d9963667ab05efbae02afa47a30f2f4621a1ac9e06f8417cd7bf1
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
$ docker pull consul@sha256:d14a07e3661a14c3f70a6a46277d5ddff6d15761200aa38735e110d92795b8f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47190988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a768df251b4b9c3f90be84577378266300c537452670db3735188ea3a0eb819`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:39:55 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 20 Oct 2022 22:39:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:39:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:39:58 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:40:03 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:40:04 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:40:05 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:40:06 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:40:07 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:40:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:40:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:40:11 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:40:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:40:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f712b9e4d340d3650f19a8cdd995f42209c9415f887b9f0a85cbecf96881236d`  
		Last Modified: Thu, 20 Oct 2022 22:41:16 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cfe44f32356432d80e3bb21313a38fb334f7fa874ea51d134df2ca45265811`  
		Last Modified: Thu, 20 Oct 2022 22:41:21 GMT  
		Size: 44.5 MB (44469224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7792720c0078947b10a70a43abb77ca4ba13ad391c4cc96b3882673aa983604`  
		Last Modified: Thu, 20 Oct 2022 22:41:16 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dff423fb62f0569b779c4ed56864c1f1953018c5af25f3ce088f7d5b170d68`  
		Last Modified: Thu, 20 Oct 2022 22:41:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc72087770eab8fe739e5082e086beea2a884ec45ee39dfbc107e6adcc4f479`  
		Last Modified: Thu, 20 Oct 2022 22:41:16 GMT  
		Size: 1.8 KB (1788 bytes)  
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
$ docker pull consul@sha256:1ccc5587660d9963667ab05efbae02afa47a30f2f4621a1ac9e06f8417cd7bf1
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

### `consul:1.12.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:d14a07e3661a14c3f70a6a46277d5ddff6d15761200aa38735e110d92795b8f0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47190988 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a768df251b4b9c3f90be84577378266300c537452670db3735188ea3a0eb819`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:39:55 GMT
ARG CONSUL_VERSION=1.12.6
# Thu, 20 Oct 2022 22:39:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:39:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:39:58 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:40:03 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:40:04 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:40:05 GMT
# ARGS: CONSUL_VERSION=1.12.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:40:06 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:40:07 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:40:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:40:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:40:11 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:40:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:40:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f712b9e4d340d3650f19a8cdd995f42209c9415f887b9f0a85cbecf96881236d`  
		Last Modified: Thu, 20 Oct 2022 22:41:16 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cfe44f32356432d80e3bb21313a38fb334f7fa874ea51d134df2ca45265811`  
		Last Modified: Thu, 20 Oct 2022 22:41:21 GMT  
		Size: 44.5 MB (44469224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7792720c0078947b10a70a43abb77ca4ba13ad391c4cc96b3882673aa983604`  
		Last Modified: Thu, 20 Oct 2022 22:41:16 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dff423fb62f0569b779c4ed56864c1f1953018c5af25f3ce088f7d5b170d68`  
		Last Modified: Thu, 20 Oct 2022 22:41:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc72087770eab8fe739e5082e086beea2a884ec45ee39dfbc107e6adcc4f479`  
		Last Modified: Thu, 20 Oct 2022 22:41:16 GMT  
		Size: 1.8 KB (1788 bytes)  
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
$ docker pull consul@sha256:f3588463271728c5e937fdc3c1536415296e666b806fce8d464d8b1030f78512
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
$ docker pull consul@sha256:d743da0391b26fb081b44661da71be8a1840a218095a4a67b0bee4649e341066
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49036591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fe0dfc2bdaea4b9c228c26a0875187f7190e8284c9bab860671a531d96da53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:39:31 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 22:39:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:39:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:39:34 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:39:41 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:39:42 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:39:42 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:39:43 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:39:44 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:39:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:39:46 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:39:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:39:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d245b5a63ecc275536a44ec811a738483bcdba171fc8d48c3bcd89dc20f4a`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30230ac319392cdf74f0c5d0ceadd0ab27ecff2cb7c53e4210a60000d4339d6`  
		Last Modified: Thu, 20 Oct 2022 22:41:02 GMT  
		Size: 46.3 MB (46314829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e0b904bae00f21198c14a5771814e5f2ad5576b4525ac1aa29b7395e421924`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa0c7ae3fb094482b97ffcd24d8e5ecaff36f0c5a2ed61359f17cd9ae6aa73e`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d911fecae9335de9011b3c9293b242a91bee0fad52788802122ed4016fe77288`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 1.8 KB (1787 bytes)  
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
$ docker pull consul@sha256:f3588463271728c5e937fdc3c1536415296e666b806fce8d464d8b1030f78512
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

### `consul:1.13.3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:d743da0391b26fb081b44661da71be8a1840a218095a4a67b0bee4649e341066
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49036591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fe0dfc2bdaea4b9c228c26a0875187f7190e8284c9bab860671a531d96da53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:39:31 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 22:39:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:39:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:39:34 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:39:41 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:39:42 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:39:42 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:39:43 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:39:44 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:39:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:39:46 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:39:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:39:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d245b5a63ecc275536a44ec811a738483bcdba171fc8d48c3bcd89dc20f4a`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30230ac319392cdf74f0c5d0ceadd0ab27ecff2cb7c53e4210a60000d4339d6`  
		Last Modified: Thu, 20 Oct 2022 22:41:02 GMT  
		Size: 46.3 MB (46314829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e0b904bae00f21198c14a5771814e5f2ad5576b4525ac1aa29b7395e421924`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa0c7ae3fb094482b97ffcd24d8e5ecaff36f0c5a2ed61359f17cd9ae6aa73e`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d911fecae9335de9011b3c9293b242a91bee0fad52788802122ed4016fe77288`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 1.8 KB (1787 bytes)  
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

## `consul:latest`

```console
$ docker pull consul@sha256:f3588463271728c5e937fdc3c1536415296e666b806fce8d464d8b1030f78512
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
$ docker pull consul@sha256:d743da0391b26fb081b44661da71be8a1840a218095a4a67b0bee4649e341066
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49036591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fe0dfc2bdaea4b9c228c26a0875187f7190e8284c9bab860671a531d96da53`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 22:39:31 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 22:39:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 22:39:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 22:39:34 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 22:39:41 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 22:39:42 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 22:39:42 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 22:39:43 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 22:39:44 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 22:39:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 22:39:46 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 22:39:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 22:39:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 22:39:49 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99d245b5a63ecc275536a44ec811a738483bcdba171fc8d48c3bcd89dc20f4a`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30230ac319392cdf74f0c5d0ceadd0ab27ecff2cb7c53e4210a60000d4339d6`  
		Last Modified: Thu, 20 Oct 2022 22:41:02 GMT  
		Size: 46.3 MB (46314829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00e0b904bae00f21198c14a5771814e5f2ad5576b4525ac1aa29b7395e421924`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa0c7ae3fb094482b97ffcd24d8e5ecaff36f0c5a2ed61359f17cd9ae6aa73e`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d911fecae9335de9011b3c9293b242a91bee0fad52788802122ed4016fe77288`  
		Last Modified: Thu, 20 Oct 2022 22:40:56 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

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
