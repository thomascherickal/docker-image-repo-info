<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.10`](#consul110)
-	[`consul:1.10.7`](#consul1107)
-	[`consul:1.11`](#consul111)
-	[`consul:1.11.2`](#consul1112)
-	[`consul:1.9`](#consul19)
-	[`consul:1.9.14`](#consul1914)
-	[`consul:latest`](#consullatest)

## `consul:1.10`

```console
$ docker pull consul@sha256:28dcafbb5fd7156a21013530335876e89d181997bf849cbfd31d1d990508083c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.10` - linux; amd64

```console
$ docker pull consul@sha256:a290083dfa23d84ea53c54913063e0dc79e09bc1a2e5b050ad82855d4098ec40
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43692494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0771bbeb951f594d65f3996422a312daf01851c87fb878416e5456d9f6b6df62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:19:40 GMT
ARG CONSUL_VERSION=1.10.6
# Thu, 16 Dec 2021 01:19:40 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:19:41 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:19:42 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:19:52 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:19:53 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:19:54 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:19:54 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:19:55 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:19:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:19:55 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:19:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:19:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:19:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d98dd5d86467518fd903fec60a410cec597d61f8ee00634d24879e234dab66d`  
		Last Modified: Thu, 16 Dec 2021 01:21:07 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b91cf4bb3871502e7763eca77c53deea4cd1104599e3ad89929f13f42bbe96c3`  
		Last Modified: Thu, 16 Dec 2021 01:21:13 GMT  
		Size: 40.9 MB (40866699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77243649b935b498d937deac29f6d2af0c688f7d874d2f8fb1c7d556ee1ce31d`  
		Last Modified: Thu, 16 Dec 2021 01:21:07 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894b1d6a77832f3d1b4cbef7a3327b0d1dce70d071012a6ab6defc8ba8ff0e1d`  
		Last Modified: Thu, 16 Dec 2021 01:21:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a990d24f5644d623b6d4533d25f7b0a4db0e13b4061517eeb8f55f281b315a21`  
		Last Modified: Thu, 16 Dec 2021 01:21:07 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm variant v6

