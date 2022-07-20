<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10`](#consul110)
-	[`consul:1.10.12`](#consul11012)
-	[`consul:1.11`](#consul111)
-	[`consul:1.11.7`](#consul1117)
-	[`consul:1.12`](#consul112)
-	[`consul:1.12.3`](#consul1123)
-	[`consul:latest`](#consullatest)

## `consul:1.10`

```console
$ docker pull consul@sha256:e1d3274ee8719cd4c122120e5cf6221c645334fa8e8cc38026a7b1ead3773120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10` - linux; amd64

```console
$ docker pull consul@sha256:6618a0f208dfc354f1d46974863a6d8040b5ef9060409c84c29a3a9536ba81ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43256110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc64d3b33abe966f1b05cade32f3799840a349e09892e1527706ecbb1cdf430f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:15:08 GMT
ARG CONSUL_VERSION=1.10.12
# Tue, 19 Jul 2022 23:15:08 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.12 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:15:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:15:09 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:15:16 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:15:16 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:15:17 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:15:17 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:15:17 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:15:17 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:15:17 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:15:17 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:15:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:15:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b644202902603dfc373f9a10b977ce3fafba47632fdc86e4cb46299ed57aa07`  
		Last Modified: Tue, 19 Jul 2022 23:16:03 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38822c7c24b1026fea688d6c82b9a78ec90aa1eaa12642a6ad771c3351d809e`  
		Last Modified: Tue, 19 Jul 2022 23:16:08 GMT  
		Size: 40.4 MB (40438084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbff5d3b5f204acb2768ecb28cb570b02b9884a579a4bba3994fdd94dab9dd8`  
		Last Modified: Tue, 19 Jul 2022 23:16:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b77335085ab4739a9566b1489cd8dc61620fd571a265d56e68b44bdac498cf`  
		Last Modified: Tue, 19 Jul 2022 23:16:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c186e1e2e6176c0bdf86dfa12b11dbb1947e72368935155c670e6e6893e1bd4`  
		Last Modified: Tue, 19 Jul 2022 23:16:03 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:e12de290a1e9cef640e8f92106c3d1b4651c5d3df27802138f8533a12baa157e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41044283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec60a8e828ec2812e7d4383734ecce6f623d4741f7aae07d1109b67d328263e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:47:01 GMT
ARG CONSUL_VERSION=1.10.12
# Tue, 19 Jul 2022 23:47:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.12 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:47:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:47:03 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:47:15 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:47:17 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:47:18 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:47:19 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:47:19 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:47:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:47:20 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:47:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:47:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f5c90d19bcd1beb919f9ded0fed9dae650a8868f45f08c1476dc7fe9ddea20`  
		Last Modified: Tue, 19 Jul 2022 23:49:18 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5bbca6c21cb6afb1292c932d06beb09a8ce6c1a1eca18240efdaff3b0cbce8`  
		Last Modified: Tue, 19 Jul 2022 23:49:40 GMT  
		Size: 38.4 MB (38418503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36619b584afb779893a5ccd3e65a65e44cfe3a452bf9325a7d3dee6149d2e6`  
		Last Modified: Tue, 19 Jul 2022 23:49:18 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db482b0c08618177abd0a50325b2b8d3c5d75aafb90bdb982437dc2135d69c2`  
		Last Modified: Tue, 19 Jul 2022 23:49:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a60dacc7e1b8672735fa1031ef76aebc6172eb18455f192e94b9cf381e96eef`  
		Last Modified: Tue, 19 Jul 2022 23:49:18 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b0220f5c3e6fb65d74aad58eae41c59c4bf7ce2192ea96ed640f9c7ed2224e7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40903187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b39a43668594bf213f27bb2f47f0738d6b4d5bc4eebb01463d01bfe91657f6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:02:37 GMT
ARG CONSUL_VERSION=1.10.12
# Wed, 20 Jul 2022 04:02:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.12 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 20 Jul 2022 04:02:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 20 Jul 2022 04:02:40 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 20 Jul 2022 04:02:46 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 20 Jul 2022 04:02:47 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 20 Jul 2022 04:02:48 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 20 Jul 2022 04:02:49 GMT
VOLUME [/consul/data]
# Wed, 20 Jul 2022 04:02:50 GMT
EXPOSE 8300
# Wed, 20 Jul 2022 04:02:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 20 Jul 2022 04:02:52 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 20 Jul 2022 04:02:54 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 04:02:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:02:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177d2d4fb07a72a1a37fad4b8c4a9e04bb3322dd742b7c353ce6e5101ff55f00`  
		Last Modified: Wed, 20 Jul 2022 04:03:51 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f1b044e3374158d10762f931a170b3caf8a5590b42b6f84df1479e4133d684`  
		Last Modified: Wed, 20 Jul 2022 04:03:57 GMT  
		Size: 38.2 MB (38182982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f25593f0a9dfbab824783104c5ee1aef96490d461e7834c95601f5c5aa81c6`  
		Last Modified: Wed, 20 Jul 2022 04:03:51 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62379f05d95c063f71b1d072d1c0de98f9a0125ec3a48df76c7c048a67390909`  
		Last Modified: Wed, 20 Jul 2022 04:03:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839ad9eb140feea7b592d2f315862286d249214fdbdf1e0ad3e31c4a08cb283b`  
		Last Modified: Wed, 20 Jul 2022 04:03:51 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; 386

