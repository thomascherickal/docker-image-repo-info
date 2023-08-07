<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.13`](#consul113)
-	[`consul:1.13.9`](#consul1139)
-	[`consul:1.14`](#consul114)
-	[`consul:1.14.8`](#consul1148)
-	[`consul:1.15`](#consul115)
-	[`consul:1.15.4`](#consul1154)

## `consul:1.13`

```console
$ docker pull consul@sha256:05101c68aed94ea886194723795347ae9210eb109a55ffb936044667d9f6b01e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13` - linux; amd64

```console
$ docker pull consul@sha256:ffecd277731710fbaaab4a55c5b887d3be93ed8df3a9af4f37421be0b491c313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52861472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa4241798b9d6bd1ac7b5cc24ed073063f272e640806f140d312ee8404a3a9ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:29:17 GMT
ARG CONSUL_VERSION=1.13.9
# Mon, 07 Aug 2023 20:29:17 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:29:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:29:18 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:29:23 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:29:24 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:29:24 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:29:24 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:29:25 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:29:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:29:25 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:29:25 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:29:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:29:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de0aad12198d17e874371efefab0ba9ebf136f656d877511fb574e92f532a1b`  
		Last Modified: Mon, 07 Aug 2023 20:30:11 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ec3a5d06b6aa7c2cbf176fd6750c0d3c997db11d1f5753ad9b948fc9f8597`  
		Last Modified: Mon, 07 Aug 2023 20:30:18 GMT  
		Size: 50.0 MB (50032037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6e327f1319094fffff0b8cc720cb02f1769de4974770cdbbabb7220f77d62b`  
		Last Modified: Mon, 07 Aug 2023 20:30:11 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef59975f882f3d818cb730b4055fff16d961dcbc749771afb4bfb024fc8d700`  
		Last Modified: Mon, 07 Aug 2023 20:30:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57e7ee14167191d52c830b6811172e861b237ed6fb776ae1ee564c9cc403390`  
		Last Modified: Mon, 07 Aug 2023 20:30:11 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm variant v6

```console
$ docker pull consul@sha256:d9a42dbfb47ff66d3e91b49975d234af085f9d4b394d9f2b317dfddda0feb614
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50352944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f38b5ed6dc44f44158fcd429c1aa98af68f2ac9a7fb00f43c29681285e8711f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Tue, 27 Jun 2023 18:49:45 GMT
ARG CONSUL_VERSION=1.13.9
# Tue, 27 Jun 2023 18:49:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 27 Jun 2023 18:49:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 27 Jun 2023 18:49:46 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 27 Jun 2023 18:49:52 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 27 Jun 2023 18:49:53 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 27 Jun 2023 18:49:54 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 27 Jun 2023 18:49:54 GMT
VOLUME [/consul/data]
# Tue, 27 Jun 2023 18:49:54 GMT
EXPOSE 8300
# Tue, 27 Jun 2023 18:49:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 27 Jun 2023 18:49:54 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 27 Jun 2023 18:49:54 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Jun 2023 18:49:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Jun 2023 18:49:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1458c6aca3a591a7d6232ee605248d5d5e328fe38be2ca5b44ab57586ccf32`  
		Last Modified: Tue, 27 Jun 2023 18:50:39 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c419287263b8403e4f5bf6edeb1f85fdbf8026284f2c940781e66d6a6bb05a`  
		Last Modified: Tue, 27 Jun 2023 18:50:46 GMT  
		Size: 47.7 MB (47716451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1a829b9a8e631e7cab4c94b2797e084e367013476c68f8a1c840f251c932e3`  
		Last Modified: Tue, 27 Jun 2023 18:50:39 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a574a11bd29d4e55b496ccbe635924696ddf30bd1d64370c61ecda1cf4ebfc3f`  
		Last Modified: Tue, 27 Jun 2023 18:50:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1af627c74a5226772ad4aaf7a9943b8483345680c2f2a15f5c632c80b6798c`  
		Last Modified: Tue, 27 Jun 2023 18:50:39 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:9ca4db9be917c4628cf40e1cbcc2c82e585adbc1f61e74549e7a01e4ae2ae60a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49887900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38653cafba99cd59468e4289b19d753083ecca1d69a3378105554224b24736d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:18:00 GMT
ARG CONSUL_VERSION=1.13.9
# Mon, 07 Aug 2023 20:18:00 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:18:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:18:00 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:18:05 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:18:05 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:18:06 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:18:06 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:18:06 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:18:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:18:06 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:18:06 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:18:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:18:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb692b9b206a6ea95e8c37d1de8d9f17283f4b82f0c084ab8052cb98e816c93`  
		Last Modified: Mon, 07 Aug 2023 20:18:45 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ee12e9352466ac63c42cda1c6f4c7c8de1a679bbd57e34e20a221a0bd4a5b8`  
		Last Modified: Mon, 07 Aug 2023 20:18:49 GMT  
		Size: 47.2 MB (47163603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63007ef03380bac6eb13b1d2f459c11a8a1678376b9e27602c49bf734eff4ef4`  
		Last Modified: Mon, 07 Aug 2023 20:18:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8386e27ddec81ad51a8d6de08a8a4c05dc34286584e52ad98c9c6e801551bc6d`  
		Last Modified: Mon, 07 Aug 2023 20:18:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db323a2b82c590e46937f6eac35b8e4c2adb2651d9427a3b1b81b671405f51e`  
		Last Modified: Mon, 07 Aug 2023 20:18:45 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; 386

