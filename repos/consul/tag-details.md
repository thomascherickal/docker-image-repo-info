<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10`](#consul110)
-	[`consul:1.10.4`](#consul1104)
-	[`consul:1.11.0-beta`](#consul1110-beta)
-	[`consul:1.11.0-beta2`](#consul1110-beta2)
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
$ docker pull consul@sha256:0101ed8ed924388d203962c7f6cd00c64946a2915aa307ae6fdb77257f35afff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.0-beta` - linux; amd64

```console
$ docker pull consul@sha256:e57b5bd1735f5669571dd93cb358dafcc1274e123f85ec9878f40ba0b506bf22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43713511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33a1fbcf9760adfc346281ab93087515248a09acd754cfa38ad65dd048a23e67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:57:45 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Fri, 12 Nov 2021 21:57:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 12 Nov 2021 21:57:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 12 Nov 2021 21:57:46 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 12 Nov 2021 21:58:02 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 12 Nov 2021 21:58:05 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 12 Nov 2021 21:58:07 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:58:07 GMT
VOLUME [/consul/data]
# Fri, 12 Nov 2021 21:58:08 GMT
EXPOSE 8300
# Fri, 12 Nov 2021 21:58:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 12 Nov 2021 21:58:09 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 12 Nov 2021 21:58:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Nov 2021 21:58:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 21:58:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9dd9907ca9dba4bf6d73592e3433bb41bfd6758f9fda5deee3ba72629b90c0`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ce0fdfb8f1545e60331c6ceb496bd4ff2cedab6c4e0533ab3d9c5132308624`  
		Last Modified: Fri, 12 Nov 2021 21:59:51 GMT  
		Size: 40.9 MB (40887721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c10085b0fae3b6f6041a1de3e35988aa036d8fd1e5a6f67aaff584f889545d`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99692da936ecbe3f732798a699a03861ea39fc25a2664db7e8fd96fa3a05b24c`  
		Last Modified: Fri, 12 Nov 2021 21:59:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518e52fae0f8177dd8b49904fe878aaeabaa0eb44d2e78187ff1357a4e88eba7`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; arm variant v6

