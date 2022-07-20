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
