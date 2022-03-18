## `consul:latest`

```console
$ docker pull consul@sha256:b7761e6091342148e2863d2381150a0a0465ce568160b6b4a765e5f9f67b23b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:0dd8f7016f84462a841fdca73a9e58dc4f64ed33dc8f087acb2f1696f7f57bef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43947220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec96db0e7ba685574152bd300682c9cb8aaa545c9440f504eb7e21e695f46f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Tue, 01 Mar 2022 02:07:13 GMT
ARG CONSUL_VERSION=1.11.4
# Tue, 01 Mar 2022 02:07:13 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 01 Mar 2022 02:07:13 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 01 Mar 2022 02:07:14 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 01 Mar 2022 02:07:51 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 01 Mar 2022 02:07:52 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 01 Mar 2022 02:07:52 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Mar 2022 02:07:53 GMT
VOLUME [/consul/data]
# Tue, 01 Mar 2022 02:07:53 GMT
EXPOSE 8300
# Tue, 01 Mar 2022 02:07:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 01 Mar 2022 02:07:53 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 01 Mar 2022 02:07:53 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Mar 2022 02:07:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 02:07:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a443d53d3f8ea4160ee69c8bade01d3a76db791c43aeec8a4df1632036bfdccc`  
		Last Modified: Tue, 01 Mar 2022 02:10:10 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddf97293f04383bdc3fca4bd3230f9e398d6f29bb085ea9256f0c4d4e479435`  
		Last Modified: Tue, 01 Mar 2022 02:10:16 GMT  
		Size: 41.1 MB (41121418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6560b30610da9f4ee48f7ef6ef1e67df4525600745350e46f1d33f9c6e9699c`  
		Last Modified: Tue, 01 Mar 2022 02:10:09 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26840f3e1ef52e9f78b48213767b49dcdc66df4a700358f287236b6054654203`  
		Last Modified: Tue, 01 Mar 2022 02:10:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fe1e03676d1a884d8b15d685b0541f4b51159a3bb439844a027f9c9a34a281`  
		Last Modified: Tue, 01 Mar 2022 02:10:09 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:abf34e60affca0c66c7c3d14cb33629da18bbc0b8a3d4afc67da60f75b70ebeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41706595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e90c4a2d1cd3657045f42b44191a2a435e1c18d92642072739803fc5ea9e1d3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:01:04 GMT
ARG CONSUL_VERSION=1.11.4
# Thu, 17 Mar 2022 15:01:04 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 17 Mar 2022 15:01:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Mar 2022 15:01:06 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Mar 2022 15:01:33 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Mar 2022 15:01:35 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Mar 2022 15:01:36 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 15:01:37 GMT
VOLUME [/consul/data]
# Thu, 17 Mar 2022 15:01:37 GMT
EXPOSE 8300
# Thu, 17 Mar 2022 15:01:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Mar 2022 15:01:38 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Mar 2022 15:01:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 15:01:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 15:01:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9c5bf708c984009dcf64d1f562e91fff73460ea160ca3e6d8834de6c5d64e2`  
		Last Modified: Thu, 17 Mar 2022 15:04:07 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2278ccd73c4449225c88fa7c1e01a3238466884d1614b87dc8943e3539f40a`  
		Last Modified: Thu, 17 Mar 2022 15:04:27 GMT  
		Size: 39.1 MB (39075299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430c6b92c0cee7151a7196b2d25e749a32a9ac97af68f404e66db04c6a24bb19`  
		Last Modified: Thu, 17 Mar 2022 15:04:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80895c4aa4b6075bdec5eb8c32c0134ff7b69b0908bd628e4758c8d455337b9b`  
		Last Modified: Thu, 17 Mar 2022 15:04:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3463c1727b45f270035d84ac880b1ba7bde5542753dca6bdc1b8eddabd04f064`  
		Last Modified: Thu, 17 Mar 2022 15:04:06 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:aa8e13b7e97dad260abf4011bc4b26aab55d2dd236005aa39a6d2e5ecee15275
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41547009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c068f418780b1e541586224eca6e776626b12641055bdc20ee943a00dcae1942`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 14:33:36 GMT
ARG CONSUL_VERSION=1.11.4
# Fri, 18 Mar 2022 14:33:37 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 18 Mar 2022 14:33:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Mar 2022 14:33:39 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Mar 2022 14:34:08 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Mar 2022 14:34:08 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Mar 2022 14:34:09 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Mar 2022 14:34:10 GMT
VOLUME [/consul/data]
# Fri, 18 Mar 2022 14:34:11 GMT
EXPOSE 8300
# Fri, 18 Mar 2022 14:34:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Mar 2022 14:34:13 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Mar 2022 14:34:15 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Mar 2022 14:34:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 14:34:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb2762b96611b8fdbe87b943df6b92d3250b95aedc75e72b589dc10e617b493`  
		Last Modified: Fri, 18 Mar 2022 14:36:14 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cbb6972494fd9daa89ebaac320e3f7f53abbff20c881f82a6aafcfdcf9ebefe`  
		Last Modified: Fri, 18 Mar 2022 14:36:19 GMT  
		Size: 38.8 MB (38824563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9201d94e21e326267f54d31a8dcc627817d195bb9a7fac263fc9d6b3dab6752`  
		Last Modified: Fri, 18 Mar 2022 14:36:14 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2322fcdb74d62f83fc6d875feb2b7802e84f05379c5036885832c858c0cdbe10`  
		Last Modified: Fri, 18 Mar 2022 14:36:14 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77e9c25f22efc815e48939f81e22ff698610002d67cb71290d8f02771328171`  
		Last Modified: Fri, 18 Mar 2022 14:36:14 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:69768a50c60a117efaa10e04e0659e55d985a4db7a10dff1a3bb400fe749b273
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42771088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a43b9eae8ee2627bbab389826c22f9808779f3a4e4caa1aa88852478b912967`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Tue, 01 Mar 2022 02:02:09 GMT
ARG CONSUL_VERSION=1.11.4
# Tue, 01 Mar 2022 02:02:09 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 01 Mar 2022 02:02:09 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 01 Mar 2022 02:02:10 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 01 Mar 2022 02:03:03 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 01 Mar 2022 02:03:03 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 01 Mar 2022 02:03:04 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Mar 2022 02:03:04 GMT
VOLUME [/consul/data]
# Tue, 01 Mar 2022 02:03:04 GMT
EXPOSE 8300
# Tue, 01 Mar 2022 02:03:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 01 Mar 2022 02:03:04 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 01 Mar 2022 02:03:04 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Mar 2022 02:03:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 02:03:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9511197d8c58e385cef16b6ebe4d92ea5c9b71a806edb0ec9b4f7e8e7c06d59f`  
		Last Modified: Tue, 01 Mar 2022 02:05:25 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed80181fb7718bb9dc52c775ecb1383acdf0efa7741d32185e2beefa273e1cd4`  
		Last Modified: Tue, 01 Mar 2022 02:05:33 GMT  
		Size: 39.9 MB (39938904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b097fcd480c2ad87b9b09d78159a35d11df7ad9ac8e5d7dc0660a94ca9d955aa`  
		Last Modified: Tue, 01 Mar 2022 02:05:25 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9022d17feed382bff697ebb156aaa949cac4b9efdbcc747155b41770283c2ea`  
		Last Modified: Tue, 01 Mar 2022 02:05:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5611c003ed95e9356d5179651cd7c2446b77deeb98aa72498b9d830201e03722`  
		Last Modified: Tue, 01 Mar 2022 02:05:26 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
