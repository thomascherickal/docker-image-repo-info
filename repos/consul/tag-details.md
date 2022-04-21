<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10`](#consul110)
-	[`consul:1.10.10`](#consul11010)
-	[`consul:1.11`](#consul111)
-	[`consul:1.11.5`](#consul1115)
-	[`consul:1.12`](#consul112)
-	[`consul:1.12.0`](#consul1120)
-	[`consul:latest`](#consullatest)

## `consul:1.10`

```console
$ docker pull consul@sha256:f651f363dc2e7d584d62cf1d84ea3c5ea09a35165addbb155332010cb2b2f8ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10` - linux; amd64

```console
$ docker pull consul@sha256:6083bc7e57d07989b58dce7b8ca2a0902c0843c406c98fa1a3e74603f42c8b2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43228177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0389f092a2bcf559540a11b017b02761fdac2b4c1475df36f3903b052616ab3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:19:39 GMT
ARG CONSUL_VERSION=1.10.10
# Thu, 14 Apr 2022 21:19:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:19:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:19:40 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:19:45 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:19:46 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:19:46 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:19:47 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:19:47 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:19:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:19:47 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:19:47 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:19:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cab786757fed054cbfaa6d7116f3af44b3dff148660e4c2ec2caac248d2e297`  
		Last Modified: Thu, 14 Apr 2022 21:20:30 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e60da82695debbf1d2a2db4b6de25c80045384801acab93bd3ecde8e9b9a541`  
		Last Modified: Thu, 14 Apr 2022 21:20:36 GMT  
		Size: 40.4 MB (40405502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f665e8f72d209104cd80dc001e1624417498b4c7039c3931ea4d7dd879aaebd`  
		Last Modified: Thu, 14 Apr 2022 21:20:30 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380c036c11378772bdb5b4c2f15df1ddcffd289cc7954dd5aa19406b93aa90ac`  
		Last Modified: Thu, 14 Apr 2022 21:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ec8ad9dff37376f540924bd2349e5a69c67df95ffd648c00fc30c40403b6aa`  
		Last Modified: Thu, 14 Apr 2022 21:20:30 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:626631c2bd87cdbccca1cc2ef099ee8248f9d53ce1ffa64346548e5b9d348b83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41020630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0242cf13dd3cdaf3ffe1e45fe8b95741f58e699e3a8569c38024de7f0df7370f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:50:05 GMT
ARG CONSUL_VERSION=1.10.10
# Thu, 14 Apr 2022 21:50:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:50:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:50:07 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:50:18 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:50:20 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:50:22 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:50:22 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:50:23 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:50:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:50:23 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:50:24 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:50:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:50:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9ea8375347b802ef63c38fb4123ad74917227975abb167f478fdd8d42a967f`  
		Last Modified: Thu, 14 Apr 2022 21:52:15 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f8d6a6270a54ae69897fb9019f5242aa511410a3c63ddb7ae07310fec3c0a4`  
		Last Modified: Thu, 14 Apr 2022 21:52:36 GMT  
		Size: 38.4 MB (38392115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db8e53501743a8917f498f67acd41b0e4d487085e9a1d88afbe9776281f9d2b`  
		Last Modified: Thu, 14 Apr 2022 21:52:15 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ea1f6514d2f42c69edfc79ae49fc590dba7a67dd1d3ae6aa5dad1ef54a69f9`  
		Last Modified: Thu, 14 Apr 2022 21:52:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a69f7cfa3085d5dea82e15ed2f4a258b0bfb496c123ab3c29e655c5894ad06`  
		Last Modified: Thu, 14 Apr 2022 21:52:15 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:0eab7b191ac3ca65ebb22704b741c54912332dac1e15ba37302ad8ab46b60432
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40865538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf34f476c2132c965c3352ff4f542615eb4a07d8bf0b46d2a06d339818188fc6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:39:54 GMT
ARG CONSUL_VERSION=1.10.10
# Thu, 14 Apr 2022 21:39:55 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:39:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:39:57 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:40:03 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:40:03 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:40:04 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:40:05 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:40:06 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:40:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:40:08 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:40:10 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:40:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59529c14dc1d7ee875407ee3e54eb9b13cafadb9674302e31d0d6573f0a9b520`  
		Last Modified: Thu, 14 Apr 2022 21:41:46 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04621dd6226cc60c10b4018a82c59a356f9f0010084f3a756a4cdd170d279c6b`  
		Last Modified: Thu, 14 Apr 2022 21:41:53 GMT  
		Size: 38.1 MB (38141335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1ec5ad62042b469cb30c7ca75694d54a0f85f19d801999eed8331e03da176f`  
		Last Modified: Thu, 14 Apr 2022 21:41:49 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a254e3a66bd1cc3078961a23c87e4b155c7b9a7ba6c962629d532c44c03c670`  
		Last Modified: Thu, 14 Apr 2022 21:41:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca4603fcdb34fa2f5077da535163fed4247e39fe645aa93c4253f740683653c`  
		Last Modified: Thu, 14 Apr 2022 21:41:48 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; 386

