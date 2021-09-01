## `consul:latest`

```console
$ docker pull consul@sha256:14986c31cd8fe6db8b685d408910f805bea22fbfcfb1675f500287e92a037deb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:2c69d8bee4e99c083f0930bc09cdd45b88365ae6b427221283502230ba1c1ed5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43219430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b74a0a01afc431799adac9d7911b8e0d6961a3b9909380ec61af211e342f7a97`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:13:55 GMT
ARG CONSUL_VERSION=1.10.2
# Wed, 01 Sep 2021 00:13:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 01 Sep 2021 00:13:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 01 Sep 2021 00:13:57 GMT
# ARGS: CONSUL_VERSION=1.10.2
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 01 Sep 2021 00:14:15 GMT
# ARGS: CONSUL_VERSION=1.10.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 01 Sep 2021 00:14:17 GMT
# ARGS: CONSUL_VERSION=1.10.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 01 Sep 2021 00:14:19 GMT
# ARGS: CONSUL_VERSION=1.10.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 00:14:19 GMT
VOLUME [/consul/data]
# Wed, 01 Sep 2021 00:14:20 GMT
EXPOSE 8300
# Wed, 01 Sep 2021 00:14:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 01 Sep 2021 00:14:21 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 01 Sep 2021 00:14:21 GMT
COPY file:f4999c9300ae549cb312108a9d1a23840829249bac4cd51e46d8466cfee3a6a1 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Sep 2021 00:14:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 00:14:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6085f992def430ed8f2556f38262c7a72f4b73b90938c7b10d23ee8948153f50`  
		Last Modified: Wed, 01 Sep 2021 00:15:39 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e185403d62712206d4d670a6dc1e9343046bcc9d308944262faeb165ab68a3`  
		Last Modified: Wed, 01 Sep 2021 00:15:47 GMT  
		Size: 40.4 MB (40402053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52efdf2644d28f50e4d3a9beec818e4edd8d3af82a0b5154e335b0278e6da441`  
		Last Modified: Wed, 01 Sep 2021 00:15:39 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585a8413c32a8e922dbaba4d4e1028376cf9f171f84083e0bdf28e5921f37486`  
		Last Modified: Wed, 01 Sep 2021 00:15:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76b82ffb99af04063532bb252dc67c726dc483d2b709022906503c446ab3725`  
		Last Modified: Wed, 01 Sep 2021 00:15:39 GMT  
		Size: 1.7 KB (1714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:1d983545c4f84b1cd3c7ce4d838e166c65a925693844cfd5ed5c4746e204c881
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39244219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbff18b6c799e1a17924a92190f3411c4726b7afbeaa5ebc1351581730b23e6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 22:30:33 GMT
ADD file:ed2b5e0fbd1e7ae37ab8f808c827d23c6841ce1edd7427552d5bf741d67ebcc0 in / 
# Tue, 31 Aug 2021 22:30:33 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 01:23:36 GMT
ARG CONSUL_VERSION=1.10.2
# Wed, 01 Sep 2021 01:23:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 01 Sep 2021 01:23:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 01 Sep 2021 01:23:38 GMT
# ARGS: CONSUL_VERSION=1.10.2
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 01 Sep 2021 01:23:53 GMT
# ARGS: CONSUL_VERSION=1.10.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 01 Sep 2021 01:23:55 GMT
# ARGS: CONSUL_VERSION=1.10.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 01 Sep 2021 01:23:57 GMT
# ARGS: CONSUL_VERSION=1.10.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Sep 2021 01:23:57 GMT
VOLUME [/consul/data]
# Wed, 01 Sep 2021 01:23:57 GMT
EXPOSE 8300
# Wed, 01 Sep 2021 01:23:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 01 Sep 2021 01:23:58 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 01 Sep 2021 01:23:59 GMT
COPY file:f4999c9300ae549cb312108a9d1a23840829249bac4cd51e46d8466cfee3a6a1 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 01 Sep 2021 01:23:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Sep 2021 01:24:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:840d18d84f6afdc3231d126fdd3f84f23f0335b61cbfa9cb8808b888a4308919`  
		Last Modified: Tue, 31 Aug 2021 22:32:11 GMT  
		Size: 2.6 MB (2623761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fffb408206870dbfae898542f9fe08defc3d55425b9287f67b4e7bc9639b04d`  
		Last Modified: Wed, 01 Sep 2021 01:25:54 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a9f1d264c506179627ab82efe2c2f5b2a52cfb7e2e736e8f3b883acb84c30c`  
		Last Modified: Wed, 01 Sep 2021 01:26:14 GMT  
		Size: 36.6 MB (36617160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f321a2bdffc01f4f3cfc903b8d00c4711968c30929a7ba2208e54efc88b8974`  
		Last Modified: Wed, 01 Sep 2021 01:25:54 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7731df45612e290f1b44073d40ca132679f33d61eb153abf17aecf4b0101f5`  
		Last Modified: Wed, 01 Sep 2021 01:25:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:313ef0d18b912146cb45f58d8570c5b193973da8ee33b986cf43d5df8f65e2df`  
		Last Modified: Wed, 01 Sep 2021 01:25:55 GMT  
		Size: 1.7 KB (1715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:0081f4b20a6b484746ee30b2ede4f64241d94721c18b9c115ce61b88ca6588d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39585136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:945c65b74aabe05fbf0444ae754a6cf8bea788f8854c719189eecb6501793f52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:03 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Tue, 15 Jun 2021 21:45:04 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:25:54 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 23 Jul 2021 04:19:33 GMT
ARG CONSUL_VERSION=1.10.1
# Fri, 23 Jul 2021 04:19:33 GMT
LABEL org.opencontainers.image.version=1.10.1
# Fri, 23 Jul 2021 04:19:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 23 Jul 2021 04:19:34 GMT
# ARGS: CONSUL_VERSION=1.10.1
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 23 Jul 2021 04:19:39 GMT
# ARGS: CONSUL_VERSION=1.10.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 23 Jul 2021 04:19:40 GMT
# ARGS: CONSUL_VERSION=1.10.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 23 Jul 2021 04:19:41 GMT
# ARGS: CONSUL_VERSION=1.10.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 23 Jul 2021 04:19:41 GMT
VOLUME [/consul/data]
# Fri, 23 Jul 2021 04:19:41 GMT
EXPOSE 8300
# Fri, 23 Jul 2021 04:19:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 23 Jul 2021 04:19:42 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 23 Jul 2021 04:19:42 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 23 Jul 2021 04:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 23 Jul 2021 04:19:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec0bca027d4ed5928a09c462f06be2502d9e6dfd78d9ba3c527dc500cfcdfca`  
		Last Modified: Fri, 23 Jul 2021 04:20:34 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b3128d8785d803695d60c92ef9482ab1ddc021eeb844a226ba40208ccb0a54`  
		Last Modified: Fri, 23 Jul 2021 04:20:40 GMT  
		Size: 36.9 MB (36869818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbf322ffab66a9b685be5eb28cf5499c409303c57282a74d1c3c7380cf2f5f7`  
		Last Modified: Fri, 23 Jul 2021 04:20:34 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:117f3c6fd6c3e6a3b608722cdf776c98efb4d2ab2be357bf99716b7e6f5e8343`  
		Last Modified: Fri, 23 Jul 2021 04:20:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418597e612cf3477bacd0c9730131f6a619802a05c2a5c37081550ec54fc2c60`  
		Last Modified: Fri, 23 Jul 2021 04:20:34 GMT  
		Size: 1.7 KB (1704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:704f9e58a7de016a0cb62eb6b1feb857af4212e93302f12b360ff7d6d8eb27fc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42606378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:235ec7a18ce3caab5b129792e612b333599a772e67b9fb38984697592a1e388b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 21:23:28 GMT
ADD file:fb9d541cffc3a5660d23426ba847aa696b59a9d7f14e00ba0a63b28c9ec272c0 in / 
# Tue, 31 Aug 2021 21:23:29 GMT
CMD ["/bin/sh"]
# Tue, 31 Aug 2021 22:13:58 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Tue, 31 Aug 2021 22:13:58 GMT
ARG CONSUL_VERSION=1.10.1
# Tue, 31 Aug 2021 22:13:58 GMT
LABEL org.opencontainers.image.version=1.10.1
# Tue, 31 Aug 2021 22:13:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 31 Aug 2021 22:14:00 GMT
# ARGS: CONSUL_VERSION=1.10.1
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 31 Aug 2021 22:14:12 GMT
# ARGS: CONSUL_VERSION=1.10.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 31 Aug 2021 22:14:13 GMT
# ARGS: CONSUL_VERSION=1.10.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 31 Aug 2021 22:14:14 GMT
# ARGS: CONSUL_VERSION=1.10.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 31 Aug 2021 22:14:14 GMT
VOLUME [/consul/data]
# Tue, 31 Aug 2021 22:14:14 GMT
EXPOSE 8300
# Tue, 31 Aug 2021 22:14:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 31 Aug 2021 22:14:14 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 31 Aug 2021 22:14:15 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 31 Aug 2021 22:14:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 31 Aug 2021 22:14:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4ed7d06bd90bc8d13b87220ccc6204a7d235ec943be9fb4289d856f9ff0a5b7b`  
		Last Modified: Tue, 31 Aug 2021 21:24:28 GMT  
		Size: 2.8 MB (2821095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:125ca2a30f54cd18e05ac235653e5a7d47c17287feb16b702ecc59fafd8d57f1`  
		Last Modified: Tue, 31 Aug 2021 22:15:14 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992210e79fef88bffd5534cd426d16e90d5ab6d645ac465be8b8a24fe84acfe2`  
		Last Modified: Tue, 31 Aug 2021 22:15:21 GMT  
		Size: 39.8 MB (39781993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b023f3b077dea6b6c7f95e0af985afdd991cc9862fdf338b31871e85da8073`  
		Last Modified: Tue, 31 Aug 2021 22:15:14 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7678dfe71e94f218ac4eaaca24a8c0c86af64cb4ef39f8c1cc86c69dbb1ce34`  
		Last Modified: Tue, 31 Aug 2021 22:15:14 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f56059d9560b4ba8d14f0cb501f1137093c6b75a5cfe4749622c462c8ca10d`  
		Last Modified: Tue, 31 Aug 2021 22:15:14 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
