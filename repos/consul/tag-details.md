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
$ docker pull consul@sha256:5bcf5c40d0ef2436d78e6f321f1e42623a89811bff16f93c726865df7575a4c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10` - linux; amd64

```console
$ docker pull consul@sha256:adb76ff3377420b5a65bbd6ff3ec8907956064b33937cc5da45fe51f3eeaad43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43743993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0728679cc4a9145cf957c7e898c9e6fc46ae5721403a84bb17b9fa6cbe9673b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:02:28 GMT
ARG CONSUL_VERSION=1.10.9
# Sat, 19 Mar 2022 01:02:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 01:02:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 01:02:29 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 01:03:11 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 01:03:12 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 01:03:13 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 01:03:13 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 01:03:14 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 01:03:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 01:03:14 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 01:03:14 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 01:03:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 01:03:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c9f8004307e44304ac225c9e5b8685fdce74948091689d103349629630da81`  
		Last Modified: Sat, 19 Mar 2022 01:04:59 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5796a6c3e94c8df1a0251d0aefacb012fd2c54b56758025d20c68ae02f2eb643`  
		Last Modified: Sat, 19 Mar 2022 01:05:07 GMT  
		Size: 40.9 MB (40923442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f957e926b9033b4493b8fcb2c2cd8165b58f47910aa96fdbd373b45fc82c6c5`  
		Last Modified: Sat, 19 Mar 2022 01:04:59 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68bb941b6b784eaf0ce8528cec546b4043166d0e96776a1f8726258ec7f9340`  
		Last Modified: Sat, 19 Mar 2022 01:04:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c48be417d6351122eaeb21b460f82a95c0d049bf4d906e90f6fec0496171f5b`  
		Last Modified: Sat, 19 Mar 2022 01:04:59 GMT  
		Size: 1.8 KB (1786 bytes)  
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
$ docker pull consul@sha256:f4ddd480e209cc866564f19258d203fd73d1fbef18bf052b9d0010133aa608b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43113410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a80462fd64a899e6e1f40c77b29b01e2a42f39046c6f07e7e772326a9c0eb61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:13:43 GMT
ARG CONSUL_VERSION=1.10.9
# Sat, 19 Mar 2022 03:13:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 03:13:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 03:13:44 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 03:14:29 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 03:14:31 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 03:14:32 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 03:14:32 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 03:14:32 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 03:14:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 03:14:33 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 03:14:33 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 03:14:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 03:14:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8220304101d181855388ef68e024211a606504847bdf574153f924b149c092`  
		Last Modified: Sat, 19 Mar 2022 03:16:33 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f842bfb423c5794c57c1d5fd5f4423d2d416ce387a0276e7f28af6da28ecca7b`  
		Last Modified: Sat, 19 Mar 2022 03:16:42 GMT  
		Size: 40.3 MB (40286417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fba2d45f1d72d6432d7355dc75571447639410302bb873be24d6b9436ebf81`  
		Last Modified: Sat, 19 Mar 2022 03:16:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced6b0459d3e1b2cf28b1d97277530ccc3314b40bed366f545778caaca5fa5c`  
		Last Modified: Sat, 19 Mar 2022 03:16:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939b01b5fc4e55484cb414c74a95d66b2a2df44a525930eb97c4b1d56aa5e6c0`  
		Last Modified: Sat, 19 Mar 2022 03:16:33 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.9`

```console
$ docker pull consul@sha256:5bcf5c40d0ef2436d78e6f321f1e42623a89811bff16f93c726865df7575a4c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.9` - linux; amd64

```console
$ docker pull consul@sha256:adb76ff3377420b5a65bbd6ff3ec8907956064b33937cc5da45fe51f3eeaad43
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43743993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0728679cc4a9145cf957c7e898c9e6fc46ae5721403a84bb17b9fa6cbe9673b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:02:28 GMT
ARG CONSUL_VERSION=1.10.9
# Sat, 19 Mar 2022 01:02:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 01:02:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 01:02:29 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 01:03:11 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 01:03:12 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 01:03:13 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 01:03:13 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 01:03:14 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 01:03:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 01:03:14 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 01:03:14 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 01:03:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 01:03:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c9f8004307e44304ac225c9e5b8685fdce74948091689d103349629630da81`  
		Last Modified: Sat, 19 Mar 2022 01:04:59 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5796a6c3e94c8df1a0251d0aefacb012fd2c54b56758025d20c68ae02f2eb643`  
		Last Modified: Sat, 19 Mar 2022 01:05:07 GMT  
		Size: 40.9 MB (40923442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f957e926b9033b4493b8fcb2c2cd8165b58f47910aa96fdbd373b45fc82c6c5`  
		Last Modified: Sat, 19 Mar 2022 01:04:59 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b68bb941b6b784eaf0ce8528cec546b4043166d0e96776a1f8726258ec7f9340`  
		Last Modified: Sat, 19 Mar 2022 01:04:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c48be417d6351122eaeb21b460f82a95c0d049bf4d906e90f6fec0496171f5b`  
		Last Modified: Sat, 19 Mar 2022 01:04:59 GMT  
		Size: 1.8 KB (1786 bytes)  
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
$ docker pull consul@sha256:f4ddd480e209cc866564f19258d203fd73d1fbef18bf052b9d0010133aa608b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43113410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a80462fd64a899e6e1f40c77b29b01e2a42f39046c6f07e7e772326a9c0eb61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:13:43 GMT
ARG CONSUL_VERSION=1.10.9
# Sat, 19 Mar 2022 03:13:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 03:13:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 03:13:44 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 03:14:29 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 03:14:31 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 03:14:32 GMT
# ARGS: CONSUL_VERSION=1.10.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 03:14:32 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 03:14:32 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 03:14:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 03:14:33 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 03:14:33 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 03:14:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 03:14:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8220304101d181855388ef68e024211a606504847bdf574153f924b149c092`  
		Last Modified: Sat, 19 Mar 2022 03:16:33 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f842bfb423c5794c57c1d5fd5f4423d2d416ce387a0276e7f28af6da28ecca7b`  
		Last Modified: Sat, 19 Mar 2022 03:16:42 GMT  
		Size: 40.3 MB (40286417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fba2d45f1d72d6432d7355dc75571447639410302bb873be24d6b9436ebf81`  
		Last Modified: Sat, 19 Mar 2022 03:16:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced6b0459d3e1b2cf28b1d97277530ccc3314b40bed366f545778caaca5fa5c`  
		Last Modified: Sat, 19 Mar 2022 03:16:33 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939b01b5fc4e55484cb414c74a95d66b2a2df44a525930eb97c4b1d56aa5e6c0`  
		Last Modified: Sat, 19 Mar 2022 03:16:33 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11`

```console
$ docker pull consul@sha256:b6a01470bd65e254bdd2d373b2cec93ea54ac922e639b8549f368a2d6e3db1d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11` - linux; amd64

```console
$ docker pull consul@sha256:4db2a9111569c724e51ddc9c60c52e424abc7abac858189ef6ee685c7932a656
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43941994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540c8e59237cbebea1d3acd1ab33992cea100b92772df5dac3eb47c3cf3f5375`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:01:29 GMT
ARG CONSUL_VERSION=1.11.4
# Sat, 19 Mar 2022 01:01:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 01:01:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 01:01:30 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 01:02:17 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 01:02:18 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 01:02:19 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 01:02:19 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 01:02:20 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 01:02:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 01:02:20 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 01:02:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 01:02:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 01:02:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110a33c89ed6c02da368732ce2023282c38989a24130b84162bc9cb9027eaf1b`  
		Last Modified: Sat, 19 Mar 2022 01:04:37 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a9b788b96ce6b05a5f7a6a310fc89a97ede80723df637de2e94c712f55e0e5`  
		Last Modified: Sat, 19 Mar 2022 01:04:45 GMT  
		Size: 41.1 MB (41121443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae32cd71ebfad804e961fa06e4190ceb300e9414a3ae32546743c96e117337c`  
		Last Modified: Sat, 19 Mar 2022 01:04:37 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef3cc1337901b6489d43e88ae9af046397330247794bba37c1e3b6e507b116e`  
		Last Modified: Sat, 19 Mar 2022 01:04:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4d93d79b03ecb4bcf493c328d7f12084cded152574fe26eb7189c134cd87a4`  
		Last Modified: Sat, 19 Mar 2022 01:04:37 GMT  
		Size: 1.8 KB (1785 bytes)  
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
$ docker pull consul@sha256:88577668324fe77ac9cb48cce40b3588fdc5d1127ea00dd47c6cc592e9a204df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42765982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e1ac3952042e28997eadd011d00555ee8b6b771b10e49fffa5313b08b41e1f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:12:43 GMT
ARG CONSUL_VERSION=1.11.4
# Sat, 19 Mar 2022 03:12:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 03:12:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 03:12:44 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 03:13:31 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 03:13:32 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 03:13:33 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 03:13:33 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 03:13:33 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 03:13:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 03:13:34 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 03:13:34 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 03:13:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 03:13:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebb666ac5124a308ddcae4270f5e22551cbcfff619b62f5e55c2124528a1c3`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fbb2a24a6c487c1af5ac7e9b20c38614190e227d967380c61fa44858c95758`  
		Last Modified: Sat, 19 Mar 2022 03:16:17 GMT  
		Size: 39.9 MB (39938993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7182c49be2cf23c66b8d97d3f2c789b8686736f288c1cb473a381969b731db`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05912b14764a34feb3f0562dc7600ea3837f8dc88703ace467cc5929602ac20`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96814ce33e9d857a6a4365841af9d279d8ae3c2c95b37cedec4fbcd600ce740a`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.4`

```console
$ docker pull consul@sha256:b6a01470bd65e254bdd2d373b2cec93ea54ac922e639b8549f368a2d6e3db1d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.4` - linux; amd64

```console
$ docker pull consul@sha256:4db2a9111569c724e51ddc9c60c52e424abc7abac858189ef6ee685c7932a656
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43941994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540c8e59237cbebea1d3acd1ab33992cea100b92772df5dac3eb47c3cf3f5375`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:01:29 GMT
ARG CONSUL_VERSION=1.11.4
# Sat, 19 Mar 2022 01:01:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 01:01:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 01:01:30 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 01:02:17 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 01:02:18 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 01:02:19 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 01:02:19 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 01:02:20 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 01:02:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 01:02:20 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 01:02:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 01:02:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 01:02:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110a33c89ed6c02da368732ce2023282c38989a24130b84162bc9cb9027eaf1b`  
		Last Modified: Sat, 19 Mar 2022 01:04:37 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a9b788b96ce6b05a5f7a6a310fc89a97ede80723df637de2e94c712f55e0e5`  
		Last Modified: Sat, 19 Mar 2022 01:04:45 GMT  
		Size: 41.1 MB (41121443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae32cd71ebfad804e961fa06e4190ceb300e9414a3ae32546743c96e117337c`  
		Last Modified: Sat, 19 Mar 2022 01:04:37 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef3cc1337901b6489d43e88ae9af046397330247794bba37c1e3b6e507b116e`  
		Last Modified: Sat, 19 Mar 2022 01:04:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4d93d79b03ecb4bcf493c328d7f12084cded152574fe26eb7189c134cd87a4`  
		Last Modified: Sat, 19 Mar 2022 01:04:37 GMT  
		Size: 1.8 KB (1785 bytes)  
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
$ docker pull consul@sha256:88577668324fe77ac9cb48cce40b3588fdc5d1127ea00dd47c6cc592e9a204df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42765982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e1ac3952042e28997eadd011d00555ee8b6b771b10e49fffa5313b08b41e1f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:12:43 GMT
ARG CONSUL_VERSION=1.11.4
# Sat, 19 Mar 2022 03:12:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 03:12:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 03:12:44 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 03:13:31 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 03:13:32 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 03:13:33 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 03:13:33 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 03:13:33 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 03:13:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 03:13:34 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 03:13:34 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 03:13:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 03:13:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebb666ac5124a308ddcae4270f5e22551cbcfff619b62f5e55c2124528a1c3`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fbb2a24a6c487c1af5ac7e9b20c38614190e227d967380c61fa44858c95758`  
		Last Modified: Sat, 19 Mar 2022 03:16:17 GMT  
		Size: 39.9 MB (39938993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7182c49be2cf23c66b8d97d3f2c789b8686736f288c1cb473a381969b731db`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05912b14764a34feb3f0562dc7600ea3837f8dc88703ace467cc5929602ac20`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96814ce33e9d857a6a4365841af9d279d8ae3c2c95b37cedec4fbcd600ce740a`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9`

```console
$ docker pull consul@sha256:24510c03967c971604c971a01009298ee4615d8ca019053a50771e1c76bd2f72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:983233d45683f24a4b5c230a08c94adacc2f0200f09b5b727855231113c606d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40151754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63ed72cc1ca51935b00360e678eb0259365540104de3e8f4b4d23ff06473a2fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:03:26 GMT
ARG CONSUL_VERSION=1.9.16
# Sat, 19 Mar 2022 01:03:26 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 01:03:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 01:03:27 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 01:04:13 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 01:04:14 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 01:04:15 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 01:04:15 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 01:04:15 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 01:04:15 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 01:04:15 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 01:04:16 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 01:04:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 01:04:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c04fc06df706a7f6166c47cbb48692af0210787196ea03999cb7a1c6d6a7953`  
		Last Modified: Sat, 19 Mar 2022 01:05:17 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05261c4f1255f142e86d0d190a3d8e0f9bd4fbac65ca875c1d2e7d4ba37fcd3`  
		Last Modified: Sat, 19 Mar 2022 01:05:24 GMT  
		Size: 37.3 MB (37331203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cf6bbc1d5d78452fba637235705bd8e2de08f442ddcd401f54b08016808ca1`  
		Last Modified: Sat, 19 Mar 2022 01:05:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2529310cf4ce54834c1a2c87917a3a258ecd8eb130d67fd165600a6b4856894`  
		Last Modified: Sat, 19 Mar 2022 01:05:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227d42fbfa3f5d8a1537f105e3d2ba244e233a9b58c020b6290b3238cfb7ae4`  
		Last Modified: Sat, 19 Mar 2022 01:05:17 GMT  
		Size: 1.8 KB (1785 bytes)  
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
$ docker pull consul@sha256:57ea61a090fba11349c42a7b48da490345edc0cc498cb39b25c73111d930b8a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39510573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aa4c21b319c38637ce91836b7c89f0bb93b211a8ab61da4f75f03638027ba54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:14:44 GMT
ARG CONSUL_VERSION=1.9.16
# Sat, 19 Mar 2022 03:14:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 03:14:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 03:14:46 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 03:15:29 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 03:15:30 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 03:15:31 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 03:15:31 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 03:15:31 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 03:15:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 03:15:32 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 03:15:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 03:15:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 03:15:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46002efbc1b8c5f86d71d407c330b2ec2e64e62860bbeba760205a099d2fb4b9`  
		Last Modified: Sat, 19 Mar 2022 03:16:54 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9b5707cfafc79d0003d7506be78ed19b063d55c60e6d9e30470f8deea57c76`  
		Last Modified: Sat, 19 Mar 2022 03:17:02 GMT  
		Size: 36.7 MB (36683582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70887ef1e32ab025a4fc80128727cde73b8a7f5da63ab3cdb8ef8c251dee188`  
		Last Modified: Sat, 19 Mar 2022 03:16:54 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c184481850c50ce48b1e5653ce71edf32e2ffb33437e511c6534b29d377d0f`  
		Last Modified: Sat, 19 Mar 2022 03:16:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866bc5f6ed21610512ded91be9cd9e91441b26ef2a9de0f045d2fb5ef89998a`  
		Last Modified: Sat, 19 Mar 2022 03:16:54 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.16`

```console
$ docker pull consul@sha256:24510c03967c971604c971a01009298ee4615d8ca019053a50771e1c76bd2f72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9.16` - linux; amd64

```console
$ docker pull consul@sha256:983233d45683f24a4b5c230a08c94adacc2f0200f09b5b727855231113c606d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40151754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63ed72cc1ca51935b00360e678eb0259365540104de3e8f4b4d23ff06473a2fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:03:26 GMT
ARG CONSUL_VERSION=1.9.16
# Sat, 19 Mar 2022 01:03:26 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 01:03:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 01:03:27 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 01:04:13 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 01:04:14 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 01:04:15 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 01:04:15 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 01:04:15 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 01:04:15 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 01:04:15 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 01:04:16 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 01:04:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 01:04:16 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c04fc06df706a7f6166c47cbb48692af0210787196ea03999cb7a1c6d6a7953`  
		Last Modified: Sat, 19 Mar 2022 01:05:17 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05261c4f1255f142e86d0d190a3d8e0f9bd4fbac65ca875c1d2e7d4ba37fcd3`  
		Last Modified: Sat, 19 Mar 2022 01:05:24 GMT  
		Size: 37.3 MB (37331203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cf6bbc1d5d78452fba637235705bd8e2de08f442ddcd401f54b08016808ca1`  
		Last Modified: Sat, 19 Mar 2022 01:05:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2529310cf4ce54834c1a2c87917a3a258ecd8eb130d67fd165600a6b4856894`  
		Last Modified: Sat, 19 Mar 2022 01:05:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227d42fbfa3f5d8a1537f105e3d2ba244e233a9b58c020b6290b3238cfb7ae4`  
		Last Modified: Sat, 19 Mar 2022 01:05:17 GMT  
		Size: 1.8 KB (1785 bytes)  
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
$ docker pull consul@sha256:57ea61a090fba11349c42a7b48da490345edc0cc498cb39b25c73111d930b8a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39510573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aa4c21b319c38637ce91836b7c89f0bb93b211a8ab61da4f75f03638027ba54`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:14:44 GMT
ARG CONSUL_VERSION=1.9.16
# Sat, 19 Mar 2022 03:14:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.16 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 03:14:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 03:14:46 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 03:15:29 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 03:15:30 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 03:15:31 GMT
# ARGS: CONSUL_VERSION=1.9.16
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 03:15:31 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 03:15:31 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 03:15:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 03:15:32 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 03:15:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 03:15:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 03:15:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46002efbc1b8c5f86d71d407c330b2ec2e64e62860bbeba760205a099d2fb4b9`  
		Last Modified: Sat, 19 Mar 2022 03:16:54 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9b5707cfafc79d0003d7506be78ed19b063d55c60e6d9e30470f8deea57c76`  
		Last Modified: Sat, 19 Mar 2022 03:17:02 GMT  
		Size: 36.7 MB (36683582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70887ef1e32ab025a4fc80128727cde73b8a7f5da63ab3cdb8ef8c251dee188`  
		Last Modified: Sat, 19 Mar 2022 03:16:54 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c184481850c50ce48b1e5653ce71edf32e2ffb33437e511c6534b29d377d0f`  
		Last Modified: Sat, 19 Mar 2022 03:16:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866bc5f6ed21610512ded91be9cd9e91441b26ef2a9de0f045d2fb5ef89998a`  
		Last Modified: Sat, 19 Mar 2022 03:16:54 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:b6a01470bd65e254bdd2d373b2cec93ea54ac922e639b8549f368a2d6e3db1d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:4db2a9111569c724e51ddc9c60c52e424abc7abac858189ef6ee685c7932a656
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43941994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:540c8e59237cbebea1d3acd1ab33992cea100b92772df5dac3eb47c3cf3f5375`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 01:01:29 GMT
ARG CONSUL_VERSION=1.11.4
# Sat, 19 Mar 2022 01:01:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 01:01:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 01:01:30 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 01:02:17 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 01:02:18 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 01:02:19 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 01:02:19 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 01:02:20 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 01:02:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 01:02:20 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 01:02:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 01:02:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 01:02:21 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:110a33c89ed6c02da368732ce2023282c38989a24130b84162bc9cb9027eaf1b`  
		Last Modified: Sat, 19 Mar 2022 01:04:37 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a9b788b96ce6b05a5f7a6a310fc89a97ede80723df637de2e94c712f55e0e5`  
		Last Modified: Sat, 19 Mar 2022 01:04:45 GMT  
		Size: 41.1 MB (41121443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae32cd71ebfad804e961fa06e4190ceb300e9414a3ae32546743c96e117337c`  
		Last Modified: Sat, 19 Mar 2022 01:04:37 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef3cc1337901b6489d43e88ae9af046397330247794bba37c1e3b6e507b116e`  
		Last Modified: Sat, 19 Mar 2022 01:04:38 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4d93d79b03ecb4bcf493c328d7f12084cded152574fe26eb7189c134cd87a4`  
		Last Modified: Sat, 19 Mar 2022 01:04:37 GMT  
		Size: 1.8 KB (1785 bytes)  
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
$ docker pull consul@sha256:88577668324fe77ac9cb48cce40b3588fdc5d1127ea00dd47c6cc592e9a204df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42765982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e1ac3952042e28997eadd011d00555ee8b6b771b10e49fffa5313b08b41e1f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 16:34:42 GMT
ADD file:fbbd764c2b3ce734329c4dc8415d55b9cefc972125c5818e78698f7b894667da in / 
# Thu, 17 Mar 2022 16:34:42 GMT
CMD ["/bin/sh"]
# Sat, 19 Mar 2022 03:12:43 GMT
ARG CONSUL_VERSION=1.11.4
# Sat, 19 Mar 2022 03:12:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 19 Mar 2022 03:12:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 19 Mar 2022 03:12:44 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 19 Mar 2022 03:13:31 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 19 Mar 2022 03:13:32 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 19 Mar 2022 03:13:33 GMT
# ARGS: CONSUL_VERSION=1.11.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 19 Mar 2022 03:13:33 GMT
VOLUME [/consul/data]
# Sat, 19 Mar 2022 03:13:33 GMT
EXPOSE 8300
# Sat, 19 Mar 2022 03:13:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 19 Mar 2022 03:13:34 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 19 Mar 2022 03:13:34 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 19 Mar 2022 03:13:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 03:13:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4fcf0d6f8c0dc4a27651b1a8218d9febdd0bc510d8a2eb8474b17c87b284c5bd`  
		Last Modified: Thu, 17 Mar 2022 16:35:37 GMT  
		Size: 2.8 MB (2823620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebb666ac5124a308ddcae4270f5e22551cbcfff619b62f5e55c2124528a1c3`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fbb2a24a6c487c1af5ac7e9b20c38614190e227d967380c61fa44858c95758`  
		Last Modified: Sat, 19 Mar 2022 03:16:17 GMT  
		Size: 39.9 MB (39938993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7182c49be2cf23c66b8d97d3f2c789b8686736f288c1cb473a381969b731db`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b05912b14764a34feb3f0562dc7600ea3837f8dc88703ace467cc5929602ac20`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96814ce33e9d857a6a4365841af9d279d8ae3c2c95b37cedec4fbcd600ce740a`  
		Last Modified: Sat, 19 Mar 2022 03:16:08 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
