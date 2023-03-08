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
