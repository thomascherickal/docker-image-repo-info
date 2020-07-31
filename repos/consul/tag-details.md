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
$ docker pull consul@sha256:f4d2b7eab05b0b11519141b3edcaf24b7a160d65eb69aae7c42c1749e99614fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6` - linux; amd64

```console
$ docker pull consul@sha256:7e451d410e93fdad86fd414a0bb1a79a084769fd37272eb2dbc536467ab5125c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42254468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d6a83de1eec544b47d40159c8bd02579659368ade63c9c0c38de3d402f6f0bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 18:22:27 GMT
ENV CONSUL_VERSION=1.6.7
# Fri, 31 Jul 2020 18:22:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 18:22:28 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 18:22:32 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 18:22:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 18:22:34 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 18:22:34 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 18:22:34 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 18:22:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 18:22:35 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 18:22:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 18:22:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 18:22:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df922bad04f5ac59efc0fa5277c0ef4f5471d712df00e069911595a4d6bed2a0`  
		Last Modified: Fri, 31 Jul 2020 18:23:07 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6fcec5029051f2c40af37ea6d467a98975548af83b8c17bbc9626a3486d15b`  
		Last Modified: Fri, 31 Jul 2020 18:23:13 GMT  
		Size: 39.5 MB (39453693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7141573529fb4863e48ef2204e81ff996063be4c4ae28aa408ea18476d2098c`  
		Last Modified: Fri, 31 Jul 2020 18:23:07 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c436a7d2ecc018e823ccd88cdf82a887885c8370bb934333a5278bf064c40319`  
		Last Modified: Fri, 31 Jul 2020 18:23:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b37a70bff180b53d72e13c88ce61e8a299f945ff6481447ce808ff8e12d412e`  
		Last Modified: Fri, 31 Jul 2020 18:23:07 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm variant v6

```console
$ docker pull consul@sha256:2015438f183e913ab8d11f4550d81b6ac973c5c2f42e8bc3ea4ae815d49aef48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37930217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b409ac9cfaaed83e0ab54eac8d0d4cd3b90ebc712c8defe099464546d91020e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:50:35 GMT
ENV CONSUL_VERSION=1.6.7
# Fri, 31 Jul 2020 17:50:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:50:38 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:50:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:50:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:50:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:50:53 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:50:55 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:50:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:50:56 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:50:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:50:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:50:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda298b877304e48bd0ec5aae542d1a75e1e085945cf39f1bc77d6c4e62bab34`  
		Last Modified: Fri, 31 Jul 2020 17:51:45 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171aafe91e7566567ebf14328105e10ca713b8c9f95bb25dfda8d8353c6570da`  
		Last Modified: Fri, 31 Jul 2020 17:51:55 GMT  
		Size: 35.3 MB (35323638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328aa30b2b10e63e52456895bc714f0bb96e59c6b0b1eaa284d8385e0501fb05`  
		Last Modified: Fri, 31 Jul 2020 17:51:46 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ea45c7cdddf86a1f86effcf53ad293ee5ddfb5fe0163824954dbaba6fcd62a`  
		Last Modified: Fri, 31 Jul 2020 17:51:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e53270b75186cdf11d5d90d08183fbcfcbbe1803022b873b88c7c1a47cb1a88`  
		Last Modified: Fri, 31 Jul 2020 17:51:46 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:ee842af81f03748b142f74ad0439d269f862f8ae9c72d5d819eb6d126d13d753
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38153144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd858edf11600f6431a6382cb835f8895836cb9713aedab8879efcd7df752157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:43:14 GMT
ENV CONSUL_VERSION=1.6.7
# Fri, 31 Jul 2020 17:43:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:43:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:43:23 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:43:25 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:43:27 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:43:28 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:43:28 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:43:29 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:43:29 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:43:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:43:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:43:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3f28fb3c9c9aa5d8bc245b56970995d694cfcf0a1d8357a778c38094fa70c8`  
		Last Modified: Fri, 31 Jul 2020 17:44:23 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9562429ca6ff99175d00aa88c5f214f69a4619a0d0e455a7c781bbaac9e75047`  
		Last Modified: Fri, 31 Jul 2020 17:44:31 GMT  
		Size: 35.4 MB (35441888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4118248e5d19f06cb1a6db13f15a117509662af9c6c6a788197bfd6a6f05067`  
		Last Modified: Fri, 31 Jul 2020 17:44:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cef3bd73b4aab629620f7c0dcbbcfe6c1cf5a67c3ce4abba1fd3e5efae17e0`  
		Last Modified: Fri, 31 Jul 2020 17:44:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8234166d30bd0e2af0500a26a007fb986e8b60003755eab7db21ec829a5761`  
		Last Modified: Fri, 31 Jul 2020 17:44:23 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6` - linux; 386

```console
$ docker pull consul@sha256:93624ab83f6062d8208ca521c9642d03a4e7e6e9f6d5523964eea8f99ec11118
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41085086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75df4e5b1f532fa134f9315d7f876e2204d0d627221bb3ace4ef3e14f13d55e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:38:59 GMT
ENV CONSUL_VERSION=1.6.7
# Fri, 31 Jul 2020 17:38:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:39:00 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:39:05 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:39:06 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:39:07 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:39:07 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:39:07 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:39:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:39:07 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:39:08 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:39:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:39:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc364ac9a142ab02ceb2d77857d6f3f3134c33baccf21cbc98ecd00dbb6fb329`  
		Last Modified: Fri, 31 Jul 2020 17:39:43 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca173127c57399f5f594b39705256c2483bfa3d6b0e49022b54ec3a36b357e7`  
		Last Modified: Fri, 31 Jul 2020 17:39:50 GMT  
		Size: 38.3 MB (38289553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fe5ad821812936b55ac10b7c9e5a385e439f0f32ebe625f96ae2c4d2821011`  
		Last Modified: Fri, 31 Jul 2020 17:39:43 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c026afc38e0ca0d479dd697dc0474da48296504d199378700b50a5d61c9baeb7`  
		Last Modified: Fri, 31 Jul 2020 17:39:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b7d2d957df9f166bbdee492fb786a3bf0076d10f161f83b0552465fcbea03`  
		Last Modified: Fri, 31 Jul 2020 17:39:43 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.6.7`

```console
$ docker pull consul@sha256:f4d2b7eab05b0b11519141b3edcaf24b7a160d65eb69aae7c42c1749e99614fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.6.7` - linux; amd64

```console
$ docker pull consul@sha256:7e451d410e93fdad86fd414a0bb1a79a084769fd37272eb2dbc536467ab5125c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42254468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d6a83de1eec544b47d40159c8bd02579659368ade63c9c0c38de3d402f6f0bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 18:22:27 GMT
ENV CONSUL_VERSION=1.6.7
# Fri, 31 Jul 2020 18:22:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 18:22:28 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 18:22:32 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 18:22:33 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 18:22:34 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 18:22:34 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 18:22:34 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 18:22:35 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 18:22:35 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 18:22:35 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 18:22:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 18:22:35 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df922bad04f5ac59efc0fa5277c0ef4f5471d712df00e069911595a4d6bed2a0`  
		Last Modified: Fri, 31 Jul 2020 18:23:07 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6fcec5029051f2c40af37ea6d467a98975548af83b8c17bbc9626a3486d15b`  
		Last Modified: Fri, 31 Jul 2020 18:23:13 GMT  
		Size: 39.5 MB (39453693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7141573529fb4863e48ef2204e81ff996063be4c4ae28aa408ea18476d2098c`  
		Last Modified: Fri, 31 Jul 2020 18:23:07 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c436a7d2ecc018e823ccd88cdf82a887885c8370bb934333a5278bf064c40319`  
		Last Modified: Fri, 31 Jul 2020 18:23:07 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b37a70bff180b53d72e13c88ce61e8a299f945ff6481447ce808ff8e12d412e`  
		Last Modified: Fri, 31 Jul 2020 18:23:07 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:2015438f183e913ab8d11f4550d81b6ac973c5c2f42e8bc3ea4ae815d49aef48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37930217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b409ac9cfaaed83e0ab54eac8d0d4cd3b90ebc712c8defe099464546d91020e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:50:35 GMT