```console
$ docker pull consul@sha256:a0752b9cdb487928b45a6ce99ebc09554eb9cce19c06b84befd434ff3913d14b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41759263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cae2485d7c395dbfeb2eac6a03df6df7a8fc58303e6a62dc1bf9756cfdb92b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:50:08 GMT
ARG CONSUL_VERSION=1.10.6
# Thu, 16 Dec 2021 01:50:09 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:50:09 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:50:11 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:50:26 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:50:27 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:50:29 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:50:29 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:50:30 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:50:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:50:31 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:50:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:50:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:50:32 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce061c299357780291c4c85c525b32f21beb673217e3107ae5666d13f315c2d`  
		Last Modified: Thu, 16 Dec 2021 01:53:08 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cf2956bf8570b0ea4e682126bc182f7d474190cdab12c0304365d71dc9f53d`  
		Last Modified: Thu, 16 Dec 2021 01:53:29 GMT  
		Size: 39.1 MB (39122544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df8832213ae2f3a64c59c42d002573bcbdb10dd0c9c2f8759112eba3878adeb`  
		Last Modified: Thu, 16 Dec 2021 01:53:08 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20603e24722912e412e52e2d5a978d57f4d518864d3ca92857179ebe652c38a8`  
		Last Modified: Thu, 16 Dec 2021 01:53:08 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7d2b319e1ca69df587401ec09d65e45cedac68c056cb6a6970c8166cab561f`  
		Last Modified: Thu, 16 Dec 2021 01:53:09 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:278b4cfaccdb2d3b5ecd2c21ea2b5736990eb769b0ad76b08aa9e838ba772d1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41703519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d2b7f8ce471eae4db1b72c96be8d1b7b16337bf3973c8807c7996ef1d3fd103`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:39:57 GMT
ARG CONSUL_VERSION=1.10.6
# Thu, 16 Dec 2021 01:39:57 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:39:58 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:39:59 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:40:05 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:40:06 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:40:07 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:40:08 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:40:09 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:40:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:40:11 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:40:13 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:40:14 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49daa1a70dbb349fb4586158e33af0139998e0a1c75a73c90fb523c7c28c4066`  
		Last Modified: Thu, 16 Dec 2021 01:41:42 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6740e8b283265c91b8e399470838b250e7a24c9118a27c874ea7bb0ff2f14a06`  
		Last Modified: Thu, 16 Dec 2021 01:41:48 GMT  
		Size: 39.0 MB (38980566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c0879dc0c089c9d87ddfcaad3a5e209ed5fe45afb6224e857acef4d7284ab5f`  
		Last Modified: Thu, 16 Dec 2021 01:41:42 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5324728f4f7387e44358f81863e92ebfbf64becfa156f2308046a95832fc9664`  
		Last Modified: Thu, 16 Dec 2021 01:41:42 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1823c9f417f7dcc01c48432e3416f49bb69634ef052f934891dd6f3814ba7b66`  
		Last Modified: Thu, 16 Dec 2021 01:41:42 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.10` - linux; 386

```console
$ docker pull consul@sha256:99afc6d098f5a3ce39f79cdbc24fb4f1996672a022fe6e3588d84d42f11fa2b1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.1 MB (43074618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0070a97ccf252b4d032e763dee24e2c02822ff35e531ac34bc52035010f9a48a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:38:47 GMT
ARG CONSUL_VERSION=1.10.6
# Thu, 16 Dec 2021 01:38:47 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.10.6 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:38:47 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:38:48 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:38:56 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:38:57 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:38:58 GMT
# ARGS: CONSUL_VERSION=1.10.6
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:38:58 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:38:58 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:38:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:38:59 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:38:59 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:38:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:39:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ed83b643354f8efa96350c80933ea54b91abf0e55d694c78b6d9e3f24500a3`  
		Last Modified: Thu, 16 Dec 2021 01:40:27 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437e258679874aa17374e6048e5e8f970f1845a5b019bcd1ebe7711c77524606`  
		Last Modified: Thu, 16 Dec 2021 01:40:32 GMT  
		Size: 40.2 MB (40242437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a053c19daa550296d6d5d85b0e288a981eda10536b7ff8ee145764870fddf84`  
		Last Modified: Thu, 16 Dec 2021 01:40:26 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abfbdc428ce186954267ebc43aef0754749e1c3e69d098abdaea1a97495a115`  
		Last Modified: Thu, 16 Dec 2021 01:40:26 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc23257eb575d3c76177e9c04a514fd16daaca2344545a79f04ede68f5e1c3c`  
		Last Modified: Thu, 16 Dec 2021 01:40:26 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.10.7`

**does not exist** (yet?)

## `consul:1.11`

```console
$ docker pull consul@sha256:05d70d30639d5e0411f92fb75dd670ec1ef8fa4a918c6e57960db1710fd38125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.11` - linux; amd64

```console
$ docker pull consul@sha256:9d53efe467e8818566d9d482b0acbb568f30cdcb57e0aa51536ddf3e91ef799f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43900354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76802375bc5c2c2e068dc9dbc8212e2f80e41675653a5c888d6d987aa0e5d6c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:19:21 GMT
ARG CONSUL_VERSION=1.11.1
# Thu, 16 Dec 2021 01:19:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:19:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:19:22 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:19:33 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:19:34 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:19:35 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:19:35 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:19:36 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:19:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:19:36 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:19:36 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:19:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:19:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a5fd22f94c9adf29a2af7825b2ade16fcae4494f1b84ce4a57733fb1990e5f`  
		Last Modified: Thu, 16 Dec 2021 01:20:43 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e2614f51b475305e8ab466a8a472c0acec77a3a27eb2a7676036c18ecc5019`  
		Last Modified: Thu, 16 Dec 2021 01:20:48 GMT  
		Size: 41.1 MB (41074551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98e494e73971ea851ce90d08927fce2fb2c6d22cd114b34d99cc148140bb855`  
		Last Modified: Thu, 16 Dec 2021 01:20:42 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e8cfc01eae3592625e450af2c60b12e41326985d40dc8e78edb62d44a2ffc5`  
		Last Modified: Thu, 16 Dec 2021 01:20:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1f421022a9242a23b4673ea66177a0e259f34cc2cb4b6b74ca820e6f95a15e`  
		Last Modified: Thu, 16 Dec 2021 01:20:42 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm variant v6

```console
$ docker pull consul@sha256:f5afc0afc447261b825baa360a5a5a7274651fae26c7a7e443acfe9037c506b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41662349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74dde06bfef1ae831d4d79c067f95ba67f0b69d87701f667d66e995c155db5a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:49:32 GMT
ARG CONSUL_VERSION=1.11.1
# Thu, 16 Dec 2021 01:49:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:49:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:49:34 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:49:50 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:49:51 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:49:53 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:49:53 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:49:54 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:49:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:49:55 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:49:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:49:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d09a964f0b40e5e85020a7d34eef59dee531ace45a46a11cdc7bd5b8d58b398`  
		Last Modified: Thu, 16 Dec 2021 01:52:30 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c25a61bab6436d1f9f60de228445ad58608e66d7d45ad5fbd77e6c549b4464`  
		Last Modified: Thu, 16 Dec 2021 01:52:52 GMT  
		Size: 39.0 MB (39025633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a0fc3380a744479073476a22c1e31e145ac6a229a45b6501084ed70ab890b1`  
		Last Modified: Thu, 16 Dec 2021 01:52:30 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240028499fbd86eae990553c88a7e097ea4466d7851d8abbf964dfd764d8a3d9`  
		Last Modified: Thu, 16 Dec 2021 01:52:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a05da9c1692a552abcda7506c4ff82daa5f445581dfbdae82fe58b44dd4449d`  
		Last Modified: Thu, 16 Dec 2021 01:52:31 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:8fedb812b099c7e2a5eebdaa6da80a648aa3b8105bc453e23a95db67ffdf183d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41483691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3bc91ab821041f3a3d9a497ee30e1217cb6eb92ad3577f49c473dfaccfca56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:39:29 GMT
ARG CONSUL_VERSION=1.11.1
# Thu, 16 Dec 2021 01:39:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:39:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:39:32 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:39:42 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:39:43 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:39:44 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:39:45 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:39:46 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:39:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:39:48 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:39:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:39:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2788b13c1ba21465ac130744840a98da8518ab8efa1d41094acaf8d4e079f0af`  
		Last Modified: Thu, 16 Dec 2021 01:41:23 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073ffc88e3a64edbac148109434933c9c71a2aab66ee9463d3ffe989467def34`  
		Last Modified: Thu, 16 Dec 2021 01:41:28 GMT  
		Size: 38.8 MB (38760733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f49cd8e866430ddf1bf4da31631a3573d01ac9bd391c4f98edc2dd660337d0`  
		Last Modified: Thu, 16 Dec 2021 01:41:23 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c51857662f75ab9d4536377742c9aa7522f6b7fbb1c5c89c36a3d3397e501a9`  
		Last Modified: Thu, 16 Dec 2021 01:41:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93f0630417786e630bd15e738032b7e5b06dc00e667f68f5ff1da107de0e19f`  
		Last Modified: Thu, 16 Dec 2021 01:41:23 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.11` - linux; 386

```console
$ docker pull consul@sha256:2e483adc0762dc126a330ef5fbd7c1cce55d9060f6370f18e95eb8d9255b97dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42719741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0809ee2a2c0047b6965f093a1b776e5b726dede831267d895aa6312a4f4c3a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:38:22 GMT
ARG CONSUL_VERSION=1.11.1
# Thu, 16 Dec 2021 01:38:22 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:38:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:38:24 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:38:36 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:38:37 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:38:38 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:38:39 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:38:39 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:38:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:38:39 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:38:40 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:38:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6191c0883651c455386871e897c2d8fccf4fe981d35a51b3e4f58fabcac9139`  
		Last Modified: Thu, 16 Dec 2021 01:40:05 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f56620ee4541a501c4bd748ee777ac33b6c1101d7955c8448365d1da035b364`  
		Last Modified: Thu, 16 Dec 2021 01:40:12 GMT  
		Size: 39.9 MB (39887558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba048955273f97b5a0fcdab98605d62d6f2c48581bf2370caab7672ec83d8e5`  
		Last Modified: Thu, 16 Dec 2021 01:40:05 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c57819266770c189747130e742dcdc8a795c8bcb08138812466f42873d2fb08`  
		Last Modified: Thu, 16 Dec 2021 01:40:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26eb210c204d185abaa3d72226261fa7b252d3ad0df651e2600083380176221`  
		Last Modified: Thu, 16 Dec 2021 01:40:05 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.11.2`

**does not exist** (yet?)

## `consul:1.9`

```console
$ docker pull consul@sha256:c67fdfcad1eef24624797dda062905f548f63428d72db900bb20f1c00558bebe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.9` - linux; amd64

```console
$ docker pull consul@sha256:dfd30f39a0d6e7ce01e7ef6ec4d88f43aae25dd20d4553ba27b12295fbba9387
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40167919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36dd903da7cbce6af261257d7151c5e4e1b7041e78d50929ee127ee0b5c5a013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:20:00 GMT
ARG CONSUL_VERSION=1.9.13
# Thu, 16 Dec 2021 01:20:00 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.13 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:20:00 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:20:01 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:20:10 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:20:11 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:20:11 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:20:12 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:20:12 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:20:12 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:20:12 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:20:12 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:20:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:20:13 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b855cf6f036b57c390f91d06bd1df372ba3a92fd5658d40d34cde2d8f3c39330`  
		Last Modified: Thu, 16 Dec 2021 01:21:23 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e609a3742737a939f71698688a1089b7b4f19b6b91467b38971f4b1757faabf0`  
		Last Modified: Thu, 16 Dec 2021 01:21:28 GMT  
		Size: 37.3 MB (37342128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616194c5f9e3385af180963432957a2794db920565d29635d5a4826dcf066b07`  
		Last Modified: Thu, 16 Dec 2021 01:21:23 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeeed422939899a3733f36659833e4f0cfb324f4d5ae138a01ab12502b38f817`  
		Last Modified: Thu, 16 Dec 2021 01:21:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8eaed7613bca667a9dee514ba1823f55b46629d39369b431f5b97709606c027`  
		Last Modified: Thu, 16 Dec 2021 01:21:23 GMT  
		Size: 1.8 KB (1785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm variant v6

```console
$ docker pull consul@sha256:d59bf2061eb79960796f0717bdf7f7d14acda13eddcf216ff5cba5fc563d48f5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38220000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd8c6ee3e815af084df26e113d8fd30f3b34088d7858933eb003333dde3eccda`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:50:43 GMT
ARG CONSUL_VERSION=1.9.13
# Thu, 16 Dec 2021 01:50:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.13 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:50:44 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:50:45 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:50:57 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:50:59 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:51:01 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:51:01 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:51:01 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:51:02 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:51:02 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:51:03 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:51:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:51:04 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0173a303c3e408e99269c7dd6a9dd0c891ed64e98b2659fac91a4acc6da14deb`  
		Last Modified: Thu, 16 Dec 2021 01:53:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409600fa920de2201a72767fd324ae07b4454f5ece91c2a3547c1eb189859206`  
		Last Modified: Thu, 16 Dec 2021 01:53:59 GMT  
		Size: 35.6 MB (35583280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80ce095113681b1778b0697464d16c8778417589050530085b232af1f93a341`  
		Last Modified: Thu, 16 Dec 2021 01:53:41 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47d7c547c4fdb16acf270bcaf3a5aa6fcf2eb3d4b10d96349d60b2fcab44147f`  
		Last Modified: Thu, 16 Dec 2021 01:53:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244dbe40c5700f4804562ff72698ee40d98243d4b7a7bb9ae39f0a62ab981540`  
		Last Modified: Thu, 16 Dec 2021 01:53:41 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:65990a2f7039bf5bdc16a53ef7d420e0988697fc004ff6935e9ede3350742b35
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38167203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bdb82e8e1467ffde2badc51c8210b2ac6e6c724568fc4723917354272bf8858`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:40:19 GMT
ARG CONSUL_VERSION=1.9.13
# Thu, 16 Dec 2021 01:40:20 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.13 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:40:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:40:22 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:40:28 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:40:29 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:40:30 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:40:31 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:40:32 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:40:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:40:34 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:40:36 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:40:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:40:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fd9f87b3aad0f1b4531aae14f4f33623bf70d90782fae693ea1bccfcfc94bd`  
		Last Modified: Thu, 16 Dec 2021 01:41:59 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748a6c72684fb8ac67932c933ccbc78443eeae1e16ed9eae6f1176859908f156`  
		Last Modified: Thu, 16 Dec 2021 01:42:04 GMT  
		Size: 35.4 MB (35444251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11e89d5a9d5a25909953c40b8cef2d42e23b9b525da432213bd54672352e1cf`  
		Last Modified: Thu, 16 Dec 2021 01:41:59 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9977f897f9b5ec538c01813af3b464d9cb2a20a9a2d340a1fed85b9b2eb70235`  
		Last Modified: Thu, 16 Dec 2021 01:41:59 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d10ff7c56dfa49ee15844b98cc1840cb4fb410960339d22c293a41d6abf857`  
		Last Modified: Thu, 16 Dec 2021 01:41:59 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.9` - linux; 386

```console
$ docker pull consul@sha256:e15d606d7c8f34ce9fb3137e620a43e51b63c84a34389aa975084195bc805202
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.5 MB (39523299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d85c8586d7ef2096cad2a0f1c6942250ba532bc6f687bf1da9758385908f880`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:39:05 GMT
ARG CONSUL_VERSION=1.9.13
# Thu, 16 Dec 2021 01:39:05 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.9.13 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:39:05 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:39:06 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:39:16 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:39:18 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:39:19 GMT
# ARGS: CONSUL_VERSION=1.9.13
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:39:19 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:39:19 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:39:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:39:20 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:39:20 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:39:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:39:20 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996069998839bbbb7f670f2cf968840d4241da37e20b5c5986ba6da20e290370`  
		Last Modified: Thu, 16 Dec 2021 01:40:44 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f40daf7d18fa1cc3a140d5a5643e2b00c5d96a3e6f9355417f4b4dbd5934d5`  
		Last Modified: Thu, 16 Dec 2021 01:40:49 GMT  
		Size: 36.7 MB (36691115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb57221f5d95114905ea60883b402d715294799788865b47e2ff96d71f4c1a27`  
		Last Modified: Thu, 16 Dec 2021 01:40:44 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54dc5ac072b154991a95a5a907d871e5be550c3bca4b7a4e9b79493bc2d3e43e`  
		Last Modified: Thu, 16 Dec 2021 01:40:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deaaf8d448958d5b7ab63fd0b61747d855b21af74ae765db36ea52a15c8e4ba9`  
		Last Modified: Thu, 16 Dec 2021 01:40:44 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.9.14`

**does not exist** (yet?)

## `consul:latest`

```console
$ docker pull consul@sha256:05d70d30639d5e0411f92fb75dd670ec1ef8fa4a918c6e57960db1710fd38125
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:9d53efe467e8818566d9d482b0acbb568f30cdcb57e0aa51536ddf3e91ef799f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43900354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76802375bc5c2c2e068dc9dbc8212e2f80e41675653a5c888d6d987aa0e5d6c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:19:21 GMT
ARG CONSUL_VERSION=1.11.1
# Thu, 16 Dec 2021 01:19:21 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:19:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:19:22 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:19:33 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:19:34 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:19:35 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:19:35 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:19:36 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:19:36 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:19:36 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:19:36 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:19:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:19:37 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a5fd22f94c9adf29a2af7825b2ade16fcae4494f1b84ce4a57733fb1990e5f`  
		Last Modified: Thu, 16 Dec 2021 01:20:43 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e2614f51b475305e8ab466a8a472c0acec77a3a27eb2a7676036c18ecc5019`  
		Last Modified: Thu, 16 Dec 2021 01:20:48 GMT  
		Size: 41.1 MB (41074551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98e494e73971ea851ce90d08927fce2fb2c6d22cd114b34d99cc148140bb855`  
		Last Modified: Thu, 16 Dec 2021 01:20:42 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e8cfc01eae3592625e450af2c60b12e41326985d40dc8e78edb62d44a2ffc5`  
		Last Modified: Thu, 16 Dec 2021 01:20:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1f421022a9242a23b4673ea66177a0e259f34cc2cb4b6b74ca820e6f95a15e`  
		Last Modified: Thu, 16 Dec 2021 01:20:42 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:f5afc0afc447261b825baa360a5a5a7274651fae26c7a7e443acfe9037c506b0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41662349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74dde06bfef1ae831d4d79c067f95ba67f0b69d87701f667d66e995c155db5a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:49:32 GMT
ARG CONSUL_VERSION=1.11.1
# Thu, 16 Dec 2021 01:49:32 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:49:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:49:34 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:49:50 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:49:51 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:49:53 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:49:53 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:49:54 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:49:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:49:55 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:49:55 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:49:56 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d09a964f0b40e5e85020a7d34eef59dee531ace45a46a11cdc7bd5b8d58b398`  
		Last Modified: Thu, 16 Dec 2021 01:52:30 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27c25a61bab6436d1f9f60de228445ad58608e66d7d45ad5fbd77e6c549b4464`  
		Last Modified: Thu, 16 Dec 2021 01:52:52 GMT  
		Size: 39.0 MB (39025633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a0fc3380a744479073476a22c1e31e145ac6a229a45b6501084ed70ab890b1`  
		Last Modified: Thu, 16 Dec 2021 01:52:30 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240028499fbd86eae990553c88a7e097ea4466d7851d8abbf964dfd764d8a3d9`  
		Last Modified: Thu, 16 Dec 2021 01:52:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a05da9c1692a552abcda7506c4ff82daa5f445581dfbdae82fe58b44dd4449d`  
		Last Modified: Thu, 16 Dec 2021 01:52:31 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:8fedb812b099c7e2a5eebdaa6da80a648aa3b8105bc453e23a95db67ffdf183d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41483691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3bc91ab821041f3a3d9a497ee30e1217cb6eb92ad3577f49c473dfaccfca56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:39:29 GMT
ARG CONSUL_VERSION=1.11.1
# Thu, 16 Dec 2021 01:39:30 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:39:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:39:32 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:39:42 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:39:43 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:39:44 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:39:45 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:39:46 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:39:47 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:39:48 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:39:50 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:39:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:39:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2788b13c1ba21465ac130744840a98da8518ab8efa1d41094acaf8d4e079f0af`  
		Last Modified: Thu, 16 Dec 2021 01:41:23 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073ffc88e3a64edbac148109434933c9c71a2aab66ee9463d3ffe989467def34`  
		Last Modified: Thu, 16 Dec 2021 01:41:28 GMT  
		Size: 38.8 MB (38760733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f49cd8e866430ddf1bf4da31631a3573d01ac9bd391c4f98edc2dd660337d0`  
		Last Modified: Thu, 16 Dec 2021 01:41:23 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c51857662f75ab9d4536377742c9aa7522f6b7fbb1c5c89c36a3d3397e501a9`  
		Last Modified: Thu, 16 Dec 2021 01:41:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93f0630417786e630bd15e738032b7e5b06dc00e667f68f5ff1da107de0e19f`  
		Last Modified: Thu, 16 Dec 2021 01:41:23 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:2e483adc0762dc126a330ef5fbd7c1cce55d9060f6370f18e95eb8d9255b97dc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42719741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0809ee2a2c0047b6965f093a1b776e5b726dede831267d895aa6312a4f4c3a7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Thu, 16 Dec 2021 01:38:22 GMT
ARG CONSUL_VERSION=1.11.1
# Thu, 16 Dec 2021 01:38:22 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.11.1 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 16 Dec 2021 01:38:23 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 16 Dec 2021 01:38:24 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 16 Dec 2021 01:38:36 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 16 Dec 2021 01:38:37 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 16 Dec 2021 01:38:38 GMT
# ARGS: CONSUL_VERSION=1.11.1
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 16 Dec 2021 01:38:39 GMT
VOLUME [/consul/data]
# Thu, 16 Dec 2021 01:38:39 GMT
EXPOSE 8300
# Thu, 16 Dec 2021 01:38:39 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 16 Dec 2021 01:38:39 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 16 Dec 2021 01:38:40 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 16 Dec 2021 01:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Dec 2021 01:38:40 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6191c0883651c455386871e897c2d8fccf4fe981d35a51b3e4f58fabcac9139`  
		Last Modified: Thu, 16 Dec 2021 01:40:05 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f56620ee4541a501c4bd748ee777ac33b6c1101d7955c8448365d1da035b364`  
		Last Modified: Thu, 16 Dec 2021 01:40:12 GMT  
		Size: 39.9 MB (39887558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba048955273f97b5a0fcdab98605d62d6f2c48581bf2370caab7672ec83d8e5`  
		Last Modified: Thu, 16 Dec 2021 01:40:05 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c57819266770c189747130e742dcdc8a795c8bcb08138812466f42873d2fb08`  
		Last Modified: Thu, 16 Dec 2021 01:40:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26eb210c204d185abaa3d72226261fa7b252d3ad0df651e2600083380176221`  
		Last Modified: Thu, 16 Dec 2021 01:40:05 GMT  
		Size: 1.8 KB (1787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
