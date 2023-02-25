<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.13`](#consul113)
-	[`consul:1.13.6`](#consul1136)
-	[`consul:1.14`](#consul114)
-	[`consul:1.14.4`](#consul1144)
-	[`consul:1.15`](#consul115)
-	[`consul:1.15.0`](#consul1150)
-	[`consul:latest`](#consullatest)

## `consul:1.13`

```console
$ docker pull consul@sha256:89699b645f70e88f0b87099cc9788ea62bce74dedf689ac39a41b0b047b80df5
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
$ docker pull consul@sha256:332f18a8527593d2563c9b833e162a92575a999135901694b59b5969bf02084b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (49993183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:304db82c19680784e71e6520cef4a224d21164e886baabe64451cbbb300a5e85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 02:33:36 GMT
ARG CONSUL_VERSION=1.13.6
# Sat, 25 Feb 2023 02:33:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 02:33:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 02:33:37 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 02:33:43 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 02:33:44 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 02:33:44 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 02:33:45 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 02:33:45 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 02:33:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 02:33:45 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 02:33:45 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 02:33:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 02:33:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66476844e684c33303f8b58239a3c8bc6e40c0501fa81ba14558fff65e799087`  
		Last Modified: Sat, 25 Feb 2023 02:34:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4712b4435bf9c4135cf59572dbabf757964253d21c60e5f5f2982681aa4c3011`  
		Last Modified: Sat, 25 Feb 2023 02:34:52 GMT  
		Size: 47.4 MB (47356154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d50ed81cb1d14a20bcc43d0fc403848978215da2166265bed3191bd4877f572`  
		Last Modified: Sat, 25 Feb 2023 02:34:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff024acb2fb9cb4877b9fcf24cea0575e528ae7d8fe50f0a5e0bfb327cfe191`  
		Last Modified: Sat, 25 Feb 2023 02:34:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a6f74c3a375f6b5f0f572eed3afaf223306e8bbf9cdb1ffda61365785e44`  
		Last Modified: Sat, 25 Feb 2023 02:34:45 GMT  
		Size: 1.8 KB (1786 bytes)  
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

## `consul:1.13.6`

```console
$ docker pull consul@sha256:89699b645f70e88f0b87099cc9788ea62bce74dedf689ac39a41b0b047b80df5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.13.6` - linux; amd64

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

### `consul:1.13.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:332f18a8527593d2563c9b833e162a92575a999135901694b59b5969bf02084b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.0 MB (49993183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:304db82c19680784e71e6520cef4a224d21164e886baabe64451cbbb300a5e85`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 02:33:36 GMT
ARG CONSUL_VERSION=1.13.6
# Sat, 25 Feb 2023 02:33:36 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 02:33:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 02:33:37 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 02:33:43 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 02:33:44 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 02:33:44 GMT
# ARGS: CONSUL_VERSION=1.13.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 02:33:45 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 02:33:45 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 02:33:45 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 02:33:45 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 02:33:45 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 02:33:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 02:33:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66476844e684c33303f8b58239a3c8bc6e40c0501fa81ba14558fff65e799087`  
		Last Modified: Sat, 25 Feb 2023 02:34:45 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4712b4435bf9c4135cf59572dbabf757964253d21c60e5f5f2982681aa4c3011`  
		Last Modified: Sat, 25 Feb 2023 02:34:52 GMT  
		Size: 47.4 MB (47356154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d50ed81cb1d14a20bcc43d0fc403848978215da2166265bed3191bd4877f572`  
		Last Modified: Sat, 25 Feb 2023 02:34:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff024acb2fb9cb4877b9fcf24cea0575e528ae7d8fe50f0a5e0bfb327cfe191`  
		Last Modified: Sat, 25 Feb 2023 02:34:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5869a6f74c3a375f6b5f0f572eed3afaf223306e8bbf9cdb1ffda61365785e44`  
		Last Modified: Sat, 25 Feb 2023 02:34:45 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.13.6` - linux; arm64 variant v8

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

### `consul:1.13.6` - linux; 386

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

## `consul:1.14`

```console
$ docker pull consul@sha256:5f3ac2854fe282542a00f6ed43d53fe9f82d3d3c2fae56a52db12c668ad558e2
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
$ docker pull consul@sha256:cab243ed17b11c1a0f83725189c45efe69220c244bab8ee4f6d0bebab09a3635
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53715728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f85beef2e073a569ffa2272a0cde01e88c6dacbd8cea5b11e2cf31cea83498e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 02:33:23 GMT
ARG CONSUL_VERSION=1.14.4
# Sat, 25 Feb 2023 02:33:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 02:33:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 02:33:24 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 02:33:30 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 02:33:31 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 02:33:31 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 02:33:32 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 02:33:32 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 02:33:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 02:33:32 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 02:33:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 02:33:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 02:33:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3f5a1168744f7ebd06856d9d53f89eb95795f7c90944d3a104a18c68685d47`  
		Last Modified: Sat, 25 Feb 2023 02:34:28 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97f60086ee52d11bc7ba54212f27e9f572c66b8214f74dd166f3769cb69d205`  
		Last Modified: Sat, 25 Feb 2023 02:34:35 GMT  
		Size: 51.1 MB (51078697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7e963515ef8c3d4c33fa57b2810a7a3257bb83b085d8f5a2b31d4f0c2226a`  
		Last Modified: Sat, 25 Feb 2023 02:34:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eeec2615e0a915f4bcf2cab37a175bc5340d1882c15275a199cecf45e3906d6`  
		Last Modified: Sat, 25 Feb 2023 02:34:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9bedbd2b663733d1b427681701aa7b7ada96d02848563e0c4ef7a282b951b`  
		Last Modified: Sat, 25 Feb 2023 02:34:28 GMT  
		Size: 1.8 KB (1786 bytes)  
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

## `consul:1.14.4`

```console
$ docker pull consul@sha256:5f3ac2854fe282542a00f6ed43d53fe9f82d3d3c2fae56a52db12c668ad558e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.14.4` - linux; amd64

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

### `consul:1.14.4` - linux; arm variant v6

```console
$ docker pull consul@sha256:cab243ed17b11c1a0f83725189c45efe69220c244bab8ee4f6d0bebab09a3635
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.7 MB (53715728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f85beef2e073a569ffa2272a0cde01e88c6dacbd8cea5b11e2cf31cea83498e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 02:33:23 GMT
ARG CONSUL_VERSION=1.14.4
# Sat, 25 Feb 2023 02:33:23 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.14.4 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 02:33:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 02:33:24 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 02:33:30 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 02:33:31 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 02:33:31 GMT
# ARGS: CONSUL_VERSION=1.14.4
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 02:33:32 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 02:33:32 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 02:33:32 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 02:33:32 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 02:33:32 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 02:33:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 02:33:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3f5a1168744f7ebd06856d9d53f89eb95795f7c90944d3a104a18c68685d47`  
		Last Modified: Sat, 25 Feb 2023 02:34:28 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a97f60086ee52d11bc7ba54212f27e9f572c66b8214f74dd166f3769cb69d205`  
		Last Modified: Sat, 25 Feb 2023 02:34:35 GMT  
		Size: 51.1 MB (51078697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc7e963515ef8c3d4c33fa57b2810a7a3257bb83b085d8f5a2b31d4f0c2226a`  
		Last Modified: Sat, 25 Feb 2023 02:34:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eeec2615e0a915f4bcf2cab37a175bc5340d1882c15275a199cecf45e3906d6`  
		Last Modified: Sat, 25 Feb 2023 02:34:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e9bedbd2b663733d1b427681701aa7b7ada96d02848563e0c4ef7a282b951b`  
		Last Modified: Sat, 25 Feb 2023 02:34:28 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.14.4` - linux; arm64 variant v8

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

### `consul:1.14.4` - linux; 386

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

## `consul:1.15`

```console
$ docker pull consul@sha256:1ea3aab5a9a83b4638338c754b2161f6860b5d7a394056a252ebcf5fe6cedb94
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
$ docker pull consul@sha256:c0b3cd5b09d97bac3fe142b7edc6bcc577010e7a548f231b5184d5bd4d36c424
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55046039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c761e9c107eba7c6814a0d7c8c31ddc221a85628ff0a0d15425dc49ea72cb835`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 02:33:08 GMT
ARG CONSUL_VERSION=1.15.0
# Sat, 25 Feb 2023 02:33:08 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 02:33:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 02:33:09 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 02:33:17 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 02:33:17 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 02:33:18 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 02:33:18 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 02:33:18 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 02:33:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 02:33:18 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 02:33:18 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 02:33:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 02:33:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37344211dbaffead73bb54ebd0262242125b2c9c9485c027e13fc0bd6392f81`  
		Last Modified: Sat, 25 Feb 2023 02:34:08 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a17b9ee24ea03e20b01ff68ea5f57637ec1794a5367f44ba8777e5b7d1e059`  
		Last Modified: Sat, 25 Feb 2023 02:34:15 GMT  
		Size: 52.4 MB (52409009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898656f19a20d3fc51cc2777e7c15bb9408ea6c92064b3118bc8b972c6d613`  
		Last Modified: Sat, 25 Feb 2023 02:34:07 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef50ec5802a7f33bc5a8771d16ab31c74f36314a44bd7635728fe452aaca335`  
		Last Modified: Sat, 25 Feb 2023 02:34:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924bb877dbbc3818ea54a416b42231f22230318ad4cc444c9718b20d3226961`  
		Last Modified: Sat, 25 Feb 2023 02:34:08 GMT  
		Size: 1.8 KB (1784 bytes)  
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

## `consul:1.15.0`

```console
$ docker pull consul@sha256:1ea3aab5a9a83b4638338c754b2161f6860b5d7a394056a252ebcf5fe6cedb94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.15.0` - linux; amd64

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

### `consul:1.15.0` - linux; arm variant v6

```console
$ docker pull consul@sha256:c0b3cd5b09d97bac3fe142b7edc6bcc577010e7a548f231b5184d5bd4d36c424
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55046039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c761e9c107eba7c6814a0d7c8c31ddc221a85628ff0a0d15425dc49ea72cb835`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 02:33:08 GMT
ARG CONSUL_VERSION=1.15.0
# Sat, 25 Feb 2023 02:33:08 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 02:33:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 02:33:09 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 02:33:17 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 02:33:17 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 02:33:18 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 02:33:18 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 02:33:18 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 02:33:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 02:33:18 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 02:33:18 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 02:33:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 02:33:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37344211dbaffead73bb54ebd0262242125b2c9c9485c027e13fc0bd6392f81`  
		Last Modified: Sat, 25 Feb 2023 02:34:08 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a17b9ee24ea03e20b01ff68ea5f57637ec1794a5367f44ba8777e5b7d1e059`  
		Last Modified: Sat, 25 Feb 2023 02:34:15 GMT  
		Size: 52.4 MB (52409009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898656f19a20d3fc51cc2777e7c15bb9408ea6c92064b3118bc8b972c6d613`  
		Last Modified: Sat, 25 Feb 2023 02:34:07 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef50ec5802a7f33bc5a8771d16ab31c74f36314a44bd7635728fe452aaca335`  
		Last Modified: Sat, 25 Feb 2023 02:34:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924bb877dbbc3818ea54a416b42231f22230318ad4cc444c9718b20d3226961`  
		Last Modified: Sat, 25 Feb 2023 02:34:08 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.15.0` - linux; arm64 variant v8

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

### `consul:1.15.0` - linux; 386

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

## `consul:latest`

```console
$ docker pull consul@sha256:1ea3aab5a9a83b4638338c754b2161f6860b5d7a394056a252ebcf5fe6cedb94
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
$ docker pull consul@sha256:c0b3cd5b09d97bac3fe142b7edc6bcc577010e7a548f231b5184d5bd4d36c424
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55046039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c761e9c107eba7c6814a0d7c8c31ddc221a85628ff0a0d15425dc49ea72cb835`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:37 GMT
ADD file:141468a99f598ddb90dbb73978d10c0f00d01ece185e157ac33a0a1414d45944 in / 
# Fri, 10 Feb 2023 20:49:37 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 02:33:08 GMT
ARG CONSUL_VERSION=1.15.0
# Sat, 25 Feb 2023 02:33:08 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.15.0 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Sat, 25 Feb 2023 02:33:08 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Sat, 25 Feb 2023 02:33:09 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN addgroup consul &&     adduser -S -G consul consul
# Sat, 25 Feb 2023 02:33:17 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Sat, 25 Feb 2023 02:33:17 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Sat, 25 Feb 2023 02:33:18 GMT
# ARGS: CONSUL_VERSION=1.15.0
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 25 Feb 2023 02:33:18 GMT
VOLUME [/consul/data]
# Sat, 25 Feb 2023 02:33:18 GMT
EXPOSE 8300
# Sat, 25 Feb 2023 02:33:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Sat, 25 Feb 2023 02:33:18 GMT
EXPOSE 8500 8600 8600/udp
# Sat, 25 Feb 2023 02:33:18 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 25 Feb 2023 02:33:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 25 Feb 2023 02:33:19 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed6cbaa656dcebfe8d252792a339ccf10dddd695875f07c9636d59a5baf85f3f`  
		Last Modified: Fri, 10 Feb 2023 20:50:51 GMT  
		Size: 2.6 MB (2633649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37344211dbaffead73bb54ebd0262242125b2c9c9485c027e13fc0bd6392f81`  
		Last Modified: Sat, 25 Feb 2023 02:34:08 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a17b9ee24ea03e20b01ff68ea5f57637ec1794a5367f44ba8777e5b7d1e059`  
		Last Modified: Sat, 25 Feb 2023 02:34:15 GMT  
		Size: 52.4 MB (52409009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba898656f19a20d3fc51cc2777e7c15bb9408ea6c92064b3118bc8b972c6d613`  
		Last Modified: Sat, 25 Feb 2023 02:34:07 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef50ec5802a7f33bc5a8771d16ab31c74f36314a44bd7635728fe452aaca335`  
		Last Modified: Sat, 25 Feb 2023 02:34:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924bb877dbbc3818ea54a416b42231f22230318ad4cc444c9718b20d3226961`  
		Last Modified: Sat, 25 Feb 2023 02:34:08 GMT  
		Size: 1.8 KB (1784 bytes)  
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