```console
$ docker pull consul@sha256:e6b605eb4ae59542c8331da9aaa1cce4e5f6ca3eb0c5b423a1d0c84ac1869668
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51689196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b73685b17d7d2000a7ca9994d1ef93b8be7f8d891fdc57c53f16ec92abce118a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:28:55 GMT
ARG CONSUL_VERSION=1.13.9
# Mon, 07 Aug 2023 20:28:55 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:28:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:28:56 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:29:03 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:29:04 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:29:04 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:29:05 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:29:05 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:29:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:29:05 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:29:05 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:29:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:29:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf61741b49cf223bba31911b7abee7b595c89d879db6ba07d9347e40c481ea88`  
		Last Modified: Mon, 07 Aug 2023 20:29:51 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c017cefef559895a7b360f6e5e54fc0d91ac29dfbe0239928d92b55b279c0d9`  
		Last Modified: Mon, 07 Aug 2023 20:29:59 GMT  
		Size: 48.9 MB (48853453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b7110fa29053f56b9575b4b2aa882d8fb03e07f1f3cce20f585cd3e8798006`  
		Last Modified: Mon, 07 Aug 2023 20:29:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5ec2f78201a40a548d9ebe371908950e0770bf9e12ff06c6ceb9b1e17bca3c`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52acf8afc3bfc715e98b38b8e3cce9e83efd9f0fb22356b3ce96926e2a21605`  
		Last Modified: Mon, 07 Aug 2023 20:29:51 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.13.9`

```console
$ docker pull consul@sha256:05101c68aed94ea886194723795347ae9210eb109a55ffb936044667d9f6b01e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13.9` - linux; amd64

```console
$ docker pull consul@sha256:ffecd277731710fbaaab4a55c5b887d3be93ed8df3a9af4f37421be0b491c313
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52861472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa4241798b9d6bd1ac7b5cc24ed073063f272e640806f140d312ee8404a3a9ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:29:17 GMT
ARG CONSUL_VERSION=1.13.9
# Mon, 07 Aug 2023 20:29:17 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:29:18 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:29:18 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:29:23 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:29:24 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:29:24 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:29:24 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:29:25 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:29:25 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:29:25 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:29:25 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:29:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:29:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de0aad12198d17e874371efefab0ba9ebf136f656d877511fb574e92f532a1b`  
		Last Modified: Mon, 07 Aug 2023 20:30:11 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8ec3a5d06b6aa7c2cbf176fd6750c0d3c997db11d1f5753ad9b948fc9f8597`  
		Last Modified: Mon, 07 Aug 2023 20:30:18 GMT  
		Size: 50.0 MB (50032037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6e327f1319094fffff0b8cc720cb02f1769de4974770cdbbabb7220f77d62b`  
		Last Modified: Mon, 07 Aug 2023 20:30:11 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef59975f882f3d818cb730b4055fff16d961dcbc749771afb4bfb024fc8d700`  
		Last Modified: Mon, 07 Aug 2023 20:30:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57e7ee14167191d52c830b6811172e861b237ed6fb776ae1ee564c9cc403390`  
		Last Modified: Mon, 07 Aug 2023 20:30:11 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:d9a42dbfb47ff66d3e91b49975d234af085f9d4b394d9f2b317dfddda0feb614
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50352944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f38b5ed6dc44f44158fcd429c1aa98af68f2ac9a7fb00f43c29681285e8711f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Tue, 27 Jun 2023 18:49:45 GMT
ARG CONSUL_VERSION=1.13.9
# Tue, 27 Jun 2023 18:49:45 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 27 Jun 2023 18:49:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 27 Jun 2023 18:49:46 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 27 Jun 2023 18:49:52 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 27 Jun 2023 18:49:53 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 27 Jun 2023 18:49:54 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 27 Jun 2023 18:49:54 GMT
VOLUME [/consul/data]
# Tue, 27 Jun 2023 18:49:54 GMT
EXPOSE 8300
# Tue, 27 Jun 2023 18:49:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 27 Jun 2023 18:49:54 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 27 Jun 2023 18:49:54 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Jun 2023 18:49:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Jun 2023 18:49:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1458c6aca3a591a7d6232ee605248d5d5e328fe38be2ca5b44ab57586ccf32`  
		Last Modified: Tue, 27 Jun 2023 18:50:39 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c419287263b8403e4f5bf6edeb1f85fdbf8026284f2c940781e66d6a6bb05a`  
		Last Modified: Tue, 27 Jun 2023 18:50:46 GMT  
		Size: 47.7 MB (47716451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1a829b9a8e631e7cab4c94b2797e084e367013476c68f8a1c840f251c932e3`  
		Last Modified: Tue, 27 Jun 2023 18:50:39 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a574a11bd29d4e55b496ccbe635924696ddf30bd1d64370c61ecda1cf4ebfc3f`  
		Last Modified: Tue, 27 Jun 2023 18:50:39 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a1af627c74a5226772ad4aaf7a9943b8483345680c2f2a15f5c632c80b6798c`  
		Last Modified: Tue, 27 Jun 2023 18:50:39 GMT  
		Size: 1.8 KB (1838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:9ca4db9be917c4628cf40e1cbcc2c82e585adbc1f61e74549e7a01e4ae2ae60a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49887900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38653cafba99cd59468e4289b19d753083ecca1d69a3378105554224b24736d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:18:00 GMT
ARG CONSUL_VERSION=1.13.9
# Mon, 07 Aug 2023 20:18:00 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:18:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:18:00 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:18:05 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:18:05 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:18:06 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:18:06 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:18:06 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:18:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:18:06 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:18:06 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:18:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:18:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb692b9b206a6ea95e8c37d1de8d9f17283f4b82f0c084ab8052cb98e816c93`  
		Last Modified: Mon, 07 Aug 2023 20:18:45 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ee12e9352466ac63c42cda1c6f4c7c8de1a679bbd57e34e20a221a0bd4a5b8`  
		Last Modified: Mon, 07 Aug 2023 20:18:49 GMT  
		Size: 47.2 MB (47163603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63007ef03380bac6eb13b1d2f459c11a8a1678376b9e27602c49bf734eff4ef4`  
		Last Modified: Mon, 07 Aug 2023 20:18:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8386e27ddec81ad51a8d6de08a8a4c05dc34286584e52ad98c9c6e801551bc6d`  
		Last Modified: Mon, 07 Aug 2023 20:18:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db323a2b82c590e46937f6eac35b8e4c2adb2651d9427a3b1b81b671405f51e`  
		Last Modified: Mon, 07 Aug 2023 20:18:45 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.9` - linux; 386

```console
$ docker pull consul@sha256:e6b605eb4ae59542c8331da9aaa1cce4e5f6ca3eb0c5b423a1d0c84ac1869668
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51689196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b73685b17d7d2000a7ca9994d1ef93b8be7f8d891fdc57c53f16ec92abce118a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:28:55 GMT
ARG CONSUL_VERSION=1.13.9
# Mon, 07 Aug 2023 20:28:55 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.9 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:28:55 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:28:56 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:29:03 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:29:04 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:29:04 GMT
# ARGS: CONSUL_VERSION=1.13.9
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:29:05 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:29:05 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:29:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:29:05 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:29:05 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:29:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:29:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf61741b49cf223bba31911b7abee7b595c89d879db6ba07d9347e40c481ea88`  
		Last Modified: Mon, 07 Aug 2023 20:29:51 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c017cefef559895a7b360f6e5e54fc0d91ac29dfbe0239928d92b55b279c0d9`  
		Last Modified: Mon, 07 Aug 2023 20:29:59 GMT  
		Size: 48.9 MB (48853453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b7110fa29053f56b9575b4b2aa882d8fb03e07f1f3cce20f585cd3e8798006`  
		Last Modified: Mon, 07 Aug 2023 20:29:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5ec2f78201a40a548d9ebe371908950e0770bf9e12ff06c6ceb9b1e17bca3c`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d52acf8afc3bfc715e98b38b8e3cce9e83efd9f0fb22356b3ce96926e2a21605`  
		Last Modified: Mon, 07 Aug 2023 20:29:51 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.14`

```console
$ docker pull consul@sha256:2fd3b945d146a182876cd616541333a7161d27b1c1017b7335af4fb87d099157
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14` - linux; amd64

```console
$ docker pull consul@sha256:81f4966d5950a83c5368ea1ea2f4f5a0826fd04e48ca024ae7b9800aeeb5802f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56667727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f572c33af973e25a629d63be2b7dd4bf9f4810cf11e029d10b0d81c51f8311d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:29:07 GMT
ARG CONSUL_VERSION=1.14.8
# Mon, 07 Aug 2023 20:29:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:29:07 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:29:08 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:29:13 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:29:14 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:29:14 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:29:14 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:29:14 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:29:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:29:14 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:29:14 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:29:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:29:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a48fa085753f7b806a05b7beb4fa300eaa8e254abba57fdf0a114edbd15a9a`  
		Last Modified: Mon, 07 Aug 2023 20:29:52 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff33c1be2dcee3520480206a86f690fa822c06af932f5b7fcd769d5bf423b98b`  
		Last Modified: Mon, 07 Aug 2023 20:29:59 GMT  
		Size: 53.8 MB (53838292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca17c1136df2489af23d1e83359357d4b1362f3f447810a255dbd75b1cc264b`  
		Last Modified: Mon, 07 Aug 2023 20:29:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c12a638fb803377b0ef99a812bc94db37f7e2440397d2c0b562c1cb893cd6a`  
		Last Modified: Mon, 07 Aug 2023 20:29:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0409a30386a38d844e8fe0ee5f6739bbff6789e9db1074cb4bacc02ad5aa9c1`  
		Last Modified: Mon, 07 Aug 2023 20:29:52 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; arm variant v6

```console
$ docker pull consul@sha256:90de44d04bed4cd48f88e51b60baed4efebb2cb2d9cd2a5149b56ee5be28c19d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53944629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e8a0433bbe41e2c8c64ea7b3294d74fb8a8d4a41577a04fd7d61a035180446f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Tue, 27 Jun 2023 18:49:34 GMT
ARG CONSUL_VERSION=1.14.8
# Tue, 27 Jun 2023 18:49:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 27 Jun 2023 18:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 27 Jun 2023 18:49:34 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 27 Jun 2023 18:49:41 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 27 Jun 2023 18:49:42 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 27 Jun 2023 18:49:43 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 27 Jun 2023 18:49:43 GMT
VOLUME [/consul/data]
# Tue, 27 Jun 2023 18:49:43 GMT
EXPOSE 8300
# Tue, 27 Jun 2023 18:49:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 27 Jun 2023 18:49:43 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 27 Jun 2023 18:49:43 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Jun 2023 18:49:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Jun 2023 18:49:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3f9b01e73756ac2c8d07491f8930f96819926a1d28746ef008d8fa779bca1a`  
		Last Modified: Tue, 27 Jun 2023 18:50:23 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88804a89a28bfb2c17a3440b287a08729ffa387653832678357a9ed435da1df8`  
		Last Modified: Tue, 27 Jun 2023 18:50:30 GMT  
		Size: 51.3 MB (51308138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543d1e08f032a5d4f5b25a317aeff7389c4fa79d203ebd38030cc8cc0e5dc138`  
		Last Modified: Tue, 27 Jun 2023 18:50:23 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a53daaa70ef1de7e8cc002a4e5ea04343f864280a9805bc60d438451688a861`  
		Last Modified: Tue, 27 Jun 2023 18:50:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9284534673e47783dede8bf1a60d67ae425691c2f4a8775cfe030edea948913`  
		Last Modified: Tue, 27 Jun 2023 18:50:23 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:bac6fe85dea2d81b469c702904a2d789d69cd4904b4b84fc1d077a00ef9a6129
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53510951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852f1ca2417bd4b123073cd6bcf571b97b784f0ae898fb11d0303dd3732aff77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:17:50 GMT
ARG CONSUL_VERSION=1.14.8
# Mon, 07 Aug 2023 20:17:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:17:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:17:51 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:17:55 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:17:56 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:17:57 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:17:57 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:17:57 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:17:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:17:57 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:17:57 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:17:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:17:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c69d01bb5e779a77b1b6be7b11e6e14b19aec1533dd63b5a65314f5b7691b6`  
		Last Modified: Mon, 07 Aug 2023 20:18:30 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce7aa33142a39195c54d295911e177b3707ef5a63ec8c4b0fcc455b1916da8f`  
		Last Modified: Mon, 07 Aug 2023 20:18:36 GMT  
		Size: 50.8 MB (50786658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4643c57e719dc24d07a83851939342452e1d28a3fe40f3a31521ee8debe52a4d`  
		Last Modified: Mon, 07 Aug 2023 20:18:31 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d856ab6a6f6a21e865284b96c4b2d2ea071950e50ff571b947c372c59e2153`  
		Last Modified: Mon, 07 Aug 2023 20:18:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e707499da1a15cf701449b919d58d13e3b02bea4d145c28b6506c33fe6630724`  
		Last Modified: Mon, 07 Aug 2023 20:18:30 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; 386

```console
$ docker pull consul@sha256:6c0dc4878c036e40a8f34b0a8de41de8d9546ea084a2312deda1e2262499a8fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.3 MB (55346322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e68227491146fa8b2b5ebaabeb2df0f7a4012c334cb2dd39d5dbef3cb347920`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:28:41 GMT
ARG CONSUL_VERSION=1.14.8
# Mon, 07 Aug 2023 20:28:42 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:28:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:28:42 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:28:50 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:28:51 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:28:51 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:28:51 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:28:51 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:28:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:28:52 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:28:52 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:28:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:28:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9727cd61e408aabce18f407d54181b9dc16cd78a91283dc9e6ca105c928de157`  
		Last Modified: Mon, 07 Aug 2023 20:29:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b37c874449c218e3b1dff71d111e100cb5ac0cc67e9d42e3e60e6a126c4d0e`  
		Last Modified: Mon, 07 Aug 2023 20:29:42 GMT  
		Size: 52.5 MB (52510580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ef26788782e2d661fa5687ec4987fdccfa2b1d89b190cf3e10f3552d56266e`  
		Last Modified: Mon, 07 Aug 2023 20:29:34 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c45703a10e2a107893650bd84f1b9ae9347468033c0a53fa155d1ee84549530`  
		Last Modified: Mon, 07 Aug 2023 20:29:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2b0d202297f4e4ee2e87ebf88811730d541606d7502bd58d2cd6a16ad671fd`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.14.8`

```console
$ docker pull consul@sha256:2fd3b945d146a182876cd616541333a7161d27b1c1017b7335af4fb87d099157
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14.8` - linux; amd64

```console
$ docker pull consul@sha256:81f4966d5950a83c5368ea1ea2f4f5a0826fd04e48ca024ae7b9800aeeb5802f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56667727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f572c33af973e25a629d63be2b7dd4bf9f4810cf11e029d10b0d81c51f8311d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:29:07 GMT
ARG CONSUL_VERSION=1.14.8
# Mon, 07 Aug 2023 20:29:07 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:29:07 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:29:08 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:29:13 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:29:14 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:29:14 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:29:14 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:29:14 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:29:14 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:29:14 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:29:14 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:29:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:29:15 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a48fa085753f7b806a05b7beb4fa300eaa8e254abba57fdf0a114edbd15a9a`  
		Last Modified: Mon, 07 Aug 2023 20:29:52 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff33c1be2dcee3520480206a86f690fa822c06af932f5b7fcd769d5bf423b98b`  
		Last Modified: Mon, 07 Aug 2023 20:29:59 GMT  
		Size: 53.8 MB (53838292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca17c1136df2489af23d1e83359357d4b1362f3f447810a255dbd75b1cc264b`  
		Last Modified: Mon, 07 Aug 2023 20:29:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c12a638fb803377b0ef99a812bc94db37f7e2440397d2c0b562c1cb893cd6a`  
		Last Modified: Mon, 07 Aug 2023 20:29:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0409a30386a38d844e8fe0ee5f6739bbff6789e9db1074cb4bacc02ad5aa9c1`  
		Last Modified: Mon, 07 Aug 2023 20:29:52 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:90de44d04bed4cd48f88e51b60baed4efebb2cb2d9cd2a5149b56ee5be28c19d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53944629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e8a0433bbe41e2c8c64ea7b3294d74fb8a8d4a41577a04fd7d61a035180446f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Tue, 27 Jun 2023 18:49:34 GMT
ARG CONSUL_VERSION=1.14.8
# Tue, 27 Jun 2023 18:49:34 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 27 Jun 2023 18:49:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 27 Jun 2023 18:49:34 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 27 Jun 2023 18:49:41 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 27 Jun 2023 18:49:42 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 27 Jun 2023 18:49:43 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 27 Jun 2023 18:49:43 GMT
VOLUME [/consul/data]
# Tue, 27 Jun 2023 18:49:43 GMT
EXPOSE 8300
# Tue, 27 Jun 2023 18:49:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 27 Jun 2023 18:49:43 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 27 Jun 2023 18:49:43 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Jun 2023 18:49:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Jun 2023 18:49:43 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3f9b01e73756ac2c8d07491f8930f96819926a1d28746ef008d8fa779bca1a`  
		Last Modified: Tue, 27 Jun 2023 18:50:23 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88804a89a28bfb2c17a3440b287a08729ffa387653832678357a9ed435da1df8`  
		Last Modified: Tue, 27 Jun 2023 18:50:30 GMT  
		Size: 51.3 MB (51308138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:543d1e08f032a5d4f5b25a317aeff7389c4fa79d203ebd38030cc8cc0e5dc138`  
		Last Modified: Tue, 27 Jun 2023 18:50:23 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a53daaa70ef1de7e8cc002a4e5ea04343f864280a9805bc60d438451688a861`  
		Last Modified: Tue, 27 Jun 2023 18:50:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9284534673e47783dede8bf1a60d67ae425691c2f4a8775cfe030edea948913`  
		Last Modified: Tue, 27 Jun 2023 18:50:23 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:bac6fe85dea2d81b469c702904a2d789d69cd4904b4b84fc1d077a00ef9a6129
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53510951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:852f1ca2417bd4b123073cd6bcf571b97b784f0ae898fb11d0303dd3732aff77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:17:50 GMT
ARG CONSUL_VERSION=1.14.8
# Mon, 07 Aug 2023 20:17:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:17:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:17:51 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:17:55 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:17:56 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:17:57 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:17:57 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:17:57 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:17:57 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:17:57 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:17:57 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:17:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:17:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c69d01bb5e779a77b1b6be7b11e6e14b19aec1533dd63b5a65314f5b7691b6`  
		Last Modified: Mon, 07 Aug 2023 20:18:30 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce7aa33142a39195c54d295911e177b3707ef5a63ec8c4b0fcc455b1916da8f`  
		Last Modified: Mon, 07 Aug 2023 20:18:36 GMT  
		Size: 50.8 MB (50786658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4643c57e719dc24d07a83851939342452e1d28a3fe40f3a31521ee8debe52a4d`  
		Last Modified: Mon, 07 Aug 2023 20:18:31 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d856ab6a6f6a21e865284b96c4b2d2ea071950e50ff571b947c372c59e2153`  
		Last Modified: Mon, 07 Aug 2023 20:18:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e707499da1a15cf701449b919d58d13e3b02bea4d145c28b6506c33fe6630724`  
		Last Modified: Mon, 07 Aug 2023 20:18:30 GMT  
		Size: 1.8 KB (1830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.8` - linux; 386

```console
$ docker pull consul@sha256:6c0dc4878c036e40a8f34b0a8de41de8d9546ea084a2312deda1e2262499a8fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.3 MB (55346322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e68227491146fa8b2b5ebaabeb2df0f7a4012c334cb2dd39d5dbef3cb347920`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:28:41 GMT
ARG CONSUL_VERSION=1.14.8
# Mon, 07 Aug 2023 20:28:42 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.8 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:28:42 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:28:42 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:28:50 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:28:51 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:28:51 GMT
# ARGS: CONSUL_VERSION=1.14.8
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:28:51 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:28:51 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:28:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:28:52 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:28:52 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:28:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:28:52 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9727cd61e408aabce18f407d54181b9dc16cd78a91283dc9e6ca105c928de157`  
		Last Modified: Mon, 07 Aug 2023 20:29:34 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b37c874449c218e3b1dff71d111e100cb5ac0cc67e9d42e3e60e6a126c4d0e`  
		Last Modified: Mon, 07 Aug 2023 20:29:42 GMT  
		Size: 52.5 MB (52510580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ef26788782e2d661fa5687ec4987fdccfa2b1d89b190cf3e10f3552d56266e`  
		Last Modified: Mon, 07 Aug 2023 20:29:34 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c45703a10e2a107893650bd84f1b9ae9347468033c0a53fa155d1ee84549530`  
		Last Modified: Mon, 07 Aug 2023 20:29:34 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2b0d202297f4e4ee2e87ebf88811730d541606d7502bd58d2cd6a16ad671fd`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 1.8 KB (1832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.15`

```console
$ docker pull consul@sha256:dccde4722b88c6674ed7b169937e80fca4d098ad1abc6ba7d4da724b73b5c3c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.15` - linux; amd64

```console
$ docker pull consul@sha256:4183646daa879eb83d812938715a39476dea498d1be05275db9d1a185054bdf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58867874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f012b134049ccd6dc2e15fb33cb577bb0076cebd1f06b9eff1c7ab3aaf156d35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:28:57 GMT
ARG CONSUL_VERSION=1.15.4
# Mon, 07 Aug 2023 20:28:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:28:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:28:57 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:29:03 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:29:03 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:29:04 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:29:04 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:29:04 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:29:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:29:04 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:29:04 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:29:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e57e19f25baaa97592e47db7535a724f667d35f9de6ed142671f313f96eee0`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020dc46acd18a2c8999d4763c6e77d0bfe6d89bee8f90b581171e4582183af10`  
		Last Modified: Mon, 07 Aug 2023 20:29:43 GMT  
		Size: 56.0 MB (56038439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbd6cbb1fb5a20db7e9065b92e93bd157606712432d1f631a707e3193999770`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5ec2f78201a40a548d9ebe371908950e0770bf9e12ff06c6ceb9b1e17bca3c`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df296a8d036f48d36ed501d8c575e96fedda1bc82c19373f2f42b432d6df128d`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15` - linux; arm variant v6

```console
$ docker pull consul@sha256:8012d555aa76088fe20156d9a053492c8dd0e9596e41752f7cc75520a35afa00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56015232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c04630ac543532a256e0742de0c22dc75a8c7e4a2d2d8f077babcce2844874e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Tue, 27 Jun 2023 18:49:14 GMT
ARG CONSUL_VERSION=1.15.4
# Tue, 27 Jun 2023 18:49:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 27 Jun 2023 18:49:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 27 Jun 2023 18:49:15 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 27 Jun 2023 18:49:28 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 27 Jun 2023 18:49:29 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 27 Jun 2023 18:49:30 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 27 Jun 2023 18:49:30 GMT
VOLUME [/consul/data]
# Tue, 27 Jun 2023 18:49:30 GMT
EXPOSE 8300
# Tue, 27 Jun 2023 18:49:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 27 Jun 2023 18:49:30 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 27 Jun 2023 18:49:30 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Jun 2023 18:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Jun 2023 18:49:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995469d5ed357beed1eda31495e57bd57a85c2b89a1ec2fd1e6ee44f93a1b675`  
		Last Modified: Tue, 27 Jun 2023 18:50:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c2eed3d26135ba81af45e33b9bd97a7b6d41b6295a708c635e52b9566b77d2`  
		Last Modified: Tue, 27 Jun 2023 18:50:12 GMT  
		Size: 53.4 MB (53378742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cadac4432d1df266b13bee9cf95158f164dec415f8721abdc5b55da281a5843`  
		Last Modified: Tue, 27 Jun 2023 18:50:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657773322b04ff357b774d8f421c01115d5912e5d7142b7b935e13cfea146a3b`  
		Last Modified: Tue, 27 Jun 2023 18:50:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247eb5ea07e57d3de66278877506be864f2e41afa9d85b385548f2be15da69c0`  
		Last Modified: Tue, 27 Jun 2023 18:50:06 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:3e252086ef0da34ea27c0dcfade9252444be163a6a18a16ebb24095c7ead916d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55603514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ea2b204bb98ec01683744f0991efb916fa505ec449149f9aff98a8645cb5f88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:17:39 GMT
ARG CONSUL_VERSION=1.15.4
# Mon, 07 Aug 2023 20:17:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:17:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:17:39 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:17:45 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:17:46 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:17:46 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:17:46 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:17:46 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:17:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:17:47 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:17:47 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:17:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:17:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc0ff86a773a4b23131c6a192cb6265108a9bb27f571f7dd5c7c6425dabdef4`  
		Last Modified: Mon, 07 Aug 2023 20:18:16 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a221f2346c39c3f6194efb140134f02a0685d643a5ea0d4814b4abef95e3afcd`  
		Last Modified: Mon, 07 Aug 2023 20:18:22 GMT  
		Size: 52.9 MB (52879216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30201693224304958e9ecef50dac60c54d179a6c785bd84f436809ee88120a3d`  
		Last Modified: Mon, 07 Aug 2023 20:18:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec582cf4de3bbc225cde18e26925f71e6de25d7b02d20398b9f27d709362fcd`  
		Last Modified: Mon, 07 Aug 2023 20:18:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be66a0761e47c07a158fa069bb3ea8990a042f836f552d64c89b29daaf4f449d`  
		Last Modified: Mon, 07 Aug 2023 20:18:16 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15` - linux; 386

```console
$ docker pull consul@sha256:df36500e40b488a5e2ba02c2d617dcebe2a6cecdb777579e651aeef499e1c295
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57428519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c7c086b3b6c90d643222a2582b3fa6cace55846f3c83991e735660b909aea2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:28:22 GMT
ARG CONSUL_VERSION=1.15.4
# Mon, 07 Aug 2023 20:28:22 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:28:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:28:23 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:28:36 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:28:36 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:28:37 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:28:37 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:28:37 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:28:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:28:37 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:28:38 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:28:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:28:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839237463244ad8fa7addb4ee8b214ca710e9be73179f1a4d481c75fb6007553`  
		Last Modified: Mon, 07 Aug 2023 20:29:17 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d3a79e0e88ffed7a72946d5847aec4e35775bf9f5436a04eb00425712f0eaa`  
		Last Modified: Mon, 07 Aug 2023 20:29:26 GMT  
		Size: 54.6 MB (54592773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc8a73d94f7aeb23b310e492bbe6faa3c194ba10785e5f5446758879acbd276`  
		Last Modified: Mon, 07 Aug 2023 20:29:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62687d6d763e66949be32cb9c9b4b38787ae35f407f59f6594421aee6de454cd`  
		Last Modified: Mon, 07 Aug 2023 20:29:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f0861dff5ccce5a271ba4a5a11fd46edadc6b527cd385eb060da57d5bb9816`  
		Last Modified: Mon, 07 Aug 2023 20:29:17 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.15.4`

```console
$ docker pull consul@sha256:dccde4722b88c6674ed7b169937e80fca4d098ad1abc6ba7d4da724b73b5c3c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.15.4` - linux; amd64

```console
$ docker pull consul@sha256:4183646daa879eb83d812938715a39476dea498d1be05275db9d1a185054bdf2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.9 MB (58867874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f012b134049ccd6dc2e15fb33cb577bb0076cebd1f06b9eff1c7ab3aaf156d35`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:37 GMT
ADD file:4faae297b6caba92e1791a5ff667be0fcb4de6a4de2df155395957ef9d8ad5e5 in / 
# Mon, 07 Aug 2023 19:20:37 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:28:57 GMT
ARG CONSUL_VERSION=1.15.4
# Mon, 07 Aug 2023 20:28:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:28:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:28:57 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:29:03 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:29:03 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:29:04 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:29:04 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:29:04 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:29:04 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:29:04 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:29:04 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:29:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:29:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3695f6c099b80e503148dbb435d044c35147f81d34b9d6fbb27b3dcf1fd7ecaf`  
		Last Modified: Mon, 07 Aug 2023 19:21:27 GMT  
		Size: 2.8 MB (2826006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e57e19f25baaa97592e47db7535a724f667d35f9de6ed142671f313f96eee0`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:020dc46acd18a2c8999d4763c6e77d0bfe6d89bee8f90b581171e4582183af10`  
		Last Modified: Mon, 07 Aug 2023 20:29:43 GMT  
		Size: 56.0 MB (56038439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcbd6cbb1fb5a20db7e9065b92e93bd157606712432d1f631a707e3193999770`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5ec2f78201a40a548d9ebe371908950e0770bf9e12ff06c6ceb9b1e17bca3c`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df296a8d036f48d36ed501d8c575e96fedda1bc82c19373f2f42b432d6df128d`  
		Last Modified: Mon, 07 Aug 2023 20:29:35 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:8012d555aa76088fe20156d9a053492c8dd0e9596e41752f7cc75520a35afa00
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.0 MB (56015232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c04630ac543532a256e0742de0c22dc75a8c7e4a2d2d8f077babcce2844874e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:32 GMT
ADD file:b987db82fa4ce6e623de49a50612c1fd91c5ab2209a62a5727ab3436c2923e91 in / 
# Wed, 14 Jun 2023 18:49:32 GMT
CMD ["/bin/sh"]
# Tue, 27 Jun 2023 18:49:14 GMT
ARG CONSUL_VERSION=1.15.4
# Tue, 27 Jun 2023 18:49:14 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Tue, 27 Jun 2023 18:49:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Tue, 27 Jun 2023 18:49:15 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN addgroup consul &&     adduser -S -G consul consul
# Tue, 27 Jun 2023 18:49:28 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Tue, 27 Jun 2023 18:49:29 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Tue, 27 Jun 2023 18:49:30 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 27 Jun 2023 18:49:30 GMT
VOLUME [/consul/data]
# Tue, 27 Jun 2023 18:49:30 GMT
EXPOSE 8300
# Tue, 27 Jun 2023 18:49:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Tue, 27 Jun 2023 18:49:30 GMT
EXPOSE 8500 8600 8600/udp
# Tue, 27 Jun 2023 18:49:30 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 27 Jun 2023 18:49:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 27 Jun 2023 18:49:30 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:41c5c5b38e13af18def277385607129664fb24993d262d4b601a381e776482a9`  
		Last Modified: Wed, 14 Jun 2023 18:50:19 GMT  
		Size: 2.6 MB (2633060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995469d5ed357beed1eda31495e57bd57a85c2b89a1ec2fd1e6ee44f93a1b675`  
		Last Modified: Tue, 27 Jun 2023 18:50:06 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9c2eed3d26135ba81af45e33b9bd97a7b6d41b6295a708c635e52b9566b77d2`  
		Last Modified: Tue, 27 Jun 2023 18:50:12 GMT  
		Size: 53.4 MB (53378742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cadac4432d1df266b13bee9cf95158f164dec415f8721abdc5b55da281a5843`  
		Last Modified: Tue, 27 Jun 2023 18:50:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657773322b04ff357b774d8f421c01115d5912e5d7142b7b935e13cfea146a3b`  
		Last Modified: Tue, 27 Jun 2023 18:50:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247eb5ea07e57d3de66278877506be864f2e41afa9d85b385548f2be15da69c0`  
		Last Modified: Tue, 27 Jun 2023 18:50:06 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15.4` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:3e252086ef0da34ea27c0dcfade9252444be163a6a18a16ebb24095c7ead916d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.6 MB (55603514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ea2b204bb98ec01683744f0991efb916fa505ec449149f9aff98a8645cb5f88`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:29 GMT
ADD file:21f240e1e33b25dacee7291cdd8c7750995aa0f460d13496a08c4a2dd92323aa in / 
# Mon, 07 Aug 2023 19:39:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:17:39 GMT
ARG CONSUL_VERSION=1.15.4
# Mon, 07 Aug 2023 20:17:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:17:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:17:39 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:17:45 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:17:46 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:17:46 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:17:46 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:17:46 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:17:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:17:47 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:17:47 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:17:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:17:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ad3fa0ea069c04e4ee9be58cf0ae9e1a8a56f649b96a96298203b055e8c903ff`  
		Last Modified: Mon, 07 Aug 2023 19:40:16 GMT  
		Size: 2.7 MB (2720868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc0ff86a773a4b23131c6a192cb6265108a9bb27f571f7dd5c7c6425dabdef4`  
		Last Modified: Mon, 07 Aug 2023 20:18:16 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a221f2346c39c3f6194efb140134f02a0685d643a5ea0d4814b4abef95e3afcd`  
		Last Modified: Mon, 07 Aug 2023 20:18:22 GMT  
		Size: 52.9 MB (52879216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30201693224304958e9ecef50dac60c54d179a6c785bd84f436809ee88120a3d`  
		Last Modified: Mon, 07 Aug 2023 20:18:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec582cf4de3bbc225cde18e26925f71e6de25d7b02d20398b9f27d709362fcd`  
		Last Modified: Mon, 07 Aug 2023 20:18:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be66a0761e47c07a158fa069bb3ea8990a042f836f552d64c89b29daaf4f449d`  
		Last Modified: Mon, 07 Aug 2023 20:18:16 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15.4` - linux; 386

```console
$ docker pull consul@sha256:df36500e40b488a5e2ba02c2d617dcebe2a6cecdb777579e651aeef499e1c295
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57428519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83c7c086b3b6c90d643222a2582b3fa6cace55846f3c83991e735660b909aea2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:38 GMT
ADD file:2d8ac62dd229ef26536f5a9af9e61df30ea68d609fa969786dfd531aea18cf3c in / 
# Mon, 07 Aug 2023 19:38:38 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:28:22 GMT
ARG CONSUL_VERSION=1.15.4
# Mon, 07 Aug 2023 20:28:22 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Mon, 07 Aug 2023 20:28:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 07 Aug 2023 20:28:23 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 07 Aug 2023 20:28:36 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 07 Aug 2023 20:28:36 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 07 Aug 2023 20:28:37 GMT
# ARGS: CONSUL_VERSION=1.15.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 07 Aug 2023 20:28:37 GMT
VOLUME [/consul/data]
# Mon, 07 Aug 2023 20:28:37 GMT
EXPOSE 8300
# Mon, 07 Aug 2023 20:28:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 07 Aug 2023 20:28:37 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 07 Aug 2023 20:28:38 GMT
COPY file:f5ba00fb9fd3a67a835a792e07b11da3b163222c18f8512aa772b36520d2a653 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 07 Aug 2023 20:28:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:28:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:add53095769493cde9110fd91f113357e53b9e0d94abf216b811fcf00107674e`  
		Last Modified: Mon, 07 Aug 2023 19:39:29 GMT  
		Size: 2.8 MB (2832316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839237463244ad8fa7addb4ee8b214ca710e9be73179f1a4d481c75fb6007553`  
		Last Modified: Mon, 07 Aug 2023 20:29:17 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d3a79e0e88ffed7a72946d5847aec4e35775bf9f5436a04eb00425712f0eaa`  
		Last Modified: Mon, 07 Aug 2023 20:29:26 GMT  
		Size: 54.6 MB (54592773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dc8a73d94f7aeb23b310e492bbe6faa3c194ba10785e5f5446758879acbd276`  
		Last Modified: Mon, 07 Aug 2023 20:29:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62687d6d763e66949be32cb9c9b4b38787ae35f407f59f6594421aee6de454cd`  
		Last Modified: Mon, 07 Aug 2023 20:29:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f0861dff5ccce5a271ba4a5a11fd46edadc6b527cd385eb060da57d5bb9816`  
		Last Modified: Mon, 07 Aug 2023 20:29:17 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