```console
$ docker pull consul@sha256:2168439ea833e969ba85cde1adb53d8b59f61606592508a52b0a190b2a6fdf98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42062660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68bf4e4133a7e177bfd14d0a522e3b4658641d72185804d38acda121a3987168`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:38:48 GMT
ARG CONSUL_VERSION=1.10.10
# Thu, 14 Apr 2022 21:38:49 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:38:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:38:51 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:38:56 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:38:57 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:38:58 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:38:59 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:39:00 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:39:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:39:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:39:04 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:39:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40455caf5eeef1290acfcf755598d444a7d6626a7f53b57188db9500ef08fe95`  
		Last Modified: Thu, 14 Apr 2022 21:40:09 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2607cdb8c9a308104e98ca4b3ed055d4ad7e1383355167a5b8f372e1fcc2e4d`  
		Last Modified: Thu, 14 Apr 2022 21:40:19 GMT  
		Size: 39.2 MB (39238818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21edf415f990f983e9caf3c818ee60e3c5c1ada137eb4a322da960db5636a857`  
		Last Modified: Thu, 14 Apr 2022 21:40:09 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b749149f7d9dc0efb53cdcfa18c8a718c5825eec86f00d095d21717c50380dd6`  
		Last Modified: Thu, 14 Apr 2022 21:40:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0a5c09591d38148e5428f0b170d486e917df824e2042fa05893ec38065cd0f`  
		Last Modified: Thu, 14 Apr 2022 21:40:09 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.10`

```console
$ docker pull consul@sha256:f651f363dc2e7d584d62cf1d84ea3c5ea09a35165addbb155332010cb2b2f8ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10.10` - linux; amd64

```console
$ docker pull consul@sha256:6083bc7e57d07989b58dce7b8ca2a0902c0843c406c98fa1a3e74603f42c8b2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43228177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0389f092a2bcf559540a11b017b02761fdac2b4c1475df36f3903b052616ab3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:19:39 GMT
ARG CONSUL_VERSION=1.10.10
# Thu, 14 Apr 2022 21:19:39 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:19:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:19:40 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:19:45 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:19:46 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:19:46 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:19:47 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:19:47 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:19:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:19:47 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:19:47 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:19:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:19:47 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cab786757fed054cbfaa6d7116f3af44b3dff148660e4c2ec2caac248d2e297`  
		Last Modified: Thu, 14 Apr 2022 21:20:30 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e60da82695debbf1d2a2db4b6de25c80045384801acab93bd3ecde8e9b9a541`  
		Last Modified: Thu, 14 Apr 2022 21:20:36 GMT  
		Size: 40.4 MB (40405502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f665e8f72d209104cd80dc001e1624417498b4c7039c3931ea4d7dd879aaebd`  
		Last Modified: Thu, 14 Apr 2022 21:20:30 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380c036c11378772bdb5b4c2f15df1ddcffd289cc7954dd5aa19406b93aa90ac`  
		Last Modified: Thu, 14 Apr 2022 21:20:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ec8ad9dff37376f540924bd2349e5a69c67df95ffd648c00fc30c40403b6aa`  
		Last Modified: Thu, 14 Apr 2022 21:20:30 GMT  
		Size: 1.8 KB (1782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:626631c2bd87cdbccca1cc2ef099ee8248f9d53ce1ffa64346548e5b9d348b83
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41020630 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0242cf13dd3cdaf3ffe1e45fe8b95741f58e699e3a8569c38024de7f0df7370f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:50:05 GMT
ARG CONSUL_VERSION=1.10.10
# Thu, 14 Apr 2022 21:50:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:50:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:50:07 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:50:18 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:50:20 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:50:22 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:50:22 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:50:23 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:50:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:50:23 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:50:24 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:50:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:50:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9ea8375347b802ef63c38fb4123ad74917227975abb167f478fdd8d42a967f`  
		Last Modified: Thu, 14 Apr 2022 21:52:15 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f8d6a6270a54ae69897fb9019f5242aa511410a3c63ddb7ae07310fec3c0a4`  
		Last Modified: Thu, 14 Apr 2022 21:52:36 GMT  
		Size: 38.4 MB (38392115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db8e53501743a8917f498f67acd41b0e4d487085e9a1d88afbe9776281f9d2b`  
		Last Modified: Thu, 14 Apr 2022 21:52:15 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ea1f6514d2f42c69edfc79ae49fc590dba7a67dd1d3ae6aa5dad1ef54a69f9`  
		Last Modified: Thu, 14 Apr 2022 21:52:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a69f7cfa3085d5dea82e15ed2f4a258b0bfb496c123ab3c29e655c5894ad06`  
		Last Modified: Thu, 14 Apr 2022 21:52:15 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:0eab7b191ac3ca65ebb22704b741c54912332dac1e15ba37302ad8ab46b60432
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40865538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf34f476c2132c965c3352ff4f542615eb4a07d8bf0b46d2a06d339818188fc6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:39:54 GMT
ARG CONSUL_VERSION=1.10.10
# Thu, 14 Apr 2022 21:39:55 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:39:56 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:39:57 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:40:03 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:40:03 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:40:04 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:40:05 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:40:06 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:40:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:40:08 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:40:10 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:40:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59529c14dc1d7ee875407ee3e54eb9b13cafadb9674302e31d0d6573f0a9b520`  
		Last Modified: Thu, 14 Apr 2022 21:41:46 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04621dd6226cc60c10b4018a82c59a356f9f0010084f3a756a4cdd170d279c6b`  
		Last Modified: Thu, 14 Apr 2022 21:41:53 GMT  
		Size: 38.1 MB (38141335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1ec5ad62042b469cb30c7ca75694d54a0f85f19d801999eed8331e03da176f`  
		Last Modified: Thu, 14 Apr 2022 21:41:49 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a254e3a66bd1cc3078961a23c87e4b155c7b9a7ba6c962629d532c44c03c670`  
		Last Modified: Thu, 14 Apr 2022 21:41:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca4603fcdb34fa2f5077da535163fed4247e39fe645aa93c4253f740683653c`  
		Last Modified: Thu, 14 Apr 2022 21:41:48 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10.10` - linux; 386

```console
$ docker pull consul@sha256:2168439ea833e969ba85cde1adb53d8b59f61606592508a52b0a190b2a6fdf98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42062660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68bf4e4133a7e177bfd14d0a522e3b4658641d72185804d38acda121a3987168`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:38:48 GMT
ARG CONSUL_VERSION=1.10.10
# Thu, 14 Apr 2022 21:38:49 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.10 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:38:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:38:51 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:38:56 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:38:57 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:38:58 GMT
# ARGS: CONSUL_VERSION=1.10.10
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:38:59 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:39:00 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:39:01 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:39:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:39:04 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:39:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40455caf5eeef1290acfcf755598d444a7d6626a7f53b57188db9500ef08fe95`  
		Last Modified: Thu, 14 Apr 2022 21:40:09 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2607cdb8c9a308104e98ca4b3ed055d4ad7e1383355167a5b8f372e1fcc2e4d`  
		Last Modified: Thu, 14 Apr 2022 21:40:19 GMT  
		Size: 39.2 MB (39238818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21edf415f990f983e9caf3c818ee60e3c5c1ada137eb4a322da960db5636a857`  
		Last Modified: Thu, 14 Apr 2022 21:40:09 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b749149f7d9dc0efb53cdcfa18c8a718c5825eec86f00d095d21717c50380dd6`  
		Last Modified: Thu, 14 Apr 2022 21:40:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0a5c09591d38148e5428f0b170d486e917df824e2042fa05893ec38065cd0f`  
		Last Modified: Thu, 14 Apr 2022 21:40:09 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11`

```console
$ docker pull consul@sha256:e9c02f6f912037d4b394062ce36743600a8e8f767c0f921a60fcb5c2ae285a23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11` - linux; amd64

```console
$ docker pull consul@sha256:a24f8b7e304d00f0aebfb896d1660370501d42769e03d777e8fde57abe6a200a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43954472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94840f9c3d714de6095d3aa1ecd3c1eecf18b08949b2f4872eaf730dee42b1cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:19:28 GMT
ARG CONSUL_VERSION=1.11.5
# Thu, 14 Apr 2022 21:19:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:19:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:19:29 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:19:34 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:19:35 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:19:36 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:19:36 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:19:36 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:19:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:19:36 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:19:36 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:19:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:19:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366e176f83f6feafec08fea5425e8ec846949df9c588dc803bede95b1cd76c15`  
		Last Modified: Thu, 14 Apr 2022 21:20:12 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3904ba849427da5c7775593539c1602dbd2b485737bd6b834b9292141c273b`  
		Last Modified: Thu, 14 Apr 2022 21:20:18 GMT  
		Size: 41.1 MB (41131797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dc1ee883bcf746b7818d21793756259a11b84efef9290267fc1909f324cf9c`  
		Last Modified: Thu, 14 Apr 2022 21:20:12 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c6f99a54b8a09665a2d1207f397c7fc7cb88820a66ff4610b727ec40715542`  
		Last Modified: Thu, 14 Apr 2022 21:20:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d084a8149104cb332535bd837732450d3cc7cf33b6ad885ffb04cb37f71a5187`  
		Last Modified: Thu, 14 Apr 2022 21:20:12 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:1cdca51f17bf9aca52600f38df9aad40234f43b62dfde291962d5b285d8dc91c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41721348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a18040b3e0efb314ad1b2fc113d154437be3b51529e0fffd451381953942af7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:49:32 GMT
ARG CONSUL_VERSION=1.11.5
# Thu, 14 Apr 2022 21:49:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:49:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:49:34 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:49:47 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:49:48 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:49:50 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:49:50 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:49:51 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:49:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:49:51 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:49:52 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:49:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:49:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9346852fac22a2ec32562eb6fa36581f2203d6b47fe3c2f212a89f56208bca09`  
		Last Modified: Thu, 14 Apr 2022 21:51:37 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7e99322feb2f96cf1b2c6e31c12fe2d1c8ddb268dcc816e0a682f219d1194b`  
		Last Modified: Thu, 14 Apr 2022 21:51:59 GMT  
		Size: 39.1 MB (39092831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6e56cd91c75f6279226badfe1a53a6da1847b4c5ebfab9f45d0f32d5dc255a`  
		Last Modified: Thu, 14 Apr 2022 21:51:38 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdafac0ee59a68a70cb10a3ef56fbeb9ac3831a683c1388038d3dd2c1e45ce0`  
		Last Modified: Thu, 14 Apr 2022 21:51:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20e49d22288c98a327fc957f2a1510e9f200543c949cea5ec1d354205d67bb4`  
		Last Modified: Thu, 14 Apr 2022 21:51:38 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:6384c74ef13620dd0a1c4a7b2f0dc612068efb0e4fd3c1efc2e9e5c75a51ba26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41544558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fefa898eb6965c609dbea2c7bf9c1cedaada6d0ce2dcf967a62441331907e59d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:39:30 GMT
ARG CONSUL_VERSION=1.11.5
# Thu, 14 Apr 2022 21:39:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:39:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:39:33 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:39:40 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:39:40 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:39:41 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:39:42 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:39:43 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:39:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:39:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:39:47 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:39:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ba83fc8974ffe9ca2de6ccfe65988eb1a36e7023d174deab4891b44ee64c7`  
		Last Modified: Thu, 14 Apr 2022 21:40:55 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872ba7fca95b7eebc6bf1ad851d1438e7b455db74d07369d00715ac330a3d4c7`  
		Last Modified: Thu, 14 Apr 2022 21:41:09 GMT  
		Size: 38.8 MB (38820352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb3a46b024bb0414904dd2a30f39d396f568b1d3f1c152412a4747c2bad50f`  
		Last Modified: Thu, 14 Apr 2022 21:40:58 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9298fc2536c2f846eb65eaf4f86631d07b60a49a49d6e6a1fec58129f1e777f8`  
		Last Modified: Thu, 14 Apr 2022 21:40:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0995681561d4261543a5804d8a830837c81ccdcd05a582fed7c4d6fdd03fd762`  
		Last Modified: Thu, 14 Apr 2022 21:40:55 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; 386

```console
$ docker pull consul@sha256:18b30515ca1134ffec0fed1304ef7843894abbb8ea383bc16649cb05329700f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42780475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c351b51815219a300fef1851c647afa6caeb61028935e2e6947c52a9b90dc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:38:22 GMT
ARG CONSUL_VERSION=1.11.5
# Thu, 14 Apr 2022 21:38:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:38:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:38:25 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:38:34 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:38:34 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:38:35 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:38:36 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:38:37 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:38:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:38:39 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:38:41 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:38:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1240e0b759fa3b673d08e0a90fbfc3e55713d526a19d514e3188f53d82918f`  
		Last Modified: Thu, 14 Apr 2022 21:39:50 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998e9c6ae24e5d10e9306c4d3bc666fca9348348dbd75a953e85cb86a8a5d3be`  
		Last Modified: Thu, 14 Apr 2022 21:39:55 GMT  
		Size: 40.0 MB (39956634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7106c7efa0be61d96bfd7cfafec1cc50d9623140c778790c290ee223902cff85`  
		Last Modified: Thu, 14 Apr 2022 21:39:50 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bff8f0aa095bd8bdbc5b1e1e4dc4b45413f9d453c752a89af27be0ba3fca5a`  
		Last Modified: Thu, 14 Apr 2022 21:39:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017abf7b48af0d7d95d7cdcb70351746484b3063c5682336431340e81631fce`  
		Last Modified: Thu, 14 Apr 2022 21:39:50 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.5`

```console
$ docker pull consul@sha256:e9c02f6f912037d4b394062ce36743600a8e8f767c0f921a60fcb5c2ae285a23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11.5` - linux; amd64

```console
$ docker pull consul@sha256:a24f8b7e304d00f0aebfb896d1660370501d42769e03d777e8fde57abe6a200a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43954472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94840f9c3d714de6095d3aa1ecd3c1eecf18b08949b2f4872eaf730dee42b1cd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:19:28 GMT
ARG CONSUL_VERSION=1.11.5
# Thu, 14 Apr 2022 21:19:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:19:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:19:29 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:19:34 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:19:35 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:19:36 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:19:36 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:19:36 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:19:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:19:36 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:19:36 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:19:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:19:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366e176f83f6feafec08fea5425e8ec846949df9c588dc803bede95b1cd76c15`  
		Last Modified: Thu, 14 Apr 2022 21:20:12 GMT  
		Size: 1.2 KB (1250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3904ba849427da5c7775593539c1602dbd2b485737bd6b834b9292141c273b`  
		Last Modified: Thu, 14 Apr 2022 21:20:18 GMT  
		Size: 41.1 MB (41131797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5dc1ee883bcf746b7818d21793756259a11b84efef9290267fc1909f324cf9c`  
		Last Modified: Thu, 14 Apr 2022 21:20:12 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c6f99a54b8a09665a2d1207f397c7fc7cb88820a66ff4610b727ec40715542`  
		Last Modified: Thu, 14 Apr 2022 21:20:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d084a8149104cb332535bd837732450d3cc7cf33b6ad885ffb04cb37f71a5187`  
		Last Modified: Thu, 14 Apr 2022 21:20:12 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.5` - linux; arm variant v6

```console
$ docker pull consul@sha256:1cdca51f17bf9aca52600f38df9aad40234f43b62dfde291962d5b285d8dc91c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41721348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a18040b3e0efb314ad1b2fc113d154437be3b51529e0fffd451381953942af7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:49:32 GMT
ARG CONSUL_VERSION=1.11.5
# Thu, 14 Apr 2022 21:49:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:49:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:49:34 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:49:47 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:49:48 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:49:50 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:49:50 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:49:51 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:49:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:49:51 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:49:52 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:49:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:49:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9346852fac22a2ec32562eb6fa36581f2203d6b47fe3c2f212a89f56208bca09`  
		Last Modified: Thu, 14 Apr 2022 21:51:37 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7e99322feb2f96cf1b2c6e31c12fe2d1c8ddb268dcc816e0a682f219d1194b`  
		Last Modified: Thu, 14 Apr 2022 21:51:59 GMT  
		Size: 39.1 MB (39092831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6e56cd91c75f6279226badfe1a53a6da1847b4c5ebfab9f45d0f32d5dc255a`  
		Last Modified: Thu, 14 Apr 2022 21:51:38 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdafac0ee59a68a70cb10a3ef56fbeb9ac3831a683c1388038d3dd2c1e45ce0`  
		Last Modified: Thu, 14 Apr 2022 21:51:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20e49d22288c98a327fc957f2a1510e9f200543c949cea5ec1d354205d67bb4`  
		Last Modified: Thu, 14 Apr 2022 21:51:38 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.5` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:6384c74ef13620dd0a1c4a7b2f0dc612068efb0e4fd3c1efc2e9e5c75a51ba26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41544558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fefa898eb6965c609dbea2c7bf9c1cedaada6d0ce2dcf967a62441331907e59d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:39:30 GMT
ARG CONSUL_VERSION=1.11.5
# Thu, 14 Apr 2022 21:39:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:39:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:39:33 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:39:40 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:39:40 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:39:41 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:39:42 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:39:43 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:39:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:39:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:39:47 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:39:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ba83fc8974ffe9ca2de6ccfe65988eb1a36e7023d174deab4891b44ee64c7`  
		Last Modified: Thu, 14 Apr 2022 21:40:55 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872ba7fca95b7eebc6bf1ad851d1438e7b455db74d07369d00715ac330a3d4c7`  
		Last Modified: Thu, 14 Apr 2022 21:41:09 GMT  
		Size: 38.8 MB (38820352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb3a46b024bb0414904dd2a30f39d396f568b1d3f1c152412a4747c2bad50f`  
		Last Modified: Thu, 14 Apr 2022 21:40:58 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9298fc2536c2f846eb65eaf4f86631d07b60a49a49d6e6a1fec58129f1e777f8`  
		Last Modified: Thu, 14 Apr 2022 21:40:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0995681561d4261543a5804d8a830837c81ccdcd05a582fed7c4d6fdd03fd762`  
		Last Modified: Thu, 14 Apr 2022 21:40:55 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11.5` - linux; 386

```console
$ docker pull consul@sha256:18b30515ca1134ffec0fed1304ef7843894abbb8ea383bc16649cb05329700f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42780475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c351b51815219a300fef1851c647afa6caeb61028935e2e6947c52a9b90dc7a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:38:22 GMT
ARG CONSUL_VERSION=1.11.5
# Thu, 14 Apr 2022 21:38:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:38:24 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:38:25 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:38:34 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:38:34 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:38:35 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:38:36 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:38:37 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:38:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:38:39 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:38:41 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:38:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:38:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b1240e0b759fa3b673d08e0a90fbfc3e55713d526a19d514e3188f53d82918f`  
		Last Modified: Thu, 14 Apr 2022 21:39:50 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998e9c6ae24e5d10e9306c4d3bc666fca9348348dbd75a953e85cb86a8a5d3be`  
		Last Modified: Thu, 14 Apr 2022 21:39:55 GMT  
		Size: 40.0 MB (39956634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7106c7efa0be61d96bfd7cfafec1cc50d9623140c778790c290ee223902cff85`  
		Last Modified: Thu, 14 Apr 2022 21:39:50 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01bff8f0aa095bd8bdbc5b1e1e4dc4b45413f9d453c752a89af27be0ba3fca5a`  
		Last Modified: Thu, 14 Apr 2022 21:39:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f017abf7b48af0d7d95d7cdcb70351746484b3063c5682336431340e81631fce`  
		Last Modified: Thu, 14 Apr 2022 21:39:50 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12`

```console
$ docker pull consul@sha256:72f0af9d3c1b8cb7d155416d68e5ce87d197d1720cf226985c49733105459a1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; 386

### `consul:1.12` - linux; amd64

```console
$ docker pull consul@sha256:e3eca84d5ff52bb0ac7ace85ad62b3b24eaf0f2f5c0a3e93b6560cd2405c2152
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49482668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5df7112c9dda54f532a46b1fdc3cb89ca137917c5843aeeebe291259a5ad3b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Thu, 21 Apr 2022 11:44:01 GMT
ARG CONSUL_VERSION=1.12.0
# Thu, 21 Apr 2022 11:44:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 21 Apr 2022 11:44:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Apr 2022 11:44:02 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Apr 2022 11:44:07 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Apr 2022 11:44:08 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Apr 2022 11:44:08 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Apr 2022 11:44:09 GMT
VOLUME [/consul/data]
# Thu, 21 Apr 2022 11:44:09 GMT
EXPOSE 8300
# Thu, 21 Apr 2022 11:44:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Apr 2022 11:44:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Apr 2022 11:44:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Apr 2022 11:44:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 11:44:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eaba874f54c72be4510131c30d5e7e9cf13730a59e4a00b8ea6fbfaf03758`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c25e7029524e8fcb858836ad4bdd5d77f917faac9354b858f6a35ba68acc70`  
		Last Modified: Thu, 21 Apr 2022 11:44:30 GMT  
		Size: 46.7 MB (46659990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4e30fdd8786d3cd5fc51b01827c51e2da03862df6f7e54fbe4191fb30925d0`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404bba1e3035647d3126bbd7e4e185569d77185bfc76b79787f5ea26997adf2`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0267f66d5e7e019e1d8c0167f5e672f9c0fee5e0fd012da55614a52af9d64b4e`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; arm variant v6

```console
$ docker pull consul@sha256:f7cd3d8b1ce65ec05bf34c7c634164a7e109ffd24bf1afcc2fedfc7fe371dba5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47360944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae7d169deff3ee350ee3045c8014b90d0c4683236da625077b09752dba083d40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Thu, 21 Apr 2022 00:04:24 GMT
ARG CONSUL_VERSION=1.12.0
# Thu, 21 Apr 2022 00:04:25 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 21 Apr 2022 00:04:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Apr 2022 00:04:31 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Apr 2022 00:04:49 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Apr 2022 00:04:55 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Apr 2022 00:05:00 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Apr 2022 00:05:00 GMT
VOLUME [/consul/data]
# Thu, 21 Apr 2022 00:05:01 GMT
EXPOSE 8300
# Thu, 21 Apr 2022 00:05:02 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Apr 2022 00:05:03 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Apr 2022 00:05:05 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Apr 2022 00:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 00:05:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36aa94121a2db80c6e4b353603909ee487e9a1650e86b8e8d1573d52fa03c45`  
		Last Modified: Thu, 21 Apr 2022 00:06:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0cc44b42ed5e016eb276e18680f5c6e16fa7e9fa579b92bc01c966cb6782f3`  
		Last Modified: Thu, 21 Apr 2022 00:06:36 GMT  
		Size: 44.7 MB (44732427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04080b49a8e9747a531f857b11027f9e8044e363fe3150daa0bea9d99055d50`  
		Last Modified: Thu, 21 Apr 2022 00:06:11 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d011bfa36c14bab9d43017308ba5a57121f5925540d21a4c2f295f30c8a6138`  
		Last Modified: Thu, 21 Apr 2022 00:06:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc1dd017c3ebab8824689b1af78412a7842106ba1ee8832c181b0f30a967b73`  
		Last Modified: Thu, 21 Apr 2022 00:06:11 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12` - linux; 386

```console
$ docker pull consul@sha256:3faef884d4731795971556dc6a845088ca9955456496325f39b480e30b69554b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48548561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a8c9785d37c5a3ec12138e3c1d53f417e0d0f7a843f97a10a411fafb9cb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Thu, 21 Apr 2022 02:08:09 GMT
ARG CONSUL_VERSION=1.12.0
# Thu, 21 Apr 2022 02:08:10 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 21 Apr 2022 02:08:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Apr 2022 02:08:12 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Apr 2022 02:08:20 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Apr 2022 02:08:20 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Apr 2022 02:08:21 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Apr 2022 02:08:22 GMT
VOLUME [/consul/data]
# Thu, 21 Apr 2022 02:08:23 GMT
EXPOSE 8300
# Thu, 21 Apr 2022 02:08:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Apr 2022 02:08:25 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Apr 2022 02:08:27 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Apr 2022 02:08:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 02:08:28 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3c3a5b846afbcaeecb22d985a5d900806ba229bc87d910ffe1f07ebd4943d7`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d520059bb9b811f92275db02d0a1941bd3bb21c81d7bc542204979f686c70bb0`  
		Last Modified: Thu, 21 Apr 2022 02:09:07 GMT  
		Size: 45.7 MB (45724718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6865f4c431db9e37e48149944b32fef7e11614794c5412b2712a707d482cec84`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ce93115025a22775d6c5c26b04b66c4ce502d090e62967443d439e0cfb1181`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9830e46d08be08c43eddd9fa87624663ba00f52292e8457a66c7bac0bb71597`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.12.0`

```console
$ docker pull consul@sha256:72f0af9d3c1b8cb7d155416d68e5ce87d197d1720cf226985c49733105459a1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; 386

### `consul:1.12.0` - linux; amd64

```console
$ docker pull consul@sha256:e3eca84d5ff52bb0ac7ace85ad62b3b24eaf0f2f5c0a3e93b6560cd2405c2152
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49482668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5df7112c9dda54f532a46b1fdc3cb89ca137917c5843aeeebe291259a5ad3b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Thu, 21 Apr 2022 11:44:01 GMT
ARG CONSUL_VERSION=1.12.0
# Thu, 21 Apr 2022 11:44:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 21 Apr 2022 11:44:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Apr 2022 11:44:02 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Apr 2022 11:44:07 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Apr 2022 11:44:08 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Apr 2022 11:44:08 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Apr 2022 11:44:09 GMT
VOLUME [/consul/data]
# Thu, 21 Apr 2022 11:44:09 GMT
EXPOSE 8300
# Thu, 21 Apr 2022 11:44:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Apr 2022 11:44:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Apr 2022 11:44:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Apr 2022 11:44:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 11:44:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eaba874f54c72be4510131c30d5e7e9cf13730a59e4a00b8ea6fbfaf03758`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c25e7029524e8fcb858836ad4bdd5d77f917faac9354b858f6a35ba68acc70`  
		Last Modified: Thu, 21 Apr 2022 11:44:30 GMT  
		Size: 46.7 MB (46659990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4e30fdd8786d3cd5fc51b01827c51e2da03862df6f7e54fbe4191fb30925d0`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404bba1e3035647d3126bbd7e4e185569d77185bfc76b79787f5ea26997adf2`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0267f66d5e7e019e1d8c0167f5e672f9c0fee5e0fd012da55614a52af9d64b4e`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.0` - linux; arm variant v6

```console
$ docker pull consul@sha256:f7cd3d8b1ce65ec05bf34c7c634164a7e109ffd24bf1afcc2fedfc7fe371dba5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47360944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae7d169deff3ee350ee3045c8014b90d0c4683236da625077b09752dba083d40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Thu, 21 Apr 2022 00:04:24 GMT
ARG CONSUL_VERSION=1.12.0
# Thu, 21 Apr 2022 00:04:25 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 21 Apr 2022 00:04:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Apr 2022 00:04:31 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Apr 2022 00:04:49 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Apr 2022 00:04:55 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Apr 2022 00:05:00 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Apr 2022 00:05:00 GMT
VOLUME [/consul/data]
# Thu, 21 Apr 2022 00:05:01 GMT
EXPOSE 8300
# Thu, 21 Apr 2022 00:05:02 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Apr 2022 00:05:03 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Apr 2022 00:05:05 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Apr 2022 00:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 00:05:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36aa94121a2db80c6e4b353603909ee487e9a1650e86b8e8d1573d52fa03c45`  
		Last Modified: Thu, 21 Apr 2022 00:06:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0cc44b42ed5e016eb276e18680f5c6e16fa7e9fa579b92bc01c966cb6782f3`  
		Last Modified: Thu, 21 Apr 2022 00:06:36 GMT  
		Size: 44.7 MB (44732427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04080b49a8e9747a531f857b11027f9e8044e363fe3150daa0bea9d99055d50`  
		Last Modified: Thu, 21 Apr 2022 00:06:11 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d011bfa36c14bab9d43017308ba5a57121f5925540d21a4c2f295f30c8a6138`  
		Last Modified: Thu, 21 Apr 2022 00:06:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc1dd017c3ebab8824689b1af78412a7842106ba1ee8832c181b0f30a967b73`  
		Last Modified: Thu, 21 Apr 2022 00:06:11 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.12.0` - linux; 386

```console
$ docker pull consul@sha256:3faef884d4731795971556dc6a845088ca9955456496325f39b480e30b69554b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48548561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a8c9785d37c5a3ec12138e3c1d53f417e0d0f7a843f97a10a411fafb9cb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Thu, 21 Apr 2022 02:08:09 GMT
ARG CONSUL_VERSION=1.12.0
# Thu, 21 Apr 2022 02:08:10 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 21 Apr 2022 02:08:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Apr 2022 02:08:12 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Apr 2022 02:08:20 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Apr 2022 02:08:20 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Apr 2022 02:08:21 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Apr 2022 02:08:22 GMT
VOLUME [/consul/data]
# Thu, 21 Apr 2022 02:08:23 GMT
EXPOSE 8300
# Thu, 21 Apr 2022 02:08:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Apr 2022 02:08:25 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Apr 2022 02:08:27 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Apr 2022 02:08:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 02:08:28 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3c3a5b846afbcaeecb22d985a5d900806ba229bc87d910ffe1f07ebd4943d7`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d520059bb9b811f92275db02d0a1941bd3bb21c81d7bc542204979f686c70bb0`  
		Last Modified: Thu, 21 Apr 2022 02:09:07 GMT  
		Size: 45.7 MB (45724718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6865f4c431db9e37e48149944b32fef7e11614794c5412b2712a707d482cec84`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ce93115025a22775d6c5c26b04b66c4ce502d090e62967443d439e0cfb1181`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9830e46d08be08c43eddd9fa87624663ba00f52292e8457a66c7bac0bb71597`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:f9214db7c1c9cbdced0ea66331802f6c17a7c1db9821e3eb77fdedee7061d569
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:e3eca84d5ff52bb0ac7ace85ad62b3b24eaf0f2f5c0a3e93b6560cd2405c2152
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49482668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5df7112c9dda54f532a46b1fdc3cb89ca137917c5843aeeebe291259a5ad3b3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Thu, 21 Apr 2022 11:44:01 GMT
ARG CONSUL_VERSION=1.12.0
# Thu, 21 Apr 2022 11:44:01 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 21 Apr 2022 11:44:01 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Apr 2022 11:44:02 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Apr 2022 11:44:07 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Apr 2022 11:44:08 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Apr 2022 11:44:08 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Apr 2022 11:44:09 GMT
VOLUME [/consul/data]
# Thu, 21 Apr 2022 11:44:09 GMT
EXPOSE 8300
# Thu, 21 Apr 2022 11:44:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Apr 2022 11:44:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Apr 2022 11:44:09 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Apr 2022 11:44:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 11:44:09 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5eaba874f54c72be4510131c30d5e7e9cf13730a59e4a00b8ea6fbfaf03758`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 1.3 KB (1253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c25e7029524e8fcb858836ad4bdd5d77f917faac9354b858f6a35ba68acc70`  
		Last Modified: Thu, 21 Apr 2022 11:44:30 GMT  
		Size: 46.7 MB (46659990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4e30fdd8786d3cd5fc51b01827c51e2da03862df6f7e54fbe4191fb30925d0`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0404bba1e3035647d3126bbd7e4e185569d77185bfc76b79787f5ea26997adf2`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0267f66d5e7e019e1d8c0167f5e672f9c0fee5e0fd012da55614a52af9d64b4e`  
		Last Modified: Thu, 21 Apr 2022 11:44:25 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:f7cd3d8b1ce65ec05bf34c7c634164a7e109ffd24bf1afcc2fedfc7fe371dba5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47360944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae7d169deff3ee350ee3045c8014b90d0c4683236da625077b09752dba083d40`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:50:07 GMT
ADD file:9e96de1fefc4e9efba26e76103eca5f1495f00a66a8d8207d493fa9eabed19c0 in / 
# Mon, 04 Apr 2022 23:50:07 GMT
CMD ["/bin/sh"]
# Thu, 21 Apr 2022 00:04:24 GMT
ARG CONSUL_VERSION=1.12.0
# Thu, 21 Apr 2022 00:04:25 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 21 Apr 2022 00:04:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Apr 2022 00:04:31 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Apr 2022 00:04:49 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Apr 2022 00:04:55 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Apr 2022 00:05:00 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Apr 2022 00:05:00 GMT
VOLUME [/consul/data]
# Thu, 21 Apr 2022 00:05:01 GMT
EXPOSE 8300
# Thu, 21 Apr 2022 00:05:02 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Apr 2022 00:05:03 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Apr 2022 00:05:05 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Apr 2022 00:05:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 00:05:07 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:83a39d5693a8029bb5246b7d72205357bcd5d8306489b586abf44bc8659dfc1e`  
		Last Modified: Mon, 04 Apr 2022 23:51:58 GMT  
		Size: 2.6 MB (2625144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36aa94121a2db80c6e4b353603909ee487e9a1650e86b8e8d1573d52fa03c45`  
		Last Modified: Thu, 21 Apr 2022 00:06:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0cc44b42ed5e016eb276e18680f5c6e16fa7e9fa579b92bc01c966cb6782f3`  
		Last Modified: Thu, 21 Apr 2022 00:06:36 GMT  
		Size: 44.7 MB (44732427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04080b49a8e9747a531f857b11027f9e8044e363fe3150daa0bea9d99055d50`  
		Last Modified: Thu, 21 Apr 2022 00:06:11 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d011bfa36c14bab9d43017308ba5a57121f5925540d21a4c2f295f30c8a6138`  
		Last Modified: Thu, 21 Apr 2022 00:06:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc1dd017c3ebab8824689b1af78412a7842106ba1ee8832c181b0f30a967b73`  
		Last Modified: Thu, 21 Apr 2022 00:06:11 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:6384c74ef13620dd0a1c4a7b2f0dc612068efb0e4fd3c1efc2e9e5c75a51ba26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41544558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fefa898eb6965c609dbea2c7bf9c1cedaada6d0ce2dcf967a62441331907e59d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Thu, 14 Apr 2022 21:39:30 GMT
ARG CONSUL_VERSION=1.11.5
# Thu, 14 Apr 2022 21:39:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 14 Apr 2022 21:39:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 14 Apr 2022 21:39:33 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 14 Apr 2022 21:39:40 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 14 Apr 2022 21:39:40 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 14 Apr 2022 21:39:41 GMT
# ARGS: CONSUL_VERSION=1.11.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 21:39:42 GMT
VOLUME [/consul/data]
# Thu, 14 Apr 2022 21:39:43 GMT
EXPOSE 8300
# Thu, 14 Apr 2022 21:39:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 14 Apr 2022 21:39:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 14 Apr 2022 21:39:47 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Apr 2022 21:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Apr 2022 21:39:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ba83fc8974ffe9ca2de6ccfe65988eb1a36e7023d174deab4891b44ee64c7`  
		Last Modified: Thu, 14 Apr 2022 21:40:55 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872ba7fca95b7eebc6bf1ad851d1438e7b455db74d07369d00715ac330a3d4c7`  
		Last Modified: Thu, 14 Apr 2022 21:41:09 GMT  
		Size: 38.8 MB (38820352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb3a46b024bb0414904dd2a30f39d396f568b1d3f1c152412a4747c2bad50f`  
		Last Modified: Thu, 14 Apr 2022 21:40:58 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9298fc2536c2f846eb65eaf4f86631d07b60a49a49d6e6a1fec58129f1e777f8`  
		Last Modified: Thu, 14 Apr 2022 21:40:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0995681561d4261543a5804d8a830837c81ccdcd05a582fed7c4d6fdd03fd762`  
		Last Modified: Thu, 14 Apr 2022 21:40:55 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:3faef884d4731795971556dc6a845088ca9955456496325f39b480e30b69554b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48548561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b61a8c9785d37c5a3ec12138e3c1d53f417e0d0f7a843f97a10a411fafb9cb4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:38 GMT
ADD file:caa278dc5cc6257518d542227fef491a89b0b4a7fc4dcb87632c2b786b65752a in / 
# Mon, 04 Apr 2022 23:38:38 GMT
CMD ["/bin/sh"]
# Thu, 21 Apr 2022 02:08:09 GMT
ARG CONSUL_VERSION=1.12.0
# Thu, 21 Apr 2022 02:08:10 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.12.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 21 Apr 2022 02:08:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 21 Apr 2022 02:08:12 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 21 Apr 2022 02:08:20 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 21 Apr 2022 02:08:20 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 21 Apr 2022 02:08:21 GMT
# ARGS: CONSUL_VERSION=1.12.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 21 Apr 2022 02:08:22 GMT
VOLUME [/consul/data]
# Thu, 21 Apr 2022 02:08:23 GMT
EXPOSE 8300
# Thu, 21 Apr 2022 02:08:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 21 Apr 2022 02:08:25 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 21 Apr 2022 02:08:27 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 21 Apr 2022 02:08:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Apr 2022 02:08:28 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:54c95c2f58283907ca735a3fe8d3ac4a49a63dc20092eb6fddd7bad2429e3f67`  
		Last Modified: Mon, 04 Apr 2022 23:39:46 GMT  
		Size: 2.8 MB (2820530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3c3a5b846afbcaeecb22d985a5d900806ba229bc87d910ffe1f07ebd4943d7`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d520059bb9b811f92275db02d0a1941bd3bb21c81d7bc542204979f686c70bb0`  
		Last Modified: Thu, 21 Apr 2022 02:09:07 GMT  
		Size: 45.7 MB (45724718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6865f4c431db9e37e48149944b32fef7e11614794c5412b2712a707d482cec84`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ce93115025a22775d6c5c26b04b66c4ce502d090e62967443d439e0cfb1181`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9830e46d08be08c43eddd9fa87624663ba00f52292e8457a66c7bac0bb71597`  
		Last Modified: Thu, 21 Apr 2022 02:09:01 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