```console
$ docker pull consul@sha256:4dd6d2717cfe35e6e42aff6ac0a3d979d74430561251962cbf62868fe8bdf3da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42095365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e64638a479631336bd242718e403c91dd798547f4a34313f14f59c93d65da8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:32 GMT
ADD file:3c11e12b5c10a13cce2dec1d5ae8d7c6a61e0ccc2b4b44b6cf5b80b97eed9869 in / 
# Tue, 19 Jul 2022 22:38:32 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:17:22 GMT
ARG CONSUL_VERSION=1.10.12
# Tue, 19 Jul 2022 23:17:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.12 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:17:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:17:25 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:17:31 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:17:31 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:17:32 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:17:33 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:17:34 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:17:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:17:36 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:17:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:17:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:17:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8bbe360ea5d414165050aeceb6ca82ed372606830e0addd5df0d1000146ab250`  
		Last Modified: Tue, 19 Jul 2022 22:39:24 GMT  
		Size: 2.8 MB (2819359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63a24266611848dbe3cce7a555f4b7fc0f06b0c4f2ed29d0de7f7606887e424`  
		Last Modified: Tue, 19 Jul 2022 23:18:42 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19ea0719431f52a06d3df655e9f92768c46067086b587cb0c3cd77fb5dc5cd`  
		Last Modified: Tue, 19 Jul 2022 23:18:47 GMT  
		Size: 39.3 MB (39272685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b030632c52a4ecc217b338c45eecc0dd950d459f788d719386637be5795f014b`  
		Last Modified: Tue, 19 Jul 2022 23:18:42 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53499bc08abc97e6c914cbb9b4ac76b2723b76a39b463d384c3f7ab684f0b244`  
		Last Modified: Tue, 19 Jul 2022 23:18:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9da9ac5bc3c64ea756554f91b6f9fa58dc9195688da327253a43d7b8ee784e`  
		Last Modified: Tue, 19 Jul 2022 23:18:42 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.12`

```console
$ docker pull consul@sha256:e1d3274ee8719cd4c122120e5cf6221c645334fa8e8cc38026a7b1ead3773120
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.12` - linux; amd64

```console
$ docker pull consul@sha256:6618a0f208dfc354f1d46974863a6d8040b5ef9060409c84c29a3a9536ba81ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.3 MB (43256110 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc64d3b33abe966f1b05cade32f3799840a349e09892e1527706ecbb1cdf430f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:15:08 GMT
ARG CONSUL_VERSION=1.10.12
# Tue, 19 Jul 2022 23:15:08 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.12 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:15:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:15:09 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:15:16 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:15:16 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:15:17 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:15:17 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:15:17 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:15:17 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:15:17 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:15:17 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:15:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:15:18 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b644202902603dfc373f9a10b977ce3fafba47632fdc86e4cb46299ed57aa07`  
		Last Modified: Tue, 19 Jul 2022 23:16:03 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38822c7c24b1026fea688d6c82b9a78ec90aa1eaa12642a6ad771c3351d809e`  
		Last Modified: Tue, 19 Jul 2022 23:16:08 GMT  
		Size: 40.4 MB (40438084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbff5d3b5f204acb2768ecb28cb570b02b9884a579a4bba3994fdd94dab9dd8`  
		Last Modified: Tue, 19 Jul 2022 23:16:03 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b77335085ab4739a9566b1489cd8dc61620fd571a265d56e68b44bdac498cf`  
		Last Modified: Tue, 19 Jul 2022 23:16:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c186e1e2e6176c0bdf86dfa12b11dbb1947e72368935155c670e6e6893e1bd4`  
		Last Modified: Tue, 19 Jul 2022 23:16:03 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.12` - linux; arm variant v6

```console
$ docker pull consul@sha256:e12de290a1e9cef640e8f92106c3d1b4651c5d3df27802138f8533a12baa157e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41044283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ec60a8e828ec2812e7d4383734ecce6f623d4741f7aae07d1109b67d328263e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:47:01 GMT
ARG CONSUL_VERSION=1.10.12
# Tue, 19 Jul 2022 23:47:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.12 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:47:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:47:03 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:47:15 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:47:17 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:47:18 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:47:19 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:47:19 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:47:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:47:20 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:47:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:47:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:47:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f5c90d19bcd1beb919f9ded0fed9dae650a8868f45f08c1476dc7fe9ddea20`  
		Last Modified: Tue, 19 Jul 2022 23:49:18 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5bbca6c21cb6afb1292c932d06beb09a8ce6c1a1eca18240efdaff3b0cbce8`  
		Last Modified: Tue, 19 Jul 2022 23:49:40 GMT  
		Size: 38.4 MB (38418503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36619b584afb779893a5ccd3e65a65e44cfe3a452bf9325a7d3dee6149d2e6`  
		Last Modified: Tue, 19 Jul 2022 23:49:18 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db482b0c08618177abd0a50325b2b8d3c5d75aafb90bdb982437dc2135d69c2`  
		Last Modified: Tue, 19 Jul 2022 23:49:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a60dacc7e1b8672735fa1031ef76aebc6172eb18455f192e94b9cf381e96eef`  
		Last Modified: Tue, 19 Jul 2022 23:49:18 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.12` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b0220f5c3e6fb65d74aad58eae41c59c4bf7ce2192ea96ed640f9c7ed2224e7f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40903187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b39a43668594bf213f27bb2f47f0738d6b4d5bc4eebb01463d01bfe91657f6f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:02:37 GMT
ARG CONSUL_VERSION=1.10.12
# Wed, 20 Jul 2022 04:02:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.12 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 20 Jul 2022 04:02:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 20 Jul 2022 04:02:40 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 20 Jul 2022 04:02:46 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 20 Jul 2022 04:02:47 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 20 Jul 2022 04:02:48 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 20 Jul 2022 04:02:49 GMT
VOLUME [/consul/data]
# Wed, 20 Jul 2022 04:02:50 GMT
EXPOSE 8300
# Wed, 20 Jul 2022 04:02:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 20 Jul 2022 04:02:52 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 20 Jul 2022 04:02:54 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 04:02:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:02:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177d2d4fb07a72a1a37fad4b8c4a9e04bb3322dd742b7c353ce6e5101ff55f00`  
		Last Modified: Wed, 20 Jul 2022 04:03:51 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f1b044e3374158d10762f931a170b3caf8a5590b42b6f84df1479e4133d684`  
		Last Modified: Wed, 20 Jul 2022 04:03:57 GMT  
		Size: 38.2 MB (38182982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2f25593f0a9dfbab824783104c5ee1aef96490d461e7834c95601f5c5aa81c6`  
		Last Modified: Wed, 20 Jul 2022 04:03:51 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62379f05d95c063f71b1d072d1c0de98f9a0125ec3a48df76c7c048a67390909`  
		Last Modified: Wed, 20 Jul 2022 04:03:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839ad9eb140feea7b592d2f315862286d249214fdbdf1e0ad3e31c4a08cb283b`  
		Last Modified: Wed, 20 Jul 2022 04:03:51 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.12` - linux; 386

```console
$ docker pull consul@sha256:4dd6d2717cfe35e6e42aff6ac0a3d979d74430561251962cbf62868fe8bdf3da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42095365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e64638a479631336bd242718e403c91dd798547f4a34313f14f59c93d65da8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:32 GMT
ADD file:3c11e12b5c10a13cce2dec1d5ae8d7c6a61e0ccc2b4b44b6cf5b80b97eed9869 in / 
# Tue, 19 Jul 2022 22:38:32 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:17:22 GMT
ARG CONSUL_VERSION=1.10.12
# Tue, 19 Jul 2022 23:17:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.12 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:17:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:17:25 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:17:31 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:17:31 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:17:32 GMT
# ARGS: CONSUL_VERSION=1.10.12
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:17:33 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:17:34 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:17:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:17:36 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:17:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:17:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:17:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8bbe360ea5d414165050aeceb6ca82ed372606830e0addd5df0d1000146ab250`  
		Last Modified: Tue, 19 Jul 2022 22:39:24 GMT  
		Size: 2.8 MB (2819359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63a24266611848dbe3cce7a555f4b7fc0f06b0c4f2ed29d0de7f7606887e424`  
		Last Modified: Tue, 19 Jul 2022 23:18:42 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a19ea0719431f52a06d3df655e9f92768c46067086b587cb0c3cd77fb5dc5cd`  
		Last Modified: Tue, 19 Jul 2022 23:18:47 GMT  
		Size: 39.3 MB (39272685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b030632c52a4ecc217b338c45eecc0dd950d459f788d719386637be5795f014b`  
		Last Modified: Tue, 19 Jul 2022 23:18:42 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53499bc08abc97e6c914cbb9b4ac76b2723b76a39b463d384c3f7ab684f0b244`  
		Last Modified: Tue, 19 Jul 2022 23:18:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9da9ac5bc3c64ea756554f91b6f9fa58dc9195688da327253a43d7b8ee784e`  
		Last Modified: Tue, 19 Jul 2022 23:18:42 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11`

```console
$ docker pull consul@sha256:701b8089e3abcf4dfa951711da2e498e715c68b8ed17d898c1aec8c851b13c9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11` - linux; amd64

```console
$ docker pull consul@sha256:0040ba1078ae1c1043813b56e512a67ad50ced25a23bf88d6aafc241c3ecb106
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43997595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ed81a7588e459112162c2f8ab54858760a2c6753b598577f288a866b012aa1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:14:58 GMT
ARG CONSUL_VERSION=1.11.7
# Tue, 19 Jul 2022 23:14:58 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:14:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:14:59 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:15:04 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:15:05 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:15:05 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:15:06 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:15:06 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:15:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:15:06 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:15:06 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:15:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:15:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f47fa60f76b0ed0e2503ebbcd86c0e25cc4383ed1e03a4428c4628865f7ccf0`  
		Last Modified: Tue, 19 Jul 2022 23:15:48 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3a39c2426defabd43a148c04403e4fe81145dce318bea8d5c4843fbe557ebe`  
		Last Modified: Tue, 19 Jul 2022 23:15:53 GMT  
		Size: 41.2 MB (41179570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4b413ba90734ba1b3f7d03323b2fe7d77b791c66553940927a91b52bfb8525`  
		Last Modified: Tue, 19 Jul 2022 23:15:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e99bc63b7d8cb6aad6a13bfd694d0fde9b26c837795d35b41dc50487009ab6c`  
		Last Modified: Tue, 19 Jul 2022 23:15:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4910b92562ba340723fe89c6e8bf88e2a0b71dba7590d65bead06cbce19b89d`  
		Last Modified: Tue, 19 Jul 2022 23:15:48 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:f0cae092bcf92b68e22871b246cfbca5a16ef1b5277af1fd77710600d50026c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41741832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d69760748c7df5c497f0ee52cb6b1447138f480983c89a35a54d7fda824c88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:46:28 GMT
ARG CONSUL_VERSION=1.11.7
# Tue, 19 Jul 2022 23:46:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:46:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:46:30 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:46:42 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:46:44 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:46:45 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:46:46 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:46:46 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:46:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:46:47 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:46:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:46:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:46:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f8b3cff6b071cb08eb988720e59dfc9f2fc27b4f5c6720d4536b48da4a2550`  
		Last Modified: Tue, 19 Jul 2022 23:48:45 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506397c2f0d2450ffc67df21070b87cea92782fba961f9eeea47496348b39663`  
		Last Modified: Tue, 19 Jul 2022 23:49:06 GMT  
		Size: 39.1 MB (39116056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85719a5b0cd0271f657d08ff20d7a64a3fd23fb9c7bf38a6708efc28f4ee7fd6`  
		Last Modified: Tue, 19 Jul 2022 23:48:45 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14755564085e1f1f968feac5f0058b12f8df18766785987644c5da62d36a7350`  
		Last Modified: Tue, 19 Jul 2022 23:48:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207bf00c098751265f647b546c9f6073f6fd2b2b7c00abf029c817a7835acdd9`  
		Last Modified: Tue, 19 Jul 2022 23:48:45 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:16dc819e009e92bdce93a36acdb43c4217e0176ad1d1d2fdc7ca695219ce7c35
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41568964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0eb66ed6f7595f1caccf1cec90a21f0c9f6d55a4123a59cdfb83a8f05be5923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:02:15 GMT
ARG CONSUL_VERSION=1.11.7
# Wed, 20 Jul 2022 04:02:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 20 Jul 2022 04:02:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 20 Jul 2022 04:02:18 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 20 Jul 2022 04:02:24 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 20 Jul 2022 04:02:24 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 20 Jul 2022 04:02:25 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 20 Jul 2022 04:02:26 GMT
VOLUME [/consul/data]
# Wed, 20 Jul 2022 04:02:27 GMT
EXPOSE 8300
# Wed, 20 Jul 2022 04:02:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 20 Jul 2022 04:02:29 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 20 Jul 2022 04:02:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 04:02:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:02:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda2b0a1e7bdfda03762d43d54d9975cfebd071325d8187ee578835ad9d9fdd1`  
		Last Modified: Wed, 20 Jul 2022 04:03:35 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084c3196206618f2e6d73a849655b9d15059539cb9721d43d53eeb09fe6319ad`  
		Last Modified: Wed, 20 Jul 2022 04:03:41 GMT  
		Size: 38.8 MB (38848756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6aed7d6ddba8fa2e7f91ab442d8ef1f3abce6583e941025c719067d452534d`  
		Last Modified: Wed, 20 Jul 2022 04:03:35 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6198e6fc50c8f1b7c7a24d68bb20cfd805ba6765610619ba16b13b422940423e`  
		Last Modified: Wed, 20 Jul 2022 04:03:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1614a731d749d7a16216b8525f3d9745c6ef53ba2f98bcd951944a340a1ff8d2`  
		Last Modified: Wed, 20 Jul 2022 04:03:35 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; 386

```console
$ docker pull consul@sha256:ff8f76b96e7e515f91a0b94e4a76c69883e0c56b6475f33aaaec5c76c5a101f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42808131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2cd7f2bf214282cb8421e3724a363e1ff66829aaf832792ef4eb342561734b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:32 GMT
ADD file:3c11e12b5c10a13cce2dec1d5ae8d7c6a61e0ccc2b4b44b6cf5b80b97eed9869 in / 
# Tue, 19 Jul 2022 22:38:32 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:17:00 GMT
ARG CONSUL_VERSION=1.11.7
# Tue, 19 Jul 2022 23:17:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:17:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:17:03 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:17:09 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:17:09 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:17:10 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:17:11 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:17:12 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:17:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:17:14 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:17:16 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:17:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:17:17 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8bbe360ea5d414165050aeceb6ca82ed372606830e0addd5df0d1000146ab250`  
		Last Modified: Tue, 19 Jul 2022 22:39:24 GMT  
		Size: 2.8 MB (2819359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9002f9f1fbf474eb0f48d60fe0da990d01cda513bc7bc0debc05c8a52d8ecee`  
		Last Modified: Tue, 19 Jul 2022 23:18:21 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ac4a71497b9860de979cf984ed4afb8d4dfe3b2c01acceaeb284b1103a1786`  
		Last Modified: Tue, 19 Jul 2022 23:18:26 GMT  
		Size: 40.0 MB (39985454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5c441a0083de5786111c373be42eabf8f614a22b3ac829d72d9c9394a37237`  
		Last Modified: Tue, 19 Jul 2022 23:18:21 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68055116f558619c33ce35a89ec37335d62cd0528415b0f2f8b15b30037482f`  
		Last Modified: Tue, 19 Jul 2022 23:18:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c532b56c35fc9723be07bc0527d7bfbf906022b6e9680d5c9e2965765dedfaa`  
		Last Modified: Tue, 19 Jul 2022 23:18:22 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.7`

```console
$ docker pull consul@sha256:701b8089e3abcf4dfa951711da2e498e715c68b8ed17d898c1aec8c851b13c9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.7` - linux; amd64

```console
$ docker pull consul@sha256:0040ba1078ae1c1043813b56e512a67ad50ced25a23bf88d6aafc241c3ecb106
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43997595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ed81a7588e459112162c2f8ab54858760a2c6753b598577f288a866b012aa1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:14:58 GMT
ARG CONSUL_VERSION=1.11.7
# Tue, 19 Jul 2022 23:14:58 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:14:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:14:59 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:15:04 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:15:05 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:15:05 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:15:06 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:15:06 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:15:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:15:06 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:15:06 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:15:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:15:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f47fa60f76b0ed0e2503ebbcd86c0e25cc4383ed1e03a4428c4628865f7ccf0`  
		Last Modified: Tue, 19 Jul 2022 23:15:48 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3a39c2426defabd43a148c04403e4fe81145dce318bea8d5c4843fbe557ebe`  
		Last Modified: Tue, 19 Jul 2022 23:15:53 GMT  
		Size: 41.2 MB (41179570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4b413ba90734ba1b3f7d03323b2fe7d77b791c66553940927a91b52bfb8525`  
		Last Modified: Tue, 19 Jul 2022 23:15:48 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e99bc63b7d8cb6aad6a13bfd694d0fde9b26c837795d35b41dc50487009ab6c`  
		Last Modified: Tue, 19 Jul 2022 23:15:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4910b92562ba340723fe89c6e8bf88e2a0b71dba7590d65bead06cbce19b89d`  
		Last Modified: Tue, 19 Jul 2022 23:15:48 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:f0cae092bcf92b68e22871b246cfbca5a16ef1b5277af1fd77710600d50026c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41741832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d69760748c7df5c497f0ee52cb6b1447138f480983c89a35a54d7fda824c88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:46:28 GMT
ARG CONSUL_VERSION=1.11.7
# Tue, 19 Jul 2022 23:46:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:46:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:46:30 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:46:42 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:46:44 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:46:45 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:46:46 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:46:46 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:46:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:46:47 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:46:48 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:46:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:46:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f8b3cff6b071cb08eb988720e59dfc9f2fc27b4f5c6720d4536b48da4a2550`  
		Last Modified: Tue, 19 Jul 2022 23:48:45 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:506397c2f0d2450ffc67df21070b87cea92782fba961f9eeea47496348b39663`  
		Last Modified: Tue, 19 Jul 2022 23:49:06 GMT  
		Size: 39.1 MB (39116056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85719a5b0cd0271f657d08ff20d7a64a3fd23fb9c7bf38a6708efc28f4ee7fd6`  
		Last Modified: Tue, 19 Jul 2022 23:48:45 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14755564085e1f1f968feac5f0058b12f8df18766785987644c5da62d36a7350`  
		Last Modified: Tue, 19 Jul 2022 23:48:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207bf00c098751265f647b546c9f6073f6fd2b2b7c00abf029c817a7835acdd9`  
		Last Modified: Tue, 19 Jul 2022 23:48:45 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:16dc819e009e92bdce93a36acdb43c4217e0176ad1d1d2fdc7ca695219ce7c35
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41568964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0eb66ed6f7595f1caccf1cec90a21f0c9f6d55a4123a59cdfb83a8f05be5923`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:02:15 GMT
ARG CONSUL_VERSION=1.11.7
# Wed, 20 Jul 2022 04:02:16 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 20 Jul 2022 04:02:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 20 Jul 2022 04:02:18 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 20 Jul 2022 04:02:24 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 20 Jul 2022 04:02:24 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 20 Jul 2022 04:02:25 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 20 Jul 2022 04:02:26 GMT
VOLUME [/consul/data]
# Wed, 20 Jul 2022 04:02:27 GMT
EXPOSE 8300
# Wed, 20 Jul 2022 04:02:28 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 20 Jul 2022 04:02:29 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 20 Jul 2022 04:02:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 04:02:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:02:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda2b0a1e7bdfda03762d43d54d9975cfebd071325d8187ee578835ad9d9fdd1`  
		Last Modified: Wed, 20 Jul 2022 04:03:35 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084c3196206618f2e6d73a849655b9d15059539cb9721d43d53eeb09fe6319ad`  
		Last Modified: Wed, 20 Jul 2022 04:03:41 GMT  
		Size: 38.8 MB (38848756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6aed7d6ddba8fa2e7f91ab442d8ef1f3abce6583e941025c719067d452534d`  
		Last Modified: Wed, 20 Jul 2022 04:03:35 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6198e6fc50c8f1b7c7a24d68bb20cfd805ba6765610619ba16b13b422940423e`  
		Last Modified: Wed, 20 Jul 2022 04:03:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1614a731d749d7a16216b8525f3d9745c6ef53ba2f98bcd951944a340a1ff8d2`  
		Last Modified: Wed, 20 Jul 2022 04:03:35 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.7` - linux; 386

```console
$ docker pull consul@sha256:ff8f76b96e7e515f91a0b94e4a76c69883e0c56b6475f33aaaec5c76c5a101f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42808131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2cd7f2bf214282cb8421e3724a363e1ff66829aaf832792ef4eb342561734b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:32 GMT
ADD file:3c11e12b5c10a13cce2dec1d5ae8d7c6a61e0ccc2b4b44b6cf5b80b97eed9869 in / 
# Tue, 19 Jul 2022 22:38:32 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:17:00 GMT
ARG CONSUL_VERSION=1.11.7
# Tue, 19 Jul 2022 23:17:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:17:02 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:17:03 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:17:09 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:17:09 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:17:10 GMT
# ARGS: CONSUL_VERSION=1.11.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:17:11 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:17:12 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:17:13 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:17:14 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:17:16 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:17:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:17:17 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8bbe360ea5d414165050aeceb6ca82ed372606830e0addd5df0d1000146ab250`  
		Last Modified: Tue, 19 Jul 2022 22:39:24 GMT  
		Size: 2.8 MB (2819359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9002f9f1fbf474eb0f48d60fe0da990d01cda513bc7bc0debc05c8a52d8ecee`  
		Last Modified: Tue, 19 Jul 2022 23:18:21 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4ac4a71497b9860de979cf984ed4afb8d4dfe3b2c01acceaeb284b1103a1786`  
		Last Modified: Tue, 19 Jul 2022 23:18:26 GMT  
		Size: 40.0 MB (39985454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5c441a0083de5786111c373be42eabf8f614a22b3ac829d72d9c9394a37237`  
		Last Modified: Tue, 19 Jul 2022 23:18:21 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68055116f558619c33ce35a89ec37335d62cd0528415b0f2f8b15b30037482f`  
		Last Modified: Tue, 19 Jul 2022 23:18:21 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c532b56c35fc9723be07bc0527d7bfbf906022b6e9680d5c9e2965765dedfaa`  
		Last Modified: Tue, 19 Jul 2022 23:18:22 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12`

```console
$ docker pull consul@sha256:1eba67d894cf99b7f94841e2101bf171248a16eb3ffb58796d0c6466ad662e65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.12` - linux; amd64

```console
$ docker pull consul@sha256:04cac9616c328dec0f3e1c6cb1ed13fbd518a1f848eadd907edfd042bece7992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49564205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7485ac1fda8bf8e50a858037d876fa230cfb9dc3b93b3232796f36e36962c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:14:47 GMT
ARG CONSUL_VERSION=1.12.3
# Tue, 19 Jul 2022 23:14:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:14:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:14:48 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:14:53 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:14:54 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:14:54 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:14:54 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:14:54 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:14:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:14:55 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:14:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:14:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:14:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a253579e1e59b7cc3cee072b49e3a7c312b48b61763cce724493e736bbece12`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfd4a7c41494d134fecdc1a5d495689691a8d3c687cc53ac42e010cb05f24ef`  
		Last Modified: Tue, 19 Jul 2022 23:15:36 GMT  
		Size: 46.7 MB (46746182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ecf178907ccb462e69d1631f31edd76b1c888f24fe3ec78c1bab8edb95a1ee`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee0b34385e5df501c1cb126fa8165030f9585511e43697069f7ddab176811f7`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5947a04e293d7b72de31fedee98476630a951c9b16fa506d289aa860bf626d1`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm variant v6

```console
$ docker pull consul@sha256:bb3cc7e3cc3c1f3c7565b6c94ff22ffa69603aeff8b8eddb685c8178f4c8e8fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47427278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815489d9085f0ccc5a0b2b1b6243235c19a9d3049c2f6fd309afda8041b1983e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:45:54 GMT
ARG CONSUL_VERSION=1.12.3
# Tue, 19 Jul 2022 23:45:55 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:45:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:45:57 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:46:09 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:46:11 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:46:13 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:46:13 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:46:14 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:46:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:46:14 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:46:15 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:46:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93258a5148743001561f014c268829757e11faaa1c20c2bcfd2f1e8277d86f07`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11e9bb44946f0ebd955aa680d466ce7126bb222f152d01e613f355399685fb6`  
		Last Modified: Tue, 19 Jul 2022 23:48:29 GMT  
		Size: 44.8 MB (44801502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4aabde443f1f67e8019f6acf1311bf794c06d63123b2137e566a84b8fba003`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162ac20183d15cfb72bdf7ac373ccc9223a63cb05c72f658612c7c62f4be73b0`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a847450062330577921bbf8edb3670a8ab9dd04b55a8a0a3d30731738b82b9`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:ba1e465aa469d5bb98992b5c7b40ea6a9b24cb72fe021231e042afbe213f9bd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47167602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d6743dd0c3a7918d8359dfb23ff48af25caec0ef898e91e62a4bdb44cc89741`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:01:49 GMT
ARG CONSUL_VERSION=1.12.3
# Wed, 20 Jul 2022 04:01:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 20 Jul 2022 04:01:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 20 Jul 2022 04:01:52 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 20 Jul 2022 04:01:59 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 20 Jul 2022 04:01:59 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 20 Jul 2022 04:02:00 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 20 Jul 2022 04:02:01 GMT
VOLUME [/consul/data]
# Wed, 20 Jul 2022 04:02:02 GMT
EXPOSE 8300
# Wed, 20 Jul 2022 04:02:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 20 Jul 2022 04:02:04 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 20 Jul 2022 04:02:06 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 04:02:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:02:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5299ba82f3beddc13a0202137d71342580f28391d53149776d47f42144c0b4`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e824b365c650f2d88df6689b7a02f6d8b413b4751c5a3b35f6db6ddb89c92c`  
		Last Modified: Wed, 20 Jul 2022 04:03:22 GMT  
		Size: 44.4 MB (44447396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fe381d39b8e88ed1c430bbaec1bc7845b014ff40a9baafcef160e18907f35c`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460ca9cdad31eeb55f6071fecf3a4deb282674e514fc3734544a145804053b`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca6c3e04b869ae2c5fbd44bfce1e0c328d5da78ad333531a3ce1341679cb761`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; 386

```console
$ docker pull consul@sha256:13bb70d0f28088ffd7d9c2213a6ac837d6a266e85915f798985ce293ef714e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48626855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca0ed72dbe6de5fc88a0a55f6db2753668a2564241110f5b1cf1f8e4fece80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:32 GMT
ADD file:3c11e12b5c10a13cce2dec1d5ae8d7c6a61e0ccc2b4b44b6cf5b80b97eed9869 in / 
# Tue, 19 Jul 2022 22:38:32 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:16:34 GMT
ARG CONSUL_VERSION=1.12.3
# Tue, 19 Jul 2022 23:16:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:16:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:16:37 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:16:44 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:16:45 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:16:46 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:16:47 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:16:48 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:16:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:16:50 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:16:52 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:16:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:16:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8bbe360ea5d414165050aeceb6ca82ed372606830e0addd5df0d1000146ab250`  
		Last Modified: Tue, 19 Jul 2022 22:39:24 GMT  
		Size: 2.8 MB (2819359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86b208735cf7f0a6685c0bf13803bb5f293292ab84582f891ecfe99eb154f2`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a036f0833abd118b1aea7eae0f379f1290c31f3d48938ef74c95d93d174ebc`  
		Last Modified: Tue, 19 Jul 2022 23:18:07 GMT  
		Size: 45.8 MB (45804176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ba49b937ff278f821824d0187f8b9082c2fd3873237c228955c80b5794cbcc`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f72a70e2b2e2eb67b9f1342600c210a37e1e5e399aae79b7457f883a069288f`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7151d8cb9fde221649471d8fd3c6fd91621598b472c3ccb07b8f73cc742a0`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12.3`

```console
$ docker pull consul@sha256:1eba67d894cf99b7f94841e2101bf171248a16eb3ffb58796d0c6466ad662e65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.12.3` - linux; amd64

```console
$ docker pull consul@sha256:04cac9616c328dec0f3e1c6cb1ed13fbd518a1f848eadd907edfd042bece7992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49564205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7485ac1fda8bf8e50a858037d876fa230cfb9dc3b93b3232796f36e36962c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:14:47 GMT
ARG CONSUL_VERSION=1.12.3
# Tue, 19 Jul 2022 23:14:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:14:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:14:48 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:14:53 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:14:54 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:14:54 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:14:54 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:14:54 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:14:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:14:55 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:14:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:14:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:14:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a253579e1e59b7cc3cee072b49e3a7c312b48b61763cce724493e736bbece12`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfd4a7c41494d134fecdc1a5d495689691a8d3c687cc53ac42e010cb05f24ef`  
		Last Modified: Tue, 19 Jul 2022 23:15:36 GMT  
		Size: 46.7 MB (46746182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ecf178907ccb462e69d1631f31edd76b1c888f24fe3ec78c1bab8edb95a1ee`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee0b34385e5df501c1cb126fa8165030f9585511e43697069f7ddab176811f7`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5947a04e293d7b72de31fedee98476630a951c9b16fa506d289aa860bf626d1`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.3` - linux; arm variant v6

```console
$ docker pull consul@sha256:bb3cc7e3cc3c1f3c7565b6c94ff22ffa69603aeff8b8eddb685c8178f4c8e8fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47427278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815489d9085f0ccc5a0b2b1b6243235c19a9d3049c2f6fd309afda8041b1983e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:45:54 GMT
ARG CONSUL_VERSION=1.12.3
# Tue, 19 Jul 2022 23:45:55 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:45:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:45:57 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:46:09 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:46:11 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:46:13 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:46:13 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:46:14 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:46:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:46:14 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:46:15 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:46:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93258a5148743001561f014c268829757e11faaa1c20c2bcfd2f1e8277d86f07`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11e9bb44946f0ebd955aa680d466ce7126bb222f152d01e613f355399685fb6`  
		Last Modified: Tue, 19 Jul 2022 23:48:29 GMT  
		Size: 44.8 MB (44801502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4aabde443f1f67e8019f6acf1311bf794c06d63123b2137e566a84b8fba003`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162ac20183d15cfb72bdf7ac373ccc9223a63cb05c72f658612c7c62f4be73b0`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a847450062330577921bbf8edb3670a8ab9dd04b55a8a0a3d30731738b82b9`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.3` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:ba1e465aa469d5bb98992b5c7b40ea6a9b24cb72fe021231e042afbe213f9bd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47167602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d6743dd0c3a7918d8359dfb23ff48af25caec0ef898e91e62a4bdb44cc89741`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:01:49 GMT
ARG CONSUL_VERSION=1.12.3
# Wed, 20 Jul 2022 04:01:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 20 Jul 2022 04:01:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 20 Jul 2022 04:01:52 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 20 Jul 2022 04:01:59 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 20 Jul 2022 04:01:59 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 20 Jul 2022 04:02:00 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 20 Jul 2022 04:02:01 GMT
VOLUME [/consul/data]
# Wed, 20 Jul 2022 04:02:02 GMT
EXPOSE 8300
# Wed, 20 Jul 2022 04:02:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 20 Jul 2022 04:02:04 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 20 Jul 2022 04:02:06 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 04:02:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:02:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5299ba82f3beddc13a0202137d71342580f28391d53149776d47f42144c0b4`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e824b365c650f2d88df6689b7a02f6d8b413b4751c5a3b35f6db6ddb89c92c`  
		Last Modified: Wed, 20 Jul 2022 04:03:22 GMT  
		Size: 44.4 MB (44447396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fe381d39b8e88ed1c430bbaec1bc7845b014ff40a9baafcef160e18907f35c`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460ca9cdad31eeb55f6071fecf3a4deb282674e514fc3734544a145804053b`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca6c3e04b869ae2c5fbd44bfce1e0c328d5da78ad333531a3ce1341679cb761`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.3` - linux; 386

```console
$ docker pull consul@sha256:13bb70d0f28088ffd7d9c2213a6ac837d6a266e85915f798985ce293ef714e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48626855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca0ed72dbe6de5fc88a0a55f6db2753668a2564241110f5b1cf1f8e4fece80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:32 GMT
ADD file:3c11e12b5c10a13cce2dec1d5ae8d7c6a61e0ccc2b4b44b6cf5b80b97eed9869 in / 
# Tue, 19 Jul 2022 22:38:32 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:16:34 GMT
ARG CONSUL_VERSION=1.12.3
# Tue, 19 Jul 2022 23:16:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:16:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:16:37 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:16:44 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:16:45 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:16:46 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:16:47 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:16:48 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:16:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:16:50 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:16:52 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:16:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:16:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8bbe360ea5d414165050aeceb6ca82ed372606830e0addd5df0d1000146ab250`  
		Last Modified: Tue, 19 Jul 2022 22:39:24 GMT  
		Size: 2.8 MB (2819359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86b208735cf7f0a6685c0bf13803bb5f293292ab84582f891ecfe99eb154f2`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a036f0833abd118b1aea7eae0f379f1290c31f3d48938ef74c95d93d174ebc`  
		Last Modified: Tue, 19 Jul 2022 23:18:07 GMT  
		Size: 45.8 MB (45804176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ba49b937ff278f821824d0187f8b9082c2fd3873237c228955c80b5794cbcc`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f72a70e2b2e2eb67b9f1342600c210a37e1e5e399aae79b7457f883a069288f`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7151d8cb9fde221649471d8fd3c6fd91621598b472c3ccb07b8f73cc742a0`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:1eba67d894cf99b7f94841e2101bf171248a16eb3ffb58796d0c6466ad662e65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:04cac9616c328dec0f3e1c6cb1ed13fbd518a1f848eadd907edfd042bece7992
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49564205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7485ac1fda8bf8e50a858037d876fa230cfb9dc3b93b3232796f36e36962c60`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:14:47 GMT
ARG CONSUL_VERSION=1.12.3
# Tue, 19 Jul 2022 23:14:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:14:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:14:48 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:14:53 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:14:54 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:14:54 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:14:54 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:14:54 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:14:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:14:55 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:14:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:14:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:14:55 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a253579e1e59b7cc3cee072b49e3a7c312b48b61763cce724493e736bbece12`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfd4a7c41494d134fecdc1a5d495689691a8d3c687cc53ac42e010cb05f24ef`  
		Last Modified: Tue, 19 Jul 2022 23:15:36 GMT  
		Size: 46.7 MB (46746182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ecf178907ccb462e69d1631f31edd76b1c888f24fe3ec78c1bab8edb95a1ee`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee0b34385e5df501c1cb126fa8165030f9585511e43697069f7ddab176811f7`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5947a04e293d7b72de31fedee98476630a951c9b16fa506d289aa860bf626d1`  
		Last Modified: Tue, 19 Jul 2022 23:15:30 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:bb3cc7e3cc3c1f3c7565b6c94ff22ffa69603aeff8b8eddb685c8178f4c8e8fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47427278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:815489d9085f0ccc5a0b2b1b6243235c19a9d3049c2f6fd309afda8041b1983e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:49:49 GMT
ADD file:4958b5356608921fe85d83047b74d1cb4a53de78c3465039ac4e60a68329da64 in / 
# Tue, 19 Jul 2022 22:49:50 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:45:54 GMT
ARG CONSUL_VERSION=1.12.3
# Tue, 19 Jul 2022 23:45:55 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:45:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:45:57 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:46:09 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:46:11 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:46:13 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:46:13 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:46:14 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:46:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:46:14 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:46:15 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:46:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:46:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fcc62ebebb3542c1aad49c3cc072a98cf619f67e914baba1ea7dfeadcb32cbdd`  
		Last Modified: Tue, 19 Jul 2022 22:51:27 GMT  
		Size: 2.6 MB (2622400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93258a5148743001561f014c268829757e11faaa1c20c2bcfd2f1e8277d86f07`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11e9bb44946f0ebd955aa680d466ce7126bb222f152d01e613f355399685fb6`  
		Last Modified: Tue, 19 Jul 2022 23:48:29 GMT  
		Size: 44.8 MB (44801502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4aabde443f1f67e8019f6acf1311bf794c06d63123b2137e566a84b8fba003`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162ac20183d15cfb72bdf7ac373ccc9223a63cb05c72f658612c7c62f4be73b0`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43a847450062330577921bbf8edb3670a8ab9dd04b55a8a0a3d30731738b82b9`  
		Last Modified: Tue, 19 Jul 2022 23:48:05 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:ba1e465aa469d5bb98992b5c7b40ea6a9b24cb72fe021231e042afbe213f9bd3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47167602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d6743dd0c3a7918d8359dfb23ff48af25caec0ef898e91e62a4bdb44cc89741`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:42 GMT
ADD file:158791ae9b4fb18e208925ce1ac7396322e741030bcd9bcae7e320e83f517dfe in / 
# Tue, 19 Jul 2022 22:39:42 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 04:01:49 GMT
ARG CONSUL_VERSION=1.12.3
# Wed, 20 Jul 2022 04:01:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 20 Jul 2022 04:01:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 20 Jul 2022 04:01:52 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 20 Jul 2022 04:01:59 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 20 Jul 2022 04:01:59 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 20 Jul 2022 04:02:00 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 20 Jul 2022 04:02:01 GMT
VOLUME [/consul/data]
# Wed, 20 Jul 2022 04:02:02 GMT
EXPOSE 8300
# Wed, 20 Jul 2022 04:02:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 20 Jul 2022 04:02:04 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 20 Jul 2022 04:02:06 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 04:02:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 04:02:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e0295fd11fe28fc9d5438734f4d9560cce203f9c2dc12b26e0cfd0c1c02548f7`  
		Last Modified: Tue, 19 Jul 2022 22:40:33 GMT  
		Size: 2.7 MB (2716890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5299ba82f3beddc13a0202137d71342580f28391d53149776d47f42144c0b4`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42e824b365c650f2d88df6689b7a02f6d8b413b4751c5a3b35f6db6ddb89c92c`  
		Last Modified: Wed, 20 Jul 2022 04:03:22 GMT  
		Size: 44.4 MB (44447396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16fe381d39b8e88ed1c430bbaec1bc7845b014ff40a9baafcef160e18907f35c`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a460ca9cdad31eeb55f6071fecf3a4deb282674e514fc3734544a145804053b`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca6c3e04b869ae2c5fbd44bfce1e0c328d5da78ad333531a3ce1341679cb761`  
		Last Modified: Wed, 20 Jul 2022 04:03:16 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:13bb70d0f28088ffd7d9c2213a6ac837d6a266e85915f798985ce293ef714e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48626855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca0ed72dbe6de5fc88a0a55f6db2753668a2564241110f5b1cf1f8e4fece80`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:32 GMT
ADD file:3c11e12b5c10a13cce2dec1d5ae8d7c6a61e0ccc2b4b44b6cf5b80b97eed9869 in / 
# Tue, 19 Jul 2022 22:38:32 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 23:16:34 GMT
ARG CONSUL_VERSION=1.12.3
# Tue, 19 Jul 2022 23:16:35 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 19 Jul 2022 23:16:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 19 Jul 2022 23:16:37 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 19 Jul 2022 23:16:44 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 19 Jul 2022 23:16:45 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 19 Jul 2022 23:16:46 GMT
# ARGS: CONSUL_VERSION=1.12.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 23:16:47 GMT
VOLUME [/consul/data]
# Tue, 19 Jul 2022 23:16:48 GMT
EXPOSE 8300
# Tue, 19 Jul 2022 23:16:49 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 19 Jul 2022 23:16:50 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 19 Jul 2022 23:16:52 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 19 Jul 2022 23:16:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 23:16:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8bbe360ea5d414165050aeceb6ca82ed372606830e0addd5df0d1000146ab250`  
		Last Modified: Tue, 19 Jul 2022 22:39:24 GMT  
		Size: 2.8 MB (2819359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd86b208735cf7f0a6685c0bf13803bb5f293292ab84582f891ecfe99eb154f2`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a036f0833abd118b1aea7eae0f379f1290c31f3d48938ef74c95d93d174ebc`  
		Last Modified: Tue, 19 Jul 2022 23:18:07 GMT  
		Size: 45.8 MB (45804176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ba49b937ff278f821824d0187f8b9082c2fd3873237c228955c80b5794cbcc`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f72a70e2b2e2eb67b9f1342600c210a37e1e5e399aae79b7457f883a069288f`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b7151d8cb9fde221649471d8fd3c6fd91621598b472c3ccb07b8f73cc742a0`  
		Last Modified: Tue, 19 Jul 2022 23:18:02 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
