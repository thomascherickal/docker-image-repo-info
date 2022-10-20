## `consul:latest`

```console
$ docker pull consul@sha256:b663240f433c056ec0b608f0611c4dd634ef943b9c6c95c5faeafbb85d7a7f3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:22ab19cf1326abbfaafec6a14eb68f96e899e88ffe9ce26fa36affcf8ffb582c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51849363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:787f84379eafbabf63b5b418b678a7908b37f951b1e04e9c3520c0c694c5b5cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 20:17:43 GMT
ARG CONSUL_VERSION=1.13.2
# Thu, 06 Oct 2022 20:17:43 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 20:17:43 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 20:17:44 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 20:17:49 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 20:17:50 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 20:17:51 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 20:17:51 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 20:17:51 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 20:17:51 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 20:17:51 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 20:17:51 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 20:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 20:17:51 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7703ab6ccaa4ba994a2db465e78c8d1a197ba9056588381d68d77b3914b3a09`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b470997b25a34c71f1f5b833f9f4352c88ee661795b819706e7fd555607568d0`  
		Last Modified: Thu, 06 Oct 2022 20:18:34 GMT  
		Size: 49.0 MB (49022471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e707243c37d0a3b90c03cc88111fffca187ded34cf343ab02b9bebc80ad34ac2`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c847e17d4f85b903ffff3b20571e5a26fef18646d229c7d52e4d0693ebca15`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de94b2ee494f8001ee861b3e4c68b18be1d5a405d690adf9fcfeb2f6afb23cf9`  
		Last Modified: Thu, 06 Oct 2022 20:18:28 GMT  
		Size: 1.8 KB (1783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:0c97b3aa222aca56cecbaa978ebfa9e0c05b44cbe16da8e8952140e6f82e7ab1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49459977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb45de66131b32714df6b11aa393597a000dd01684193476b8e1929e658e9a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 20 Oct 2022 21:49:22 GMT
ARG CONSUL_VERSION=1.13.3
# Thu, 20 Oct 2022 21:49:22 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.3 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 20 Oct 2022 21:49:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 20 Oct 2022 21:49:22 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 20 Oct 2022 21:49:29 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 20 Oct 2022 21:49:30 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 20 Oct 2022 21:49:31 GMT
# ARGS: CONSUL_VERSION=1.13.3
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 20 Oct 2022 21:49:31 GMT
VOLUME [/consul/data]
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8300
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 20 Oct 2022 21:49:31 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 20 Oct 2022 21:49:31 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 20 Oct 2022 21:49:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 20 Oct 2022 21:49:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443048d871c8058ca30aa43173b7e7f60c743418207efcb821589f96f6e15bb5`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf2e718f1353961618d3a54eef0029a66ed70877ea3c71e04399f7fd644f186`  
		Last Modified: Thu, 20 Oct 2022 21:50:31 GMT  
		Size: 46.8 MB (46825465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bce47262e4e154a175c36db31d1032a04e1fbd602ab8925e4b71ee917747fe5`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f5d4969c34c70c6dcbfd0450bbfce0f5822deb44e72aae301b34f7a9f24f60`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6edc3c2492164b420fc5b116dbe565199d792dfdd0bd9fec0d027f8c540298`  
		Last Modified: Thu, 20 Oct 2022 21:50:25 GMT  
		Size: 1.8 KB (1790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:a57ab8fdec89d3ddddf86d54c7a5f4333fbf1af45b976ed7bcfeb0c5fd689774
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49011371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:221874175f695865d68383786e479f2bafc221a5eff46ca573fbf1a79633ae03`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:54:55 GMT
ARG CONSUL_VERSION=1.13.2
# Thu, 06 Oct 2022 19:54:56 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 19:54:57 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 19:54:58 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 19:55:04 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 19:55:04 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 19:55:05 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:55:06 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 19:55:07 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 19:55:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 19:55:09 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 19:55:11 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 19:55:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:55:12 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6f27f6d0561ce2ff87a56b6f6f45a7eeab78da890685fa3da49b9735c85919`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b33f6c35637f39fdcd8cf012bf51af6a98cc994d0f810c97ad861d3d1aeb19c3`  
		Last Modified: Thu, 06 Oct 2022 19:56:24 GMT  
		Size: 46.3 MB (46289610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9caeda6f8e23b0768329412dc32e4ed22d825e0e019831bcec0ad9482781d859`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e377af9fdd97c446d4f87829785a24d0aea12da0efd5d2a2e79fc2d9577c97c`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b50148ce95ff394b0f186ddfc88759a280c44aada4170d0a6f93aa2f791bd1f`  
		Last Modified: Thu, 06 Oct 2022 19:56:18 GMT  
		Size: 1.8 KB (1786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:e086f100acad2a5464d6787393c9d970acaabb7edeb7f51a4cef44582618745c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50733141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8180c331613d1f241929f14722a9ccd2e7381ab8463d05fe5456ca16a170b868`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 19:20:30 GMT
ARG CONSUL_VERSION=1.13.2
# Thu, 06 Oct 2022 19:20:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com> org.opencontainers.image.url=https://www.consul.io/ org.opencontainers.image.documentation=https://www.consul.io/docs org.opencontainers.image.source=https://github.com/hashicorp/consul org.opencontainers.image.version=1.13.2 org.opencontainers.image.vendor=HashiCorp org.opencontainers.image.title=consul org.opencontainers.image.description=Consul is a datacenter runtime that provides service discovery, configuration, and orchestration.
# Thu, 06 Oct 2022 19:20:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 06 Oct 2022 19:20:33 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 06 Oct 2022 19:20:39 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat iptables tzdata &&     gpg --keyserver keyserver.ubuntu.com --recv-keys C874011F0AB405110D02105534365D9472D7468F &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='arm' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cp /tmp/build/consul /bin/consul &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/EULA.txt /usr/share/doc/consul/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/consul; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/consul/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 06 Oct 2022 19:20:40 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 06 Oct 2022 19:20:41 GMT
# ARGS: CONSUL_VERSION=1.13.2
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 06 Oct 2022 19:20:42 GMT
VOLUME [/consul/data]
# Thu, 06 Oct 2022 19:20:43 GMT
EXPOSE 8300
# Thu, 06 Oct 2022 19:20:44 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 06 Oct 2022 19:20:45 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 06 Oct 2022 19:20:47 GMT
COPY file:54fea1810b618dd421534c8fbe34fd9d05aa23929d2290f19c325d1c23d960c3 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 06 Oct 2022 19:20:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Oct 2022 19:20:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67739f835a25118040edfe4f1036773c67b02effd1fc9736ae6d099acd2c9a9`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b084d44964631840ce9d61d85e1bfec9b363703ed46455a85ed998e27e260df`  
		Last Modified: Thu, 06 Oct 2022 19:22:10 GMT  
		Size: 47.9 MB (47901306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251f74b33858a8729ffa21f71626e5d464cf8ed93b00ba6691a61d4e2e76b465`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1089b15843a17da8448c7f79aa2fe2a063889614cd6bbfbe38b6069d63da78`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66e77f6cf894d98b0480bbcf1d653d364b51a70102e42e53124a5e4cc3cd57c`  
		Last Modified: Thu, 06 Oct 2022 19:22:03 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
