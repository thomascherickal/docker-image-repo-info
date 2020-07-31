<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.6`](#consul16)
-	[`consul:1.6.7`](#consul167)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.5`](#consul175)
-	[`consul:1.8`](#consul18)
-	[`consul:1.8.1`](#consul181)
-	[`consul:latest`](#consullatest)

## `consul:1.6`

```console
$ docker pull consul@sha256:9f65ef887fec2868c3b281992d0d90775f3b82492efa1c54ef84fdf628e84354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6` - linux; amd64

```console
$ docker pull consul@sha256:40d7e75ddd3d514ef9b1709cb87c2ca33e19b618c22ac0603070d5a75b9137a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41785900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:557584fdffd2a3a632160c850a8bd2cfa2258ade07f0e15c407b95112c3c18e9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Wed, 10 Jun 2020 23:19:52 GMT
ENV CONSUL_VERSION=1.6.6
# Wed, 10 Jun 2020 23:19:53 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 10 Jun 2020 23:19:53 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 10 Jun 2020 23:19:58 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 10 Jun 2020 23:19:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 10 Jun 2020 23:19:59 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Jun 2020 23:19:59 GMT
VOLUME [/consul/data]
# Wed, 10 Jun 2020 23:20:00 GMT
EXPOSE 8300
# Wed, 10 Jun 2020 23:20:00 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 10 Jun 2020 23:20:00 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 10 Jun 2020 23:20:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Jun 2020 23:20:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 23:20:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ac53e9273a6631bf2d5674b065cbc34e838804bcb7a02e4f2973bc0df43638`  
		Last Modified: Wed, 10 Jun 2020 23:20:21 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fc33632573831d594e7751c05ef6720e99832947c328f22022e303161710fc`  
		Last Modified: Wed, 10 Jun 2020 23:20:28 GMT  
		Size: 39.0 MB (39009229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd07a2712252e591e67b6a8485ffaa24ddecbabee498414af06df5699b21e6`  
		Last Modified: Wed, 10 Jun 2020 23:20:21 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d17d4d773a3e93e2ba4698a6dadb7ff51d7487c00e5b0692ba682749377321`  
		Last Modified: Wed, 10 Jun 2020 23:20:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37494dc97a13f5b140c9959f831c840476d49e18043f52976edeea39d7b9f1e9`  
		Last Modified: Wed, 10 Jun 2020 23:20:21 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:93f7c68c2e2823e004790ff9accc7714dd39e5f06078a03c48972b13ea936ebe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39248161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3671de116cabbc8ef1982f71c906d34013edeeb9bc6e8bd7637b3815ddf4eb7b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Wed, 10 Jun 2020 23:50:24 GMT
ENV CONSUL_VERSION=1.6.6
# Wed, 10 Jun 2020 23:50:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 10 Jun 2020 23:50:37 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 10 Jun 2020 23:50:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 10 Jun 2020 23:50:49 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 10 Jun 2020 23:50:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Jun 2020 23:50:53 GMT
VOLUME [/consul/data]
# Wed, 10 Jun 2020 23:50:53 GMT
EXPOSE 8300
# Wed, 10 Jun 2020 23:50:54 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 10 Jun 2020 23:50:57 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 10 Jun 2020 23:50:58 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Jun 2020 23:50:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 23:51:00 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ea78b3e5ff961bdecd7242e924c4825de54f1aa91ea7fff47216d65d52ff2f`  
		Last Modified: Wed, 10 Jun 2020 23:51:36 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc03b057e6ccf81c079c5eb09662cba86b0495d0283588b78fc9cd9300593637`  
		Last Modified: Wed, 10 Jun 2020 23:51:56 GMT  
		Size: 36.7 MB (36696113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f5436840d497ea6d2d9f855279103d22a159ac582e78907ba4c942b2c2dcb9`  
		Last Modified: Wed, 10 Jun 2020 23:51:34 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d58befdefd3ab606ccc1bd4497f3d2424830e5540d86cf9c1ce3b7612f2fe0`  
		Last Modified: Wed, 10 Jun 2020 23:51:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf47ad086384fcf77cf5c78626048d1e49f9e824eb9f71bc5b429e850f56b9b`  
		Last Modified: Wed, 10 Jun 2020 23:51:35 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:669c2f7c1e196a6d68d2d8adcd81d2eda2b516a7960bd0a13d513e8cf6ea29ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39576774 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3594b5c10062182fbc7369164308d40cb870f647cf38fd3f472d9489702f4dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Wed, 10 Jun 2020 23:40:17 GMT
ENV CONSUL_VERSION=1.6.6
# Wed, 10 Jun 2020 23:40:17 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 10 Jun 2020 23:40:19 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 10 Jun 2020 23:40:26 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 10 Jun 2020 23:40:29 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 10 Jun 2020 23:40:32 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Jun 2020 23:40:32 GMT
VOLUME [/consul/data]
# Wed, 10 Jun 2020 23:40:33 GMT
EXPOSE 8300
# Wed, 10 Jun 2020 23:40:34 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 10 Jun 2020 23:40:34 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 10 Jun 2020 23:40:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Jun 2020 23:40:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 23:40:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28aaa6f085ab7db28cb9ef47583f46d1525195131f004c4d51dedde87ec53aa8`  
		Last Modified: Wed, 10 Jun 2020 23:41:06 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67dea3834d8d17be0bb3652c87e5b0db1ba070d8012f6591aca0cbecde0ef4fa`  
		Last Modified: Wed, 10 Jun 2020 23:41:16 GMT  
		Size: 36.9 MB (36878987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83c27fc8d14976cec565c466dd1395e7ce8d24a45da1f948540007d8075d820`  
		Last Modified: Wed, 10 Jun 2020 23:41:06 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1665e5ec36ee72322d605a8282775cc31c411d338bacbae60714c916a9018041`  
		Last Modified: Wed, 10 Jun 2020 23:41:06 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b09c54f488d3a5bd012ee57ef00ab85a82170b57960ef84402c13fd12c010d`  
		Last Modified: Wed, 10 Jun 2020 23:41:06 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; 386

```console
$ docker pull consul@sha256:df14af3d6b94ea8e320258f24aa73ebd5e8f743208eaf434b853d5e487906b80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40640355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e0e73663a8b017f5d717f2a4a28de4bc31f396e4fc32716563381a96fc49131`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Wed, 10 Jun 2020 23:38:40 GMT
ENV CONSUL_VERSION=1.6.6
# Wed, 10 Jun 2020 23:38:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 10 Jun 2020 23:38:41 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 10 Jun 2020 23:38:50 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 10 Jun 2020 23:38:51 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 10 Jun 2020 23:38:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Jun 2020 23:38:52 GMT
VOLUME [/consul/data]
# Wed, 10 Jun 2020 23:38:52 GMT
EXPOSE 8300
# Wed, 10 Jun 2020 23:38:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 10 Jun 2020 23:38:53 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 10 Jun 2020 23:38:53 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Jun 2020 23:38:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 23:38:53 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf61795be87f90e988eecc2112c4f87b3cfb7e877f007cd0d318e7a18ff3678`  
		Last Modified: Wed, 10 Jun 2020 23:39:14 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b877955d9c838bfcbba1eb247e775002adb22f3763c67585d04c332390845656`  
		Last Modified: Wed, 10 Jun 2020 23:39:25 GMT  
		Size: 37.9 MB (37867361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d936cf5e14a7d5816ba031621f8e17d420ab3c00dff2ac643751c6ae78cc27`  
		Last Modified: Wed, 10 Jun 2020 23:39:14 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d4c5344f86d21bf06c20351bd9c2713c31e94763b2dd4bdf1c73137afc74ca`  
		Last Modified: Wed, 10 Jun 2020 23:39:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2e17b3aba181deb2f1c4cc16f29792bbf9c97979b12415f3840f488c56ac7d`  
		Last Modified: Wed, 10 Jun 2020 23:39:14 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6.7`

**does not exist** (yet?)

## `consul:1.7`

```console
$ docker pull consul@sha256:af68cbd5d9b5bc162eb66236b5ec56019a60d7ae0ebec7cd752516196fd40ecf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:3356df0bf0c8e482ddc3462489ad1013dcaa1eb09890e56cdcf29c0b417b1601
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44099054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:204ef3cdcad68903b722086e140cfaf8031ef2b4863ae742717fe3fcc026b29d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Wed, 10 Jun 2020 23:19:40 GMT
ENV CONSUL_VERSION=1.7.4
# Wed, 10 Jun 2020 23:19:40 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 10 Jun 2020 23:19:41 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 10 Jun 2020 23:19:45 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 10 Jun 2020 23:19:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 10 Jun 2020 23:19:47 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Jun 2020 23:19:47 GMT
VOLUME [/consul/data]
# Wed, 10 Jun 2020 23:19:47 GMT
EXPOSE 8300
# Wed, 10 Jun 2020 23:19:48 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 10 Jun 2020 23:19:48 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 10 Jun 2020 23:19:48 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Jun 2020 23:19:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 23:19:48 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0465b8cf0977f50aed94df554640cb2066044ec1803f29694c8496776f25c689`  
		Last Modified: Wed, 10 Jun 2020 23:20:09 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cec2b629a7a81ee0b987f3889e12e2e6940b7f61457025b2d57a1ce7f75030a`  
		Last Modified: Wed, 10 Jun 2020 23:20:17 GMT  
		Size: 41.3 MB (41322383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cb892e0d284fa5a5db0231c8b49c90b4c759be688ff3c58426ed2aeb3f7748`  
		Last Modified: Wed, 10 Jun 2020 23:20:10 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4ec2c2805d0f5eb7ec0baef620fa74a943784adc16dec8c8df113217b5eb48`  
		Last Modified: Wed, 10 Jun 2020 23:20:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaa3b18a522fdaadc0cb3099ccfa4d71714901c98383cadcd81d7e33adcea036`  
		Last Modified: Wed, 10 Jun 2020 23:20:10 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:03137ff5d61d5e43c69752cc939640f392653f58f95fda32653f0d4b305f63ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41434220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f2e70713400a1a58721bcc87afbebfa23cf43b217463e729dda0f98641d5f84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Wed, 10 Jun 2020 23:49:36 GMT
ENV CONSUL_VERSION=1.7.4
# Wed, 10 Jun 2020 23:49:37 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 10 Jun 2020 23:49:40 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 10 Jun 2020 23:49:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 10 Jun 2020 23:49:58 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 10 Jun 2020 23:50:01 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Jun 2020 23:50:02 GMT
VOLUME [/consul/data]
# Wed, 10 Jun 2020 23:50:06 GMT
EXPOSE 8300
# Wed, 10 Jun 2020 23:50:08 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 10 Jun 2020 23:50:09 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 10 Jun 2020 23:50:09 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Jun 2020 23:50:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 23:50:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86f3dbcee5101461e0a83033a652280865641a280055f2174470c3335ae484c`  
		Last Modified: Wed, 10 Jun 2020 23:51:13 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449bc1b18965fe6c1d263b3eca05349c1dcc88351368aca53fc1df5e38c96204`  
		Last Modified: Wed, 10 Jun 2020 23:51:25 GMT  
		Size: 38.9 MB (38882175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:668b0c3733cfd900c5024a93e56c00acecfbdbc3f6172695e386ace10245a696`  
		Last Modified: Wed, 10 Jun 2020 23:51:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ccb3533507cf6574ce01286c45bc979b4370889929869ce5aac146aacc8059`  
		Last Modified: Wed, 10 Jun 2020 23:51:13 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d6cb9be9e08c2b48c235acb05b6e4bada611ab2391deb26fab2d4e685469e6`  
		Last Modified: Wed, 10 Jun 2020 23:51:13 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:0f8dfca25e95e921ae48c7e709ef7de25cba27169fada5d546bed64bbd6051a3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41772283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fcccc7151bfaea5bb8cae131415db088440cf13d52db75a1f47c20d82453cf6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Wed, 10 Jun 2020 23:39:50 GMT
ENV CONSUL_VERSION=1.7.4
# Wed, 10 Jun 2020 23:39:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 10 Jun 2020 23:39:53 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 10 Jun 2020 23:40:03 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 10 Jun 2020 23:40:05 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 10 Jun 2020 23:40:07 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Jun 2020 23:40:08 GMT
VOLUME [/consul/data]
# Wed, 10 Jun 2020 23:40:08 GMT
EXPOSE 8300
# Wed, 10 Jun 2020 23:40:09 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 10 Jun 2020 23:40:09 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 10 Jun 2020 23:40:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Jun 2020 23:40:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 23:40:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815a7d71f9fa89e99be3094575057804d8ecc36dd1fb3cc12d159a57523cb9d4`  
		Last Modified: Wed, 10 Jun 2020 23:40:49 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776a8ab02ab9abbe6426dc61384fbf5ac0bb15cdb266988bf7d9af0a42f18b5f`  
		Last Modified: Wed, 10 Jun 2020 23:41:00 GMT  
		Size: 39.1 MB (39074495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf8342ce55141e6a7030ae3e129c208fb15d2598c99401a116c340d25cd6d4d`  
		Last Modified: Wed, 10 Jun 2020 23:40:50 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7550c905bded8413906231b61da64bea6b0c36bd42633256d88895c6d1173f7f`  
		Last Modified: Wed, 10 Jun 2020 23:40:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d7d150b0ed0d60eb6163603a3e8d680dea88106d060f569d38435eb44497cd`  
		Last Modified: Wed, 10 Jun 2020 23:40:49 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:f961c6182c617d9d825ab2e29d923abfe1f9a4bf6438380b96e465651c051816
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42871720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e30070deda2beffa554b6b99a9b781085345ac3dc5dbdd82e1648e046aef1e6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Wed, 10 Jun 2020 23:38:26 GMT
ENV CONSUL_VERSION=1.7.4
# Wed, 10 Jun 2020 23:38:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Wed, 10 Jun 2020 23:38:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Wed, 10 Jun 2020 23:38:33 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Wed, 10 Jun 2020 23:38:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Wed, 10 Jun 2020 23:38:34 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Jun 2020 23:38:34 GMT
VOLUME [/consul/data]
# Wed, 10 Jun 2020 23:38:35 GMT
EXPOSE 8300
# Wed, 10 Jun 2020 23:38:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Wed, 10 Jun 2020 23:38:35 GMT
EXPOSE 8500 8600 8600/udp
# Wed, 10 Jun 2020 23:38:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 10 Jun 2020 23:38:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Jun 2020 23:38:36 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e675cae2850aa9f4965d31fd03a15ff080c72e9654883092fe7042469f21d86`  
		Last Modified: Wed, 10 Jun 2020 23:39:01 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd51efa59c7e9b7d96d3bdba2cde13fd5c09933f103a6328859d8cb8a20cfa38`  
		Last Modified: Wed, 10 Jun 2020 23:39:09 GMT  
		Size: 40.1 MB (40098724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733333db3be1389966761d9f86ea4abce6500c519db029e2a02f87bd749ba595`  
		Last Modified: Wed, 10 Jun 2020 23:39:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c92f2a02da1df2df1df14eda9bcb23601dba8416c6820fd18dc353a4411ad20`  
		Last Modified: Wed, 10 Jun 2020 23:39:02 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1569a81f625f55afc9d55100ce4e8268330fa26358918b7a5ca5e559114cd7`  
		Last Modified: Wed, 10 Jun 2020 23:39:01 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.5`

**does not exist** (yet?)

## `consul:1.8`

```console
$ docker pull consul@sha256:0e660ca8ae28d864e3eaaed0e273b2f8cd348af207e2b715237e869d7a8b5dcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:e233561c4866571086a6615bf049f9ebcd112c4106b10c596dd6683d02f9d814
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47074061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:941109e2896d418d13924ff4c9119ba67dc00ca9e9de0e081b255cce9eeecd77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 18 Jun 2020 21:19:25 GMT
ENV CONSUL_VERSION=1.8.0
# Thu, 18 Jun 2020 21:19:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 18 Jun 2020 21:19:26 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 18 Jun 2020 21:19:31 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 18 Jun 2020 21:19:32 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 18 Jun 2020 21:19:33 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Jun 2020 21:19:33 GMT
VOLUME [/consul/data]
# Thu, 18 Jun 2020 21:19:33 GMT
EXPOSE 8300
# Thu, 18 Jun 2020 21:19:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 18 Jun 2020 21:19:33 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 18 Jun 2020 21:19:34 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Jun 2020 21:19:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Jun 2020 21:19:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63107527bd50e84b5ab08eed704952e4e712b944a0c6d4b2aed8f2a2831914dc`  
		Last Modified: Thu, 18 Jun 2020 21:19:48 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a2bb8f5fba9742a3727445293e7650ea44dd64abd084aed85225e7608f651`  
		Last Modified: Thu, 18 Jun 2020 21:19:55 GMT  
		Size: 44.3 MB (44297385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbeef6d591983ae6e8974100916fad1e82b0125575edbee709f49fec3ad699bc`  
		Last Modified: Thu, 18 Jun 2020 21:19:48 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f004e44699b3259ca1ceed12d409fa5d9bd6b3eade8d9dfc4a135e74217f17a5`  
		Last Modified: Thu, 18 Jun 2020 21:19:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b16c132cbda34532a9e953bbf8f3a05560232a264cbe2ddeeec9660d88bb3f6`  
		Last Modified: Thu, 18 Jun 2020 21:19:48 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:8b795f097369c9a8b88158a7a6c74e34bdcea3ab1430c7c2203292bfd0b6376c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42149425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55333853496b4819188211dcae6bdfbe0e29b07149ebaea63f01786a0fa511fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 18 Jun 2020 21:49:51 GMT
ENV CONSUL_VERSION=1.8.0
# Thu, 18 Jun 2020 21:49:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 18 Jun 2020 21:49:57 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 18 Jun 2020 21:50:10 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 18 Jun 2020 21:50:14 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 18 Jun 2020 21:50:16 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Jun 2020 21:50:17 GMT
VOLUME [/consul/data]
# Thu, 18 Jun 2020 21:50:18 GMT
EXPOSE 8300
# Thu, 18 Jun 2020 21:50:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 18 Jun 2020 21:50:20 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 18 Jun 2020 21:50:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Jun 2020 21:50:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Jun 2020 21:50:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2754231772db598bc69a198a882b6b55b2c0c0b0acbc8595b093c413fd0b16f5`  
		Last Modified: Thu, 18 Jun 2020 21:50:49 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90407def8d08fcc8c39aa2201d510e4e1abc0bfdac9edd772ff9a4df990efb75`  
		Last Modified: Thu, 18 Jun 2020 21:51:01 GMT  
		Size: 39.6 MB (39597379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5373d7576b565360a753dbf509e389e8b5f2564a65952e4c839e709a2b3afa1`  
		Last Modified: Thu, 18 Jun 2020 21:50:49 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d87ccab463eb46b6150408675801bf7f4055d1f8373688cb15bd438a88be4d`  
		Last Modified: Thu, 18 Jun 2020 21:50:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5894dcff1d1274c5ea94e557a1e4933481ec3506b39b49896c22ba7674aaf9`  
		Last Modified: Thu, 18 Jun 2020 21:50:49 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:266753598047a982f884fd16b0c7c4d293a35fda3e2542205a02ce89acf3c2c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42397134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6246d2dfaccff4f715581f879067a6fcdafb39170693a762ca4f9bb70dfa1754`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 18 Jun 2020 21:39:38 GMT
ENV CONSUL_VERSION=1.8.0
# Thu, 18 Jun 2020 21:39:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 18 Jun 2020 21:39:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 18 Jun 2020 21:39:53 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 18 Jun 2020 21:39:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 18 Jun 2020 21:39:57 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Jun 2020 21:39:57 GMT
VOLUME [/consul/data]
# Thu, 18 Jun 2020 21:39:58 GMT
EXPOSE 8300
# Thu, 18 Jun 2020 21:39:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 18 Jun 2020 21:40:00 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 18 Jun 2020 21:40:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Jun 2020 21:40:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Jun 2020 21:40:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c62d7d2a7dc49c360560cae61c091486c1c24ac03fd34b6869635a92dce5fb8`  
		Last Modified: Thu, 18 Jun 2020 21:40:24 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc98caf0c68306a78ed54f82e00c95afbd9ef917457db428e9287ca5304876e`  
		Last Modified: Thu, 18 Jun 2020 21:40:34 GMT  
		Size: 39.7 MB (39699344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fca3e93a033a25c291c52f812998843b5a8697f252d14bf06c38b3a29b3f0b`  
		Last Modified: Thu, 18 Jun 2020 21:40:25 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebcb4658c39ce46ae2c5da07e7c06b1d3ae67d73d493a08907eb038c5ac8dbf`  
		Last Modified: Thu, 18 Jun 2020 21:40:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d51dd1887d7912775dd80344979baaa67585ac709976a8166e7a0f97d3d313a`  
		Last Modified: Thu, 18 Jun 2020 21:40:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:9198f49897334e1e647664f3b5ab9a95c1f4b22523dc693281fbb792e56f4ea0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46512858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a0ecd9ac2104e4deebab21d46f56697c741cb988f8084f4a5d84d17dadd85a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 18 Jun 2020 21:38:21 GMT
ENV CONSUL_VERSION=1.8.0
# Thu, 18 Jun 2020 21:38:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 18 Jun 2020 21:38:22 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 18 Jun 2020 21:38:28 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 18 Jun 2020 21:38:28 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 18 Jun 2020 21:38:29 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Jun 2020 21:38:29 GMT
VOLUME [/consul/data]
# Thu, 18 Jun 2020 21:38:30 GMT
EXPOSE 8300
# Thu, 18 Jun 2020 21:38:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 18 Jun 2020 21:38:30 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 18 Jun 2020 21:38:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Jun 2020 21:38:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Jun 2020 21:38:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00127ab7c2809a649ef2dcdf53750dc4327bb66d05d975d94a4189b6184a65ee`  
		Last Modified: Thu, 18 Jun 2020 21:38:47 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436ff31cabc835ccb9432504266923e2ceb6515f0d06c9ff0147ec17bd69b762`  
		Last Modified: Thu, 18 Jun 2020 21:38:53 GMT  
		Size: 43.7 MB (43739863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361c6767c5dbd0371aeea804fe4dac5fd3ec45e7b7be8ae70931c1e2e32a4b0f`  
		Last Modified: Thu, 18 Jun 2020 21:38:46 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075b384adfb58b589949193dc450cfbbde9e7c779a2e7fbe64ae4b851d5cc0f4`  
		Last Modified: Thu, 18 Jun 2020 21:38:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439ee1a7f0e800c206672170ea2bc0ce04a8fa6699f3a35bbad44d994cf02a3`  
		Last Modified: Thu, 18 Jun 2020 21:38:46 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.1`

**does not exist** (yet?)

## `consul:latest`

```console
$ docker pull consul@sha256:0e660ca8ae28d864e3eaaed0e273b2f8cd348af207e2b715237e869d7a8b5dcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:e233561c4866571086a6615bf049f9ebcd112c4106b10c596dd6683d02f9d814
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47074061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:941109e2896d418d13924ff4c9119ba67dc00ca9e9de0e081b255cce9eeecd77`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 18 Jun 2020 21:19:25 GMT
ENV CONSUL_VERSION=1.8.0
# Thu, 18 Jun 2020 21:19:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 18 Jun 2020 21:19:26 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 18 Jun 2020 21:19:31 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 18 Jun 2020 21:19:32 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 18 Jun 2020 21:19:33 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Jun 2020 21:19:33 GMT
VOLUME [/consul/data]
# Thu, 18 Jun 2020 21:19:33 GMT
EXPOSE 8300
# Thu, 18 Jun 2020 21:19:33 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 18 Jun 2020 21:19:33 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 18 Jun 2020 21:19:34 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Jun 2020 21:19:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Jun 2020 21:19:34 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63107527bd50e84b5ab08eed704952e4e712b944a0c6d4b2aed8f2a2831914dc`  
		Last Modified: Thu, 18 Jun 2020 21:19:48 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6a2bb8f5fba9742a3727445293e7650ea44dd64abd084aed85225e7608f651`  
		Last Modified: Thu, 18 Jun 2020 21:19:55 GMT  
		Size: 44.3 MB (44297385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbeef6d591983ae6e8974100916fad1e82b0125575edbee709f49fec3ad699bc`  
		Last Modified: Thu, 18 Jun 2020 21:19:48 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f004e44699b3259ca1ceed12d409fa5d9bd6b3eade8d9dfc4a135e74217f17a5`  
		Last Modified: Thu, 18 Jun 2020 21:19:48 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b16c132cbda34532a9e953bbf8f3a05560232a264cbe2ddeeec9660d88bb3f6`  
		Last Modified: Thu, 18 Jun 2020 21:19:48 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:8b795f097369c9a8b88158a7a6c74e34bdcea3ab1430c7c2203292bfd0b6376c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42149425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55333853496b4819188211dcae6bdfbe0e29b07149ebaea63f01786a0fa511fc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 18 Jun 2020 21:49:51 GMT
ENV CONSUL_VERSION=1.8.0
# Thu, 18 Jun 2020 21:49:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 18 Jun 2020 21:49:57 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 18 Jun 2020 21:50:10 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 18 Jun 2020 21:50:14 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 18 Jun 2020 21:50:16 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Jun 2020 21:50:17 GMT
VOLUME [/consul/data]
# Thu, 18 Jun 2020 21:50:18 GMT
EXPOSE 8300
# Thu, 18 Jun 2020 21:50:19 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 18 Jun 2020 21:50:20 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 18 Jun 2020 21:50:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Jun 2020 21:50:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Jun 2020 21:50:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2754231772db598bc69a198a882b6b55b2c0c0b0acbc8595b093c413fd0b16f5`  
		Last Modified: Thu, 18 Jun 2020 21:50:49 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90407def8d08fcc8c39aa2201d510e4e1abc0bfdac9edd772ff9a4df990efb75`  
		Last Modified: Thu, 18 Jun 2020 21:51:01 GMT  
		Size: 39.6 MB (39597379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5373d7576b565360a753dbf509e389e8b5f2564a65952e4c839e709a2b3afa1`  
		Last Modified: Thu, 18 Jun 2020 21:50:49 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4d87ccab463eb46b6150408675801bf7f4055d1f8373688cb15bd438a88be4d`  
		Last Modified: Thu, 18 Jun 2020 21:50:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5894dcff1d1274c5ea94e557a1e4933481ec3506b39b49896c22ba7674aaf9`  
		Last Modified: Thu, 18 Jun 2020 21:50:49 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:266753598047a982f884fd16b0c7c4d293a35fda3e2542205a02ce89acf3c2c6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.4 MB (42397134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6246d2dfaccff4f715581f879067a6fcdafb39170693a762ca4f9bb70dfa1754`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 18 Jun 2020 21:39:38 GMT
ENV CONSUL_VERSION=1.8.0
# Thu, 18 Jun 2020 21:39:39 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 18 Jun 2020 21:39:42 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 18 Jun 2020 21:39:53 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 18 Jun 2020 21:39:55 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 18 Jun 2020 21:39:57 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Jun 2020 21:39:57 GMT
VOLUME [/consul/data]
# Thu, 18 Jun 2020 21:39:58 GMT
EXPOSE 8300
# Thu, 18 Jun 2020 21:39:58 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 18 Jun 2020 21:40:00 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 18 Jun 2020 21:40:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Jun 2020 21:40:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Jun 2020 21:40:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c62d7d2a7dc49c360560cae61c091486c1c24ac03fd34b6869635a92dce5fb8`  
		Last Modified: Thu, 18 Jun 2020 21:40:24 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc98caf0c68306a78ed54f82e00c95afbd9ef917457db428e9287ca5304876e`  
		Last Modified: Thu, 18 Jun 2020 21:40:34 GMT  
		Size: 39.7 MB (39699344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fca3e93a033a25c291c52f812998843b5a8697f252d14bf06c38b3a29b3f0b`  
		Last Modified: Thu, 18 Jun 2020 21:40:25 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebcb4658c39ce46ae2c5da07e7c06b1d3ae67d73d493a08907eb038c5ac8dbf`  
		Last Modified: Thu, 18 Jun 2020 21:40:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d51dd1887d7912775dd80344979baaa67585ac709976a8166e7a0f97d3d313a`  
		Last Modified: Thu, 18 Jun 2020 21:40:24 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:9198f49897334e1e647664f3b5ab9a95c1f4b22523dc693281fbb792e56f4ea0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46512858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a0ecd9ac2104e4deebab21d46f56697c741cb988f8084f4a5d84d17dadd85a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Thu, 18 Jun 2020 21:38:21 GMT
ENV CONSUL_VERSION=1.8.0
# Thu, 18 Jun 2020 21:38:21 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Thu, 18 Jun 2020 21:38:22 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Thu, 18 Jun 2020 21:38:28 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Thu, 18 Jun 2020 21:38:28 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Thu, 18 Jun 2020 21:38:29 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 18 Jun 2020 21:38:29 GMT
VOLUME [/consul/data]
# Thu, 18 Jun 2020 21:38:30 GMT
EXPOSE 8300
# Thu, 18 Jun 2020 21:38:30 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Thu, 18 Jun 2020 21:38:30 GMT
EXPOSE 8500 8600 8600/udp
# Thu, 18 Jun 2020 21:38:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 18 Jun 2020 21:38:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 18 Jun 2020 21:38:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00127ab7c2809a649ef2dcdf53750dc4327bb66d05d975d94a4189b6184a65ee`  
		Last Modified: Thu, 18 Jun 2020 21:38:47 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436ff31cabc835ccb9432504266923e2ceb6515f0d06c9ff0147ec17bd69b762`  
		Last Modified: Thu, 18 Jun 2020 21:38:53 GMT  
		Size: 43.7 MB (43739863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:361c6767c5dbd0371aeea804fe4dac5fd3ec45e7b7be8ae70931c1e2e32a4b0f`  
		Last Modified: Thu, 18 Jun 2020 21:38:46 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075b384adfb58b589949193dc450cfbbde9e7c779a2e7fbe64ae4b851d5cc0f4`  
		Last Modified: Thu, 18 Jun 2020 21:38:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439ee1a7f0e800c206672170ea2bc0ce04a8fa6699f3a35bbad44d994cf02a3`  
		Last Modified: Thu, 18 Jun 2020 21:38:46 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