ENV CONSUL_VERSION=1.6.7
# Fri, 31 Jul 2020 17:50:36 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:50:38 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:50:47 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:50:50 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:50:52 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:50:53 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:50:55 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:50:55 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:50:56 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:50:57 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:50:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:50:58 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda298b877304e48bd0ec5aae542d1a75e1e085945cf39f1bc77d6c4e62bab34`  
		Last Modified: Fri, 31 Jul 2020 17:51:45 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171aafe91e7566567ebf14328105e10ca713b8c9f95bb25dfda8d8353c6570da`  
		Last Modified: Fri, 31 Jul 2020 17:51:55 GMT  
		Size: 35.3 MB (35323638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328aa30b2b10e63e52456895bc714f0bb96e59c6b0b1eaa284d8385e0501fb05`  
		Last Modified: Fri, 31 Jul 2020 17:51:46 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ea45c7cdddf86a1f86effcf53ad293ee5ddfb5fe0163824954dbaba6fcd62a`  
		Last Modified: Fri, 31 Jul 2020 17:51:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e53270b75186cdf11d5d90d08183fbcfcbbe1803022b873b88c7c1a47cb1a88`  
		Last Modified: Fri, 31 Jul 2020 17:51:46 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:ee842af81f03748b142f74ad0439d269f862f8ae9c72d5d819eb6d126d13d753
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38153144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd858edf11600f6431a6382cb835f8895836cb9713aedab8879efcd7df752157`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:43:14 GMT
ENV CONSUL_VERSION=1.6.7
# Fri, 31 Jul 2020 17:43:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:43:17 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:43:23 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:43:25 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:43:27 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:43:28 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:43:28 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:43:29 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:43:29 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:43:30 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:43:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:43:31 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3f28fb3c9c9aa5d8bc245b56970995d694cfcf0a1d8357a778c38094fa70c8`  
		Last Modified: Fri, 31 Jul 2020 17:44:23 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9562429ca6ff99175d00aa88c5f214f69a4619a0d0e455a7c781bbaac9e75047`  
		Last Modified: Fri, 31 Jul 2020 17:44:31 GMT  
		Size: 35.4 MB (35441888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4118248e5d19f06cb1a6db13f15a117509662af9c6c6a788197bfd6a6f05067`  
		Last Modified: Fri, 31 Jul 2020 17:44:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9cef3bd73b4aab629620f7c0dcbbcfe6c1cf5a67c3ce4abba1fd3e5efae17e0`  
		Last Modified: Fri, 31 Jul 2020 17:44:23 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8234166d30bd0e2af0500a26a007fb986e8b60003755eab7db21ec829a5761`  
		Last Modified: Fri, 31 Jul 2020 17:44:23 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.6.7` - linux; 386

```console
$ docker pull consul@sha256:93624ab83f6062d8208ca521c9642d03a4e7e6e9f6d5523964eea8f99ec11118
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41085086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75df4e5b1f532fa134f9315d7f876e2204d0d627221bb3ace4ef3e14f13d55e2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:38:59 GMT
ENV CONSUL_VERSION=1.6.7
# Fri, 31 Jul 2020 17:38:59 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:39:00 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:39:05 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:39:06 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:39:07 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:39:07 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:39:07 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:39:07 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:39:07 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:39:08 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:39:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:39:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc364ac9a142ab02ceb2d77857d6f3f3134c33baccf21cbc98ecd00dbb6fb329`  
		Last Modified: Fri, 31 Jul 2020 17:39:43 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca173127c57399f5f594b39705256c2483bfa3d6b0e49022b54ec3a36b357e7`  
		Last Modified: Fri, 31 Jul 2020 17:39:50 GMT  
		Size: 38.3 MB (38289553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50fe5ad821812936b55ac10b7c9e5a385e439f0f32ebe625f96ae2c4d2821011`  
		Last Modified: Fri, 31 Jul 2020 17:39:43 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c026afc38e0ca0d479dd697dc0474da48296504d199378700b50a5d61c9baeb7`  
		Last Modified: Fri, 31 Jul 2020 17:39:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2b7d2d957df9f166bbdee492fb786a3bf0076d10f161f83b0552465fcbea03`  
		Last Modified: Fri, 31 Jul 2020 17:39:43 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7`

```console
$ docker pull consul@sha256:974195228a3f48789053b4de1052fd7b938a73d37ec067452073db2f31dfa4dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7` - linux; amd64

```console
$ docker pull consul@sha256:7a569b995bc597407df0787e95b3f75d365d5197c960d960fae5dbb61fb68151
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.5 MB (43471815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e17c5eba17757cb96b91e4a00ad5a4dd3fdf637b036df7fe9044901b87abe1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 18:22:15 GMT
ENV CONSUL_VERSION=1.7.5
# Fri, 31 Jul 2020 18:22:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 18:22:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 18:22:20 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 18:22:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 18:22:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 18:22:22 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 18:22:22 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 18:22:22 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 18:22:23 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 18:22:23 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 18:22:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 18:22:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423e0a9e281e88f774cfbfa2ce7624d9a630e2b40e931fe0f554758e441a488f`  
		Last Modified: Fri, 31 Jul 2020 18:22:56 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be861351ed7cb3a876cace7f9fb0e9ee5ae8363f98c418c0a4539960d6956daa`  
		Last Modified: Fri, 31 Jul 2020 18:23:03 GMT  
		Size: 40.7 MB (40671039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca6a3fe0d3cd03789ac9f98de3f91d6d994a56dcacc80da1683be74a4142d7d`  
		Last Modified: Fri, 31 Jul 2020 18:22:56 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a0731915b4dddab77ba67051bb33267129ae6519267ba08a754cd64fe9d07c`  
		Last Modified: Fri, 31 Jul 2020 18:22:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eea61a9a84126ebaa7ebe0f943862774547d9f4f21f26d812152b60b43df973`  
		Last Modified: Fri, 31 Jul 2020 18:22:57 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm variant v6

```console
$ docker pull consul@sha256:d6fbd75d9ab7c6ffbe84eaf7b5f8a820109f8e7c191a7f747c7a0226075da0c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39159653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b0fa8363efd4c1f917dd20d70f8750248688cbb2fe17e74998c3479ed2be928`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:50:03 GMT
ENV CONSUL_VERSION=1.7.5
# Fri, 31 Jul 2020 17:50:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:50:06 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:50:17 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:50:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:50:21 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:50:22 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:50:22 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:50:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:50:24 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:50:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:50:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d48fe862a70fcd8ffc7f4f308571d7dd97aa5c6c0e9c5aca53339e28ff2b636`  
		Last Modified: Fri, 31 Jul 2020 17:51:30 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1748148a878cff411e25df6de741b5eddfb1a639d4b240dda9a7211ecb689e`  
		Last Modified: Fri, 31 Jul 2020 17:51:40 GMT  
		Size: 36.6 MB (36553073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7ef7a1b2e154f040524b61d62bc5c1b76c2c06d61ef7100844957ba0c4c128`  
		Last Modified: Fri, 31 Jul 2020 17:51:30 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae31ccf32c20c8a6c0a504b045e5ebf3bf3bbadf37161e7e10f462d99887ec`  
		Last Modified: Fri, 31 Jul 2020 17:51:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ddfb092bdd961e3ab932bc974851b3854a807b5a77c6535a90d9b44204fb88`  
		Last Modified: Fri, 31 Jul 2020 17:51:30 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b4c207f40bd03c29f1d058a97c582ac8bbd49883d363d772be9b69a63b785fb7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.4 MB (39390589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1505a07314eb391526f38eb33dd97ad1f1c1730f65c6b57c371a0bab4135997d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:42:51 GMT
ENV CONSUL_VERSION=1.7.5
# Fri, 31 Jul 2020 17:42:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:42:53 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:42:59 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:43:01 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:43:03 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:43:04 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:43:04 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:43:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:43:06 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:43:06 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:43:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e636f6d6e717e7e1071947603be177ca2ed25a81f259dcc2812111653701af5c`  
		Last Modified: Fri, 31 Jul 2020 17:44:06 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4d552730bae025cf262a6f48812bb0b1e3d176c8680a48771adeb79dd06998`  
		Last Modified: Fri, 31 Jul 2020 17:44:15 GMT  
		Size: 36.7 MB (36679332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca3b099b122c2a9af551af5c0e0aed3125998ed6dba8df0a77ae3aea143006`  
		Last Modified: Fri, 31 Jul 2020 17:44:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149be8b177253429ddd6154e45333b83e5375870e3f8adaba97e10c11f8ec3fc`  
		Last Modified: Fri, 31 Jul 2020 17:44:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f26b0288efa75c7cd9c48a16cd4da2bca900ba465f52c344dcd75e403b10d5`  
		Last Modified: Fri, 31 Jul 2020 17:44:06 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7` - linux; 386

```console
$ docker pull consul@sha256:9342fea5f08f16c8c0c268682712b7376c44ee6b9b78d0da15f41a747c71d693
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42262488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599c1ab93da5b12e48a8c4b6383bf37657b224f0047fc11efe8be2ccf34bf8b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:38:45 GMT
ENV CONSUL_VERSION=1.7.5
# Fri, 31 Jul 2020 17:38:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:38:46 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:38:51 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:38:52 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:38:53 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:38:53 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:38:53 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:38:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:38:53 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:38:54 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:38:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:38:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde0bccade9e9fa56f42a8e764aa4c2b08c56d85777a7b252ccc224919415ee`  
		Last Modified: Fri, 31 Jul 2020 17:39:31 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a5fe301507d08374c125e827b1c8d31ec0ef88816286fd3a8ff6708166934f`  
		Last Modified: Fri, 31 Jul 2020 17:39:39 GMT  
		Size: 39.5 MB (39466956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aa3c2b0263bb4e0056563908c6eb22fcf172596977c37db1224b01277909d0`  
		Last Modified: Fri, 31 Jul 2020 17:39:31 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374477c9f66b6c69d709eb88f646f5ab1a9b5adb3700577f416e069429dec80c`  
		Last Modified: Fri, 31 Jul 2020 17:39:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a7a2ce8d3f6a65d77a62e9228c64bced408ab044de88e64eb043f483362c9`  
		Last Modified: Fri, 31 Jul 2020 17:39:31 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.7.5`

```console
$ docker pull consul@sha256:974195228a3f48789053b4de1052fd7b938a73d37ec067452073db2f31dfa4dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.7.5` - linux; amd64

```console
$ docker pull consul@sha256:7a569b995bc597407df0787e95b3f75d365d5197c960d960fae5dbb61fb68151
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.5 MB (43471815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e17c5eba17757cb96b91e4a00ad5a4dd3fdf637b036df7fe9044901b87abe1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 18:22:15 GMT
ENV CONSUL_VERSION=1.7.5
# Fri, 31 Jul 2020 18:22:15 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 18:22:16 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 18:22:20 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 18:22:21 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 18:22:22 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 18:22:22 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 18:22:22 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 18:22:22 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 18:22:23 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 18:22:23 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 18:22:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 18:22:23 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423e0a9e281e88f774cfbfa2ce7624d9a630e2b40e931fe0f554758e441a488f`  
		Last Modified: Fri, 31 Jul 2020 18:22:56 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be861351ed7cb3a876cace7f9fb0e9ee5ae8363f98c418c0a4539960d6956daa`  
		Last Modified: Fri, 31 Jul 2020 18:23:03 GMT  
		Size: 40.7 MB (40671039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca6a3fe0d3cd03789ac9f98de3f91d6d994a56dcacc80da1683be74a4142d7d`  
		Last Modified: Fri, 31 Jul 2020 18:22:56 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a0731915b4dddab77ba67051bb33267129ae6519267ba08a754cd64fe9d07c`  
		Last Modified: Fri, 31 Jul 2020 18:22:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eea61a9a84126ebaa7ebe0f943862774547d9f4f21f26d812152b60b43df973`  
		Last Modified: Fri, 31 Jul 2020 18:22:57 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.5` - linux; arm variant v6

```console
$ docker pull consul@sha256:d6fbd75d9ab7c6ffbe84eaf7b5f8a820109f8e7c191a7f747c7a0226075da0c9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.2 MB (39159653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b0fa8363efd4c1f917dd20d70f8750248688cbb2fe17e74998c3479ed2be928`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:50:03 GMT
ENV CONSUL_VERSION=1.7.5
# Fri, 31 Jul 2020 17:50:04 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:50:06 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:50:17 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:50:19 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:50:21 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:50:22 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:50:22 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:50:23 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:50:24 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:50:24 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:50:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:50:25 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d48fe862a70fcd8ffc7f4f308571d7dd97aa5c6c0e9c5aca53339e28ff2b636`  
		Last Modified: Fri, 31 Jul 2020 17:51:30 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1748148a878cff411e25df6de741b5eddfb1a639d4b240dda9a7211ecb689e`  
		Last Modified: Fri, 31 Jul 2020 17:51:40 GMT  
		Size: 36.6 MB (36553073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7ef7a1b2e154f040524b61d62bc5c1b76c2c06d61ef7100844957ba0c4c128`  
		Last Modified: Fri, 31 Jul 2020 17:51:30 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ae31ccf32c20c8a6c0a504b045e5ebf3bf3bbadf37161e7e10f462d99887ec`  
		Last Modified: Fri, 31 Jul 2020 17:51:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ddfb092bdd961e3ab932bc974851b3854a807b5a77c6535a90d9b44204fb88`  
		Last Modified: Fri, 31 Jul 2020 17:51:30 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.5` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:b4c207f40bd03c29f1d058a97c582ac8bbd49883d363d772be9b69a63b785fb7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.4 MB (39390589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1505a07314eb391526f38eb33dd97ad1f1c1730f65c6b57c371a0bab4135997d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:42:51 GMT
ENV CONSUL_VERSION=1.7.5
# Fri, 31 Jul 2020 17:42:51 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:42:53 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:42:59 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:43:01 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:43:03 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:43:04 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:43:04 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:43:05 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:43:06 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:43:06 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:43:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:43:08 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e636f6d6e717e7e1071947603be177ca2ed25a81f259dcc2812111653701af5c`  
		Last Modified: Fri, 31 Jul 2020 17:44:06 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4d552730bae025cf262a6f48812bb0b1e3d176c8680a48771adeb79dd06998`  
		Last Modified: Fri, 31 Jul 2020 17:44:15 GMT  
		Size: 36.7 MB (36679332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca3b099b122c2a9af551af5c0e0aed3125998ed6dba8df0a77ae3aea143006`  
		Last Modified: Fri, 31 Jul 2020 17:44:06 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149be8b177253429ddd6154e45333b83e5375870e3f8adaba97e10c11f8ec3fc`  
		Last Modified: Fri, 31 Jul 2020 17:44:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f26b0288efa75c7cd9c48a16cd4da2bca900ba465f52c344dcd75e403b10d5`  
		Last Modified: Fri, 31 Jul 2020 17:44:06 GMT  
		Size: 1.7 KB (1708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.7.5` - linux; 386

```console
$ docker pull consul@sha256:9342fea5f08f16c8c0c268682712b7376c44ee6b9b78d0da15f41a747c71d693
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42262488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:599c1ab93da5b12e48a8c4b6383bf37657b224f0047fc11efe8be2ccf34bf8b8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:38:45 GMT
ENV CONSUL_VERSION=1.7.5
# Fri, 31 Jul 2020 17:38:45 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:38:46 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:38:51 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:38:52 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:38:53 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:38:53 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:38:53 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:38:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:38:53 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:38:54 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:38:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:38:54 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fde0bccade9e9fa56f42a8e764aa4c2b08c56d85777a7b252ccc224919415ee`  
		Last Modified: Fri, 31 Jul 2020 17:39:31 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a5fe301507d08374c125e827b1c8d31ec0ef88816286fd3a8ff6708166934f`  
		Last Modified: Fri, 31 Jul 2020 17:39:39 GMT  
		Size: 39.5 MB (39466956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aa3c2b0263bb4e0056563908c6eb22fcf172596977c37db1224b01277909d0`  
		Last Modified: Fri, 31 Jul 2020 17:39:31 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374477c9f66b6c69d709eb88f646f5ab1a9b5adb3700577f416e069429dec80c`  
		Last Modified: Fri, 31 Jul 2020 17:39:31 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a7a2ce8d3f6a65d77a62e9228c64bced408ab044de88e64eb043f483362c9`  
		Last Modified: Fri, 31 Jul 2020 17:39:31 GMT  
		Size: 1.7 KB (1706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8`

```console
$ docker pull consul@sha256:5b66b9781bea2c07fa1b1ceaf5e91c0ed95b1870f3f501731ebab0f0c84c8f1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8` - linux; amd64

```console
$ docker pull consul@sha256:2a5ddca1929c5e648fe69ac13eb9e23049f249e763c73677ad7cd0d6849e3b66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46709469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c8f1c8872c4eaae98e9a70a6dc42266b2aa35c26c1014d70fd35f7b334520`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 18:22:03 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 18:22:03 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 18:22:04 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 18:22:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 18:22:09 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 18:22:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 18:22:10 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 18:22:10 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 18:22:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 18:22:10 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 18:22:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 18:22:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 18:22:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc867292762be8dd9acce45a84106283f82fcf761880f48abb17bbda49aaae`  
		Last Modified: Fri, 31 Jul 2020 18:22:44 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a6bf4b5df2c0de7dd2d03c2c677c65163b177a24be41f5390af6677231891`  
		Last Modified: Fri, 31 Jul 2020 18:22:50 GMT  
		Size: 43.9 MB (43908692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33980ad85a4aff457107f89b4cb0381380ea383972301a4213e0f0326e63f76c`  
		Last Modified: Fri, 31 Jul 2020 18:22:44 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136109e5fe41668451f92ac3736ad9b13beaad345c444a2b8f1beae285845482`  
		Last Modified: Fri, 31 Jul 2020 18:22:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bfc5d689879bdf1417ed17a4792d986ff0a5362ad5a5eb0d689528aff65c02`  
		Last Modified: Fri, 31 Jul 2020 18:22:44 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm variant v6

```console
$ docker pull consul@sha256:592640a5b6da14fbc6e567fcd3c548080165306757af6e44b56b7bb75417b7ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41985414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb7861098a63733e866711b9cf1c74d8d9fb88ac4ff92b74ec98f1750f1af6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:49:28 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 17:49:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:49:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:49:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:49:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:49:50 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:49:51 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:49:52 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:49:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:49:55 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:49:56 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:49:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de1a03b3fc13a9075c1250be5493249912dce5e15e9753c9c9398980eb0d4ae`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8576d5c294e84e34f5b6237fb10073612fc291b0dc50cdd1526917bc33b2aa03`  
		Last Modified: Fri, 31 Jul 2020 17:51:22 GMT  
		Size: 39.4 MB (39378833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25df97f4a8ecd778d45756f729f6bc2c626419c09a6072c01536086127a2e871`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bb43074732055b48125b8d9073ca4051536d35f6d81ea39db553cd7a2d0f83`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed22160e4f87cae26a2799e49602e3cf17654ba2c678d34cb908b71dfc299ff8`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:f57b1adc53a6d9932920ac8de3b37a1dfde422a9b90e76ef4fe5f7fa2871a5cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42152129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba17a8a4a8191d58f893174738af22daca381bd6bac52f42bcfa6c4f9f0274e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:42:28 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 17:42:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:42:30 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:42:37 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:42:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:42:41 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:42:41 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:42:42 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:42:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:42:43 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:42:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:42:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:42:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b146c3825218c5e7651bb021f92e1366507e68b8a99f0f97d00976ab4a0e868d`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957c0502ca05193161542898e53baa24ff657bd0c507e55f6e1a431eee739235`  
		Last Modified: Fri, 31 Jul 2020 17:43:52 GMT  
		Size: 39.4 MB (39440872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6c0ecf4d0b8014b45db6555f9970db686bf7e0b1c5d6ce000153a5f088c255`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4563f0e1a06f87f9f67e5dcb7fb65f26d9f6ffcb96e056c0b33ebd3545ae73ba`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47d80ad7fa7726ed08e48df0df4073518b69ea9ce9e3d3cbc891450d83c0424`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8` - linux; 386

```console
$ docker pull consul@sha256:924569f2b8413a2d01c1b0bc066b27ab804c4c6a955d39e043f9659ce755b9c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46175418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e753bfbe5b552bbd08a454d93eaa3909c299d88c428da9315c8ae0946727c8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:38:31 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 17:38:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:38:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:38:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:38:38 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:38:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:38:39 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:38:39 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:38:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:38:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:38:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636640751b3378f0b762b46d4a92d24f67b4ff649d0cb789d642efd860e9c440`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d967afa7eb052c7fe31647177581ee6250623e5bbe192573158161455433af`  
		Last Modified: Fri, 31 Jul 2020 17:39:26 GMT  
		Size: 43.4 MB (43379882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfac606b9f8946bdb49fef9b75a2fec581594e24467a92124024be017173cb6b`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21de90667d06e1073368670c3a4366a4ef515bc95218e3b7a4b2346153e0642`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee55c145f43f961fa78a7d9dd968745ad604b215508541c8972aacd06f8d1b3`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:1.8.1`

```console
$ docker pull consul@sha256:5b66b9781bea2c07fa1b1ceaf5e91c0ed95b1870f3f501731ebab0f0c84c8f1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:1.8.1` - linux; amd64

```console
$ docker pull consul@sha256:2a5ddca1929c5e648fe69ac13eb9e23049f249e763c73677ad7cd0d6849e3b66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46709469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c8f1c8872c4eaae98e9a70a6dc42266b2aa35c26c1014d70fd35f7b334520`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 18:22:03 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 18:22:03 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 18:22:04 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 18:22:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 18:22:09 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 18:22:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 18:22:10 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 18:22:10 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 18:22:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 18:22:10 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 18:22:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 18:22:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 18:22:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc867292762be8dd9acce45a84106283f82fcf761880f48abb17bbda49aaae`  
		Last Modified: Fri, 31 Jul 2020 18:22:44 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a6bf4b5df2c0de7dd2d03c2c677c65163b177a24be41f5390af6677231891`  
		Last Modified: Fri, 31 Jul 2020 18:22:50 GMT  
		Size: 43.9 MB (43908692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33980ad85a4aff457107f89b4cb0381380ea383972301a4213e0f0326e63f76c`  
		Last Modified: Fri, 31 Jul 2020 18:22:44 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136109e5fe41668451f92ac3736ad9b13beaad345c444a2b8f1beae285845482`  
		Last Modified: Fri, 31 Jul 2020 18:22:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bfc5d689879bdf1417ed17a4792d986ff0a5362ad5a5eb0d689528aff65c02`  
		Last Modified: Fri, 31 Jul 2020 18:22:44 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.1` - linux; arm variant v6

```console
$ docker pull consul@sha256:592640a5b6da14fbc6e567fcd3c548080165306757af6e44b56b7bb75417b7ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41985414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb7861098a63733e866711b9cf1c74d8d9fb88ac4ff92b74ec98f1750f1af6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:49:28 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 17:49:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:49:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:49:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:49:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:49:50 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:49:51 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:49:52 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:49:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:49:55 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:49:56 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:49:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de1a03b3fc13a9075c1250be5493249912dce5e15e9753c9c9398980eb0d4ae`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8576d5c294e84e34f5b6237fb10073612fc291b0dc50cdd1526917bc33b2aa03`  
		Last Modified: Fri, 31 Jul 2020 17:51:22 GMT  
		Size: 39.4 MB (39378833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25df97f4a8ecd778d45756f729f6bc2c626419c09a6072c01536086127a2e871`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bb43074732055b48125b8d9073ca4051536d35f6d81ea39db553cd7a2d0f83`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed22160e4f87cae26a2799e49602e3cf17654ba2c678d34cb908b71dfc299ff8`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.1` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:f57b1adc53a6d9932920ac8de3b37a1dfde422a9b90e76ef4fe5f7fa2871a5cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42152129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba17a8a4a8191d58f893174738af22daca381bd6bac52f42bcfa6c4f9f0274e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:42:28 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 17:42:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:42:30 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:42:37 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:42:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:42:41 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:42:41 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:42:42 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:42:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:42:43 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:42:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:42:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:42:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b146c3825218c5e7651bb021f92e1366507e68b8a99f0f97d00976ab4a0e868d`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957c0502ca05193161542898e53baa24ff657bd0c507e55f6e1a431eee739235`  
		Last Modified: Fri, 31 Jul 2020 17:43:52 GMT  
		Size: 39.4 MB (39440872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6c0ecf4d0b8014b45db6555f9970db686bf7e0b1c5d6ce000153a5f088c255`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4563f0e1a06f87f9f67e5dcb7fb65f26d9f6ffcb96e056c0b33ebd3545ae73ba`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47d80ad7fa7726ed08e48df0df4073518b69ea9ce9e3d3cbc891450d83c0424`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:1.8.1` - linux; 386

```console
$ docker pull consul@sha256:924569f2b8413a2d01c1b0bc066b27ab804c4c6a955d39e043f9659ce755b9c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46175418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e753bfbe5b552bbd08a454d93eaa3909c299d88c428da9315c8ae0946727c8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:38:31 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 17:38:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:38:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:38:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:38:38 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:38:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:38:39 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:38:39 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:38:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:38:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:38:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636640751b3378f0b762b46d4a92d24f67b4ff649d0cb789d642efd860e9c440`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d967afa7eb052c7fe31647177581ee6250623e5bbe192573158161455433af`  
		Last Modified: Fri, 31 Jul 2020 17:39:26 GMT  
		Size: 43.4 MB (43379882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfac606b9f8946bdb49fef9b75a2fec581594e24467a92124024be017173cb6b`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21de90667d06e1073368670c3a4366a4ef515bc95218e3b7a4b2346153e0642`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee55c145f43f961fa78a7d9dd968745ad604b215508541c8972aacd06f8d1b3`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `consul:latest`

```console
$ docker pull consul@sha256:5b66b9781bea2c07fa1b1ceaf5e91c0ed95b1870f3f501731ebab0f0c84c8f1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `consul:latest` - linux; amd64

```console
$ docker pull consul@sha256:2a5ddca1929c5e648fe69ac13eb9e23049f249e763c73677ad7cd0d6849e3b66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.7 MB (46709469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b5c8f1c8872c4eaae98e9a70a6dc42266b2aa35c26c1014d70fd35f7b334520`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 18:22:03 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 18:22:03 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 18:22:03 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 18:22:04 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 18:22:08 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 18:22:09 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 18:22:10 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 18:22:10 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 18:22:10 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 18:22:10 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 18:22:10 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 18:22:11 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 18:22:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 18:22:11 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc867292762be8dd9acce45a84106283f82fcf761880f48abb17bbda49aaae`  
		Last Modified: Fri, 31 Jul 2020 18:22:44 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505a6bf4b5df2c0de7dd2d03c2c677c65163b177a24be41f5390af6677231891`  
		Last Modified: Fri, 31 Jul 2020 18:22:50 GMT  
		Size: 43.9 MB (43908692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33980ad85a4aff457107f89b4cb0381380ea383972301a4213e0f0326e63f76c`  
		Last Modified: Fri, 31 Jul 2020 18:22:44 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136109e5fe41668451f92ac3736ad9b13beaad345c444a2b8f1beae285845482`  
		Last Modified: Fri, 31 Jul 2020 18:22:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28bfc5d689879bdf1417ed17a4792d986ff0a5362ad5a5eb0d689528aff65c02`  
		Last Modified: Fri, 31 Jul 2020 18:22:44 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm variant v6

```console
$ docker pull consul@sha256:592640a5b6da14fbc6e567fcd3c548080165306757af6e44b56b7bb75417b7ba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41985414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb7861098a63733e866711b9cf1c74d8d9fb88ac4ff92b74ec98f1750f1af6e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:49:28 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:49:28 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 17:49:29 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:49:31 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:49:42 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:49:46 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:49:50 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:49:51 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:49:52 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:49:53 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:49:55 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:49:56 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:49:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:49:57 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de1a03b3fc13a9075c1250be5493249912dce5e15e9753c9c9398980eb0d4ae`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8576d5c294e84e34f5b6237fb10073612fc291b0dc50cdd1526917bc33b2aa03`  
		Last Modified: Fri, 31 Jul 2020 17:51:22 GMT  
		Size: 39.4 MB (39378833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25df97f4a8ecd778d45756f729f6bc2c626419c09a6072c01536086127a2e871`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bb43074732055b48125b8d9073ca4051536d35f6d81ea39db553cd7a2d0f83`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed22160e4f87cae26a2799e49602e3cf17654ba2c678d34cb908b71dfc299ff8`  
		Last Modified: Fri, 31 Jul 2020 17:51:11 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; arm64 variant v8

```console
$ docker pull consul@sha256:f57b1adc53a6d9932920ac8de3b37a1dfde422a9b90e76ef4fe5f7fa2871a5cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42152129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ba17a8a4a8191d58f893174738af22daca381bd6bac52f42bcfa6c4f9f0274e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:42:27 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:42:28 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 17:42:28 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:42:30 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:42:37 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:42:39 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:42:41 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:42:41 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:42:42 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:42:43 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:42:43 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:42:44 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:42:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:42:45 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b146c3825218c5e7651bb021f92e1366507e68b8a99f0f97d00976ab4a0e868d`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957c0502ca05193161542898e53baa24ff657bd0c507e55f6e1a431eee739235`  
		Last Modified: Fri, 31 Jul 2020 17:43:52 GMT  
		Size: 39.4 MB (39440872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6c0ecf4d0b8014b45db6555f9970db686bf7e0b1c5d6ce000153a5f088c255`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4563f0e1a06f87f9f67e5dcb7fb65f26d9f6ffcb96e056c0b33ebd3545ae73ba`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47d80ad7fa7726ed08e48df0df4073518b69ea9ce9e3d3cbc891450d83c0424`  
		Last Modified: Fri, 31 Jul 2020 17:43:43 GMT  
		Size: 1.7 KB (1709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `consul:latest` - linux; 386

```console
$ docker pull consul@sha256:924569f2b8413a2d01c1b0bc066b27ab804c4c6a955d39e043f9659ce755b9c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46175418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e753bfbe5b552bbd08a454d93eaa3909c299d88c428da9315c8ae0946727c8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["agent","-dev","-client","0.0.0.0"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Fri, 31 Jul 2020 17:38:31 GMT
LABEL org.opencontainers.image.authors=Consul Team <consul@hashicorp.com>
# Fri, 31 Jul 2020 17:38:31 GMT
ENV CONSUL_VERSION=1.8.1
# Fri, 31 Jul 2020 17:38:31 GMT
ENV HASHICORP_RELEASES=https://releases.hashicorp.com
# Fri, 31 Jul 2020 17:38:32 GMT
RUN addgroup consul &&     adduser -S -G consul consul
# Fri, 31 Jul 2020 17:38:38 GMT
RUN set -eux &&     apk add --no-cache ca-certificates curl dumb-init gnupg libcap openssl su-exec iputils jq libc6-compat &&     gpg --keyserver pgp.mit.edu --recv-keys 91A6E7F85D05C65630BEF18951852D87348FFC4C &&     mkdir -p /tmp/build &&     cd /tmp/build &&     apkArch="$(apk --print-arch)" &&     case "${apkArch}" in         aarch64) consulArch='arm64' ;;         armhf) consulArch='armhfv6' ;;         x86) consulArch='386' ;;         x86_64) consulArch='amd64' ;;         *) echo >&2 "error: unsupported architecture: ${apkArch} (see ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/)" && exit 1 ;;     esac &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS &&     wget ${HASHICORP_RELEASES}/consul/${CONSUL_VERSION}/consul_${CONSUL_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify consul_${CONSUL_VERSION}_SHA256SUMS.sig consul_${CONSUL_VERSION}_SHA256SUMS &&     grep consul_${CONSUL_VERSION}_linux_${consulArch}.zip consul_${CONSUL_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin consul_${CONSUL_VERSION}_linux_${consulArch}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill all &&     apk del gnupg openssl &&     rm -rf /root/.gnupg &&     consul version
# Fri, 31 Jul 2020 17:38:38 GMT
RUN mkdir -p /consul/data &&     mkdir -p /consul/config &&     chown -R consul:consul /consul
# Fri, 31 Jul 2020 17:38:39 GMT
RUN test -e /etc/nsswitch.conf || echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 31 Jul 2020 17:38:39 GMT
VOLUME [/consul/data]
# Fri, 31 Jul 2020 17:38:39 GMT
EXPOSE 8300
# Fri, 31 Jul 2020 17:38:40 GMT
EXPOSE 8301 8301/udp 8302 8302/udp
# Fri, 31 Jul 2020 17:38:40 GMT
EXPOSE 8500 8600 8600/udp
# Fri, 31 Jul 2020 17:38:40 GMT
COPY file:247b557dfc58d59b4f83bd2bd196c7a03ff835064b0d7fef7dfe91b84120ff30 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 31 Jul 2020 17:38:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 31 Jul 2020 17:38:41 GMT
CMD ["agent" "-dev" "-client" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636640751b3378f0b762b46d4a92d24f67b4ff649d0cb789d642efd860e9c440`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d967afa7eb052c7fe31647177581ee6250623e5bbe192573158161455433af`  
		Last Modified: Fri, 31 Jul 2020 17:39:26 GMT  
		Size: 43.4 MB (43379882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfac606b9f8946bdb49fef9b75a2fec581594e24467a92124024be017173cb6b`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21de90667d06e1073368670c3a4366a4ef515bc95218e3b7a4b2346153e0642`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee55c145f43f961fa78a7d9dd968745ad604b215508541c8972aacd06f8d1b3`  
		Last Modified: Fri, 31 Jul 2020 17:39:17 GMT  
		Size: 1.7 KB (1710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
