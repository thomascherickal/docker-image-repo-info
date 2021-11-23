<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10`](#consul110)
-	[`consul:1.10.4`](#consul1104)
-	[`consul:1.11.0-beta`](#consul1110-beta)
-	[`consul:1.11.0-beta3`](#consul1110-beta3)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.17`](#consul1817)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.11`](#consul1911)
-	[`consul:latest`](#consullatest)

## `consul:1.10`

```console
$ docker pull consul@sha256:701275d51948239f213ec3122d1d8006ac12159a211fdc1c060634677d8af91a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10` - linux; amd64

```console
$ docker pull consul@sha256:bd47456d9d5113ed9f1598711c4f09bbfddf6ba90834e656522a3d40c18f46b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43680607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60b5d5d7aa05804e07d8d6c740bc7418dd1f5ba1b85c6921362fcd4a43b97065`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:23:55 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:23:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:23:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:23:57 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:24:10 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:24:11 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:24:12 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:24:12 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:24:12 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:24:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:24:13 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:24:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:24:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:24:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8346c4c2c7acddb91fe63704bf85338e56c691fe7e48caa8a9fba6e7e16df095`  
		Last Modified: Mon, 15 Nov 2021 20:25:09 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f79386c0f7a4808f3eec56a09d42ac405acc2fd96f076dc0f6678d8bbc0486`  
		Last Modified: Mon, 15 Nov 2021 20:25:15 GMT  
		Size: 40.9 MB (40854814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716e8306345a5b03bffda8e3e9bcc2248e73e36693d31986f314fb6b34c7ac9d`  
		Last Modified: Mon, 15 Nov 2021 20:25:09 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abab715aa08f3bce73846825adb35731c130d5c8ea987b6900210146b200012`  
		Last Modified: Mon, 15 Nov 2021 20:25:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ffcce388ca4a335635a00115c98cb98ad497ed565f9be669d7f3d96bc66ad9`  
		Last Modified: Mon, 15 Nov 2021 20:25:10 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:5e52ada1ee506abf00ecdf71eaf7cca79277ac9ff42a267c246f29e56a4e397f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41745889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:833c0bf37139c939bff692c0ed026e2dac3f17f4df27f97dc676e034eb984f62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:49:43 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:49:44 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:49:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:49:46 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:50:03 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:50:05 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:50:07 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:50:07 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:50:08 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:50:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:50:09 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:50:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:50:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:50:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599027c88ab7fba9b363add5e85b1cfed7c2ed7a268d39b9d903447a56cd4964`  
		Last Modified: Mon, 15 Nov 2021 20:52:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dd5b4f9634aad38db027711e09712af5bd06e9acc0711ca4d186afc10e167c`  
		Last Modified: Mon, 15 Nov 2021 20:52:37 GMT  
		Size: 39.1 MB (39109173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0c6b2fd0e6fe5c66f30f9d0d156e0f39a28d2baf79cceb14ea4570998a49e9`  
		Last Modified: Mon, 15 Nov 2021 20:52:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49dc9ca4c1e90f9d8544916ce818b3ece76da1b75cb91a65055b4376d2e02bd`  
		Last Modified: Mon, 15 Nov 2021 20:52:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6583eb09f599ee7493254844b0c446e2c15e7f678da336e7f3312fa0d87a222`  
		Last Modified: Mon, 15 Nov 2021 20:52:16 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:53f6d5f8cb6cbd660622386aac46e18db66f839e4fabbc8b3af4556ce7013bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41693581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:919a111a440fad2646f22011543d55f9828d23143cbaa17883e2813994e810e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:39:33 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:39:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:39:36 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:39:49 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:39:50 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:39:50 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:39:51 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:39:52 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:39:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:39:54 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:39:56 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:39:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:39:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ec0dc3b53307c831eeab0ff2ca66c2ba920d35cdb7aef6797947eae6627b30`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3111f504ed97ecd3b4a24a4fca9128145ed4f676141777803ea21951c925a66c`  
		Last Modified: Mon, 15 Nov 2021 20:41:24 GMT  
		Size: 39.0 MB (38970628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9327a3a3328dacb9c1e1e9a671e69525c5b1a602ee29d0e396cac83f9f2a46ea`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d1ecde7662d3fd2578666467cbb5881fdf7501616f10a6e923036482dcbcbe`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33656f5ca4619fb5de521818b485d007b57dbdbb06f289aad9e48942d11c822`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; 386

```console
$ docker pull consul@sha256:197e09ba241dbb63bc41b59c9f57ec9d898bb3e7bfa7969f6cdf4f95719b0f68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43065393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72354e9f46b4a02d3e3ff31febbc09b1eb7a4c3da2d6b1578c3e064ae204df31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:38:27 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:38:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:38:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:38:29 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:38:41 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:38:42 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:38:43 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:38:43 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:38:44 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:38:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:38:44 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:38:44 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:38:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:38:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4536d099d46227da1d6bd8d679ef4f73244926c2e9a57f086fd4674c2e29b3b`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee00223e3240f6226f08e73dac4bf1da82986fc97b3d0ccf04074d6ca360163`  
		Last Modified: Mon, 15 Nov 2021 20:40:04 GMT  
		Size: 40.2 MB (40233212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910a1c818e60d30b4058f37ae0fab42090c4fad3f1ec35c0b8e55ddb611d954`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5367fa6ffd2e7e1ddf111b01561fc9ae792cd49696e586280fdbd77949ed93d6`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a5348717f1dadeca6442f041c3c7b3b3d661ab36be2689d8e83c3de608ea92`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.4`

```console
$ docker pull consul@sha256:701275d51948239f213ec3122d1d8006ac12159a211fdc1c060634677d8af91a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.4` - linux; amd64

```console
$ docker pull consul@sha256:bd47456d9d5113ed9f1598711c4f09bbfddf6ba90834e656522a3d40c18f46b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43680607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60b5d5d7aa05804e07d8d6c740bc7418dd1f5ba1b85c6921362fcd4a43b97065`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:23:55 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:23:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:23:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:23:57 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:24:10 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:24:11 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:24:12 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:24:12 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:24:12 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:24:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:24:13 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:24:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:24:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:24:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8346c4c2c7acddb91fe63704bf85338e56c691fe7e48caa8a9fba6e7e16df095`  
		Last Modified: Mon, 15 Nov 2021 20:25:09 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f79386c0f7a4808f3eec56a09d42ac405acc2fd96f076dc0f6678d8bbc0486`  
		Last Modified: Mon, 15 Nov 2021 20:25:15 GMT  
		Size: 40.9 MB (40854814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716e8306345a5b03bffda8e3e9bcc2248e73e36693d31986f314fb6b34c7ac9d`  
		Last Modified: Mon, 15 Nov 2021 20:25:09 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abab715aa08f3bce73846825adb35731c130d5c8ea987b6900210146b200012`  
		Last Modified: Mon, 15 Nov 2021 20:25:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ffcce388ca4a335635a00115c98cb98ad497ed565f9be669d7f3d96bc66ad9`  
		Last Modified: Mon, 15 Nov 2021 20:25:10 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:5e52ada1ee506abf00ecdf71eaf7cca79277ac9ff42a267c246f29e56a4e397f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41745889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:833c0bf37139c939bff692c0ed026e2dac3f17f4df27f97dc676e034eb984f62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:49:43 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:49:44 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:49:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:49:46 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:50:03 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:50:05 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:50:07 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:50:07 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:50:08 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:50:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:50:09 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:50:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:50:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:50:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599027c88ab7fba9b363add5e85b1cfed7c2ed7a268d39b9d903447a56cd4964`  
		Last Modified: Mon, 15 Nov 2021 20:52:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dd5b4f9634aad38db027711e09712af5bd06e9acc0711ca4d186afc10e167c`  
		Last Modified: Mon, 15 Nov 2021 20:52:37 GMT  
		Size: 39.1 MB (39109173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0c6b2fd0e6fe5c66f30f9d0d156e0f39a28d2baf79cceb14ea4570998a49e9`  
		Last Modified: Mon, 15 Nov 2021 20:52:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49dc9ca4c1e90f9d8544916ce818b3ece76da1b75cb91a65055b4376d2e02bd`  
		Last Modified: Mon, 15 Nov 2021 20:52:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6583eb09f599ee7493254844b0c446e2c15e7f678da336e7f3312fa0d87a222`  
		Last Modified: Mon, 15 Nov 2021 20:52:16 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:53f6d5f8cb6cbd660622386aac46e18db66f839e4fabbc8b3af4556ce7013bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41693581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:919a111a440fad2646f22011543d55f9828d23143cbaa17883e2813994e810e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:39:33 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:39:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:39:36 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:39:49 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:39:50 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:39:50 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:39:51 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:39:52 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:39:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:39:54 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:39:56 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:39:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:39:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ec0dc3b53307c831eeab0ff2ca66c2ba920d35cdb7aef6797947eae6627b30`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3111f504ed97ecd3b4a24a4fca9128145ed4f676141777803ea21951c925a66c`  
		Last Modified: Mon, 15 Nov 2021 20:41:24 GMT  
		Size: 39.0 MB (38970628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9327a3a3328dacb9c1e1e9a671e69525c5b1a602ee29d0e396cac83f9f2a46ea`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d1ecde7662d3fd2578666467cbb5881fdf7501616f10a6e923036482dcbcbe`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33656f5ca4619fb5de521818b485d007b57dbdbb06f289aad9e48942d11c822`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.4` - linux; 386

```console
$ docker pull consul@sha256:197e09ba241dbb63bc41b59c9f57ec9d898bb3e7bfa7969f6cdf4f95719b0f68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43065393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72354e9f46b4a02d3e3ff31febbc09b1eb7a4c3da2d6b1578c3e064ae204df31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:38:27 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:38:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:38:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:38:29 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:38:41 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:38:42 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:38:43 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:38:43 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:38:44 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:38:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:38:44 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:38:44 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:38:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:38:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4536d099d46227da1d6bd8d679ef4f73244926c2e9a57f086fd4674c2e29b3b`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee00223e3240f6226f08e73dac4bf1da82986fc97b3d0ccf04074d6ca360163`  
		Last Modified: Mon, 15 Nov 2021 20:40:04 GMT  
		Size: 40.2 MB (40233212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910a1c818e60d30b4058f37ae0fab42090c4fad3f1ec35c0b8e55ddb611d954`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5367fa6ffd2e7e1ddf111b01561fc9ae792cd49696e586280fdbd77949ed93d6`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a5348717f1dadeca6442f041c3c7b3b3d661ab36be2689d8e83c3de608ea92`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.0-beta`

```console
$ docker pull consul@sha256:b65caa85b885338a6a5ff8f11b5588ccc32f6534329b4ba39191f5d4292d2331
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.0-beta` - linux; amd64

```console
$ docker pull consul@sha256:52a71ee874601c8950aa28629a35e099bb0dc24847bc0b5d14d13f14cd584360
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.8 MB (43783223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0829aee119e4fdb501973904e56a18ca62c1069d2710b110bb38eabe5249c4a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Tue, 23 Nov 2021 19:19:18 GMT
ARG CONSUL_VERSION=1.11.0-beta3
# Tue, 23 Nov 2021 19:19:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 23 Nov 2021 19:19:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 23 Nov 2021 19:19:19 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 23 Nov 2021 19:19:33 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 23 Nov 2021 19:19:34 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 23 Nov 2021 19:19:35 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 23 Nov 2021 19:19:35 GMT
VOLUME [/consul/data]
# Tue, 23 Nov 2021 19:19:35 GMT
EXPOSE 8300
# Tue, 23 Nov 2021 19:19:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 23 Nov 2021 19:19:36 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 23 Nov 2021 19:19:36 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 23 Nov 2021 19:19:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Nov 2021 19:19:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73381c19459765aa22ca5dd0ee5491588020084ecccbddd026ad50ddf056fea5`  
		Last Modified: Tue, 23 Nov 2021 19:20:00 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d17f77e4418b6299e2e1b6b625de81198d2554ea630e8b017af09596ca7465`  
		Last Modified: Tue, 23 Nov 2021 19:20:05 GMT  
		Size: 41.0 MB (40957427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3916d11a8424c9d4f67814e94fd4865297a0fcaf338a8af0d22f9adb8b8f8fce`  
		Last Modified: Tue, 23 Nov 2021 19:20:00 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddcf5f99182864f19cdca74347c7c5521f56fc3405125776c327b5688ed5d4ed`  
		Last Modified: Tue, 23 Nov 2021 19:20:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905c58ec0ca6ec64894e4aa2aa439d0172207e08be634fee1d4af21b098906ad`  
		Last Modified: Tue, 23 Nov 2021 19:20:00 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; arm variant v6

```console
$ docker pull consul@sha256:0024e041bcf0aefa04ebe1677b6ad4787787565359e7fb971f7e5fd1c8861191
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41551086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c584a46c47f66ea85020652500bde0e9fad1e9bf0c87a469932d1ec5c98e7f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Tue, 23 Nov 2021 18:49:59 GMT
ARG CONSUL_VERSION=1.11.0-beta3
# Tue, 23 Nov 2021 18:50:00 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 23 Nov 2021 18:50:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 23 Nov 2021 18:50:02 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 23 Nov 2021 18:50:18 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 23 Nov 2021 18:50:20 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 23 Nov 2021 18:50:21 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 23 Nov 2021 18:50:22 GMT
VOLUME [/consul/data]
# Tue, 23 Nov 2021 18:50:22 GMT
EXPOSE 8300
# Tue, 23 Nov 2021 18:50:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 23 Nov 2021 18:50:23 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 23 Nov 2021 18:50:23 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 23 Nov 2021 18:50:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Nov 2021 18:50:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ef87264a077c1ecf85fc3a91c5871c49bd30a2ede423401d27fbd8fc6e0d9d`  
		Last Modified: Tue, 23 Nov 2021 18:51:55 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f03b632272b8c52cebe8fcf9bd308c9c33092e59969822199abc39056dff5`  
		Last Modified: Tue, 23 Nov 2021 18:52:17 GMT  
		Size: 38.9 MB (38914368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859261bff8af64bf1dd074c0db6f66600549a8f0c62916a992a5c22b22f89131`  
		Last Modified: Tue, 23 Nov 2021 18:51:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa94cd9ccec3a706f8de8b229a651068dd7a46d684045588d6d8a26fcbc81f40`  
		Last Modified: Tue, 23 Nov 2021 18:51:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047fddf3c992c47996add1b8f01edf00e9d65ba72628a1011ff74e7651e7ac7`  
		Last Modified: Tue, 23 Nov 2021 18:51:56 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2526d50f45d5b1b0eef62c4d3f8bc832b1f21ff1963626a6af80d3579f7234dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41372190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc21ac26013d490dcb7afd843193b8b68f5b46f4f0bd557f54660fa5da81cb61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Tue, 23 Nov 2021 19:39:23 GMT
ARG CONSUL_VERSION=1.11.0-beta3
# Tue, 23 Nov 2021 19:39:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 23 Nov 2021 19:39:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 23 Nov 2021 19:39:25 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 23 Nov 2021 19:39:38 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 23 Nov 2021 19:39:38 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 23 Nov 2021 19:39:39 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 23 Nov 2021 19:39:40 GMT
VOLUME [/consul/data]
# Tue, 23 Nov 2021 19:39:41 GMT
EXPOSE 8300
# Tue, 23 Nov 2021 19:39:42 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 23 Nov 2021 19:39:43 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 23 Nov 2021 19:39:45 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 23 Nov 2021 19:39:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Nov 2021 19:39:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d1ae6c8bcb01b3d601117d2d945d49de0f1b217d29602cd187ae26cee50719`  
		Last Modified: Tue, 23 Nov 2021 19:40:26 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ad6d2e338b5ce664e8890aa919ccd3f6567de48903fe4c71e5d20060a5e0e6`  
		Last Modified: Tue, 23 Nov 2021 19:40:31 GMT  
		Size: 38.6 MB (38649236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c572704fba3032e705c8b61b416877cd7dda2a72997d246c665c97f7bdc4cd24`  
		Last Modified: Tue, 23 Nov 2021 19:40:26 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593c975c48d9650222de382f136a74107f7c6c5c97e2d320c1511433b2a1837e`  
		Last Modified: Tue, 23 Nov 2021 19:40:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3aab2b512665d530fd135f83f267afcf1b1961d0ba64b9c0b3149aa6f70aec`  
		Last Modified: Tue, 23 Nov 2021 19:40:26 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; 386

```console
$ docker pull consul@sha256:9b717ed38d9d78a3411a23a76f73ec75d08717456042b4e43d8fe8f33e9c6492
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42604671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf90f45c09a1ce18c47c11acbfa96deeacad20c61db2da0880c3d5ac11169e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Tue, 23 Nov 2021 19:38:22 GMT
ARG CONSUL_VERSION=1.11.0-beta3
# Tue, 23 Nov 2021 19:38:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 23 Nov 2021 19:38:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 23 Nov 2021 19:38:24 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 23 Nov 2021 19:38:40 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 23 Nov 2021 19:38:41 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 23 Nov 2021 19:38:42 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 23 Nov 2021 19:38:43 GMT
VOLUME [/consul/data]
# Tue, 23 Nov 2021 19:38:43 GMT
EXPOSE 8300
# Tue, 23 Nov 2021 19:38:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 23 Nov 2021 19:38:43 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 23 Nov 2021 19:38:44 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 23 Nov 2021 19:38:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Nov 2021 19:38:44 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fe9dda4d6ab5d7c90434d71d7a564ab47164e3884d0d0183d97298220b3f4a`  
		Last Modified: Tue, 23 Nov 2021 19:39:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444468b267e25ec9f9f22813ed20f5ebb77f06a599f02e8bf03b7a382640aae5`  
		Last Modified: Tue, 23 Nov 2021 19:39:31 GMT  
		Size: 39.8 MB (39772491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136215fa8a89d261b79549ad123d9d89174e378887da6f9ef6698876de4753d3`  
		Last Modified: Tue, 23 Nov 2021 19:39:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e978ec332e47545959cfd85eccf817a1753bfe558642403b7e918a94372c1e3f`  
		Last Modified: Tue, 23 Nov 2021 19:39:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66521b03ff59815b8d220297fd5e7871811706aec776a78d3e1b137b5d4fa2b4`  
		Last Modified: Tue, 23 Nov 2021 19:39:25 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.0-beta3`

```console
$ docker pull consul@sha256:b65caa85b885338a6a5ff8f11b5588ccc32f6534329b4ba39191f5d4292d2331
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.0-beta3` - linux; amd64

```console
$ docker pull consul@sha256:52a71ee874601c8950aa28629a35e099bb0dc24847bc0b5d14d13f14cd584360
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.8 MB (43783223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0829aee119e4fdb501973904e56a18ca62c1069d2710b110bb38eabe5249c4a4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Tue, 23 Nov 2021 19:19:18 GMT
ARG CONSUL_VERSION=1.11.0-beta3
# Tue, 23 Nov 2021 19:19:18 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 23 Nov 2021 19:19:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 23 Nov 2021 19:19:19 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 23 Nov 2021 19:19:33 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 23 Nov 2021 19:19:34 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 23 Nov 2021 19:19:35 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 23 Nov 2021 19:19:35 GMT
VOLUME [/consul/data]
# Tue, 23 Nov 2021 19:19:35 GMT
EXPOSE 8300
# Tue, 23 Nov 2021 19:19:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 23 Nov 2021 19:19:36 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 23 Nov 2021 19:19:36 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 23 Nov 2021 19:19:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Nov 2021 19:19:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73381c19459765aa22ca5dd0ee5491588020084ecccbddd026ad50ddf056fea5`  
		Last Modified: Tue, 23 Nov 2021 19:20:00 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d17f77e4418b6299e2e1b6b625de81198d2554ea630e8b017af09596ca7465`  
		Last Modified: Tue, 23 Nov 2021 19:20:05 GMT  
		Size: 41.0 MB (40957427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3916d11a8424c9d4f67814e94fd4865297a0fcaf338a8af0d22f9adb8b8f8fce`  
		Last Modified: Tue, 23 Nov 2021 19:20:00 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddcf5f99182864f19cdca74347c7c5521f56fc3405125776c327b5688ed5d4ed`  
		Last Modified: Tue, 23 Nov 2021 19:20:00 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905c58ec0ca6ec64894e4aa2aa439d0172207e08be634fee1d4af21b098906ad`  
		Last Modified: Tue, 23 Nov 2021 19:20:00 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta3` - linux; arm variant v6

```console
$ docker pull consul@sha256:0024e041bcf0aefa04ebe1677b6ad4787787565359e7fb971f7e5fd1c8861191
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41551086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c584a46c47f66ea85020652500bde0e9fad1e9bf0c87a469932d1ec5c98e7f2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Tue, 23 Nov 2021 18:49:59 GMT
ARG CONSUL_VERSION=1.11.0-beta3
# Tue, 23 Nov 2021 18:50:00 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 23 Nov 2021 18:50:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 23 Nov 2021 18:50:02 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 23 Nov 2021 18:50:18 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 23 Nov 2021 18:50:20 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 23 Nov 2021 18:50:21 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 23 Nov 2021 18:50:22 GMT
VOLUME [/consul/data]
# Tue, 23 Nov 2021 18:50:22 GMT
EXPOSE 8300
# Tue, 23 Nov 2021 18:50:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 23 Nov 2021 18:50:23 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 23 Nov 2021 18:50:23 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 23 Nov 2021 18:50:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Nov 2021 18:50:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24ef87264a077c1ecf85fc3a91c5871c49bd30a2ede423401d27fbd8fc6e0d9d`  
		Last Modified: Tue, 23 Nov 2021 18:51:55 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993f03b632272b8c52cebe8fcf9bd308c9c33092e59969822199abc39056dff5`  
		Last Modified: Tue, 23 Nov 2021 18:52:17 GMT  
		Size: 38.9 MB (38914368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:859261bff8af64bf1dd074c0db6f66600549a8f0c62916a992a5c22b22f89131`  
		Last Modified: Tue, 23 Nov 2021 18:51:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa94cd9ccec3a706f8de8b229a651068dd7a46d684045588d6d8a26fcbc81f40`  
		Last Modified: Tue, 23 Nov 2021 18:51:55 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047fddf3c992c47996add1b8f01edf00e9d65ba72628a1011ff74e7651e7ac7`  
		Last Modified: Tue, 23 Nov 2021 18:51:56 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:2526d50f45d5b1b0eef62c4d3f8bc832b1f21ff1963626a6af80d3579f7234dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41372190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc21ac26013d490dcb7afd843193b8b68f5b46f4f0bd557f54660fa5da81cb61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Tue, 23 Nov 2021 19:39:23 GMT
ARG CONSUL_VERSION=1.11.0-beta3
# Tue, 23 Nov 2021 19:39:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 23 Nov 2021 19:39:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 23 Nov 2021 19:39:25 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 23 Nov 2021 19:39:38 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 23 Nov 2021 19:39:38 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 23 Nov 2021 19:39:39 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 23 Nov 2021 19:39:40 GMT
VOLUME [/consul/data]
# Tue, 23 Nov 2021 19:39:41 GMT
EXPOSE 8300
# Tue, 23 Nov 2021 19:39:42 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 23 Nov 2021 19:39:43 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 23 Nov 2021 19:39:45 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 23 Nov 2021 19:39:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Nov 2021 19:39:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d1ae6c8bcb01b3d601117d2d945d49de0f1b217d29602cd187ae26cee50719`  
		Last Modified: Tue, 23 Nov 2021 19:40:26 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ad6d2e338b5ce664e8890aa919ccd3f6567de48903fe4c71e5d20060a5e0e6`  
		Last Modified: Tue, 23 Nov 2021 19:40:31 GMT  
		Size: 38.6 MB (38649236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c572704fba3032e705c8b61b416877cd7dda2a72997d246c665c97f7bdc4cd24`  
		Last Modified: Tue, 23 Nov 2021 19:40:26 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593c975c48d9650222de382f136a74107f7c6c5c97e2d320c1511433b2a1837e`  
		Last Modified: Tue, 23 Nov 2021 19:40:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3aab2b512665d530fd135f83f267afcf1b1961d0ba64b9c0b3149aa6f70aec`  
		Last Modified: Tue, 23 Nov 2021 19:40:26 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta3` - linux; 386

```console
$ docker pull consul@sha256:9b717ed38d9d78a3411a23a76f73ec75d08717456042b4e43d8fe8f33e9c6492
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42604671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acf90f45c09a1ce18c47c11acbfa96deeacad20c61db2da0880c3d5ac11169e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Tue, 23 Nov 2021 19:38:22 GMT
ARG CONSUL_VERSION=1.11.0-beta3
# Tue, 23 Nov 2021 19:38:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 23 Nov 2021 19:38:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 23 Nov 2021 19:38:24 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 23 Nov 2021 19:38:40 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 23 Nov 2021 19:38:41 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 23 Nov 2021 19:38:42 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 23 Nov 2021 19:38:43 GMT
VOLUME [/consul/data]
# Tue, 23 Nov 2021 19:38:43 GMT
EXPOSE 8300
# Tue, 23 Nov 2021 19:38:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 23 Nov 2021 19:38:43 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 23 Nov 2021 19:38:44 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 23 Nov 2021 19:38:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 23 Nov 2021 19:38:44 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61fe9dda4d6ab5d7c90434d71d7a564ab47164e3884d0d0183d97298220b3f4a`  
		Last Modified: Tue, 23 Nov 2021 19:39:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444468b267e25ec9f9f22813ed20f5ebb77f06a599f02e8bf03b7a382640aae5`  
		Last Modified: Tue, 23 Nov 2021 19:39:31 GMT  
		Size: 39.8 MB (39772491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136215fa8a89d261b79549ad123d9d89174e378887da6f9ef6698876de4753d3`  
		Last Modified: Tue, 23 Nov 2021 19:39:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e978ec332e47545959cfd85eccf817a1753bfe558642403b7e918a94372c1e3f`  
		Last Modified: Tue, 23 Nov 2021 19:39:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66521b03ff59815b8d220297fd5e7871811706aec776a78d3e1b137b5d4fa2b4`  
		Last Modified: Tue, 23 Nov 2021 19:39:25 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:d9ac98cfc598100a954e31201354bf8c9b30b95cf52fcfc9c8be0d070be49f9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:9983a7a89652a2218943efb9daa74365974d317c2b06b0e50b4e2c8f78c0f68e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47875152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dd1fdf91d11d64482954f1504f2689264a5a73c953fabd9f130a9497aa28b8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:24:32 GMT
ARG CONSUL_VERSION=1.8.17
# Mon, 15 Nov 2021 20:24:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.17 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:24:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:24:33 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:24:47 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:24:48 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:24:49 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:24:49 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:24:49 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:24:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:24:50 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:24:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:24:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:24:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d344b293099861acc14536e269f0ba63c3e56b0bdff98ba4aea25a4b86521af`  
		Last Modified: Mon, 15 Nov 2021 20:25:45 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3734432cf175532a51994e77fd0792a2ca5388763166230fd72c679d196dc96a`  
		Last Modified: Mon, 15 Nov 2021 20:25:50 GMT  
		Size: 45.0 MB (45049362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecb0127f7060faca4236b8c9fbe48365493c428e2cdd94113c3a217b4a04e5`  
		Last Modified: Mon, 15 Nov 2021 20:25:45 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3ddf90960014b8c2bcf333ad4f7426a16639787ec972b315015d5e18044806`  
		Last Modified: Mon, 15 Nov 2021 20:25:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e82abc6e83e9ec6214295544373cb61fa4a17112b7c0fcef33ef0d87f461321`  
		Last Modified: Mon, 15 Nov 2021 20:25:44 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:abf0e099a025cdd81a9f7430d9e6d516e51291558909a553a95b284490db46c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45180457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6086c2bf646398f71fa4d2e1b84b2370d388e555f1afda97b8351e6faa2b464e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:51:00 GMT
ARG CONSUL_VERSION=1.8.17
# Mon, 15 Nov 2021 20:51:00 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.17 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:51:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:51:02 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:51:15 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:51:17 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:51:18 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:51:19 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:51:19 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:51:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:51:20 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:51:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:51:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:51:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c48c9ed7e7b64c0d7cc9ecb99049aab3f58a925d2e06b96173ae3115a602cf0`  
		Last Modified: Mon, 15 Nov 2021 20:53:28 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb1317cc3caf2eaf04d08c46b7cff4eb65a81bdb31ba0f440b3dc45d203e0c9`  
		Last Modified: Mon, 15 Nov 2021 20:53:51 GMT  
		Size: 42.5 MB (42543744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bc64da0fe4c8086ba1027607883d6e4ac0f8a82976033948a40785e99fa41d`  
		Last Modified: Mon, 15 Nov 2021 20:53:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddd0497a930f3aec1da37737117ad1e11bfb4d22e45560c8bb3529f4f8c1705`  
		Last Modified: Mon, 15 Nov 2021 20:53:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3932812eafe2c9e912bd9d2ed539801940dc589ad75bd5b908ee6c118ee101`  
		Last Modified: Mon, 15 Nov 2021 20:53:28 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a14e64e1c91facb9e7390ae92e2c3b9739da418fa215d4ce88bca435f9b51668
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45375384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe12e8938069aceac6622bf87d500c4610a1a219fc26215c627d017725eb0bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:40:31 GMT
ARG CONSUL_VERSION=1.8.17
# Mon, 15 Nov 2021 20:40:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.17 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:40:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:40:34 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:40:41 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:40:42 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:40:43 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:40:44 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:40:45 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:40:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:40:47 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:40:49 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:40:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:40:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee4612ef07a9bd61350a0704fe2c1cd72a3a9de2949dbe843ab408e58f5d179`  
		Last Modified: Mon, 15 Nov 2021 20:41:54 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8ecd3d73dcd8d00708ee34fcf5261cedb58c89e9e89def527e73fa6978cff9`  
		Last Modified: Mon, 15 Nov 2021 20:42:00 GMT  
		Size: 42.7 MB (42652429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d04b65e7070ea58533a4942bbac9368584a83b44df7f443632ca9f30b1f20`  
		Last Modified: Mon, 15 Nov 2021 20:41:54 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c406bf24ff2a56cbb3de6e7849729ea8243e490b196398ccb3c0aaa3cc85dec`  
		Last Modified: Mon, 15 Nov 2021 20:41:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63983b2883844436ebb6bebf583ea2a0d3c16dfab7b89fa14a162b5f60b5aa`  
		Last Modified: Mon, 15 Nov 2021 20:41:54 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:88ddf2c4c62eba938d32a33c377c0564282bb99ca54c3bfcd8957c0679813b4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47437798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80bf00a059a1bd43e2de7d233d271d3fa73a45163e7a4230e2df30b5431e243a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:39:13 GMT
ARG CONSUL_VERSION=1.8.17
# Mon, 15 Nov 2021 20:39:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.17 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:39:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:39:15 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:39:23 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:39:24 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:39:25 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:39:25 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:39:25 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:39:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:39:26 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:39:26 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:39:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86251b5f6a583cfdcbad811e64cea36761c786c5e1256237a1ec1a069ebdf8d6`  
		Last Modified: Mon, 15 Nov 2021 20:40:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368c7d7d91e44f89227e2538056eee5b44974ba65d345e7870a69c9cd6c43f3`  
		Last Modified: Mon, 15 Nov 2021 20:40:45 GMT  
		Size: 44.6 MB (44605616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b70b8483ebe69c47acecc74b959242ce657f3a58f0b2d12e979c12794f19f3b`  
		Last Modified: Mon, 15 Nov 2021 20:40:38 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1bf56447f25206a064e6a42a685b02b3c0ee05b3abd60ef09559a86a2976a7`  
		Last Modified: Mon, 15 Nov 2021 20:40:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2d8f7155897598020e4f7761cb8581e326bcd2ac5f7c137d9777ad97b6ff64`  
		Last Modified: Mon, 15 Nov 2021 20:40:37 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.17`

```console
$ docker pull consul@sha256:d9ac98cfc598100a954e31201354bf8c9b30b95cf52fcfc9c8be0d070be49f9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.17` - linux; amd64

```console
$ docker pull consul@sha256:9983a7a89652a2218943efb9daa74365974d317c2b06b0e50b4e2c8f78c0f68e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47875152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1dd1fdf91d11d64482954f1504f2689264a5a73c953fabd9f130a9497aa28b8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:24:32 GMT
ARG CONSUL_VERSION=1.8.17
# Mon, 15 Nov 2021 20:24:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.17 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:24:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:24:33 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:24:47 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:24:48 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:24:49 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:24:49 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:24:49 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:24:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:24:50 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:24:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:24:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:24:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d344b293099861acc14536e269f0ba63c3e56b0bdff98ba4aea25a4b86521af`  
		Last Modified: Mon, 15 Nov 2021 20:25:45 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3734432cf175532a51994e77fd0792a2ca5388763166230fd72c679d196dc96a`  
		Last Modified: Mon, 15 Nov 2021 20:25:50 GMT  
		Size: 45.0 MB (45049362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecb0127f7060faca4236b8c9fbe48365493c428e2cdd94113c3a217b4a04e5`  
		Last Modified: Mon, 15 Nov 2021 20:25:45 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3ddf90960014b8c2bcf333ad4f7426a16639787ec972b315015d5e18044806`  
		Last Modified: Mon, 15 Nov 2021 20:25:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e82abc6e83e9ec6214295544373cb61fa4a17112b7c0fcef33ef0d87f461321`  
		Last Modified: Mon, 15 Nov 2021 20:25:44 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.17` - linux; arm variant v6

```console
$ docker pull consul@sha256:abf0e099a025cdd81a9f7430d9e6d516e51291558909a553a95b284490db46c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45180457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6086c2bf646398f71fa4d2e1b84b2370d388e555f1afda97b8351e6faa2b464e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:51:00 GMT
ARG CONSUL_VERSION=1.8.17
# Mon, 15 Nov 2021 20:51:00 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.17 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:51:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:51:02 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:51:15 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:51:17 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:51:18 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:51:19 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:51:19 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:51:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:51:20 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:51:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:51:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:51:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c48c9ed7e7b64c0d7cc9ecb99049aab3f58a925d2e06b96173ae3115a602cf0`  
		Last Modified: Mon, 15 Nov 2021 20:53:28 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb1317cc3caf2eaf04d08c46b7cff4eb65a81bdb31ba0f440b3dc45d203e0c9`  
		Last Modified: Mon, 15 Nov 2021 20:53:51 GMT  
		Size: 42.5 MB (42543744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bc64da0fe4c8086ba1027607883d6e4ac0f8a82976033948a40785e99fa41d`  
		Last Modified: Mon, 15 Nov 2021 20:53:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddd0497a930f3aec1da37737117ad1e11bfb4d22e45560c8bb3529f4f8c1705`  
		Last Modified: Mon, 15 Nov 2021 20:53:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3932812eafe2c9e912bd9d2ed539801940dc589ad75bd5b908ee6c118ee101`  
		Last Modified: Mon, 15 Nov 2021 20:53:28 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.17` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a14e64e1c91facb9e7390ae92e2c3b9739da418fa215d4ce88bca435f9b51668
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45375384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fe12e8938069aceac6622bf87d500c4610a1a219fc26215c627d017725eb0bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:40:31 GMT
ARG CONSUL_VERSION=1.8.17
# Mon, 15 Nov 2021 20:40:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.17 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:40:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:40:34 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:40:41 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:40:42 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:40:43 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:40:44 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:40:45 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:40:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:40:47 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:40:49 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:40:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:40:50 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee4612ef07a9bd61350a0704fe2c1cd72a3a9de2949dbe843ab408e58f5d179`  
		Last Modified: Mon, 15 Nov 2021 20:41:54 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8ecd3d73dcd8d00708ee34fcf5261cedb58c89e9e89def527e73fa6978cff9`  
		Last Modified: Mon, 15 Nov 2021 20:42:00 GMT  
		Size: 42.7 MB (42652429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8d04b65e7070ea58533a4942bbac9368584a83b44df7f443632ca9f30b1f20`  
		Last Modified: Mon, 15 Nov 2021 20:41:54 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c406bf24ff2a56cbb3de6e7849729ea8243e490b196398ccb3c0aaa3cc85dec`  
		Last Modified: Mon, 15 Nov 2021 20:41:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d63983b2883844436ebb6bebf583ea2a0d3c16dfab7b89fa14a162b5f60b5aa`  
		Last Modified: Mon, 15 Nov 2021 20:41:54 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.17` - linux; 386

```console
$ docker pull consul@sha256:88ddf2c4c62eba938d32a33c377c0564282bb99ca54c3bfcd8957c0679813b4b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47437798 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80bf00a059a1bd43e2de7d233d271d3fa73a45163e7a4230e2df30b5431e243a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:39:13 GMT
ARG CONSUL_VERSION=1.8.17
# Mon, 15 Nov 2021 20:39:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.8.17 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:39:14 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:39:15 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:39:23 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:39:24 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:39:25 GMT
# ARGS: CONSUL_VERSION=1.8.17
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:39:25 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:39:25 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:39:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:39:26 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:39:26 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:39:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86251b5f6a583cfdcbad811e64cea36761c786c5e1256237a1ec1a069ebdf8d6`  
		Last Modified: Mon, 15 Nov 2021 20:40:37 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0368c7d7d91e44f89227e2538056eee5b44974ba65d345e7870a69c9cd6c43f3`  
		Last Modified: Mon, 15 Nov 2021 20:40:45 GMT  
		Size: 44.6 MB (44605616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b70b8483ebe69c47acecc74b959242ce657f3a58f0b2d12e979c12794f19f3b`  
		Last Modified: Mon, 15 Nov 2021 20:40:38 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1bf56447f25206a064e6a42a685b02b3c0ee05b3abd60ef09559a86a2976a7`  
		Last Modified: Mon, 15 Nov 2021 20:40:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2d8f7155897598020e4f7761cb8581e326bcd2ac5f7c137d9777ad97b6ff64`  
		Last Modified: Mon, 15 Nov 2021 20:40:37 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:4718f4114396b87963654407d1ef6540134796c6e540e263f7e37d827488b263
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:9fb22811c2a466b42376b0e9a0e6ad229b16d059f458b61f112ff9dfb97a2e2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46347589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a8d3400e10d3a4d3f8fde74914a8c286fcbb769079131a689e5bd505d13fb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:24:18 GMT
ARG CONSUL_VERSION=1.9.11
# Mon, 15 Nov 2021 20:24:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:24:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:24:20 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:24:26 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:24:27 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:24:28 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:24:28 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:24:28 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:24:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:24:29 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:24:29 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:24:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:24:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379896a44a3ffc19ec943a74d85cc689742af673ecfa12fc81ebdc84ece43dac`  
		Last Modified: Mon, 15 Nov 2021 20:25:28 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2921a3837a162ad587502d4992fa3f46adde08a13d8db28a461f5ce1c17f57f`  
		Last Modified: Mon, 15 Nov 2021 20:25:34 GMT  
		Size: 43.5 MB (43521792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8079d6a33a1ef4a4c7c19cb6a47954e20f3978023b21b56d00059e111f94d54f`  
		Last Modified: Mon, 15 Nov 2021 20:25:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd09fcf3d2ccf62e402d956312db114542b1c08eff458a987e53345abb3a9fa`  
		Last Modified: Mon, 15 Nov 2021 20:25:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abac1e88238dcaad1726a976ff82b4bfacb902132d0455078e2c766d3c806eb`  
		Last Modified: Mon, 15 Nov 2021 20:25:28 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:a627280d3ca6924027973289a9ebe21418852f6f9479ee02014762f182815606
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43630224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9815924f87a42e0d46325bcebfe54227a20dbd5401336399ab20a12d73b916c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:50:22 GMT
ARG CONSUL_VERSION=1.9.11
# Mon, 15 Nov 2021 20:50:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:50:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:50:25 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:50:40 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:50:42 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:50:44 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:50:44 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:50:44 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:50:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:50:45 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:50:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:50:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09550d8b2803c2e6ebb9257a16d5bc8ed4ed0904adf18afa77f45393269444aa`  
		Last Modified: Mon, 15 Nov 2021 20:52:53 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6180dd5f0d53a9b3fcbc701561853f5f2bd77039d91be2cf84f68a2fa5512246`  
		Last Modified: Mon, 15 Nov 2021 20:53:15 GMT  
		Size: 41.0 MB (40993511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80be56cdd8805d3720193171e2dcd3c44f1b3901250f82228127e37da3936e42`  
		Last Modified: Mon, 15 Nov 2021 20:52:53 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac510b2182b3b504b9a0c44aa53ad1a816fe427f2b75aa7b2a7f954aa75fd04`  
		Last Modified: Mon, 15 Nov 2021 20:52:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af66850e55aed81a67afb64a80b6a9fcc0bb8055d3fea63842b00eea7289693`  
		Last Modified: Mon, 15 Nov 2021 20:52:53 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b07cfbd4b65940483ad57c474670ed2d08b4488f8fd796c84c78d6f995b4352e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43917707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51eef30e01419ed905798a42a7d4b77917cc6add9b45c02a42ff645b5bc1d5bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:40:04 GMT
ARG CONSUL_VERSION=1.9.11
# Mon, 15 Nov 2021 20:40:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:40:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:40:07 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:40:17 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:40:18 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:40:18 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:40:19 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:40:20 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:40:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:40:22 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:40:24 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:40:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:40:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106b4db9e8ad433f93eb1a44f1fe8556833cdafaa5a3469791adf7470c2c8023`  
		Last Modified: Mon, 15 Nov 2021 20:41:38 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496a6c93c75197418d28e5ed311d2eb8b79f281bee8082af531701ac6f3d4cd8`  
		Last Modified: Mon, 15 Nov 2021 20:41:43 GMT  
		Size: 41.2 MB (41194756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef20f840498681c30c35fbf596622eee8bd993d479e93b4b4154624f2566ffa`  
		Last Modified: Mon, 15 Nov 2021 20:41:38 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e1534f5820f2088eb34f30f117ee934da17c694307f31e46fba9a47ff3641b`  
		Last Modified: Mon, 15 Nov 2021 20:41:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e3cfdd0f155fb1beefef1401a437a3406548848222359f2d3031b03c21d621`  
		Last Modified: Mon, 15 Nov 2021 20:41:38 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:d27510860c82182881a649f0f0d6b02d0779a9a06cccf9f918cdad0f3b5b5301
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45728906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68a2390539f7635654f5c9430ee2007e95132c48a81d69416de4f8bc3f6ff81f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:38:52 GMT
ARG CONSUL_VERSION=1.9.11
# Mon, 15 Nov 2021 20:38:53 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:38:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:38:54 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:39:04 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:39:06 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:39:07 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:39:07 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:39:07 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:39:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:39:08 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:39:08 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:39:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:39:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f4bab377d3f918a0d8c2ddb05f9de86badd9f39a7d3d6a3ecbbe5ebfc5512d`  
		Last Modified: Mon, 15 Nov 2021 20:40:19 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e691eb3c1cc789ce2d2e5ce77693fd80627adee9529cb900296b0818fb3ca0`  
		Last Modified: Mon, 15 Nov 2021 20:40:26 GMT  
		Size: 42.9 MB (42896727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd1f22f20de7c48eda673c9429704c94f8394918b88878a8e2d778e67976ea2`  
		Last Modified: Mon, 15 Nov 2021 20:40:19 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f4bd3655e4095f284118dde5ef3eae8c0b1c8dcc7ae955e7381a826f056497`  
		Last Modified: Mon, 15 Nov 2021 20:40:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f7f12b4f466339cfb54f7526fd43237224e9fc71359c0c4296366a7041651`  
		Last Modified: Mon, 15 Nov 2021 20:40:19 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.11`

```console
$ docker pull consul@sha256:4718f4114396b87963654407d1ef6540134796c6e540e263f7e37d827488b263
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.11` - linux; amd64

```console
$ docker pull consul@sha256:9fb22811c2a466b42376b0e9a0e6ad229b16d059f458b61f112ff9dfb97a2e2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46347589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a8d3400e10d3a4d3f8fde74914a8c286fcbb769079131a689e5bd505d13fb7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:24:18 GMT
ARG CONSUL_VERSION=1.9.11
# Mon, 15 Nov 2021 20:24:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:24:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:24:20 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:24:26 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:24:27 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:24:28 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:24:28 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:24:28 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:24:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:24:29 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:24:29 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:24:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:24:29 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379896a44a3ffc19ec943a74d85cc689742af673ecfa12fc81ebdc84ece43dac`  
		Last Modified: Mon, 15 Nov 2021 20:25:28 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2921a3837a162ad587502d4992fa3f46adde08a13d8db28a461f5ce1c17f57f`  
		Last Modified: Mon, 15 Nov 2021 20:25:34 GMT  
		Size: 43.5 MB (43521792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8079d6a33a1ef4a4c7c19cb6a47954e20f3978023b21b56d00059e111f94d54f`  
		Last Modified: Mon, 15 Nov 2021 20:25:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd09fcf3d2ccf62e402d956312db114542b1c08eff458a987e53345abb3a9fa`  
		Last Modified: Mon, 15 Nov 2021 20:25:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abac1e88238dcaad1726a976ff82b4bfacb902132d0455078e2c766d3c806eb`  
		Last Modified: Mon, 15 Nov 2021 20:25:28 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:a627280d3ca6924027973289a9ebe21418852f6f9479ee02014762f182815606
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.6 MB (43630224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9815924f87a42e0d46325bcebfe54227a20dbd5401336399ab20a12d73b916c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:50:22 GMT
ARG CONSUL_VERSION=1.9.11
# Mon, 15 Nov 2021 20:50:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:50:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:50:25 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:50:40 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:50:42 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:50:44 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:50:44 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:50:44 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:50:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:50:45 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:50:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:50:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:50:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09550d8b2803c2e6ebb9257a16d5bc8ed4ed0904adf18afa77f45393269444aa`  
		Last Modified: Mon, 15 Nov 2021 20:52:53 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6180dd5f0d53a9b3fcbc701561853f5f2bd77039d91be2cf84f68a2fa5512246`  
		Last Modified: Mon, 15 Nov 2021 20:53:15 GMT  
		Size: 41.0 MB (40993511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80be56cdd8805d3720193171e2dcd3c44f1b3901250f82228127e37da3936e42`  
		Last Modified: Mon, 15 Nov 2021 20:52:53 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac510b2182b3b504b9a0c44aa53ad1a816fe427f2b75aa7b2a7f954aa75fd04`  
		Last Modified: Mon, 15 Nov 2021 20:52:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af66850e55aed81a67afb64a80b6a9fcc0bb8055d3fea63842b00eea7289693`  
		Last Modified: Mon, 15 Nov 2021 20:52:53 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b07cfbd4b65940483ad57c474670ed2d08b4488f8fd796c84c78d6f995b4352e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43917707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51eef30e01419ed905798a42a7d4b77917cc6add9b45c02a42ff645b5bc1d5bf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:40:04 GMT
ARG CONSUL_VERSION=1.9.11
# Mon, 15 Nov 2021 20:40:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:40:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:40:07 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:40:17 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:40:18 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:40:18 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:40:19 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:40:20 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:40:21 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:40:22 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:40:24 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:40:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:40:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106b4db9e8ad433f93eb1a44f1fe8556833cdafaa5a3469791adf7470c2c8023`  
		Last Modified: Mon, 15 Nov 2021 20:41:38 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496a6c93c75197418d28e5ed311d2eb8b79f281bee8082af531701ac6f3d4cd8`  
		Last Modified: Mon, 15 Nov 2021 20:41:43 GMT  
		Size: 41.2 MB (41194756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef20f840498681c30c35fbf596622eee8bd993d479e93b4b4154624f2566ffa`  
		Last Modified: Mon, 15 Nov 2021 20:41:38 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e1534f5820f2088eb34f30f117ee934da17c694307f31e46fba9a47ff3641b`  
		Last Modified: Mon, 15 Nov 2021 20:41:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e3cfdd0f155fb1beefef1401a437a3406548848222359f2d3031b03c21d621`  
		Last Modified: Mon, 15 Nov 2021 20:41:38 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.11` - linux; 386

```console
$ docker pull consul@sha256:d27510860c82182881a649f0f0d6b02d0779a9a06cccf9f918cdad0f3b5b5301
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45728906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68a2390539f7635654f5c9430ee2007e95132c48a81d69416de4f8bc3f6ff81f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:38:52 GMT
ARG CONSUL_VERSION=1.9.11
# Mon, 15 Nov 2021 20:38:53 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.11 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:38:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:38:54 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:39:04 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:39:06 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:39:07 GMT
# ARGS: CONSUL_VERSION=1.9.11
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:39:07 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:39:07 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:39:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:39:08 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:39:08 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:39:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:39:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4f4bab377d3f918a0d8c2ddb05f9de86badd9f39a7d3d6a3ecbbe5ebfc5512d`  
		Last Modified: Mon, 15 Nov 2021 20:40:19 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e691eb3c1cc789ce2d2e5ce77693fd80627adee9529cb900296b0818fb3ca0`  
		Last Modified: Mon, 15 Nov 2021 20:40:26 GMT  
		Size: 42.9 MB (42896727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd1f22f20de7c48eda673c9429704c94f8394918b88878a8e2d778e67976ea2`  
		Last Modified: Mon, 15 Nov 2021 20:40:19 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f4bd3655e4095f284118dde5ef3eae8c0b1c8dcc7ae955e7381a826f056497`  
		Last Modified: Mon, 15 Nov 2021 20:40:19 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390f7f12b4f466339cfb54f7526fd43237224e9fc71359c0c4296366a7041651`  
		Last Modified: Mon, 15 Nov 2021 20:40:19 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:701275d51948239f213ec3122d1d8006ac12159a211fdc1c060634677d8af91a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:bd47456d9d5113ed9f1598711c4f09bbfddf6ba90834e656522a3d40c18f46b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43680607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60b5d5d7aa05804e07d8d6c740bc7418dd1f5ba1b85c6921362fcd4a43b97065`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:23:55 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:23:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:23:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:23:57 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:24:10 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:24:11 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:24:12 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:24:12 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:24:12 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:24:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:24:13 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:24:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:24:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:24:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8346c4c2c7acddb91fe63704bf85338e56c691fe7e48caa8a9fba6e7e16df095`  
		Last Modified: Mon, 15 Nov 2021 20:25:09 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f79386c0f7a4808f3eec56a09d42ac405acc2fd96f076dc0f6678d8bbc0486`  
		Last Modified: Mon, 15 Nov 2021 20:25:15 GMT  
		Size: 40.9 MB (40854814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:716e8306345a5b03bffda8e3e9bcc2248e73e36693d31986f314fb6b34c7ac9d`  
		Last Modified: Mon, 15 Nov 2021 20:25:09 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abab715aa08f3bce73846825adb35731c130d5c8ea987b6900210146b200012`  
		Last Modified: Mon, 15 Nov 2021 20:25:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ffcce388ca4a335635a00115c98cb98ad497ed565f9be669d7f3d96bc66ad9`  
		Last Modified: Mon, 15 Nov 2021 20:25:10 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:5e52ada1ee506abf00ecdf71eaf7cca79277ac9ff42a267c246f29e56a4e397f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41745889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:833c0bf37139c939bff692c0ed026e2dac3f17f4df27f97dc676e034eb984f62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:49:43 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:49:44 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:49:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:49:46 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:50:03 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:50:05 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:50:07 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:50:07 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:50:08 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:50:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:50:09 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:50:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:50:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:50:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599027c88ab7fba9b363add5e85b1cfed7c2ed7a268d39b9d903447a56cd4964`  
		Last Modified: Mon, 15 Nov 2021 20:52:16 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dd5b4f9634aad38db027711e09712af5bd06e9acc0711ca4d186afc10e167c`  
		Last Modified: Mon, 15 Nov 2021 20:52:37 GMT  
		Size: 39.1 MB (39109173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0c6b2fd0e6fe5c66f30f9d0d156e0f39a28d2baf79cceb14ea4570998a49e9`  
		Last Modified: Mon, 15 Nov 2021 20:52:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49dc9ca4c1e90f9d8544916ce818b3ece76da1b75cb91a65055b4376d2e02bd`  
		Last Modified: Mon, 15 Nov 2021 20:52:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6583eb09f599ee7493254844b0c446e2c15e7f678da336e7f3312fa0d87a222`  
		Last Modified: Mon, 15 Nov 2021 20:52:16 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:53f6d5f8cb6cbd660622386aac46e18db66f839e4fabbc8b3af4556ce7013bd3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41693581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:919a111a440fad2646f22011543d55f9828d23143cbaa17883e2813994e810e0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:39:33 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:39:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:39:35 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:39:36 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:39:49 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:39:50 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:39:50 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:39:51 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:39:52 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:39:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:39:54 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:39:56 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:39:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:39:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ec0dc3b53307c831eeab0ff2ca66c2ba920d35cdb7aef6797947eae6627b30`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3111f504ed97ecd3b4a24a4fca9128145ed4f676141777803ea21951c925a66c`  
		Last Modified: Mon, 15 Nov 2021 20:41:24 GMT  
		Size: 39.0 MB (38970628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9327a3a3328dacb9c1e1e9a671e69525c5b1a602ee29d0e396cac83f9f2a46ea`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d1ecde7662d3fd2578666467cbb5881fdf7501616f10a6e923036482dcbcbe`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e33656f5ca4619fb5de521818b485d007b57dbdbb06f289aad9e48942d11c822`  
		Last Modified: Mon, 15 Nov 2021 20:41:18 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:197e09ba241dbb63bc41b59c9f57ec9d898bb3e7bfa7969f6cdf4f95719b0f68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43065393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72354e9f46b4a02d3e3ff31febbc09b1eb7a4c3da2d6b1578c3e064ae204df31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Mon, 15 Nov 2021 20:38:27 GMT
ARG CONSUL_VERSION=1.10.4
# Mon, 15 Nov 2021 20:38:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 15 Nov 2021 20:38:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 15 Nov 2021 20:38:29 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 15 Nov 2021 20:38:41 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 15 Nov 2021 20:38:42 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 15 Nov 2021 20:38:43 GMT
# ARGS: CONSUL_VERSION=1.10.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 15 Nov 2021 20:38:43 GMT
VOLUME [/consul/data]
# Mon, 15 Nov 2021 20:38:44 GMT
EXPOSE 8300
# Mon, 15 Nov 2021 20:38:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 15 Nov 2021 20:38:44 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 15 Nov 2021 20:38:44 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 15 Nov 2021 20:38:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 15 Nov 2021 20:38:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4536d099d46227da1d6bd8d679ef4f73244926c2e9a57f086fd4674c2e29b3b`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee00223e3240f6226f08e73dac4bf1da82986fc97b3d0ccf04074d6ca360163`  
		Last Modified: Mon, 15 Nov 2021 20:40:04 GMT  
		Size: 40.2 MB (40233212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910a1c818e60d30b4058f37ae0fab42090c4fad3f1ec35c0b8e55ddb611d954`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5367fa6ffd2e7e1ddf111b01561fc9ae792cd49696e586280fdbd77949ed93d6`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a5348717f1dadeca6442f041c3c7b3b3d661ab36be2689d8e83c3de608ea92`  
		Last Modified: Mon, 15 Nov 2021 20:39:56 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
