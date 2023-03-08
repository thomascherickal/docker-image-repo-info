<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.13`](#consul113)
-	[`consul:1.13.7`](#consul1137)
-	[`consul:1.14`](#consul114)
-	[`consul:1.14.5`](#consul1145)
-	[`consul:1.15`](#consul115)
-	[`consul:1.15.1`](#consul1151)
-	[`consul:latest`](#consullatest)

## `consul:1.13`

```console
$ docker pull consul@sha256:9793f279c772eef0a6b7f1515072297d96b89fa998bef45807fadefa86c5396a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13` - linux; amd64

```console
$ docker pull consul@sha256:0015ec0747199b32abb071ec3d930570d0d5d62fc17af7d2c8788d81be0ccbb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52262347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966327d1c07f1973c56c359f805dd748c30a7d14810bcd8ded875a3439738fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:42:27 GMT
ARG CONSUL_VERSION=1.13.6
# Sat, 11 Feb 2023 07:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 11 Feb 2023 07:42:27 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 11 Feb 2023 07:42:28 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 11 Feb 2023 07:42:33 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 11 Feb 2023 07:42:34 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 11 Feb 2023 07:42:35 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 11 Feb 2023 07:42:35 GMT
VOLUME [/consul/data]
# Sat, 11 Feb 2023 07:42:35 GMT
EXPOSE 8300
# Sat, 11 Feb 2023 07:42:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 11 Feb 2023 07:42:35 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 11 Feb 2023 07:42:35 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 07:42:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 07:42:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c503564c0fee8dafc813caf8aec1a4c62114dc7cdbe18b0607a2467d39a9799e`  
		Last Modified: Sat, 11 Feb 2023 07:43:16 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06346382abe5a9ec96d5c299eafb8e44be7ffea6b2f22a4a92448137a7cbd19d`  
		Last Modified: Sat, 11 Feb 2023 07:43:22 GMT  
		Size: 49.4 MB (49432824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a5d487d3902df0932dc4b4e8749fd1be96713cc029134a5cd9cf209b67f48a`  
		Last Modified: Sat, 11 Feb 2023 07:43:16 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433be6497e10fab617cb2d6f8ef86360bfb0bd5e72370b6c73051185c7ad124d`  
		Last Modified: Sat, 11 Feb 2023 07:43:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4603bb92103758c0e9d8df33c4ea78aaa6f31e0867e1f9163dc49d1e18865a`  
		Last Modified: Sat, 11 Feb 2023 07:43:16 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm variant v6

