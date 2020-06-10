<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `consul`

-	[`consul:1.6`](#consul16)
-	[`consul:1.6.6`](#consul166)
-	[`consul:1.7`](#consul17)
-	[`consul:1.7.4`](#consul174)
-	[`consul:1.8.0-beta`](#consul180-beta)
-	[`consul:1.8.0-beta2`](#consul180-beta2)
-	[`consul:latest`](#consullatest)

## `consul:1.6`

```console
$ docker pull consul@sha256:d2043c5cf46ef98acf07ed63d7e16acb656c549daad418bf314083f7b69a2aea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6` - linux; amd64

```console
$ docker pull consul@sha256:f3c1a46ccb551f51cc9be33060d5b241847bd4f3c7da158157629cae92ee0bc1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41783441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72dd2904ebc83c486c89ecb8c15feae5c04d30fdd4c9cfe9d877d440d5e3d5a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Mon, 11 May 2020 15:23:02 GMT
ENV CONSUL_VERSION=1.6.5
# Mon, 11 May 2020 15:23:03 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 11 May 2020 15:23:03 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 11 May 2020 15:23:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 11 May 2020 15:23:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 11 May 2020 15:23:09 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 11 May 2020 15:23:09 GMT
VOLUME [/consul/data]
# Mon, 11 May 2020 15:23:10 GMT
EXPOSE 8300
# Mon, 11 May 2020 15:23:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 11 May 2020 15:23:10 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 11 May 2020 15:23:10 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 11 May 2020 15:23:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 May 2020 15:23:10 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0641c4b25eaa0f33a2f426b10d5f9d2c0e98de44b4a351fd57ed3a2c1c62d7d`  
		Last Modified: Mon, 11 May 2020 15:23:48 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de30f196b08465db81cb40678d630f6f7c76e0f7233ccfe13950c12d04751029`  
		Last Modified: Mon, 11 May 2020 15:23:53 GMT  
		Size: 39.0 MB (39006771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270000dcd0f32760a1a4289b46ae4c32a9cf71fd9c178272402d42d8004bff7a`  
		Last Modified: Mon, 11 May 2020 15:23:47 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405fc018c7455c0701167ac63f9db46314fd3f0bf28cf4d61814918e2365034f`  
		Last Modified: Mon, 11 May 2020 15:23:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7830c846754ca77f31d2d600d39e33e3bece03394ec3fa503214d2e31a8c3778`  
		Last Modified: Mon, 11 May 2020 15:23:47 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:3ae67b0e23c340d08abc43a6737b9d1ac926f5b56aac4f1f2e1851aa1b74ec40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39253152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32863f89f1307478aba31a49cde6d5122d5bc1f54eed16a72f52fbf3d15963b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Mon, 11 May 2020 15:51:11 GMT
ENV CONSUL_VERSION=1.6.5
# Mon, 11 May 2020 15:51:11 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 11 May 2020 15:51:14 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 11 May 2020 15:51:23 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 11 May 2020 15:51:25 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 11 May 2020 15:51:27 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 11 May 2020 15:51:27 GMT
VOLUME [/consul/data]
# Mon, 11 May 2020 15:51:28 GMT
EXPOSE 8300
# Mon, 11 May 2020 15:51:29 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 11 May 2020 15:51:29 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 11 May 2020 15:51:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 11 May 2020 15:51:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 May 2020 15:51:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2177f11b8d0adc1055c3de9f7590c2b4f7fd7cedfea7fb70c3d4dc71a54580f`  
		Last Modified: Mon, 11 May 2020 15:52:21 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72ecce272b42a3751bbb55cbb55b89e731d0a1c14c4169258847036c4d9b356`  
		Last Modified: Mon, 11 May 2020 15:52:31 GMT  
		Size: 36.7 MB (36701104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465a55dd78f3858e5496883f5175353886022d10d3d0884ad6066861d51aaa40`  
		Last Modified: Mon, 11 May 2020 15:52:21 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f543d970f147a2272b0e6c94bfae4c6bd18bb1f45ed9e543b6fd75a7542cd19`  
		Last Modified: Mon, 11 May 2020 15:52:21 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189253e0063ec02a63abda02182fd9306fb3635cec08b6ed13d682a2987336d2`  
		Last Modified: Mon, 11 May 2020 15:52:21 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:69203bc34dc5dbc8555ab0d5619ba4f9a0186178ff305bc3100fb630dec9d8b2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.6 MB (39584243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3658346d7c5d49340f8f2f374206036ffc78e54bb9451eecad30834da239eb4c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Mon, 11 May 2020 15:41:05 GMT
ENV CONSUL_VERSION=1.6.5
# Mon, 11 May 2020 15:41:06 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 11 May 2020 15:41:08 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 11 May 2020 15:41:14 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 11 May 2020 15:41:16 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 11 May 2020 15:41:18 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 11 May 2020 15:41:19 GMT
VOLUME [/consul/data]
# Mon, 11 May 2020 15:41:19 GMT
EXPOSE 8300
# Mon, 11 May 2020 15:41:20 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 11 May 2020 15:41:20 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 11 May 2020 15:41:21 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 11 May 2020 15:41:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 May 2020 15:41:22 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2bdb5c818c059f3f52fb01831a413b40c5c7bc8bb03c498ec73b1f2d701a24`  
		Last Modified: Mon, 11 May 2020 15:42:13 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcd412aec0042805d17d40fce4c528313807089cadc17276855e547f8e036b2`  
		Last Modified: Mon, 11 May 2020 15:42:23 GMT  
		Size: 36.9 MB (36886458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055732aa318b7a9bd7d17a142104ae0af06f0a80e730daf0e1c64dbe379391c6`  
		Last Modified: Mon, 11 May 2020 15:42:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67ea0068837670219fe33ec3dec7ec7d80c5d9c7d99d9b3a9e4c709188875e8`  
		Last Modified: Mon, 11 May 2020 15:42:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8046c072348db111b11a1668f3cdaaa892aee8cbc928a89904398bf7e28ef0cc`  
		Last Modified: Mon, 11 May 2020 15:42:13 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; 386

```console
$ docker pull consul@sha256:65529f49a44ab9e2f218615c3acf439501e949ac1c4137559f5d8d0ed5d0e973
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40647251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61945d13908669cc206932ced14beca1eed2223b0d43af5c9b41a26446743d52`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Mon, 11 May 2020 15:39:15 GMT
ENV CONSUL_VERSION=1.6.5
# Mon, 11 May 2020 15:39:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Mon, 11 May 2020 15:39:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Mon, 11 May 2020 15:39:21 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Mon, 11 May 2020 15:39:22 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Mon, 11 May 2020 15:39:23 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 11 May 2020 15:39:23 GMT
VOLUME [/consul/data]
# Mon, 11 May 2020 15:39:23 GMT
EXPOSE 8300
# Mon, 11 May 2020 15:39:24 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Mon, 11 May 2020 15:39:24 GMT
EXPOSE 8500 8600 8600/udp
# Mon, 11 May 2020 15:39:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 11 May 2020 15:39:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 11 May 2020 15:39:24 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a04a102b7a32801c32eca7b9b47d6eedd0a84fa6d62e670b637224950af17b`  
		Last Modified: Mon, 11 May 2020 15:40:03 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d57500e3543cead9e7c8fa18881269a31ab722556d05a060960f5aa74d9309`  
		Last Modified: Mon, 11 May 2020 15:40:09 GMT  
		Size: 37.9 MB (37874257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84a3ee3410b826f70b57b8eda43662d2b4f8068a9c7962d599977583c534aa1`  
		Last Modified: Mon, 11 May 2020 15:40:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505c85af10149f69eb5430f85d7b11d550ad3e4204abb66c2927878470fecc1c`  
		Last Modified: Mon, 11 May 2020 15:40:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7915a117c99d7995278e3bde8978af93a2677fa0c09f8a0151542a57db4fd2`  
		Last Modified: Mon, 11 May 2020 15:40:02 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6.6`

**does not exist** (yet?)

## `consul:1.7`

```console
$ docker pull consul@sha256:1cb6f7247472638c470c1bcf059a1f74a4d54c6b49c57c80651feb08cc0a80cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:0a606f4056339c29027ab9461b6f83867e8d4efb4b984a46325c797bf8e3f995
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44104265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0544f375e878888ce2af68572e5f4ffad83f3d6c7df5f269dfc2db80d0817c8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 08 May 2020 15:19:33 GMT
ENV CONSUL_VERSION=1.7.3
# Fri, 08 May 2020 15:19:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 08 May 2020 15:19:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 08 May 2020 15:19:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 08 May 2020 15:19:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 08 May 2020 15:19:40 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 08 May 2020 15:19:40 GMT
VOLUME [/consul/data]
# Fri, 08 May 2020 15:19:40 GMT
EXPOSE 8300
# Fri, 08 May 2020 15:19:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 08 May 2020 15:19:41 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 08 May 2020 15:19:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 08 May 2020 15:19:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 May 2020 15:19:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e424a2a1e4f7b1e5a5b73c75ddef199733bdbe3241f27436067c245745edcbdd`  
		Last Modified: Fri, 08 May 2020 15:20:20 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2472846eab82d7c74c5ed3d3e8025f6cab616962340e1a00014524c754fd6ca6`  
		Last Modified: Fri, 08 May 2020 15:20:29 GMT  
		Size: 41.3 MB (41327597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24473b564e4af30b3c96f976564fc0a9aa400fd4102b5a41076434346538e290`  
		Last Modified: Fri, 08 May 2020 15:20:19 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3caf5938c68049e00ccb772a72f4af5cc3a8cc7d488f83a788ac7e909ce2859`  
		Last Modified: Fri, 08 May 2020 15:20:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f50757bb0c02ba79888de98489c8e9c7c434e41c4e4499fa948a28fadcda90`  
		Last Modified: Fri, 08 May 2020 15:20:19 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:d7a2693862e09f6bf5702ce81c56334f5593fca2163e91d1a07f8ccc66f0ef38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41440608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee64ebe85e4653ded9455fb565b411f2ff3e179d25d53a28d54e782d90e5952`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 08 May 2020 15:49:38 GMT
ENV CONSUL_VERSION=1.7.3
# Fri, 08 May 2020 15:49:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 08 May 2020 15:49:40 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 08 May 2020 15:49:54 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 08 May 2020 15:49:56 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 08 May 2020 15:49:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 08 May 2020 15:49:58 GMT
VOLUME [/consul/data]
# Fri, 08 May 2020 15:49:59 GMT
EXPOSE 8300
# Fri, 08 May 2020 15:49:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 08 May 2020 15:50:00 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 08 May 2020 15:50:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 08 May 2020 15:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 May 2020 15:50:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc3bccf0d17423118ac6395f8eaa016da3b2e496d31bf45190efc5692457fb4`  
		Last Modified: Fri, 08 May 2020 15:51:09 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efb95a4c93adcb4adbea593f3cbd417cd1c557d64eb39e34be81c9d23cd75a5`  
		Last Modified: Fri, 08 May 2020 15:51:21 GMT  
		Size: 38.9 MB (38888562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6723c1359ff86ad2d057762d978f5c0f9c53ad59877c1bb5f380d1420cc4b85`  
		Last Modified: Fri, 08 May 2020 15:51:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d6d6216a70a5cf1c24e0f8abe7e03a9aa324ecaf0b4335c69fa238829de71`  
		Last Modified: Fri, 08 May 2020 15:51:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a1446285d05800f53ed6003000c48fbed16db6eec8bda321ea376a45660ab`  
		Last Modified: Fri, 08 May 2020 15:51:08 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:86501067a9ca95b5cdc54f579c2742b9d4b33d5f253f2b2f0ec80c36074c0851
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41787020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c0b7a8b8e367d46f88327f6835080eccdbdd4bdbcf41996903faa84ed528437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 08 May 2020 15:39:47 GMT
ENV CONSUL_VERSION=1.7.3
# Fri, 08 May 2020 15:39:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 08 May 2020 15:39:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 08 May 2020 15:39:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 08 May 2020 15:39:59 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 08 May 2020 15:40:01 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 08 May 2020 15:40:02 GMT
VOLUME [/consul/data]
# Fri, 08 May 2020 15:40:02 GMT
EXPOSE 8300
# Fri, 08 May 2020 15:40:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 08 May 2020 15:40:04 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 08 May 2020 15:40:04 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 08 May 2020 15:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 May 2020 15:40:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c965350641ccc4f06d866b7da9077ef62140d972f634976f33c6a934869ca4`  
		Last Modified: Fri, 08 May 2020 15:41:02 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a422bea653b19aca71b27e90c24b574e90b9823e420e7239607643a63a30798a`  
		Last Modified: Fri, 08 May 2020 15:41:11 GMT  
		Size: 39.1 MB (39089233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107cbcca6f085aa5037d6051fe1a2c6835a998576ea8dcba9190ccf63edbb097`  
		Last Modified: Fri, 08 May 2020 15:41:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915dcd281194510e63650be226e6022e7da54a8747ca4b37b52b092cee935dc8`  
		Last Modified: Fri, 08 May 2020 15:41:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c70ac9c81703adac5ce50b289fa3a6c4ca1d5587ba749650c579db4a8d85755`  
		Last Modified: Fri, 08 May 2020 15:41:02 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:70ac805f21815bc6d4d8587e5f3f2809a6eba420fb2d304f536e5d9d7e622437
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42869621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f59fe46d1901cb3ede390618645737ae926f3655871619b6df3a6a1716c9b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 08 May 2020 15:38:22 GMT
ENV CONSUL_VERSION=1.7.3
# Fri, 08 May 2020 15:38:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 08 May 2020 15:38:23 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 08 May 2020 15:38:29 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 08 May 2020 15:38:29 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 08 May 2020 15:38:30 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 08 May 2020 15:38:30 GMT
VOLUME [/consul/data]
# Fri, 08 May 2020 15:38:30 GMT
EXPOSE 8300
# Fri, 08 May 2020 15:38:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 08 May 2020 15:38:31 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 08 May 2020 15:38:31 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 08 May 2020 15:38:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 May 2020 15:38:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67074ad1fa4d58af37c0bc0130a94be26d035bd30f386af5d57614208fd199`  
		Last Modified: Fri, 08 May 2020 15:39:12 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7d620f1fd009173372baa9be163f1170240114369e8418c37b8e0a57722936`  
		Last Modified: Fri, 08 May 2020 15:39:19 GMT  
		Size: 40.1 MB (40096626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7726eaf58abac434cdaa79e2c60e50718265a6b5887ec472615e2538996967c`  
		Last Modified: Fri, 08 May 2020 15:39:11 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4188c467045be0ffd8e6f9e951af242f4eaf6d33f196c0eeb4defc748b0129`  
		Last Modified: Fri, 08 May 2020 15:39:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be8f60cd2fa0fefffeb140780b2b368a3d0b7914e0b66d89e8993a67aaed3e2`  
		Last Modified: Fri, 08 May 2020 15:39:12 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.4`

**does not exist** (yet?)

## `consul:1.8.0-beta`

```console
$ docker pull consul@sha256:97eeab4adc2165606e92fad01392076fc82a5920adb6ef3fa1399bba3cb5f871
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.0-beta` - linux; amd64

```console
$ docker pull consul@sha256:a3f79a26b65e1d9084f743809cdb0db0efae394c79f7b2a4c278d172bdf7fcbd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47000131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a35984aceaa5222ead885ffe2c9c4e289d1dca382028cf13b3b14296496ee8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 22 May 2020 01:19:34 GMT
ENV CONSUL_VERSION=1.8.0-beta2
# Fri, 22 May 2020 01:19:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 May 2020 01:19:35 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 May 2020 01:19:39 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 May 2020 01:19:40 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 May 2020 01:19:41 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 May 2020 01:19:41 GMT
VOLUME [/consul/data]
# Fri, 22 May 2020 01:19:41 GMT
EXPOSE 8300
# Fri, 22 May 2020 01:19:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 May 2020 01:19:42 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 May 2020 01:19:42 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 May 2020 01:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 May 2020 01:19:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fbab0ab291593d034c6ed046dc219a0cf069cab9607bdc0f16db4ac03cd74d`  
		Last Modified: Fri, 22 May 2020 01:19:56 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d64c1a8230d35e89a829b46c2ad0d006a58186e658ea8f641303a5d3a25ae35`  
		Last Modified: Fri, 22 May 2020 01:20:04 GMT  
		Size: 44.2 MB (44223456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f4934f753c4e730032f40063d2c205a82e4e30154ab560fcf9422c5756a904`  
		Last Modified: Fri, 22 May 2020 01:19:57 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c934aec1029e378561f92608d0f4b51a51081e6aee5d3ba0168954d9cd11971a`  
		Last Modified: Fri, 22 May 2020 01:19:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2800aefb707471d33a8f3a0235370f0cff1228a2fc1573edc00c2a536e513b91`  
		Last Modified: Fri, 22 May 2020 01:19:56 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.0-beta` - linux; arm variant v6

```console
$ docker pull consul@sha256:e18c83498e7433cbcfbe979218ec5f6554b58b78e308d831a3c69516ee22b011
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44238520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5e51dd062127f10a730a23d809497dc2cb2a67fa2275cdfb6d49da7500ed23`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 22 May 2020 01:50:31 GMT
ENV CONSUL_VERSION=1.8.0-beta2
# Fri, 22 May 2020 01:50:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 May 2020 01:50:35 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 May 2020 01:50:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 May 2020 01:51:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 May 2020 01:51:13 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 May 2020 01:51:16 GMT
VOLUME [/consul/data]
# Fri, 22 May 2020 01:51:17 GMT
EXPOSE 8300
# Fri, 22 May 2020 01:51:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 May 2020 01:51:19 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 May 2020 01:51:20 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 May 2020 01:51:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 May 2020 01:51:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe2795ce9be8eb2c9875f02d5c2d7452be6699b70f05d85062d6726b68e1c95`  
		Last Modified: Fri, 22 May 2020 01:51:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535519dae6dc4934f66c13d33939c6dbd517a087bbf86cb159620d0213e113a`  
		Last Modified: Fri, 22 May 2020 01:52:06 GMT  
		Size: 41.7 MB (41686470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce87bd8fac36022c913489fd6e85a1767fa8bd1264ec0c540495123102c5798`  
		Last Modified: Fri, 22 May 2020 01:51:56 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9be375ddcd8314eb4fffbdcc68d60b0e3822ec17222fb30470eef9bc8657ef`  
		Last Modified: Fri, 22 May 2020 01:51:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14de88825729be62bd48b66be794297608a165297503c08b2d6d1340007e43f`  
		Last Modified: Fri, 22 May 2020 01:51:56 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.0-beta` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:648e4bf374969f78d88edddc67775c0e8f496e8f6bce9d8edabb44d3d4291b1c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44560245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99fdee285030eb00ef40847b798795ea4f675a8bf6edc1cfcf0e6b40aa40bbf8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 22 May 2020 01:39:49 GMT
ENV CONSUL_VERSION=1.8.0-beta2
# Fri, 22 May 2020 01:39:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 May 2020 01:39:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 May 2020 01:40:00 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 May 2020 01:40:02 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 May 2020 01:40:04 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 May 2020 01:40:04 GMT
VOLUME [/consul/data]
# Fri, 22 May 2020 01:40:05 GMT
EXPOSE 8300
# Fri, 22 May 2020 01:40:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 May 2020 01:40:06 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 May 2020 01:40:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 May 2020 01:40:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 May 2020 01:40:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f7fc8b735c9973cab032757f5028602ab42d6f42f0cbb5b95709f56ac9f600`  
		Last Modified: Fri, 22 May 2020 01:40:33 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f4d61f648cd6005396c5bda6555ab768be7dd9c15f6b088164f85116baf6a6`  
		Last Modified: Fri, 22 May 2020 01:40:43 GMT  
		Size: 41.9 MB (41862453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76290f4d8b4e7f41b0f9147b4b4766937d2d9813608c4ac3efb2356abb86c83c`  
		Last Modified: Fri, 22 May 2020 01:40:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188c54394c5ad2ae54446bd23069c5161b2320a68ff2f4f9f4d54ac6a75c3e67`  
		Last Modified: Fri, 22 May 2020 01:40:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc03ba883de31e297f859bfb3acadf9f1a832c0dc12815b7f5bb0e14f8a7c90e`  
		Last Modified: Fri, 22 May 2020 01:40:33 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.0-beta` - linux; 386

```console
$ docker pull consul@sha256:8a21c4e141a6bd96810a3c0cdb97acc398e38075c10f0febdf244e6a92399ac2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46453148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ef20c6c1a666ebf82647cb6e64caccc764e727d147fcf109699f68e3e4cba1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 22 May 2020 01:38:25 GMT
ENV CONSUL_VERSION=1.8.0-beta2
# Fri, 22 May 2020 01:38:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 May 2020 01:38:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 May 2020 01:38:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 May 2020 01:38:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 May 2020 01:38:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 May 2020 01:38:36 GMT
VOLUME [/consul/data]
# Fri, 22 May 2020 01:38:36 GMT
EXPOSE 8300
# Fri, 22 May 2020 01:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 May 2020 01:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 May 2020 01:38:37 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 May 2020 01:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 May 2020 01:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f70a9d705ca96a2c6c47577979b1540aafcb807763ea1d6cd039ce72567a81b`  
		Last Modified: Fri, 22 May 2020 01:38:52 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2e9a5b9d774917a193d13385978b8e0984ab555e4a43283d6bedddba10d382`  
		Last Modified: Fri, 22 May 2020 01:39:00 GMT  
		Size: 43.7 MB (43680152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8ca3ddff0e8db5199da27485a0be1579a78a88197a33d1e7721215e47548d0`  
		Last Modified: Fri, 22 May 2020 01:38:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e32bb133eeab92cd581c73d57d3d9e500cff76a2321a894dff8c8a6d89e3f8`  
		Last Modified: Fri, 22 May 2020 01:38:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1d7502b59d78b87dac1d71d771a34a7e78f10282cf978d919346324e284e9`  
		Last Modified: Fri, 22 May 2020 01:38:53 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.0-beta2`

```console
$ docker pull consul@sha256:97eeab4adc2165606e92fad01392076fc82a5920adb6ef3fa1399bba3cb5f871
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.0-beta2` - linux; amd64

```console
$ docker pull consul@sha256:a3f79a26b65e1d9084f743809cdb0db0efae394c79f7b2a4c278d172bdf7fcbd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (47000131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a35984aceaa5222ead885ffe2c9c4e289d1dca382028cf13b3b14296496ee8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 22 May 2020 01:19:34 GMT
ENV CONSUL_VERSION=1.8.0-beta2
# Fri, 22 May 2020 01:19:34 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 May 2020 01:19:35 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 May 2020 01:19:39 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 May 2020 01:19:40 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 May 2020 01:19:41 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 May 2020 01:19:41 GMT
VOLUME [/consul/data]
# Fri, 22 May 2020 01:19:41 GMT
EXPOSE 8300
# Fri, 22 May 2020 01:19:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 May 2020 01:19:42 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 May 2020 01:19:42 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 May 2020 01:19:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 May 2020 01:19:42 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fbab0ab291593d034c6ed046dc219a0cf069cab9607bdc0f16db4ac03cd74d`  
		Last Modified: Fri, 22 May 2020 01:19:56 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d64c1a8230d35e89a829b46c2ad0d006a58186e658ea8f641303a5d3a25ae35`  
		Last Modified: Fri, 22 May 2020 01:20:04 GMT  
		Size: 44.2 MB (44223456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f4934f753c4e730032f40063d2c205a82e4e30154ab560fcf9422c5756a904`  
		Last Modified: Fri, 22 May 2020 01:19:57 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c934aec1029e378561f92608d0f4b51a51081e6aee5d3ba0168954d9cd11971a`  
		Last Modified: Fri, 22 May 2020 01:19:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2800aefb707471d33a8f3a0235370f0cff1228a2fc1573edc00c2a536e513b91`  
		Last Modified: Fri, 22 May 2020 01:19:56 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.0-beta2` - linux; arm variant v6

```console
$ docker pull consul@sha256:e18c83498e7433cbcfbe979218ec5f6554b58b78e308d831a3c69516ee22b011
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44238520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5e51dd062127f10a730a23d809497dc2cb2a67fa2275cdfb6d49da7500ed23`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 22 May 2020 01:50:31 GMT
ENV CONSUL_VERSION=1.8.0-beta2
# Fri, 22 May 2020 01:50:32 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 May 2020 01:50:35 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 May 2020 01:50:56 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 May 2020 01:51:08 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 May 2020 01:51:13 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 May 2020 01:51:16 GMT
VOLUME [/consul/data]
# Fri, 22 May 2020 01:51:17 GMT
EXPOSE 8300
# Fri, 22 May 2020 01:51:18 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 May 2020 01:51:19 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 May 2020 01:51:20 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 May 2020 01:51:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 May 2020 01:51:26 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe2795ce9be8eb2c9875f02d5c2d7452be6699b70f05d85062d6726b68e1c95`  
		Last Modified: Fri, 22 May 2020 01:51:56 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3535519dae6dc4934f66c13d33939c6dbd517a087bbf86cb159620d0213e113a`  
		Last Modified: Fri, 22 May 2020 01:52:06 GMT  
		Size: 41.7 MB (41686470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce87bd8fac36022c913489fd6e85a1767fa8bd1264ec0c540495123102c5798`  
		Last Modified: Fri, 22 May 2020 01:51:56 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9be375ddcd8314eb4fffbdcc68d60b0e3822ec17222fb30470eef9bc8657ef`  
		Last Modified: Fri, 22 May 2020 01:51:56 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14de88825729be62bd48b66be794297608a165297503c08b2d6d1340007e43f`  
		Last Modified: Fri, 22 May 2020 01:51:56 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.0-beta2` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:648e4bf374969f78d88edddc67775c0e8f496e8f6bce9d8edabb44d3d4291b1c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44560245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99fdee285030eb00ef40847b798795ea4f675a8bf6edc1cfcf0e6b40aa40bbf8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 22 May 2020 01:39:49 GMT
ENV CONSUL_VERSION=1.8.0-beta2
# Fri, 22 May 2020 01:39:50 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 May 2020 01:39:52 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 May 2020 01:40:00 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 May 2020 01:40:02 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 May 2020 01:40:04 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 May 2020 01:40:04 GMT
VOLUME [/consul/data]
# Fri, 22 May 2020 01:40:05 GMT
EXPOSE 8300
# Fri, 22 May 2020 01:40:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 May 2020 01:40:06 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 May 2020 01:40:07 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 May 2020 01:40:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 May 2020 01:40:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f7fc8b735c9973cab032757f5028602ab42d6f42f0cbb5b95709f56ac9f600`  
		Last Modified: Fri, 22 May 2020 01:40:33 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f4d61f648cd6005396c5bda6555ab768be7dd9c15f6b088164f85116baf6a6`  
		Last Modified: Fri, 22 May 2020 01:40:43 GMT  
		Size: 41.9 MB (41862453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76290f4d8b4e7f41b0f9147b4b4766937d2d9813608c4ac3efb2356abb86c83c`  
		Last Modified: Fri, 22 May 2020 01:40:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188c54394c5ad2ae54446bd23069c5161b2320a68ff2f4f9f4d54ac6a75c3e67`  
		Last Modified: Fri, 22 May 2020 01:40:33 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc03ba883de31e297f859bfb3acadf9f1a832c0dc12815b7f5bb0e14f8a7c90e`  
		Last Modified: Fri, 22 May 2020 01:40:33 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.0-beta2` - linux; 386

```console
$ docker pull consul@sha256:8a21c4e141a6bd96810a3c0cdb97acc398e38075c10f0febdf244e6a92399ac2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46453148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14ef20c6c1a666ebf82647cb6e64caccc764e727d147fcf109699f68e3e4cba1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 22 May 2020 01:38:25 GMT
ENV CONSUL_VERSION=1.8.0-beta2
# Fri, 22 May 2020 01:38:26 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 22 May 2020 01:38:27 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 22 May 2020 01:38:34 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 22 May 2020 01:38:35 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 22 May 2020 01:38:36 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 22 May 2020 01:38:36 GMT
VOLUME [/consul/data]
# Fri, 22 May 2020 01:38:36 GMT
EXPOSE 8300
# Fri, 22 May 2020 01:38:37 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 22 May 2020 01:38:37 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 22 May 2020 01:38:37 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 22 May 2020 01:38:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 22 May 2020 01:38:38 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f70a9d705ca96a2c6c47577979b1540aafcb807763ea1d6cd039ce72567a81b`  
		Last Modified: Fri, 22 May 2020 01:38:52 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2e9a5b9d774917a193d13385978b8e0984ab555e4a43283d6bedddba10d382`  
		Last Modified: Fri, 22 May 2020 01:39:00 GMT  
		Size: 43.7 MB (43680152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8ca3ddff0e8db5199da27485a0be1579a78a88197a33d1e7721215e47548d0`  
		Last Modified: Fri, 22 May 2020 01:38:52 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e32bb133eeab92cd581c73d57d3d9e500cff76a2321a894dff8c8a6d89e3f8`  
		Last Modified: Fri, 22 May 2020 01:38:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e1d7502b59d78b87dac1d71d771a34a7e78f10282cf978d919346324e284e9`  
		Last Modified: Fri, 22 May 2020 01:38:53 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:1cb6f7247472638c470c1bcf059a1f74a4d54c6b49c57c80651feb08cc0a80cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:0a606f4056339c29027ab9461b6f83867e8d4efb4b984a46325c797bf8e3f995
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44104265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0544f375e878888ce2af68572e5f4ffad83f3d6c7df5f269dfc2db80d0817c8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:17:15 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 08 May 2020 15:19:33 GMT
ENV CONSUL_VERSION=1.7.3
# Fri, 08 May 2020 15:19:33 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 08 May 2020 15:19:34 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 08 May 2020 15:19:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 08 May 2020 15:19:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 08 May 2020 15:19:40 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 08 May 2020 15:19:40 GMT
VOLUME [/consul/data]
# Fri, 08 May 2020 15:19:40 GMT
EXPOSE 8300
# Fri, 08 May 2020 15:19:41 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 08 May 2020 15:19:41 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 08 May 2020 15:19:41 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 08 May 2020 15:19:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 May 2020 15:19:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e424a2a1e4f7b1e5a5b73c75ddef199733bdbe3241f27436067c245745edcbdd`  
		Last Modified: Fri, 08 May 2020 15:20:20 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2472846eab82d7c74c5ed3d3e8025f6cab616962340e1a00014524c754fd6ca6`  
		Last Modified: Fri, 08 May 2020 15:20:29 GMT  
		Size: 41.3 MB (41327597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24473b564e4af30b3c96f976564fc0a9aa400fd4102b5a41076434346538e290`  
		Last Modified: Fri, 08 May 2020 15:20:19 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3caf5938c68049e00ccb772a72f4af5cc3a8cc7d488f83a788ac7e909ce2859`  
		Last Modified: Fri, 08 May 2020 15:20:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f50757bb0c02ba79888de98489c8e9c7c434e41c4e4499fa948a28fadcda90`  
		Last Modified: Fri, 08 May 2020 15:20:19 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:d7a2693862e09f6bf5702ce81c56334f5593fca2163e91d1a07f8ccc66f0ef38
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41440608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ee64ebe85e4653ded9455fb565b411f2ff3e179d25d53a28d54e782d90e5952`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:44 GMT
ADD file:7dd2657543fac7f63a125194d27bd38a8e472a3076831a2331c43a471794c210 in / 
# Thu, 23 Apr 2020 15:51:45 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 16:53:13 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 08 May 2020 15:49:38 GMT
ENV CONSUL_VERSION=1.7.3
# Fri, 08 May 2020 15:49:38 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 08 May 2020 15:49:40 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 08 May 2020 15:49:54 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 08 May 2020 15:49:56 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 08 May 2020 15:49:58 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 08 May 2020 15:49:58 GMT
VOLUME [/consul/data]
# Fri, 08 May 2020 15:49:59 GMT
EXPOSE 8300
# Fri, 08 May 2020 15:49:59 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 08 May 2020 15:50:00 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 08 May 2020 15:50:00 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 08 May 2020 15:50:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 May 2020 15:50:01 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:27da80392aebe463671b839837d59af1261218364b4261ceb2eca0f814075270`  
		Last Modified: Thu, 23 Apr 2020 15:52:21 GMT  
		Size: 2.5 MB (2548725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc3bccf0d17423118ac6395f8eaa016da3b2e496d31bf45190efc5692457fb4`  
		Last Modified: Fri, 08 May 2020 15:51:09 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efb95a4c93adcb4adbea593f3cbd417cd1c557d64eb39e34be81c9d23cd75a5`  
		Last Modified: Fri, 08 May 2020 15:51:21 GMT  
		Size: 38.9 MB (38888562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6723c1359ff86ad2d057762d978f5c0f9c53ad59877c1bb5f380d1420cc4b85`  
		Last Modified: Fri, 08 May 2020 15:51:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9d6d6216a70a5cf1c24e0f8abe7e03a9aa324ecaf0b4335c69fa238829de71`  
		Last Modified: Fri, 08 May 2020 15:51:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9a1446285d05800f53ed6003000c48fbed16db6eec8bda321ea376a45660ab`  
		Last Modified: Fri, 08 May 2020 15:51:08 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:86501067a9ca95b5cdc54f579c2742b9d4b33d5f253f2b2f0ec80c36074c0851
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41787020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c0b7a8b8e367d46f88327f6835080eccdbdd4bdbcf41996903faa84ed528437`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 00:15:12 GMT
ADD file:da3ddeca2212f561c1f428b662a1f1f1200e2d18a42bffb28a0322c235f06582 in / 
# Fri, 24 Apr 2020 00:15:15 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:22:17 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 08 May 2020 15:39:47 GMT
ENV CONSUL_VERSION=1.7.3
# Fri, 08 May 2020 15:39:48 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 08 May 2020 15:39:50 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 08 May 2020 15:39:57 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 08 May 2020 15:39:59 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 08 May 2020 15:40:01 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 08 May 2020 15:40:02 GMT
VOLUME [/consul/data]
# Fri, 08 May 2020 15:40:02 GMT
EXPOSE 8300
# Fri, 08 May 2020 15:40:03 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 08 May 2020 15:40:04 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 08 May 2020 15:40:04 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 08 May 2020 15:40:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 May 2020 15:40:05 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:941f399634ec37b35e6764d0e6cf350593652f06f76586d45ddfc0d77de7a701`  
		Last Modified: Fri, 24 Apr 2020 00:16:02 GMT  
		Size: 2.7 MB (2694467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c965350641ccc4f06d866b7da9077ef62140d972f634976f33c6a934869ca4`  
		Last Modified: Fri, 08 May 2020 15:41:02 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a422bea653b19aca71b27e90c24b574e90b9823e420e7239607643a63a30798a`  
		Last Modified: Fri, 08 May 2020 15:41:11 GMT  
		Size: 39.1 MB (39089233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107cbcca6f085aa5037d6051fe1a2c6835a998576ea8dcba9190ccf63edbb097`  
		Last Modified: Fri, 08 May 2020 15:41:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915dcd281194510e63650be226e6022e7da54a8747ca4b37b52b092cee935dc8`  
		Last Modified: Fri, 08 May 2020 15:41:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c70ac9c81703adac5ce50b289fa3a6c4ca1d5587ba749650c579db4a8d85755`  
		Last Modified: Fri, 08 May 2020 15:41:02 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:70ac805f21815bc6d4d8587e5f3f2809a6eba420fb2d304f536e5d9d7e622437
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.9 MB (42869621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f59fe46d1901cb3ede390618645737ae926f3655871619b6df3a6a1716c9b6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:18 GMT
ADD file:68d5786259963a2b97cf808d79de83cbd0281dfea284e1a401bc851a3585e1bd in / 
# Thu, 23 Apr 2020 21:16:19 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 04:30:33 GMT
MAINTAINER Consul Team <consul@hashicorp.com>
# Fri, 08 May 2020 15:38:22 GMT
ENV CONSUL_VERSION=1.7.3
# Fri, 08 May 2020 15:38:22 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 08 May 2020 15:38:23 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 08 May 2020 15:38:29 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 08 May 2020 15:38:29 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 08 May 2020 15:38:30 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 08 May 2020 15:38:30 GMT
VOLUME [/consul/data]
# Fri, 08 May 2020 15:38:30 GMT
EXPOSE 8300
# Fri, 08 May 2020 15:38:31 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 08 May 2020 15:38:31 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 08 May 2020 15:38:31 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 08 May 2020 15:38:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 08 May 2020 15:38:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2f4fdbe0599cb5bbd0664b1cdad4997f428ce2495ae3eabf942129dc197d991c`  
		Last Modified: Thu, 23 Apr 2020 21:16:41 GMT  
		Size: 2.8 MB (2769736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b67074ad1fa4d58af37c0bc0130a94be26d035bd30f386af5d57614208fd199`  
		Last Modified: Fri, 08 May 2020 15:39:12 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a7d620f1fd009173372baa9be163f1170240114369e8418c37b8e0a57722936`  
		Last Modified: Fri, 08 May 2020 15:39:19 GMT  
		Size: 40.1 MB (40096626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7726eaf58abac434cdaa79e2c60e50718265a6b5887ec472615e2538996967c`  
		Last Modified: Fri, 08 May 2020 15:39:11 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4188c467045be0ffd8e6f9e951af242f4eaf6d33f196c0eeb4defc748b0129`  
		Last Modified: Fri, 08 May 2020 15:39:11 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be8f60cd2fa0fefffeb140780b2b368a3d0b7914e0b66d89e8993a67aaed3e2`  
		Last Modified: Fri, 08 May 2020 15:39:12 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
