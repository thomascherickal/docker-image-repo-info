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