```console
$ docker pull consul@sha256:175aa7fe7e859e02d65ee697db3e1d552a7757badc113ac48fd22c394ab1dc58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50888063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6ac1a5f63c3a86a03c16d2c8f2c9501921428da95664e4ec5aae20f5346054`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 19:49:50 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 08 Mar 2023 19:49:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 19:49:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 19:49:50 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 19:49:57 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 19:49:58 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 19:49:58 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 19:49:59 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 19:49:59 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 19:49:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 19:49:59 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 19:49:59 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 19:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 19:49:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef23f129ff09f6d0cd82cb6f79be06288467eafd2e7ff2423163f06247fef049`  
		Last Modified: Wed, 08 Mar 2023 19:51:01 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7873b4dd1c4fc69e1b2aedef64987d5bd6f1b0e8a0a2c5723fdefc7f3bc45f9a`  
		Last Modified: Wed, 08 Mar 2023 19:51:07 GMT  
		Size: 48.3 MB (48251028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ccdbfcbd94bd05182cdec5e1affa2ca0c7064882a06fd5327d8010e288a18d`  
		Last Modified: Wed, 08 Mar 2023 19:51:01 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316fb9a64f64055175d5d21c35b88aa131806a9ae11db672d00766e4546a383a`  
		Last Modified: Wed, 08 Mar 2023 19:51:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b45d251ef0330d6c52f39cbf36d7b2b96121b97056931912724afc9a15dc51`  
		Last Modified: Wed, 08 Mar 2023 19:51:01 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:cc34a54ce28264593ccfa395890a6687d22a7ba363a0a731248b7e1ce8da455f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49477028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4525bb7e0c28b613b571a39d5234a929f369694b167ba25560d386a3c5309d61`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:01:38 GMT
ARG CONSUL_VERSION=1.13.6
# Fri, 10 Feb 2023 22:01:38 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 10 Feb 2023 22:01:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 10 Feb 2023 22:01:38 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 10 Feb 2023 22:01:44 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 10 Feb 2023 22:01:45 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 10 Feb 2023 22:01:46 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 10 Feb 2023 22:01:46 GMT
VOLUME [/consul/data]
# Fri, 10 Feb 2023 22:01:46 GMT
EXPOSE 8300
# Fri, 10 Feb 2023 22:01:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 10 Feb 2023 22:01:46 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 10 Feb 2023 22:01:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:01:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:01:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478927a30de417c03bdd408b7ca5da00b21dc15193298aca9c443aecaaf793d9`  
		Last Modified: Fri, 10 Feb 2023 22:02:29 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01361edbe24ab319960c2afe4008ab6b2be34b7501a415ef27acc53310e7dff4`  
		Last Modified: Fri, 10 Feb 2023 22:02:33 GMT  
		Size: 46.8 MB (46752091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4bb18b1fc6d3283090e0200dd958c01dc19086beb605a3c93ba9b80b6634cf`  
		Last Modified: Fri, 10 Feb 2023 22:02:28 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbcb79adf5399e3b4d77c2afa78efdef76825f6253e474648c77199b77a90ac`  
		Last Modified: Fri, 10 Feb 2023 22:02:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd5fa1afae393b3e16ae75e072f091a42f8e532a2f21db71406ef9cb53ca702`  
		Last Modified: Fri, 10 Feb 2023 22:02:28 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13` - linux; 386

```console
$ docker pull consul@sha256:db2c353eb1d5321a4d05c3f4ac019607f33d8ff0e78090cea19df8c4b27388e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51104344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a889c33cf650dd0207e3bda14637c5e80ceb3e7fe97883dae9488d923ae35852`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:34 GMT
ADD file:35855658886412913d05c0f9e29bf8f650c0d37e20100a9de118b468f86f7f30 in / 
# Fri, 10 Feb 2023 21:24:34 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 07:45:56 GMT
ARG CONSUL_VERSION=1.13.6
# Sat, 25 Feb 2023 07:45:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 07:45:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 07:45:57 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 07:46:04 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 07:46:05 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 07:46:06 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 07:46:06 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 07:46:06 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 07:46:06 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 07:46:06 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 07:46:06 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 07:46:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 07:46:06 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13a1d7e543968b1c2bd92ca5f2fb2e964b31713fc7707305c1cdfb935ca3e631`  
		Last Modified: Fri, 10 Feb 2023 21:25:40 GMT  
		Size: 2.8 MB (2832331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946843a5234dd03d6030cbde75040b3392eee2660bcd414c51a9793a44bbef76`  
		Last Modified: Sat, 25 Feb 2023 07:47:09 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d640bdd14f36f3f009d8a581a11cb217bf1e7bc18618b4782585eb3cd1419485`  
		Last Modified: Sat, 25 Feb 2023 07:47:17 GMT  
		Size: 48.3 MB (48268634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75d6928e8a05e079aa98e30c34f7a695f4dc14b9c75303d15855a13b7b16e3e`  
		Last Modified: Sat, 25 Feb 2023 07:47:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15711d2bef344bb61ccd95512113952a76b85844ecc817b7be415e6cfc92fc1`  
		Last Modified: Sat, 25 Feb 2023 07:47:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fc492adda313e9e6506679d347972245cd4cbf161fe42e5722633117ab3c3a`  
		Last Modified: Sat, 25 Feb 2023 07:47:09 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.13.7`

```console
$ docker pull consul@sha256:174dcd022c13cca4c3cad02c97c76667d2ec835f3d25cf81d417241f72f8bd92
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `consul:1.13.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:175aa7fe7e859e02d65ee697db3e1d552a7757badc113ac48fd22c394ab1dc58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50888063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6ac1a5f63c3a86a03c16d2c8f2c9501921428da95664e4ec5aae20f5346054`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 19:49:50 GMT
ARG CONSUL_VERSION=1.13.7
# Wed, 08 Mar 2023 19:49:50 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.7 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 19:49:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 19:49:50 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 19:49:57 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 19:49:58 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 19:49:58 GMT
# ARGS: CONSUL_VERSION=1.13.7
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 19:49:59 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 19:49:59 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 19:49:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 19:49:59 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 19:49:59 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 19:49:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 19:49:59 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef23f129ff09f6d0cd82cb6f79be06288467eafd2e7ff2423163f06247fef049`  
		Last Modified: Wed, 08 Mar 2023 19:51:01 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7873b4dd1c4fc69e1b2aedef64987d5bd6f1b0e8a0a2c5723fdefc7f3bc45f9a`  
		Last Modified: Wed, 08 Mar 2023 19:51:07 GMT  
		Size: 48.3 MB (48251028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ccdbfcbd94bd05182cdec5e1affa2ca0c7064882a06fd5327d8010e288a18d`  
		Last Modified: Wed, 08 Mar 2023 19:51:01 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316fb9a64f64055175d5d21c35b88aa131806a9ae11db672d00766e4546a383a`  
		Last Modified: Wed, 08 Mar 2023 19:51:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b45d251ef0330d6c52f39cbf36d7b2b96121b97056931912724afc9a15dc51`  
		Last Modified: Wed, 08 Mar 2023 19:51:01 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.14`

```console
$ docker pull consul@sha256:5ebf7ff6f7457e65959ad855208aaff8d714e9fa4f8841a93d7acc7d26c76260
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14` - linux; amd64

```console
$ docker pull consul@sha256:a859fd24671b6baee53de25ca9aa19ccbc3b7fbb7afc8b20e92ee9ce835f00c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.3 MB (56316372 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:041dc476cc20f574ae7816f88da51c47f055f94053ad6d018e4d27bf8c5753a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 07:42:15 GMT
ARG CONSUL_VERSION=1.14.4
# Sat, 11 Feb 2023 07:42:15 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 11 Feb 2023 07:42:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 11 Feb 2023 07:42:16 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 11 Feb 2023 07:42:22 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 11 Feb 2023 07:42:22 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 11 Feb 2023 07:42:23 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 11 Feb 2023 07:42:23 GMT
VOLUME [/consul/data]
# Sat, 11 Feb 2023 07:42:23 GMT
EXPOSE 8300
# Sat, 11 Feb 2023 07:42:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 11 Feb 2023 07:42:23 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 11 Feb 2023 07:42:23 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 07:42:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 07:42:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8ecfd7194bf52cc635a09f166d65bd7e3e2606742a80b92b5f20f62e0dc5c9`  
		Last Modified: Sat, 11 Feb 2023 07:43:00 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68aafa623d724662b3de9830489da6d0c72f9a8c068008fe4c014d11a065fcb`  
		Last Modified: Sat, 11 Feb 2023 07:43:06 GMT  
		Size: 53.5 MB (53486847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cb2d1beebfdb525fec637835291e977821122b6ef2bb2ca0ead87c9846ef77`  
		Last Modified: Sat, 11 Feb 2023 07:43:00 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a563b41aad02911ebb8da0a822af67e06a9ad256e2a5c5f083fa3058938d90a7`  
		Last Modified: Sat, 11 Feb 2023 07:43:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9917a9cd9617563b1b88ebb2c1b3054e0f53c990c3c89c069bb4ca74b2713fcb`  
		Last Modified: Sat, 11 Feb 2023 07:43:00 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; arm variant v6

```console
$ docker pull consul@sha256:73d5be8c4aded4baa44b29f115942e28b244005020846cc46745be378cce3c2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53943357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b69ac5737413a460ec034c9e6e87576f40f2053610be75c564708f4c9692ed29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 19:49:37 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 08 Mar 2023 19:49:37 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 19:49:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 19:49:38 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 19:49:45 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 19:49:45 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 19:49:46 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 19:49:46 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 19:49:46 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 19:49:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 19:49:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 19:49:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 19:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 19:49:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f27e01b47cb95e665a2f42b1614da69eeb64ecf0426993694c2959f74bdb21`  
		Last Modified: Wed, 08 Mar 2023 19:50:44 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297d17a3352c621fa85086965e3f922c094f01fe6a2064d3243c91dda1dac2e6`  
		Last Modified: Wed, 08 Mar 2023 19:50:50 GMT  
		Size: 51.3 MB (51306320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f18e6466417c2b80e99cee3fe4f6816fd99b5a6956e3efb22d5151ac3dbdb09`  
		Last Modified: Wed, 08 Mar 2023 19:50:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd85e1b23685890b2df617ce295104d51f6fe1b41b2fc3a3f1fbf86eb6f11409`  
		Last Modified: Wed, 08 Mar 2023 19:50:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5e1b0709e2a076ea419b3e3ff4c5c43e1c09cdf5dfcc92fff96232ebb7d7c4`  
		Last Modified: Wed, 08 Mar 2023 19:50:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:57355f6f632f1a78305ffc430d940e6630c809eb9a80db54c498489dac3504a1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53141443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d655387a1164567de86de6dd008ac7777c23224421b37ede5ddec85dedbdaf2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:01:26 GMT
ARG CONSUL_VERSION=1.14.4
# Fri, 10 Feb 2023 22:01:26 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Fri, 10 Feb 2023 22:01:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 10 Feb 2023 22:01:27 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 10 Feb 2023 22:01:33 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 10 Feb 2023 22:01:34 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 10 Feb 2023 22:01:34 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 10 Feb 2023 22:01:34 GMT
VOLUME [/consul/data]
# Fri, 10 Feb 2023 22:01:34 GMT
EXPOSE 8300
# Fri, 10 Feb 2023 22:01:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 10 Feb 2023 22:01:35 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 10 Feb 2023 22:01:35 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:01:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:01:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5f5a93605265de2bf7d1ce0a04b31e9206424042dd482959fa40ae232e004c`  
		Last Modified: Fri, 10 Feb 2023 22:02:11 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2643ebb7531da6503768460e59c74886ed8290708898a767795e01cc43ff35d`  
		Last Modified: Fri, 10 Feb 2023 22:02:16 GMT  
		Size: 50.4 MB (50416508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d229f64652a58dfbe39028360c58d336eeb0d20c9d25472dd0530766bb84bf`  
		Last Modified: Fri, 10 Feb 2023 22:02:11 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833943f861feda487a0c0d67bd4db9cb122b2a3c32160d897d3b30ae71e01924`  
		Last Modified: Fri, 10 Feb 2023 22:02:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8986cc9f0209a2e424ae170ce3a41bdcf3a0e14e1d6ff01d0106d0c979a1eecb`  
		Last Modified: Fri, 10 Feb 2023 22:02:11 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14` - linux; 386

```console
$ docker pull consul@sha256:ec8ee2ae50cb780e8177e3d20262f2e0439164a3ee72606bc044d3b449c1d0e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.1 MB (55106489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b301d671c80261483c2afba3a052e11165598f087f0375feaccc123ea35d13`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:34 GMT
ADD file:35855658886412913d05c0f9e29bf8f650c0d37e20100a9de118b468f86f7f30 in / 
# Fri, 10 Feb 2023 21:24:34 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 07:45:44 GMT
ARG CONSUL_VERSION=1.14.4
# Sat, 25 Feb 2023 07:45:44 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 07:45:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 07:45:45 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 07:45:51 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 07:45:52 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 07:45:52 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 07:45:53 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 07:45:53 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 07:45:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 07:45:53 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 07:45:53 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 07:45:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 07:45:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13a1d7e543968b1c2bd92ca5f2fb2e964b31713fc7707305c1cdfb935ca3e631`  
		Last Modified: Fri, 10 Feb 2023 21:25:40 GMT  
		Size: 2.8 MB (2832331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501fa0d2270d99410b804c51c9a48310c830527e0373d235ddd9a73fb19a0d9d`  
		Last Modified: Sat, 25 Feb 2023 07:46:51 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38627f00c0d2c5e6f7a70c7645c533ea9aac2d58c156aa621fdcc724a3e236e`  
		Last Modified: Sat, 25 Feb 2023 07:46:59 GMT  
		Size: 52.3 MB (52270781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d38c3f60ea18c0dbd484ee641ec5591162d2bf439a605df9fda1cc14742c0a`  
		Last Modified: Sat, 25 Feb 2023 07:46:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49a7c0c142b459d073e80adf615a89c7f0e72c5072ad4ea6f832dd5f02fb799`  
		Last Modified: Sat, 25 Feb 2023 07:46:51 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca7a4f11aaf919b50b93b8068034bbd8f58e77cfd91e9cd99dd3d85fa27d4c2`  
		Last Modified: Sat, 25 Feb 2023 07:46:51 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.14.5`

```console
$ docker pull consul@sha256:233fa301390eda272d51c8ef3bbf23b03028db2764a7493829eb6e4268302b4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `consul:1.14.5` - linux; arm variant v6

```console
$ docker pull consul@sha256:73d5be8c4aded4baa44b29f115942e28b244005020846cc46745be378cce3c2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.9 MB (53943357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b69ac5737413a460ec034c9e6e87576f40f2053610be75c564708f4c9692ed29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 19:49:37 GMT
ARG CONSUL_VERSION=1.14.5
# Wed, 08 Mar 2023 19:49:37 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.5 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 19:49:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 19:49:38 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 19:49:45 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 19:49:45 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 19:49:46 GMT
# ARGS: CONSUL_VERSION=1.14.5
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 19:49:46 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 19:49:46 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 19:49:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 19:49:46 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 19:49:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 19:49:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 19:49:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f27e01b47cb95e665a2f42b1614da69eeb64ecf0426993694c2959f74bdb21`  
		Last Modified: Wed, 08 Mar 2023 19:50:44 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297d17a3352c621fa85086965e3f922c094f01fe6a2064d3243c91dda1dac2e6`  
		Last Modified: Wed, 08 Mar 2023 19:50:50 GMT  
		Size: 51.3 MB (51306320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f18e6466417c2b80e99cee3fe4f6816fd99b5a6956e3efb22d5151ac3dbdb09`  
		Last Modified: Wed, 08 Mar 2023 19:50:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd85e1b23685890b2df617ce295104d51f6fe1b41b2fc3a3f1fbf86eb6f11409`  
		Last Modified: Wed, 08 Mar 2023 19:50:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5e1b0709e2a076ea419b3e3ff4c5c43e1c09cdf5dfcc92fff96232ebb7d7c4`  
		Last Modified: Wed, 08 Mar 2023 19:50:44 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.15`

```console
$ docker pull consul@sha256:2942008c40b7d720f4e879872acb230f47b68e1cf9f848596485ed87454df4d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.15` - linux; amd64

```console
$ docker pull consul@sha256:61821744f422575e14dc2e71e884cbc9890942a0fc5bfdffa77a044cfc11ab61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57850971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9976413d3a8199bbdc513bff41028d8b638395ea76387dc3e9989316ba6936`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 00:36:36 GMT
ARG CONSUL_VERSION=1.15.0
# Sat, 25 Feb 2023 00:36:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 00:36:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 00:36:37 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 00:36:44 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 00:36:45 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 00:36:46 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 00:36:46 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 00:36:46 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 00:36:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 00:36:46 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 00:36:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 00:36:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 00:36:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd42e3c5627afe1a57d4230be5dc11b0c1de3e793939a10bc9aa4ff9836517f5`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51dfee8f0af07ba1221883e60ce52f0205c116d4946b2beb6e1587ecf2c0023`  
		Last Modified: Sat, 25 Feb 2023 00:37:11 GMT  
		Size: 55.0 MB (55021446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfbefd36cf65c7bdef5ef877f0e20ff7e6bcf6a77a92aebb718168ded978643`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e952e991c0aa96b1d031d8c08e85b06d7a99d339bee758fa79bf3c6d4fccec4f`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6d554e81cd6ac67ccad4bfeea60bf62a2e6ae7a26ca8a48049191118415a90`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15` - linux; arm variant v6

```console
$ docker pull consul@sha256:adcf8d842097f380014cb9e0131cec76868ce257d5bc9216d24ac1f95e290bc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.4 MB (55446504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f44aac14a1ae89c1fcc960a020c1530fc7720cf23aa188b1d342c43429226c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 19:49:19 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 08 Mar 2023 19:49:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 19:49:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 19:49:20 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 19:49:29 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 19:49:30 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 19:49:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 19:49:31 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 19:49:31 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 19:49:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 19:49:31 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 19:49:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 19:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 19:49:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff914a8109146895cb1fe14d712fc33bb9c03739484d2ad93282bae602c1dfe1`  
		Last Modified: Wed, 08 Mar 2023 19:50:22 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1a9d819dbd7cba07bd74163f219b9c3ebd4db3b86b26b8b67ecdfd0797d75f`  
		Last Modified: Wed, 08 Mar 2023 19:50:28 GMT  
		Size: 52.8 MB (52809472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c51b881df972b13d5d89622495dad00c655780c955a4a5adce748d1a7e9fd6`  
		Last Modified: Wed, 08 Mar 2023 19:50:22 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754c59cf1a0c78bd07f1fc2858585b0ef4c27947baab5a810df1ffdc64e98ea`  
		Last Modified: Wed, 08 Mar 2023 19:50:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b3caf70cb5b2f9223c0582616d563e67432885d8904c1314a18b72beb5262a`  
		Last Modified: Wed, 08 Mar 2023 19:50:21 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:c5f3fe77d3c8b1b81e543b82e46643cff93f1e4ef2c6d62f9bcfdcb6b20ec923
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54574164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca40d8f6ba01cfb2597b7f52356ec21aa14b249613d6f04f5155f9dc5a15fbe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 01:21:30 GMT
ARG CONSUL_VERSION=1.15.0
# Sat, 25 Feb 2023 01:21:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 01:21:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 01:21:31 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 01:21:36 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 01:21:38 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 01:21:38 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 01:21:38 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 01:21:38 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 01:21:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 01:21:38 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 01:21:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 01:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 01:21:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f216e177df132c82fd24465f65346f46c4cd4b09f3e2bbd0531df38b921593fc`  
		Last Modified: Sat, 25 Feb 2023 01:21:55 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a09089494b024ce326ad5140007ce551c0b4510372ef3ebd7c494043651e7ee`  
		Last Modified: Sat, 25 Feb 2023 01:22:01 GMT  
		Size: 51.8 MB (51849230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2501fa3ea5460f16ea46fa3816756598a9517b1ac357d155e4054291ce65146b`  
		Last Modified: Sat, 25 Feb 2023 01:21:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9fd5c0bdabea77df1b82eb2f4ea581dbf10c960d1f5af61a7cb2ed3ab50e51`  
		Last Modified: Sat, 25 Feb 2023 01:21:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116c9d8f034dc32e99023debebaec89a9afab24975adde1c93119d48165f0b05`  
		Last Modified: Sat, 25 Feb 2023 01:21:55 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15` - linux; 386

```console
$ docker pull consul@sha256:30ca7af17b319e25e603ccf2dcd9b79288ce54090c42c4d7c376fa9068f8ce9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56467775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b47bc4707499c7dd01f766746e0766f73d2d69ef0ef5006750f9ab25c4cefe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:34 GMT
ADD file:35855658886412913d05c0f9e29bf8f650c0d37e20100a9de118b468f86f7f30 in / 
# Fri, 10 Feb 2023 21:24:34 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 07:45:29 GMT
ARG CONSUL_VERSION=1.15.0
# Sat, 25 Feb 2023 07:45:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 07:45:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 07:45:30 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 07:45:38 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 07:45:39 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 07:45:40 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 07:45:40 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 07:45:40 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 07:45:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 07:45:40 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 07:45:40 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 07:45:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 07:45:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13a1d7e543968b1c2bd92ca5f2fb2e964b31713fc7707305c1cdfb935ca3e631`  
		Last Modified: Fri, 10 Feb 2023 21:25:40 GMT  
		Size: 2.8 MB (2832331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d10cb28cec66b11197c600ad55cf3f47d249f67c6eb6d437c5576ddd38bd29`  
		Last Modified: Sat, 25 Feb 2023 07:46:29 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead3da331181adb8ca1138d414e9a5b1196d9358b08a2df35b40ef5e6d8bd342`  
		Last Modified: Sat, 25 Feb 2023 07:46:38 GMT  
		Size: 53.6 MB (53632065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e7e93cb8697b7b99a339d6cda3eee3b3016861a303ab9bad1446749e209050`  
		Last Modified: Sat, 25 Feb 2023 07:46:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331791ab913c681bb08fe440e3d2e3d3d17e68160c08210b36b0b288c3accdc8`  
		Last Modified: Sat, 25 Feb 2023 07:46:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a564f0c931d70c31343449949582e13677bda54baeedb27407283b12ecdefe`  
		Last Modified: Sat, 25 Feb 2023 07:46:29 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.15.1`

```console
$ docker pull consul@sha256:7ecd6ccd971e8f6070b996ce82827571e3240dc24c596859d7b64c00127e4676
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `consul:1.15.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:adcf8d842097f380014cb9e0131cec76868ce257d5bc9216d24ac1f95e290bc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.4 MB (55446504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f44aac14a1ae89c1fcc960a020c1530fc7720cf23aa188b1d342c43429226c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 19:49:19 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 08 Mar 2023 19:49:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 19:49:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 19:49:20 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 19:49:29 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 19:49:30 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 19:49:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 19:49:31 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 19:49:31 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 19:49:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 19:49:31 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 19:49:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 19:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 19:49:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff914a8109146895cb1fe14d712fc33bb9c03739484d2ad93282bae602c1dfe1`  
		Last Modified: Wed, 08 Mar 2023 19:50:22 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1a9d819dbd7cba07bd74163f219b9c3ebd4db3b86b26b8b67ecdfd0797d75f`  
		Last Modified: Wed, 08 Mar 2023 19:50:28 GMT  
		Size: 52.8 MB (52809472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c51b881df972b13d5d89622495dad00c655780c955a4a5adce748d1a7e9fd6`  
		Last Modified: Wed, 08 Mar 2023 19:50:22 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754c59cf1a0c78bd07f1fc2858585b0ef4c27947baab5a810df1ffdc64e98ea`  
		Last Modified: Wed, 08 Mar 2023 19:50:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b3caf70cb5b2f9223c0582616d563e67432885d8904c1314a18b72beb5262a`  
		Last Modified: Wed, 08 Mar 2023 19:50:21 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:2942008c40b7d720f4e879872acb230f47b68e1cf9f848596485ed87454df4d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:61821744f422575e14dc2e71e884cbc9890942a0fc5bfdffa77a044cfc11ab61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.9 MB (57850971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb9976413d3a8199bbdc513bff41028d8b638395ea76387dc3e9989316ba6936`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:54 GMT
ADD file:cdac18271416ac5bf6876b7ea9af1129108d03f9813589dfda113e5f09d6b80b in / 
# Sat, 11 Feb 2023 04:46:55 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 00:36:36 GMT
ARG CONSUL_VERSION=1.15.0
# Sat, 25 Feb 2023 00:36:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 00:36:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 00:36:37 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 00:36:44 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 00:36:45 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 00:36:46 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 00:36:46 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 00:36:46 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 00:36:46 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 00:36:46 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 00:36:46 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 00:36:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 00:36:46 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:895e193edb5191bf66fb5ccb29f5d3659e05eec5953255180cbdd66520e7c517`  
		Last Modified: Sat, 11 Feb 2023 04:47:40 GMT  
		Size: 2.8 MB (2826146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd42e3c5627afe1a57d4230be5dc11b0c1de3e793939a10bc9aa4ff9836517f5`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51dfee8f0af07ba1221883e60ce52f0205c116d4946b2beb6e1587ecf2c0023`  
		Last Modified: Sat, 25 Feb 2023 00:37:11 GMT  
		Size: 55.0 MB (55021446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dfbefd36cf65c7bdef5ef877f0e20ff7e6bcf6a77a92aebb718168ded978643`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e952e991c0aa96b1d031d8c08e85b06d7a99d339bee758fa79bf3c6d4fccec4f`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6d554e81cd6ac67ccad4bfeea60bf62a2e6ae7a26ca8a48049191118415a90`  
		Last Modified: Sat, 25 Feb 2023 00:37:04 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:adcf8d842097f380014cb9e0131cec76868ce257d5bc9216d24ac1f95e290bc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.4 MB (55446504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62f44aac14a1ae89c1fcc960a020c1530fc7720cf23aa188b1d342c43429226c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Wed, 08 Mar 2023 19:49:19 GMT
ARG CONSUL_VERSION=1.15.1
# Wed, 08 Mar 2023 19:49:19 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Wed, 08 Mar 2023 19:49:19 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 08 Mar 2023 19:49:20 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 08 Mar 2023 19:49:29 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 08 Mar 2023 19:49:30 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 08 Mar 2023 19:49:31 GMT
# ARGS: CONSUL_VERSION=1.15.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 08 Mar 2023 19:49:31 GMT
VOLUME [/consul/data]
# Wed, 08 Mar 2023 19:49:31 GMT
EXPOSE 8300
# Wed, 08 Mar 2023 19:49:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 08 Mar 2023 19:49:31 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 08 Mar 2023 19:49:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 08 Mar 2023 19:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 08 Mar 2023 19:49:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff914a8109146895cb1fe14d712fc33bb9c03739484d2ad93282bae602c1dfe1`  
		Last Modified: Wed, 08 Mar 2023 19:50:22 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1a9d819dbd7cba07bd74163f219b9c3ebd4db3b86b26b8b67ecdfd0797d75f`  
		Last Modified: Wed, 08 Mar 2023 19:50:28 GMT  
		Size: 52.8 MB (52809472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79c51b881df972b13d5d89622495dad00c655780c955a4a5adce748d1a7e9fd6`  
		Last Modified: Wed, 08 Mar 2023 19:50:22 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3754c59cf1a0c78bd07f1fc2858585b0ef4c27947baab5a810df1ffdc64e98ea`  
		Last Modified: Wed, 08 Mar 2023 19:50:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b3caf70cb5b2f9223c0582616d563e67432885d8904c1314a18b72beb5262a`  
		Last Modified: Wed, 08 Mar 2023 19:50:21 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:c5f3fe77d3c8b1b81e543b82e46643cff93f1e4ef2c6d62f9bcfdcb6b20ec923
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.6 MB (54574164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca40d8f6ba01cfb2597b7f52356ec21aa14b249613d6f04f5155f9dc5a15fbe3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:16 GMT
ADD file:a73970ac03f28a1d3b9aaee19e859d958867b42fb91f29efb1259fbddc66ffb1 in / 
# Fri, 10 Feb 2023 21:24:16 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 01:21:30 GMT
ARG CONSUL_VERSION=1.15.0
# Sat, 25 Feb 2023 01:21:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 01:21:30 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 01:21:31 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 01:21:36 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 01:21:38 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 01:21:38 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 01:21:38 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 01:21:38 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 01:21:38 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 01:21:38 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 01:21:38 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 01:21:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 01:21:39 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:404f35918b797abb27547df3b530ec55a77c499c4dce88f3b90867115087f9e7`  
		Last Modified: Fri, 10 Feb 2023 21:25:01 GMT  
		Size: 2.7 MB (2721556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f216e177df132c82fd24465f65346f46c4cd4b09f3e2bbd0531df38b921593fc`  
		Last Modified: Sat, 25 Feb 2023 01:21:55 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a09089494b024ce326ad5140007ce551c0b4510372ef3ebd7c494043651e7ee`  
		Last Modified: Sat, 25 Feb 2023 01:22:01 GMT  
		Size: 51.8 MB (51849230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2501fa3ea5460f16ea46fa3816756598a9517b1ac357d155e4054291ce65146b`  
		Last Modified: Sat, 25 Feb 2023 01:21:56 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9fd5c0bdabea77df1b82eb2f4ea581dbf10c960d1f5af61a7cb2ed3ab50e51`  
		Last Modified: Sat, 25 Feb 2023 01:21:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116c9d8f034dc32e99023debebaec89a9afab24975adde1c93119d48165f0b05`  
		Last Modified: Sat, 25 Feb 2023 01:21:55 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:30ca7af17b319e25e603ccf2dcd9b79288ce54090c42c4d7c376fa9068f8ce9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.5 MB (56467775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1b47bc4707499c7dd01f766746e0766f73d2d69ef0ef5006750f9ab25c4cefe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:34 GMT
ADD file:35855658886412913d05c0f9e29bf8f650c0d37e20100a9de118b468f86f7f30 in / 
# Fri, 10 Feb 2023 21:24:34 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 07:45:29 GMT
ARG CONSUL_VERSION=1.15.0
# Sat, 25 Feb 2023 07:45:29 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 07:45:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 07:45:30 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 07:45:38 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 07:45:39 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 07:45:40 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 07:45:40 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 07:45:40 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 07:45:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 07:45:40 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 07:45:40 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 07:45:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 07:45:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13a1d7e543968b1c2bd92ca5f2fb2e964b31713fc7707305c1cdfb935ca3e631`  
		Last Modified: Fri, 10 Feb 2023 21:25:40 GMT  
		Size: 2.8 MB (2832331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d10cb28cec66b11197c600ad55cf3f47d249f67c6eb6d437c5576ddd38bd29`  
		Last Modified: Sat, 25 Feb 2023 07:46:29 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead3da331181adb8ca1138d414e9a5b1196d9358b08a2df35b40ef5e6d8bd342`  
		Last Modified: Sat, 25 Feb 2023 07:46:38 GMT  
		Size: 53.6 MB (53632065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e7e93cb8697b7b99a339d6cda3eee3b3016861a303ab9bad1446749e209050`  
		Last Modified: Sat, 25 Feb 2023 07:46:30 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331791ab913c681bb08fe440e3d2e3d3d17e68160c08210b36b0b288c3accdc8`  
		Last Modified: Sat, 25 Feb 2023 07:46:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a564f0c931d70c31343449949582e13677bda54baeedb27407283b12ecdefe`  
		Last Modified: Sat, 25 Feb 2023 07:46:29 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
