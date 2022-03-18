<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10`](#consul110)
-	[`consul:1.10.9`](#consul1109)
-	[`consul:1.11`](#consul111)
-	[`consul:1.11.4`](#consul1114)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.16`](#consul1916)
-	[`consul:latest`](#consullatest)

## `consul:1.10`

```console
$ docker pull consul@sha256:d51f42577622f1e199fa506ce3799570087e5d7e3a048c110b49efcd95030c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10` - linux; amd64

```console
$ docker pull consul@sha256:17f53a8c175a98aa9b5d214b6c1c65dba74c84799891bb478533b915fe8662f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43749079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fd65892192f381ecbbbae904bd17bc484cb299b26457d3b13766af273a68a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Tue, 01 Mar 2022 02:08:01 GMT
ARG CONSUL_VERSION=1.10.9
# Tue, 01 Mar 2022 02:08:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 01 Mar 2022 02:08:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 01 Mar 2022 02:08:02 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 01 Mar 2022 02:08:47 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 01 Mar 2022 02:08:47 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 01 Mar 2022 02:08:48 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Mar 2022 02:08:48 GMT
VOLUME [/consul/data]
# Tue, 01 Mar 2022 02:08:48 GMT
EXPOSE 8300
# Tue, 01 Mar 2022 02:08:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 01 Mar 2022 02:08:48 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 01 Mar 2022 02:08:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Mar 2022 02:08:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 02:08:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3206213cb80b8563b090d7a3909c9823b121155bbb4f340924a98e4a96d6b7`  
		Last Modified: Tue, 01 Mar 2022 02:10:28 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64aa1b447a7a8b3a67a9c64c8f68c05894a4083f35ce5055f4543f02f038b06e`  
		Last Modified: Tue, 01 Mar 2022 02:10:34 GMT  
		Size: 40.9 MB (40923290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f664ef6bc4b483b31613ca7d3d5f356ae34962216073bec1e08fc42e94dd8`  
		Last Modified: Tue, 01 Mar 2022 02:10:28 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a51dcd256c6437ce6c123728335285c0f0332d52e6d4c5651c1720643cdb15c`  
		Last Modified: Tue, 01 Mar 2022 02:10:28 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef16602b9a165c664d41e8e4227590dfe06a3df0471e29cf5ceefded15b17ee`  
		Last Modified: Tue, 01 Mar 2022 02:10:28 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:113dabdbf5c2cb51df24729d5840fb6c7f816ed3b2023a6faf6fb5ccbaeda5ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41806201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8ae2c74d7d26813999b814ea5323c844a4f071c92bc978b99ac0003a536be1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:01:54 GMT
ARG CONSUL_VERSION=1.10.9
# Thu, 17 Mar 2022 15:01:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 17 Mar 2022 15:01:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Mar 2022 15:01:56 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Mar 2022 15:02:25 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Mar 2022 15:02:27 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Mar 2022 15:02:28 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 15:02:29 GMT
VOLUME [/consul/data]
# Thu, 17 Mar 2022 15:02:29 GMT
EXPOSE 8300
# Thu, 17 Mar 2022 15:02:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Mar 2022 15:02:30 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Mar 2022 15:02:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 15:02:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 15:02:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973431bb8cb6b431ddda12842fdb25ff83605f8d4ba530461b332a66e5cce059`  
		Last Modified: Thu, 17 Mar 2022 15:04:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edfaa24b3e799bad0740029a867b395d800f2a9d47fdf85888121ebf75501f6`  
		Last Modified: Thu, 17 Mar 2022 15:05:05 GMT  
		Size: 39.2 MB (39174901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d5d67ad40c156753ebbeb641bc6e25e616fadb2d38cbd74750c1cf53c3d6c4`  
		Last Modified: Thu, 17 Mar 2022 15:04:43 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ccd6b631dbee3438b0730488ab227f541738dff775145ede51d4f47391f20`  
		Last Modified: Thu, 17 Mar 2022 15:04:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738f440dadea355e7787bceb157579978a3b1c1f5c2e2f219678caf0df14fb0b`  
		Last Modified: Thu, 17 Mar 2022 15:04:43 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:d1cbfb33209c48b6dcaa6935840063e6f2e35dff1b7e96c2b6b9932f3e429008
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41772469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a874c7d280e942c2eb99c7e771c9a3faef4526a1d0aef90ef11e170bcf51fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 14:34:27 GMT
ARG CONSUL_VERSION=1.10.9
# Fri, 18 Mar 2022 14:34:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 18 Mar 2022 14:34:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Mar 2022 14:34:30 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Mar 2022 14:35:03 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Mar 2022 14:35:04 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Mar 2022 14:35:05 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Mar 2022 14:35:06 GMT
VOLUME [/consul/data]
# Fri, 18 Mar 2022 14:35:07 GMT
EXPOSE 8300
# Fri, 18 Mar 2022 14:35:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Mar 2022 14:35:09 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Mar 2022 14:35:11 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Mar 2022 14:35:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 14:35:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5222cbbcb7849f356e1f62f742b0b6f00163a70d1d827e442018d984913df8d`  
		Last Modified: Fri, 18 Mar 2022 14:36:34 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f98041bdcc7776b7ae042b587d48cffac08b6fd178c5335654769f0e9dae403`  
		Last Modified: Fri, 18 Mar 2022 14:36:39 GMT  
		Size: 39.1 MB (39050022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7fe8ba9ccbd8c4c4aea96c16f3fe82701fefd8adfd9cbec238721ac1a5f165`  
		Last Modified: Fri, 18 Mar 2022 14:36:34 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e638d299d985b02ed853ad9464bb9a73a5029c9c912ff24e7419075193d2a5`  
		Last Modified: Fri, 18 Mar 2022 14:36:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49038f362efb0816c0bf5e78f8d802debf02c99dea1bf8ce091828b087947693`  
		Last Modified: Fri, 18 Mar 2022 14:36:34 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; 386

```console
$ docker pull consul@sha256:3628e720982924a4adc41322acb4d0287a78e657616bd2347ad628fd6cad280c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43118415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4c9435c954bb6c2da729bdf46454f7994e03dc11de93e4fdd4c72b476615463`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Tue, 01 Mar 2022 02:03:19 GMT
ARG CONSUL_VERSION=1.10.9
# Tue, 01 Mar 2022 02:03:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 01 Mar 2022 02:03:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 01 Mar 2022 02:03:20 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 01 Mar 2022 02:04:02 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 01 Mar 2022 02:04:02 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 01 Mar 2022 02:04:03 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Mar 2022 02:04:03 GMT
VOLUME [/consul/data]
# Tue, 01 Mar 2022 02:04:03 GMT
EXPOSE 8300
# Tue, 01 Mar 2022 02:04:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 01 Mar 2022 02:04:03 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 01 Mar 2022 02:04:04 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Mar 2022 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 02:04:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a70bc6500b8fd8b95656f886a61351fe8a789ef44cff8203160d2f33005fe23`  
		Last Modified: Tue, 01 Mar 2022 02:05:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7106cb8d848c66fa6cd8e95c324f354c3c8f83c29e4323148bc771b6b37d03`  
		Last Modified: Tue, 01 Mar 2022 02:05:56 GMT  
		Size: 40.3 MB (40286230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab99e66a59b6e871df5340969b2a3991037f6779bfd69ec88310964e956d7c1`  
		Last Modified: Tue, 01 Mar 2022 02:05:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2db7261b391bf2dda992288190e7d6bbfed0fc60637d9a36644c25c63fd76f4`  
		Last Modified: Tue, 01 Mar 2022 02:05:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d87d80a1bd5e92dc3d780a05181a64020c4252952364c0c576cfc29836a6174`  
		Last Modified: Tue, 01 Mar 2022 02:05:49 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.9`

```console
$ docker pull consul@sha256:d51f42577622f1e199fa506ce3799570087e5d7e3a048c110b49efcd95030c2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.9` - linux; amd64

```console
$ docker pull consul@sha256:17f53a8c175a98aa9b5d214b6c1c65dba74c84799891bb478533b915fe8662f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43749079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5fd65892192f381ecbbbae904bd17bc484cb299b26457d3b13766af273a68a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Tue, 01 Mar 2022 02:08:01 GMT
ARG CONSUL_VERSION=1.10.9
# Tue, 01 Mar 2022 02:08:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 01 Mar 2022 02:08:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 01 Mar 2022 02:08:02 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 01 Mar 2022 02:08:47 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 01 Mar 2022 02:08:47 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 01 Mar 2022 02:08:48 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Mar 2022 02:08:48 GMT
VOLUME [/consul/data]
# Tue, 01 Mar 2022 02:08:48 GMT
EXPOSE 8300
# Tue, 01 Mar 2022 02:08:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 01 Mar 2022 02:08:48 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 01 Mar 2022 02:08:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Mar 2022 02:08:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 02:08:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3206213cb80b8563b090d7a3909c9823b121155bbb4f340924a98e4a96d6b7`  
		Last Modified: Tue, 01 Mar 2022 02:10:28 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64aa1b447a7a8b3a67a9c64c8f68c05894a4083f35ce5055f4543f02f038b06e`  
		Last Modified: Tue, 01 Mar 2022 02:10:34 GMT  
		Size: 40.9 MB (40923290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9f664ef6bc4b483b31613ca7d3d5f356ae34962216073bec1e08fc42e94dd8`  
		Last Modified: Tue, 01 Mar 2022 02:10:28 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a51dcd256c6437ce6c123728335285c0f0332d52e6d4c5651c1720643cdb15c`  
		Last Modified: Tue, 01 Mar 2022 02:10:28 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef16602b9a165c664d41e8e4227590dfe06a3df0471e29cf5ceefded15b17ee`  
		Last Modified: Tue, 01 Mar 2022 02:10:28 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:113dabdbf5c2cb51df24729d5840fb6c7f816ed3b2023a6faf6fb5ccbaeda5ae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41806201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8ae2c74d7d26813999b814ea5323c844a4f071c92bc978b99ac0003a536be1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:01:54 GMT
ARG CONSUL_VERSION=1.10.9
# Thu, 17 Mar 2022 15:01:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 17 Mar 2022 15:01:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Mar 2022 15:01:56 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Mar 2022 15:02:25 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Mar 2022 15:02:27 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Mar 2022 15:02:28 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 15:02:29 GMT
VOLUME [/consul/data]
# Thu, 17 Mar 2022 15:02:29 GMT
EXPOSE 8300
# Thu, 17 Mar 2022 15:02:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Mar 2022 15:02:30 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Mar 2022 15:02:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 15:02:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 15:02:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973431bb8cb6b431ddda12842fdb25ff83605f8d4ba530461b332a66e5cce059`  
		Last Modified: Thu, 17 Mar 2022 15:04:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edfaa24b3e799bad0740029a867b395d800f2a9d47fdf85888121ebf75501f6`  
		Last Modified: Thu, 17 Mar 2022 15:05:05 GMT  
		Size: 39.2 MB (39174901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d5d67ad40c156753ebbeb641bc6e25e616fadb2d38cbd74750c1cf53c3d6c4`  
		Last Modified: Thu, 17 Mar 2022 15:04:43 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473ccd6b631dbee3438b0730488ab227f541738dff775145ede51d4f47391f20`  
		Last Modified: Thu, 17 Mar 2022 15:04:43 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738f440dadea355e7787bceb157579978a3b1c1f5c2e2f219678caf0df14fb0b`  
		Last Modified: Thu, 17 Mar 2022 15:04:43 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:d1cbfb33209c48b6dcaa6935840063e6f2e35dff1b7e96c2b6b9932f3e429008
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41772469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a874c7d280e942c2eb99c7e771c9a3faef4526a1d0aef90ef11e170bcf51fe4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 14:34:27 GMT
ARG CONSUL_VERSION=1.10.9
# Fri, 18 Mar 2022 14:34:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 18 Mar 2022 14:34:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Mar 2022 14:34:30 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Mar 2022 14:35:03 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Mar 2022 14:35:04 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Mar 2022 14:35:05 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Mar 2022 14:35:06 GMT
VOLUME [/consul/data]
# Fri, 18 Mar 2022 14:35:07 GMT
EXPOSE 8300
# Fri, 18 Mar 2022 14:35:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Mar 2022 14:35:09 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Mar 2022 14:35:11 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Mar 2022 14:35:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 14:35:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5222cbbcb7849f356e1f62f742b0b6f00163a70d1d827e442018d984913df8d`  
		Last Modified: Fri, 18 Mar 2022 14:36:34 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f98041bdcc7776b7ae042b587d48cffac08b6fd178c5335654769f0e9dae403`  
		Last Modified: Fri, 18 Mar 2022 14:36:39 GMT  
		Size: 39.1 MB (39050022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7fe8ba9ccbd8c4c4aea96c16f3fe82701fefd8adfd9cbec238721ac1a5f165`  
		Last Modified: Fri, 18 Mar 2022 14:36:34 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e638d299d985b02ed853ad9464bb9a73a5029c9c912ff24e7419075193d2a5`  
		Last Modified: Fri, 18 Mar 2022 14:36:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49038f362efb0816c0bf5e78f8d802debf02c99dea1bf8ce091828b087947693`  
		Last Modified: Fri, 18 Mar 2022 14:36:34 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.9` - linux; 386

```console
$ docker pull consul@sha256:3628e720982924a4adc41322acb4d0287a78e657616bd2347ad628fd6cad280c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43118415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4c9435c954bb6c2da729bdf46454f7994e03dc11de93e4fdd4c72b476615463`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Tue, 01 Mar 2022 02:03:19 GMT
ARG CONSUL_VERSION=1.10.9
# Tue, 01 Mar 2022 02:03:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 01 Mar 2022 02:03:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 01 Mar 2022 02:03:20 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 01 Mar 2022 02:04:02 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 01 Mar 2022 02:04:02 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 01 Mar 2022 02:04:03 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Mar 2022 02:04:03 GMT
VOLUME [/consul/data]
# Tue, 01 Mar 2022 02:04:03 GMT
EXPOSE 8300
# Tue, 01 Mar 2022 02:04:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 01 Mar 2022 02:04:03 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 01 Mar 2022 02:04:04 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Mar 2022 02:04:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 02:04:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a70bc6500b8fd8b95656f886a61351fe8a789ef44cff8203160d2f33005fe23`  
		Last Modified: Tue, 01 Mar 2022 02:05:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7106cb8d848c66fa6cd8e95c324f354c3c8f83c29e4323148bc771b6b37d03`  
		Last Modified: Tue, 01 Mar 2022 02:05:56 GMT  
		Size: 40.3 MB (40286230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab99e66a59b6e871df5340969b2a3991037f6779bfd69ec88310964e956d7c1`  
		Last Modified: Tue, 01 Mar 2022 02:05:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2db7261b391bf2dda992288190e7d6bbfed0fc60637d9a36644c25c63fd76f4`  
		Last Modified: Tue, 01 Mar 2022 02:05:49 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d87d80a1bd5e92dc3d780a05181a64020c4252952364c0c576cfc29836a6174`  
		Last Modified: Tue, 01 Mar 2022 02:05:49 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11`

```console
$ docker pull consul@sha256:b7761e6091342148e2863d2381150a0a0465ce568160b6b4a765e5f9f67b23b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11` - linux; amd64

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

### `consul:1.11` - linux; arm variant v6

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

### `consul:1.11` - linux; arm64 variant v8

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

### `consul:1.11` - linux; 386

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

## `consul:1.11.4`

```console
$ docker pull consul@sha256:b7761e6091342148e2863d2381150a0a0465ce568160b6b4a765e5f9f67b23b3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.4` - linux; amd64

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

### `consul:1.11.4` - linux; arm variant v6

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

### `consul:1.11.4` - linux; arm64 variant v8

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

### `consul:1.11.4` - linux; 386

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

## `consul:1.9`

```console
$ docker pull consul@sha256:23a9b65b74925e45bc871925980a9ea4ca7e3c2db08f14a4e40d1c50dcd79f9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:58223761c9e081382eacd41b97f451e7b8447ec0d589bfeb59c98e569cac53de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40156977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ce655101379df5daf5f5c6a8e7ed43f0b27067847a70c5e76c23a867d15cd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Tue, 01 Mar 2022 02:08:59 GMT
ARG CONSUL_VERSION=1.9.16
# Tue, 01 Mar 2022 02:08:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 01 Mar 2022 02:08:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 01 Mar 2022 02:09:00 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 01 Mar 2022 02:09:44 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 01 Mar 2022 02:09:44 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 01 Mar 2022 02:09:45 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Mar 2022 02:09:45 GMT
VOLUME [/consul/data]
# Tue, 01 Mar 2022 02:09:45 GMT
EXPOSE 8300
# Tue, 01 Mar 2022 02:09:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 01 Mar 2022 02:09:45 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 01 Mar 2022 02:09:45 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Mar 2022 02:09:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 02:09:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de20bec57603062f5c4d1e8fe6fc6b5504082f0ae0cad1f2200d236d420ec0ba`  
		Last Modified: Tue, 01 Mar 2022 02:10:44 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1510cc0bb728330a02cc28e451cad91b28222fc7ea8baba282c33a4dce768c`  
		Last Modified: Tue, 01 Mar 2022 02:10:50 GMT  
		Size: 37.3 MB (37331177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3441e72eaea91332d44c0b0741006a2ed972da3d4ba228abb3cc74bdd2ed3dd4`  
		Last Modified: Tue, 01 Mar 2022 02:10:44 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9bcbf580aa6574f0dcd72344b47b86330d30763282ff6c672a74b0066e61a66`  
		Last Modified: Tue, 01 Mar 2022 02:10:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d4581a629b5a9a1d062d04579a84311ad44a0877307397bc89386e9dd949b5`  
		Last Modified: Tue, 01 Mar 2022 02:10:44 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:8a1d9bc1fa91c78556f8d9eda80e34d7f4b1810ba50560d9efe583e84f32956a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38205080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201f6604c4d955de0069fc91b7530de3ca8572d3da8ba0166623e51b5b76801d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:02:44 GMT
ARG CONSUL_VERSION=1.9.16
# Thu, 17 Mar 2022 15:02:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 17 Mar 2022 15:02:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Mar 2022 15:02:47 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Mar 2022 15:03:15 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Mar 2022 15:03:16 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Mar 2022 15:03:18 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 15:03:18 GMT
VOLUME [/consul/data]
# Thu, 17 Mar 2022 15:03:19 GMT
EXPOSE 8300
# Thu, 17 Mar 2022 15:03:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Mar 2022 15:03:20 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Mar 2022 15:03:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 15:03:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 15:03:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca5a6486379980e79ce642f585ee3bd2ced7feccfcb63986b3022e78030208e`  
		Last Modified: Thu, 17 Mar 2022 15:05:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3163997b02164582d859f2aabd2033c0d724e9134786ee24879b69f800c742c`  
		Last Modified: Thu, 17 Mar 2022 15:05:36 GMT  
		Size: 35.6 MB (35573787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba661a8b1318f98603a54fa933125be61448a966e9a12705b44a24ab14b942a7`  
		Last Modified: Thu, 17 Mar 2022 15:05:18 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e026114e6b1612a5cdbf4543ece2f1931480a1bc0df978b4c4ff94f35796b8c`  
		Last Modified: Thu, 17 Mar 2022 15:05:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce093693994c134a364ff61cb65a0755b7c697f1cb778b06f4b2ae579ac82eb5`  
		Last Modified: Thu, 17 Mar 2022 15:05:18 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:f7fe09a4c56602a7e74e7c6ec6b7bf04e32dfb396e439c56858e74243106beaa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38168399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b74db4890443f9dea38654608d0b7d22c829c82b41efebf54efd7f81579dc58`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 14:35:19 GMT
ARG CONSUL_VERSION=1.9.16
# Fri, 18 Mar 2022 14:35:20 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 18 Mar 2022 14:35:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Mar 2022 14:35:22 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Mar 2022 14:35:42 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Mar 2022 14:35:43 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Mar 2022 14:35:44 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Mar 2022 14:35:45 GMT
VOLUME [/consul/data]
# Fri, 18 Mar 2022 14:35:46 GMT
EXPOSE 8300
# Fri, 18 Mar 2022 14:35:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Mar 2022 14:35:48 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Mar 2022 14:35:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Mar 2022 14:35:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 14:35:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa70f347ad89009bc95cbea48a8b0009e25da6f8901034942ee152ad145740f`  
		Last Modified: Fri, 18 Mar 2022 14:36:50 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93aecb2d054c1f9d0754a47c68aa480cba72221715e11d04b63b7858271c7640`  
		Last Modified: Fri, 18 Mar 2022 14:36:55 GMT  
		Size: 35.4 MB (35445951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1faa8fb6a252494b3b6fd1b4e48ea8d589458624a822901b3eb874995e1600`  
		Last Modified: Fri, 18 Mar 2022 14:36:50 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837d64db1c797479f6756af49c997a12c2d874486536173ee0717301b680c562`  
		Last Modified: Fri, 18 Mar 2022 14:36:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17279af7a9c65f0e43d6832eb8941c27b09f6d04a1a9c4ac9c00bbb371c225c5`  
		Last Modified: Fri, 18 Mar 2022 14:36:51 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:f86c813984406d39d3991fd31e16bf8750caf291098b95c4109c8d14614f9557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39515687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cecf06e370aec674af48da627037d681119af3dc13dbd91b6c6c8e2e068c297d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Tue, 01 Mar 2022 02:04:09 GMT
ARG CONSUL_VERSION=1.9.16
# Tue, 01 Mar 2022 02:04:09 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 01 Mar 2022 02:04:09 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 01 Mar 2022 02:04:10 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 01 Mar 2022 02:04:55 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 01 Mar 2022 02:04:56 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 01 Mar 2022 02:04:56 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Mar 2022 02:04:56 GMT
VOLUME [/consul/data]
# Tue, 01 Mar 2022 02:04:56 GMT
EXPOSE 8300
# Tue, 01 Mar 2022 02:04:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 01 Mar 2022 02:04:57 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 01 Mar 2022 02:04:57 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Mar 2022 02:04:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 02:04:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfc7f9e90e738f44b615eb913a41ca3c06f9e9f644aa8ae7367108a487a4013`  
		Last Modified: Tue, 01 Mar 2022 02:06:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36ed7bb130b98d5b3941286a3b18e66106de11ab8fba756aefee5972065bd2f`  
		Last Modified: Tue, 01 Mar 2022 02:06:14 GMT  
		Size: 36.7 MB (36683502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545729e55c0df18e4995e742baa7a802e73eeca61e14358d588769aad6749a0a`  
		Last Modified: Tue, 01 Mar 2022 02:06:07 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598812672afaa386e0f3fb63af60ed9158615d9c828f0d21641df8d4c516b29`  
		Last Modified: Tue, 01 Mar 2022 02:06:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9c5062862aa77b9344e5a9cd395108ff566cd5cad5bf0d6f80d6f26cdd31a0`  
		Last Modified: Tue, 01 Mar 2022 02:06:07 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.16`

```console
$ docker pull consul@sha256:23a9b65b74925e45bc871925980a9ea4ca7e3c2db08f14a4e40d1c50dcd79f9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.16` - linux; amd64

```console
$ docker pull consul@sha256:58223761c9e081382eacd41b97f451e7b8447ec0d589bfeb59c98e569cac53de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40156977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ce655101379df5daf5f5c6a8e7ed43f0b27067847a70c5e76c23a867d15cd6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Tue, 01 Mar 2022 02:08:59 GMT
ARG CONSUL_VERSION=1.9.16
# Tue, 01 Mar 2022 02:08:59 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 01 Mar 2022 02:08:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 01 Mar 2022 02:09:00 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 01 Mar 2022 02:09:44 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 01 Mar 2022 02:09:44 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 01 Mar 2022 02:09:45 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Mar 2022 02:09:45 GMT
VOLUME [/consul/data]
# Tue, 01 Mar 2022 02:09:45 GMT
EXPOSE 8300
# Tue, 01 Mar 2022 02:09:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 01 Mar 2022 02:09:45 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 01 Mar 2022 02:09:45 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Mar 2022 02:09:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 02:09:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de20bec57603062f5c4d1e8fe6fc6b5504082f0ae0cad1f2200d236d420ec0ba`  
		Last Modified: Tue, 01 Mar 2022 02:10:44 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1510cc0bb728330a02cc28e451cad91b28222fc7ea8baba282c33a4dce768c`  
		Last Modified: Tue, 01 Mar 2022 02:10:50 GMT  
		Size: 37.3 MB (37331177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3441e72eaea91332d44c0b0741006a2ed972da3d4ba228abb3cc74bdd2ed3dd4`  
		Last Modified: Tue, 01 Mar 2022 02:10:44 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9bcbf580aa6574f0dcd72344b47b86330d30763282ff6c672a74b0066e61a66`  
		Last Modified: Tue, 01 Mar 2022 02:10:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d4581a629b5a9a1d062d04579a84311ad44a0877307397bc89386e9dd949b5`  
		Last Modified: Tue, 01 Mar 2022 02:10:44 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.16` - linux; arm variant v6

```console
$ docker pull consul@sha256:8a1d9bc1fa91c78556f8d9eda80e34d7f4b1810ba50560d9efe583e84f32956a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38205080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201f6604c4d955de0069fc91b7530de3ca8572d3da8ba0166623e51b5b76801d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 14:32:45 GMT
ADD file:85dfb53147cadaa6ec9595f75c71284523f862af4b9edb32c7f8ccebb0ef50a8 in / 
# Thu, 17 Mar 2022 14:32:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:02:44 GMT
ARG CONSUL_VERSION=1.9.16
# Thu, 17 Mar 2022 15:02:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 17 Mar 2022 15:02:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 17 Mar 2022 15:02:47 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 17 Mar 2022 15:03:15 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 17 Mar 2022 15:03:16 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 17 Mar 2022 15:03:18 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 17 Mar 2022 15:03:18 GMT
VOLUME [/consul/data]
# Thu, 17 Mar 2022 15:03:19 GMT
EXPOSE 8300
# Thu, 17 Mar 2022 15:03:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 17 Mar 2022 15:03:20 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 17 Mar 2022 15:03:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Mar 2022 15:03:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 15:03:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:84104bbf59c688eb09fa3dfa49f67ee18a001947cd8e75d4c8d09e92926d6b31`  
		Last Modified: Thu, 17 Mar 2022 14:34:22 GMT  
		Size: 2.6 MB (2627924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca5a6486379980e79ce642f585ee3bd2ced7feccfcb63986b3022e78030208e`  
		Last Modified: Thu, 17 Mar 2022 15:05:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3163997b02164582d859f2aabd2033c0d724e9134786ee24879b69f800c742c`  
		Last Modified: Thu, 17 Mar 2022 15:05:36 GMT  
		Size: 35.6 MB (35573787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba661a8b1318f98603a54fa933125be61448a966e9a12705b44a24ab14b942a7`  
		Last Modified: Thu, 17 Mar 2022 15:05:18 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e026114e6b1612a5cdbf4543ece2f1931480a1bc0df978b4c4ff94f35796b8c`  
		Last Modified: Thu, 17 Mar 2022 15:05:18 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce093693994c134a364ff61cb65a0755b7c697f1cb778b06f4b2ae579ac82eb5`  
		Last Modified: Thu, 17 Mar 2022 15:05:18 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.16` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:f7fe09a4c56602a7e74e7c6ec6b7bf04e32dfb396e439c56858e74243106beaa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38168399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b74db4890443f9dea38654608d0b7d22c829c82b41efebf54efd7f81579dc58`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:19 GMT
ADD file:0bbbf3ca52651bbef2547689474beafcef779899da63743efd8166a01d9f3f7a in / 
# Thu, 17 Mar 2022 18:43:20 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 14:35:19 GMT
ARG CONSUL_VERSION=1.9.16
# Fri, 18 Mar 2022 14:35:20 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 18 Mar 2022 14:35:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 18 Mar 2022 14:35:22 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 18 Mar 2022 14:35:42 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 18 Mar 2022 14:35:43 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 18 Mar 2022 14:35:44 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 18 Mar 2022 14:35:45 GMT
VOLUME [/consul/data]
# Fri, 18 Mar 2022 14:35:46 GMT
EXPOSE 8300
# Fri, 18 Mar 2022 14:35:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 18 Mar 2022 14:35:48 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 18 Mar 2022 14:35:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Mar 2022 14:35:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 14:35:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6b5c040bf1f18956758f68628afdc8e179044ac75bcd411134da39a661a772e0`  
		Last Modified: Thu, 17 Mar 2022 18:44:11 GMT  
		Size: 2.7 MB (2719134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa70f347ad89009bc95cbea48a8b0009e25da6f8901034942ee152ad145740f`  
		Last Modified: Fri, 18 Mar 2022 14:36:50 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93aecb2d054c1f9d0754a47c68aa480cba72221715e11d04b63b7858271c7640`  
		Last Modified: Fri, 18 Mar 2022 14:36:55 GMT  
		Size: 35.4 MB (35445951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da1faa8fb6a252494b3b6fd1b4e48ea8d589458624a822901b3eb874995e1600`  
		Last Modified: Fri, 18 Mar 2022 14:36:50 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837d64db1c797479f6756af49c997a12c2d874486536173ee0717301b680c562`  
		Last Modified: Fri, 18 Mar 2022 14:36:50 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17279af7a9c65f0e43d6832eb8941c27b09f6d04a1a9c4ac9c00bbb371c225c5`  
		Last Modified: Fri, 18 Mar 2022 14:36:51 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9.16` - linux; 386

```console
$ docker pull consul@sha256:f86c813984406d39d3991fd31e16bf8750caf291098b95c4109c8d14614f9557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39515687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cecf06e370aec674af48da627037d681119af3dc13dbd91b6c6c8e2e068c297d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Tue, 01 Mar 2022 02:04:09 GMT
ARG CONSUL_VERSION=1.9.16
# Tue, 01 Mar 2022 02:04:09 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 01 Mar 2022 02:04:09 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 01 Mar 2022 02:04:10 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 01 Mar 2022 02:04:55 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 01 Mar 2022 02:04:56 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 01 Mar 2022 02:04:56 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 01 Mar 2022 02:04:56 GMT
VOLUME [/consul/data]
# Tue, 01 Mar 2022 02:04:56 GMT
EXPOSE 8300
# Tue, 01 Mar 2022 02:04:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 01 Mar 2022 02:04:57 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 01 Mar 2022 02:04:57 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 01 Mar 2022 02:04:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Mar 2022 02:04:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfc7f9e90e738f44b615eb913a41ca3c06f9e9f644aa8ae7367108a487a4013`  
		Last Modified: Tue, 01 Mar 2022 02:06:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36ed7bb130b98d5b3941286a3b18e66106de11ab8fba756aefee5972065bd2f`  
		Last Modified: Tue, 01 Mar 2022 02:06:14 GMT  
		Size: 36.7 MB (36683502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545729e55c0df18e4995e742baa7a802e73eeca61e14358d588769aad6749a0a`  
		Last Modified: Tue, 01 Mar 2022 02:06:07 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0598812672afaa386e0f3fb63af60ed9158615d9c828f0d21641df8d4c516b29`  
		Last Modified: Tue, 01 Mar 2022 02:06:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9c5062862aa77b9344e5a9cd395108ff566cd5cad5bf0d6f80d6f26cdd31a0`  
		Last Modified: Tue, 01 Mar 2022 02:06:07 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