```console
$ docker pull consul@sha256:409f4b4355391f1bcc0b8bd49175b308adcc70ddca9bd5dc2dcb3977c5eb23aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39508868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2fcd863378dba6a3d8e0d211cb0030306cf1eeda473f430c45b66185d9f40dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:39 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 06:02:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:02:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:02:42 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:02:55 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:02:57 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:02:59 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:02:59 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:03:00 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:03:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:03:01 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:03:01 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:03:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:03:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2d7260b8a655c8d28c28f40ef7d386ecdf21ec4e683fca1ada03fb077990b1`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d05d8b05f792a5f378b768ab68755d34efcd88553097ba4c11fe6fd0a4fe9b7`  
		Last Modified: Sat, 13 Nov 2021 06:05:56 GMT  
		Size: 36.9 MB (36872153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4c08e221c3a9944278928e0d5a5349f02e20378f200537c7bc0abc72fc4c5b`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc684001062a2334874602425ae1f7f3321952ce632b97090c30715e183b3b6e`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5703c46ca3d761e767f57a57cc7a942a7fd182112bbb0067a92544c78775fec6`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:fb76a00c0c2adc167cd5c1aeca7241360b4a1aa891a892b0a78359a69e206a42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39287714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ebbfccc7daa528654052fa7daeffb5ebbd9e9e26102394b284b36249c55be2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:15:15 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 11:15:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 11:15:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 11:15:18 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 11:15:30 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 11:15:31 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 11:15:32 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:15:33 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 11:15:34 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 11:15:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 11:15:36 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 11:15:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 11:15:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:15:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144af28d402c6aa398c230374e0796f8b1bc72bc894128628950b7e9809cb014`  
		Last Modified: Sat, 13 Nov 2021 11:17:23 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f6468fc5c085fb9f1f7f5be01d4280e6d581d4c0288eb7c853d68b70f84189`  
		Last Modified: Sat, 13 Nov 2021 11:17:28 GMT  
		Size: 36.6 MB (36564764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910209e84ce7afdb47a37c422bb2f445b7a4c4475ad552485d2ee6266a607fc2`  
		Last Modified: Sat, 13 Nov 2021 11:17:23 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287bbf38f5b8c1472195d191f1bed4a366432659146c5082d51de5ea49d59678`  
		Last Modified: Sat, 13 Nov 2021 11:17:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c8e4ce91e5c66b30bdf7716289d2386f28e41ad88c5e9f5690556b9636dd05`  
		Last Modified: Sat, 13 Nov 2021 11:17:22 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta` - linux; 386

```console
$ docker pull consul@sha256:c329aff5d47eba46e1f6992fbe91dcf9010d6f80005286be9155f965921e7975
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42543628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb87f43018f823068831b78d7e4d452fe84225256e1edaf0aa81e8387567bbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:18:29 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 06:18:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:18:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:18:31 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:18:45 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:18:46 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:18:47 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:18:47 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:18:47 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:18:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:18:48 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:18:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:18:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c847a2ae3f27130e208c92ba400b0bc215dfbd6e6dc859cd2e39ad3aa520a`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a3c64b15b1543034c6e04bb4f1ffb5db0907892bf0e51163848219a87482d`  
		Last Modified: Sat, 13 Nov 2021 06:20:24 GMT  
		Size: 39.7 MB (39711445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bfeef4b841e5af9bbff9cb8f23fcee225725b3fede95993108c92b9061c9e9`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472433ffd68a273b7d32b1483f7cd063212e7d8dab63fec46149bda5b1bd7012`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6aec6a6bafe0942f394cf46f8857811ba95bf92af292b58b37ef99635d59af`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.0-beta2`

```console
$ docker pull consul@sha256:0101ed8ed924388d203962c7f6cd00c64946a2915aa307ae6fdb77257f35afff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.0-beta2` - linux; amd64

```console
$ docker pull consul@sha256:e57b5bd1735f5669571dd93cb358dafcc1274e123f85ec9878f40ba0b506bf22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43713511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33a1fbcf9760adfc346281ab93087515248a09acd754cfa38ad65dd048a23e67`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:57:45 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Fri, 12 Nov 2021 21:57:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 12 Nov 2021 21:57:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 12 Nov 2021 21:57:46 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 12 Nov 2021 21:58:02 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 12 Nov 2021 21:58:05 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 12 Nov 2021 21:58:07 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:58:07 GMT
VOLUME [/consul/data]
# Fri, 12 Nov 2021 21:58:08 GMT
EXPOSE 8300
# Fri, 12 Nov 2021 21:58:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 12 Nov 2021 21:58:09 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 12 Nov 2021 21:58:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Nov 2021 21:58:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Nov 2021 21:58:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9dd9907ca9dba4bf6d73592e3433bb41bfd6758f9fda5deee3ba72629b90c0`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2ce0fdfb8f1545e60331c6ceb496bd4ff2cedab6c4e0533ab3d9c5132308624`  
		Last Modified: Fri, 12 Nov 2021 21:59:51 GMT  
		Size: 40.9 MB (40887721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c10085b0fae3b6f6041a1de3e35988aa036d8fd1e5a6f67aaff584f889545d`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99692da936ecbe3f732798a699a03861ea39fc25a2664db7e8fd96fa3a05b24c`  
		Last Modified: Fri, 12 Nov 2021 21:59:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518e52fae0f8177dd8b49904fe878aaeabaa0eb44d2e78187ff1357a4e88eba7`  
		Last Modified: Fri, 12 Nov 2021 21:59:45 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta2` - linux; arm variant v6

```console
$ docker pull consul@sha256:409f4b4355391f1bcc0b8bd49175b308adcc70ddca9bd5dc2dcb3977c5eb23aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39508868 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2fcd863378dba6a3d8e0d211cb0030306cf1eeda473f430c45b66185d9f40dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:39 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 06:02:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:02:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:02:42 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:02:55 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:02:57 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:02:59 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:02:59 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:03:00 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:03:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:03:01 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:03:01 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:03:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:03:02 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2d7260b8a655c8d28c28f40ef7d386ecdf21ec4e683fca1ada03fb077990b1`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d05d8b05f792a5f378b768ab68755d34efcd88553097ba4c11fe6fd0a4fe9b7`  
		Last Modified: Sat, 13 Nov 2021 06:05:56 GMT  
		Size: 36.9 MB (36872153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4c08e221c3a9944278928e0d5a5349f02e20378f200537c7bc0abc72fc4c5b`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc684001062a2334874602425ae1f7f3321952ce632b97090c30715e183b3b6e`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5703c46ca3d761e767f57a57cc7a942a7fd182112bbb0067a92544c78775fec6`  
		Last Modified: Sat, 13 Nov 2021 06:05:43 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:fb76a00c0c2adc167cd5c1aeca7241360b4a1aa891a892b0a78359a69e206a42
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39287714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68ebbfccc7daa528654052fa7daeffb5ebbd9e9e26102394b284b36249c55be2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:15:15 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 11:15:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 11:15:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 11:15:18 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 11:15:30 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 11:15:31 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 11:15:32 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:15:33 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 11:15:34 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 11:15:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 11:15:36 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 11:15:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 11:15:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 11:15:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144af28d402c6aa398c230374e0796f8b1bc72bc894128628950b7e9809cb014`  
		Last Modified: Sat, 13 Nov 2021 11:17:23 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f6468fc5c085fb9f1f7f5be01d4280e6d581d4c0288eb7c853d68b70f84189`  
		Last Modified: Sat, 13 Nov 2021 11:17:28 GMT  
		Size: 36.6 MB (36564764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910209e84ce7afdb47a37c422bb2f445b7a4c4475ad552485d2ee6266a607fc2`  
		Last Modified: Sat, 13 Nov 2021 11:17:23 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287bbf38f5b8c1472195d191f1bed4a366432659146c5082d51de5ea49d59678`  
		Last Modified: Sat, 13 Nov 2021 11:17:22 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c8e4ce91e5c66b30bdf7716289d2386f28e41ad88c5e9f5690556b9636dd05`  
		Last Modified: Sat, 13 Nov 2021 11:17:22 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.0-beta2` - linux; 386

```console
$ docker pull consul@sha256:c329aff5d47eba46e1f6992fbe91dcf9010d6f80005286be9155f965921e7975
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42543628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bdb87f43018f823068831b78d7e4d452fe84225256e1edaf0aa81e8387567bbc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:18:29 GMT
ARG CONSUL_VERSION=1.11.0-beta2
# Sat, 13 Nov 2021 06:18:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.0-beta2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 13 Nov 2021 06:18:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 13 Nov 2021 06:18:31 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 13 Nov 2021 06:18:45 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 13 Nov 2021 06:18:46 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 13 Nov 2021 06:18:47 GMT
# ARGS: CONSUL_VERSION=1.11.0-beta2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 06:18:47 GMT
VOLUME [/consul/data]
# Sat, 13 Nov 2021 06:18:47 GMT
EXPOSE 8300
# Sat, 13 Nov 2021 06:18:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 13 Nov 2021 06:18:48 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 13 Nov 2021 06:18:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:18:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:18:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c847a2ae3f27130e208c92ba400b0bc215dfbd6e6dc859cd2e39ad3aa520a`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746a3c64b15b1543034c6e04bb4f1ffb5db0907892bf0e51163848219a87482d`  
		Last Modified: Sat, 13 Nov 2021 06:20:24 GMT  
		Size: 39.7 MB (39711445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9bfeef4b841e5af9bbff9cb8f23fcee225725b3fede95993108c92b9061c9e9`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472433ffd68a273b7d32b1483f7cd063212e7d8dab63fec46149bda5b1bd7012`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6aec6a6bafe0942f394cf46f8857811ba95bf92af292b58b37ef99635d59af`  
		Last Modified: Sat, 13 Nov 2021 06:20:17 GMT  
		Size: 1.8 KB (1786 bytes)  
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
